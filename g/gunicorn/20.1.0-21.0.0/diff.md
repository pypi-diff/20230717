# Comparing `tmp/gunicorn-20.1.0.tar.gz` & `tmp/gunicorn-21.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gunicorn-20.1.0.tar", last modified: Sat Mar 27 01:49:35 2021, max compression
+gzip compressed data, was "gunicorn-21.0.0.tar", last modified: Mon Jul 17 20:28:19 2023, max compression
```

## Comparing `gunicorn-20.1.0.tar` & `gunicorn-21.0.0.tar`

### file list

```diff
@@ -1,350 +1,357 @@
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/
--rw-r--r--   0 benoitc    (501) staff       (20)     4093 2021-03-27 01:49:35.000000 gunicorn-20.1.0/PKG-INFO
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn.egg-info/
--rw-r--r--   0 benoitc    (501) staff       (20)     4093 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn.egg-info/PKG-INFO
--rw-r--r--   0 benoitc    (501) staff       (20)        1 2021-03-27 01:47:37.000000 gunicorn-20.1.0/gunicorn.egg-info/not-zip-safe
--rw-r--r--   0 benoitc    (501) staff       (20)     9037 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn.egg-info/SOURCES.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      130 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn.egg-info/entry_points.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      133 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn.egg-info/requires.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        9 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn.egg-info/top_level.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        1 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn.egg-info/dependency_links.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     1136 2021-01-08 10:46:21.000000 gunicorn-20.1.0/LICENSE
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/tests/
--rw-r--r--   0 benoitc    (501) staff       (20)      597 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_invalid_requests.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1745 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/support.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4449 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_statsd.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1525 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_pidfile.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/tests/config/
--rw-r--r--   0 benoitc    (501) staff       (20)       24 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/config/test_cfg_alt.py
--rw-r--r--   0 benoitc    (501) staff       (20)       88 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/config/test_cfg.py
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/config/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)       23 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/config/test_cfg_with_wsgi_app.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2052 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_systemd.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4367 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_util.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/tests/requests/
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/tests/requests/valid/
--rw-r--r--   0 benoitc    (501) staff       (20)      258 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/018.py
--rw-r--r--   0 benoitc    (501) staff       (20)       51 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/006.http
--rw-r--r--   0 benoitc    (501) staff       (20)      178 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/008.py
--rw-r--r--   0 benoitc    (501) staff       (20)      134 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/010.http
--rw-r--r--   0 benoitc    (501) staff       (20)      129 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/030.http
--rw-r--r--   0 benoitc    (501) staff       (20)      261 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/028.py
--rw-r--r--   0 benoitc    (501) staff       (20)     8233 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/026.http
--rw-r--r--   0 benoitc    (501) staff       (20)      278 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/029.py
--rw-r--r--   0 benoitc    (501) staff       (20)      359 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/pp_01.py
--rw-r--r--   0 benoitc    (501) staff       (20)       30 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/027.http
--rw-r--r--   0 benoitc    (501) staff       (20)      125 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/011.http
--rw-r--r--   0 benoitc    (501) staff       (20)      119 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/019.py
--rw-r--r--   0 benoitc    (501) staff       (20)       61 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/007.http
--rw-r--r--   0 benoitc    (501) staff       (20)      264 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/009.py
--rw-r--r--   0 benoitc    (501) staff       (20)     8463 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/026.py
--rw-r--r--   0 benoitc    (501) staff       (20)       81 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/020.http
--rw-r--r--   0 benoitc    (501) staff       (20)      285 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/012.py
--rw-r--r--   0 benoitc    (501) staff       (20)      296 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/002.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2376 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/016.py
--rw-r--r--   0 benoitc    (501) staff       (20)      286 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/022.py
--rw-r--r--   0 benoitc    (501) staff       (20)      361 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/pp_02.http
--rw-r--r--   0 benoitc    (501) staff       (20)      142 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/006.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2234 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/016.http
--rw-r--r--   0 benoitc    (501) staff       (20)       91 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/017.http
--rw-r--r--   0 benoitc    (501) staff       (20)      207 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/017.py
--rw-r--r--   0 benoitc    (501) staff       (20)      335 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/023.py
--rw-r--r--   0 benoitc    (501) staff       (20)      149 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/001.http
--rw-r--r--   0 benoitc    (501) staff       (20)      167 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/007.py
--rw-r--r--   0 benoitc    (501) staff       (20)      130 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/027.py
--rw-r--r--   0 benoitc    (501) staff       (20)      192 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/013.py
--rw-r--r--   0 benoitc    (501) staff       (20)     9909 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/099.http
--rw-r--r--   0 benoitc    (501) staff       (20)      577 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/003.py
--rw-r--r--   0 benoitc    (501) staff       (20)       80 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/021.http
--rw-r--r--   0 benoitc    (501) staff       (20)       58 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/018.http
--rw-r--r--   0 benoitc    (501) staff       (20)      137 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/014.py
--rw-r--r--   0 benoitc    (501) staff       (20)      171 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/020.py
--rw-r--r--   0 benoitc    (501) staff       (20)      278 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/030.py
--rw-r--r--   0 benoitc    (501) staff       (20)      164 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/004.py
--rw-r--r--   0 benoitc    (501) staff       (20)       85 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/022.http
--rw-r--r--   0 benoitc    (501) staff       (20)       46 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/014.http
--rw-r--r--   0 benoitc    (501) staff       (20)    16639 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/024.py
--rw-r--r--   0 benoitc    (501) staff       (20)      218 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/010.py
--rw-r--r--   0 benoitc    (501) staff       (20)      168 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/002.http
--rw-r--r--   0 benoitc    (501) staff       (20)      476 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/025.py
--rw-r--r--   0 benoitc    (501) staff       (20)      196 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/011.py
--rw-r--r--   0 benoitc    (501) staff       (20)      199 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/pp_01.http
--rw-r--r--   0 benoitc    (501) staff       (20)      131 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/100.py
--rw-r--r--   0 benoitc    (501) staff       (20)      394 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/003.http
--rw-r--r--   0 benoitc    (501) staff       (20)      275 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/001.py
--rw-r--r--   0 benoitc    (501) staff       (20)       98 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/015.http
--rw-r--r--   0 benoitc    (501) staff       (20)      226 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/015.py
--rw-r--r--   0 benoitc    (501) staff       (20)      155 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/023.http
--rw-r--r--   0 benoitc    (501) staff       (20)      142 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/021.py
--rw-r--r--   0 benoitc    (501) staff       (20)      153 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/005.py
--rw-r--r--   0 benoitc    (501) staff       (20)       58 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/019.http
--rw-r--r--   0 benoitc    (501) staff       (20)      166 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/012.http
--rw-r--r--   0 benoitc    (501) staff       (20)       41 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/100.http
--rw-r--r--   0 benoitc    (501) staff       (20)       57 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/004.http
--rw-r--r--   0 benoitc    (501) staff       (20)      639 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/pp_02.py
--rw-r--r--   0 benoitc    (501) staff       (20)       68 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/028.http
--rw-r--r--   0 benoitc    (501) staff       (20)       73 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/008.http
--rw-r--r--   0 benoitc    (501) staff       (20)    16408 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/024.http
--rw-r--r--   0 benoitc    (501) staff       (20)      364 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/025.http
--rw-r--r--   0 benoitc    (501) staff       (20)      137 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/009.http
--rw-r--r--   0 benoitc    (501) staff       (20)      129 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/029.http
--rw-r--r--   0 benoitc    (501) staff       (20)       62 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/005.http
--rw-r--r--   0 benoitc    (501) staff       (20)     9135 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/099.py
--rw-r--r--   0 benoitc    (501) staff       (20)      159 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/valid/013.http
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/tests/requests/invalid/
--rw-r--r--   0 benoitc    (501) staff       (20)       81 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/018.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4122 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/006.http
--rw-r--r--   0 benoitc    (501) staff       (20)       83 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/008.py
--rw-r--r--   0 benoitc    (501) staff       (20)       44 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/010.http
--rw-r--r--   0 benoitc    (501) staff       (20)      161 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/pp_01.py
--rw-r--r--   0 benoitc    (501) staff       (20)      169 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/011.http
--rw-r--r--   0 benoitc    (501) staff       (20)      172 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/019.py
--rw-r--r--   0 benoitc    (501) staff       (20)     8358 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/007.http
--rw-r--r--   0 benoitc    (501) staff       (20)       83 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/009.py
--rw-r--r--   0 benoitc    (501) staff       (20)       69 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/020.http
--rw-r--r--   0 benoitc    (501) staff       (20)      174 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/012.py
--rw-r--r--   0 benoitc    (501) staff       (20)       81 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/002.py
--rw-r--r--   0 benoitc    (501) staff       (20)       82 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/016.py
--rw-r--r--   0 benoitc    (501) staff       (20)       53 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/pp_02.http
--rw-r--r--   0 benoitc    (501) staff       (20)       77 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/006.py
--rw-r--r--   0 benoitc    (501) staff       (20)       33 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/016.http
--rw-r--r--   0 benoitc    (501) staff       (20)     8222 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/017.http
--rw-r--r--   0 benoitc    (501) staff       (20)      134 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/017.py
--rw-r--r--   0 benoitc    (501) staff       (20)       29 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/001.http
--rw-r--r--   0 benoitc    (501) staff       (20)       83 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/007.py
--rw-r--r--   0 benoitc    (501) staff       (20)      174 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/013.py
--rw-r--r--   0 benoitc    (501) staff       (20)       84 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/003.py
--rw-r--r--   0 benoitc    (501) staff       (20)       90 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/021.http
--rw-r--r--   0 benoitc    (501) staff       (20)       48 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/018.http
--rw-r--r--   0 benoitc    (501) staff       (20)       72 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/014.py
--rw-r--r--   0 benoitc    (501) staff       (20)      130 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/020.py
--rw-r--r--   0 benoitc    (501) staff       (20)       80 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/004.py
--rw-r--r--   0 benoitc    (501) staff       (20)       78 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/014.http
--rw-r--r--   0 benoitc    (501) staff       (20)      174 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/010.py
--rw-r--r--   0 benoitc    (501) staff       (20)       21 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/002.http
--rw-r--r--   0 benoitc    (501) staff       (20)      169 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/011.py
--rw-r--r--   0 benoitc    (501) staff       (20)       37 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/pp_01.http
--rw-r--r--   0 benoitc    (501) staff       (20)       30 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/003.http
--rw-r--r--   0 benoitc    (501) staff       (20)       64 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/001.py
--rw-r--r--   0 benoitc    (501) staff       (20)       88 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/015.http
--rw-r--r--   0 benoitc    (501) staff       (20)       72 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/015.py
--rw-r--r--   0 benoitc    (501) staff       (20)      122 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/021.py
--rw-r--r--   0 benoitc    (501) staff       (20)       78 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/005.py
--rw-r--r--   0 benoitc    (501) staff       (20)       82 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/019.http
--rw-r--r--   0 benoitc    (501) staff       (20)      169 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/012.http
--rw-r--r--   0 benoitc    (501) staff       (20)       25 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/004.http
--rw-r--r--   0 benoitc    (501) staff       (20)      161 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/pp_02.py
--rw-r--r--   0 benoitc    (501) staff       (20)    12418 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/008.http
--rw-r--r--   0 benoitc    (501) staff       (20)     1829 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/009.http
--rw-r--r--   0 benoitc    (501) staff       (20)       41 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/005.http
--rw-r--r--   0 benoitc    (501) staff       (20)       49 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/requests/invalid/013.http
--rw-r--r--   0 benoitc    (501) staff       (20)     6113 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_arbiter.py
--rw-r--r--   0 benoitc    (501) staff       (20)     9434 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/treq.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2277 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_ssl.py
--rw-r--r--   0 benoitc    (501) staff       (20)     6856 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_http.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1878 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_sock.py
--rw-r--r--   0 benoitc    (501) staff       (20)      608 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_valid_requests.py
--rw-r--r--   0 benoitc    (501) staff       (20)    14482 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_config.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1851 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_reload.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/tests/workers/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/workers/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)      190 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/workers/test_ggevent.py
--rw-r--r--   0 benoitc    (501) staff       (20)      192 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/workers/test_geventlet.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1614 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/t.py
--rw-r--r--   0 benoitc    (501) staff       (20)     3140 2021-01-08 10:46:21.000000 gunicorn-20.1.0/tests/test_logger.py
--rw-r--r--   0 benoitc    (501) staff       (20)      324 2021-01-08 10:46:21.000000 gunicorn-20.1.0/MANIFEST.in
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn/
--rw-r--r--   0 benoitc    (501) staff       (20)     2367 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/pidfile.py
--rw-r--r--   0 benoitc    (501) staff       (20)     3777 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/reloader.py
--rw-r--r--   0 benoitc    (501) staff       (20)    58636 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/config.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn/app/
--rw-r--r--   0 benoitc    (501) staff       (20)     1926 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/app/wsgiapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)      127 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/app/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2038 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/app/pasterapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)     7150 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/app/base.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn/instrument/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/instrument/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4633 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/instrument/statsd.py
--rw-r--r--   0 benoitc    (501) staff       (20)    18516 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/util.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2511 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/systemd.py
--rw-r--r--   0 benoitc    (501) staff       (20)      279 2021-02-12 21:43:35.000000 gunicorn-20.1.0/gunicorn/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     6110 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/sock.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn/http/
--rw-r--r--   0 benoitc    (501) staff       (20)     7297 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/http/body.py
--rw-r--r--   0 benoitc    (501) staff       (20)      277 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/http/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)    11759 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/http/message.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1943 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/http/unreader.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1364 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/http/parser.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2850 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/http/errors.py
--rw-r--r--   0 benoitc    (501) staff       (20)    12328 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/http/wsgi.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2289 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/debug.py
--rw-r--r--   0 benoitc    (501) staff       (20)    20521 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/arbiter.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/gunicorn/workers/
--rw-r--r--   0 benoitc    (501) staff       (20)     7327 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/workers/sync.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5693 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/workers/base_async.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5988 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/workers/gtornado.py
--rw-r--r--   0 benoitc    (501) staff       (20)      594 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/workers/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5713 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/workers/geventlet.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1649 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/workers/workertmp.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5733 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/workers/ggevent.py
--rw-r--r--   0 benoitc    (501) staff       (20)    12194 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/workers/gthread.py
--rw-r--r--   0 benoitc    (501) staff       (20)     9103 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/workers/base.py
--rw-r--r--   0 benoitc    (501) staff       (20)      919 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/errors.py
--rw-r--r--   0 benoitc    (501) staff       (20)    14913 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/glogging.py
--rw-r--r--   0 benoitc    (501) staff       (20)      171 2021-01-08 10:46:21.000000 gunicorn-20.1.0/gunicorn/__main__.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/docs/
--rw-r--r--   0 benoitc    (501) staff       (20)     5791 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/Makefile
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/docs/source/
--rw-r--r--   0 benoitc    (501) staff       (20)     5551 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/install.rst
--rw-r--r--   0 benoitc    (501) staff       (20)    32740 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/settings.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1927 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/custom.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1040 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/index.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2956 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/2018-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     4786 2021-01-08 11:20:26.000000 gunicorn-20.1.0/docs/source/2019-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2005 2021-02-12 21:42:54.000000 gunicorn-20.1.0/docs/source/news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6454 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/design.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     5420 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/signals.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     4183 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/2012-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     3270 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/2013-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1903 2021-02-12 21:40:54.000000 gunicorn-20.1.0/docs/source/2021-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1885 2021-01-08 11:20:01.000000 gunicorn-20.1.0/docs/source/2020-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1755 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/conf.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5702 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/2015-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6834 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/2014-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)    11588 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/deploy.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1375 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/community.rst
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/docs/source/_static/
--rw-r--r--   0 benoitc    (501) staff       (20)    14398 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/_static/gunicorn.png
--rw-r--r--   0 benoitc    (501) staff       (20)     2092 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/2011-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6643 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/2010-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1325 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/instrumentation.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6485 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/run.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     3849 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/configure.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2911 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/2016-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2100 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/2017-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     8402 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/source/faq.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2088 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/sitemap_gen.py
--rwxr-xr-x   0 benoitc    (501) staff       (20)     2965 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/gunicorn_ext.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5109 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/make.bat
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/docs/logo/
--rw-r--r--   0 benoitc    (501) staff       (20)    21550 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/logo/gunicorn.png
--rw-r--r--   0 benoitc    (501) staff       (20)    12798 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/logo/gunicorn.svg
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/docs/site/
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/tuning.html
--rw-r--r--   0 benoitc    (501) staff       (20)      298 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/install.html
--rw-r--r--   0 benoitc    (501) staff       (20)      297 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/design.html
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/run.html
--rw-r--r--   0 benoitc    (501) staff       (20)      340 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/community.html
--rw-r--r--   0 benoitc    (501) staff       (20)     7854 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/index.html
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/docs/site/css/
--rw-r--r--   0 benoitc    (501) staff       (20)     6671 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/css/style.css
--rw-r--r--   0 benoitc    (501) staff       (20)       13 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/CNAME
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/docs/site/images/
--rw-r--r--   0 benoitc    (501) staff       (20)     3450 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/title.png
--rw-r--r--   0 benoitc    (501) staff       (20)    15593 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/community.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)    15962 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/downloads.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)      408 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/arrow.png
--rw-r--r--   0 benoitc    (501) staff       (20)      577 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/redbutton.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)    17566 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/documents.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     1771 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/favicon.png
--rw-r--r--   0 benoitc    (501) staff       (20)      255 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/footer-arrow.png
--rw-r--r--   0 benoitc    (501) staff       (20)     2184 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/user1.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)    10238 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/logo.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     7343 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/logo.png
--rw-r--r--   0 benoitc    (501) staff       (20)      335 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/greenbutton.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     1553 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/gunicorn.png
--rw-r--r--   0 benoitc    (501) staff       (20)     3145 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/logo-bottom.png
--rw-r--r--   0 benoitc    (501) staff       (20)      611 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/banner-bg.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)    17551 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/about.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     2499 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/footer-logo.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)      440 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/separator.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)    21956 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/images/large_gunicorn.png
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/docs/site/js/
--rwxr-xr-x   0 benoitc    (501) staff       (20)     1479 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/js/main.js
--rw-r--r--   0 benoitc    (501) staff       (20)      304 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/configuration.html
--rw-r--r--   0 benoitc    (501) staff       (20)      295 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/news.html
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/.nojekyll
--rw-r--r--   0 benoitc    (501) staff       (20)      300 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/configure.html
--rw-r--r--   0 benoitc    (501) staff       (20)      343 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/deploy.html
--rw-r--r--   0 benoitc    (501) staff       (20)     1990 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/sitemap.xml
--rw-r--r--   0 benoitc    (501) staff       (20)      342 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/deployment.html
--rw-r--r--   0 benoitc    (501) staff       (20)      298 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/installation.html
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/usage.html
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/site/faq.html
--rw-r--r--   0 benoitc    (501) staff       (20)      288 2021-01-08 10:46:21.000000 gunicorn-20.1.0/docs/README.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     3777 2021-01-08 10:46:21.000000 gunicorn-20.1.0/NOTICE
--rw-r--r--   0 benoitc    (501) staff       (20)     3650 2021-01-08 10:46:21.000000 gunicorn-20.1.0/setup.py
--rwxr-xr-x   0 benoitc    (501) staff       (20)      267 2021-01-08 10:46:21.000000 gunicorn-20.1.0/.gitignore
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/examples/
--rw-r--r--   0 benoitc    (501) staff       (20)      993 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/multidomainapp.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/examples/websocket/
--rw-r--r--   0 benoitc    (501) staff       (20)    15684 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/websocket/gevent_websocket.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1320 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/websocket/websocket.html
--rw-r--r--   0 benoitc    (501) staff       (20)    15729 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/websocket/websocket.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1679 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/server.key
--rw-r--r--   0 benoitc    (501) staff       (20)      584 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/sendfile.py
--rw-r--r--   0 benoitc    (501) staff       (20)      182 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/supervisor.conf
--rw-r--r--   0 benoitc    (501) staff       (20)      620 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/timeout.py
--rw-r--r--   0 benoitc    (501) staff       (20)      108 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/boot_fail.py
--rw-r--r--   0 benoitc    (501) staff       (20)      403 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/read_django_settings.py
--rw-r--r--   0 benoitc    (501) staff       (20)      738 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/alt_spec.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/examples/deep/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/deep/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)      659 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/deep/test.py
--rw-r--r--   0 benoitc    (501) staff       (20)      659 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/test.py
--rw-r--r--   0 benoitc    (501) staff       (20)      841 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/logging.conf
--rw-r--r--   0 benoitc    (501) staff       (20)      372 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/log_app.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1257 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/server.crt
--rw-r--r--   0 benoitc    (501) staff       (20)      737 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/longpoll.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1470 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/multiapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1339 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/standalone_app.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1020 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/when_ready.conf.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1015 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/readline_app.py
--rw-r--r--   0 benoitc    (501) staff       (20)      448 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/log_app.ini
--rw-r--r--   0 benoitc    (501) staff       (20)      604 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/slowclient.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1980 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/nginx.conf
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/examples/frameworks/
--rw-r--r--   0 benoitc    (501) staff       (20)      873 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/tornadoapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)        7 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/requirements_webpyapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      150 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/requirements.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      198 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/cherryapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)        6 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/requirements_flaskapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        9 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/requirements_cherryapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      338 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/pyramidapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)      197 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/webpyapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)      147 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/flaskapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)       10 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/requirements_tornadoapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      291 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/flask_sendfile.py
--rw-r--r--   0 benoitc    (501) staff       (20)        8 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/requirements_pyramidapp.txt
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/examples/frameworks/django/
--rw-r--r--   0 benoitc    (501) staff       (20)       60 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/README
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/examples/frameworks/django/testing/
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5730 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/settings.py
--rw-r--r--   0 benoitc    (501) staff       (20)      577 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/urls.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/__init__.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/models.py
--rwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/__init__.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2021-03-27 01:49:35.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/templates/
--rw-r--r--   0 benoitc    (501) staff       (20)      471 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/templates/home.html
--rw-r--r--   0 benoitc    (501) staff       (20)      759 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html
--rwxr-xr-x   0 benoitc    (501) staff       (20)      513 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/tests.py
--rw-r--r--   0 benoitc    (501) staff       (20)      133 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/urls.py
--rw-r--r--   0 benoitc    (501) staff       (20)      627 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/middleware.py
--rwxr-xr-x   0 benoitc    (501) staff       (20)     1548 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/views.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1359 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/testing/wsgi.py
--rwxr-xr-x   0 benoitc    (501) staff       (20)      244 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/django/testing/manage.py
--rw-r--r--   0 benoitc    (501) staff       (20)      501 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/frameworks/flaskapp_aiohttp_wsgi.py
--rwxr-xr-x   0 benoitc    (501) staff       (20)      215 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/gunicorn_rc
--rw-r--r--   0 benoitc    (501) staff       (20)      676 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/echo.py
--rw-r--r--   0 benoitc    (501) staff       (20)       13 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/hello.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      204 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/bad.py
--rw-r--r--   0 benoitc    (501) staff       (20)     6691 2021-01-08 10:46:21.000000 gunicorn-20.1.0/examples/example_config.py
--rw-r--r--   0 benoitc    (501) staff       (20)      203 2021-03-27 01:49:35.000000 gunicorn-20.1.0/setup.cfg
--rw-r--r--   0 benoitc    (501) staff       (20)     6638 2021-01-08 10:46:21.000000 gunicorn-20.1.0/THANKS
--rw-r--r--   0 benoitc    (501) staff       (20)       51 2021-01-08 10:46:21.000000 gunicorn-20.1.0/requirements_test.txt
--rw-r--r--   0 benoitc    (501) staff       (20)     1762 2021-01-08 10:46:21.000000 gunicorn-20.1.0/README.rst
--rw-r--r--   0 benoitc    (501) staff       (20)       50 2021-01-08 10:46:21.000000 gunicorn-20.1.0/requirements_dev.txt
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.048336 gunicorn-21.0.0/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      267 2023-07-17 19:03:36.000000 gunicorn-21.0.0/.gitignore
+-rw-r--r--   0 benoitc    (501) staff       (20)     1136 2023-07-17 19:03:36.000000 gunicorn-21.0.0/LICENSE
+-rw-r--r--   0 benoitc    (501) staff       (20)      324 2023-07-17 19:03:36.000000 gunicorn-21.0.0/MANIFEST.in
+-rw-r--r--   0 benoitc    (501) staff       (20)     3777 2023-07-17 19:03:36.000000 gunicorn-21.0.0/NOTICE
+-rw-r--r--   0 benoitc    (501) staff       (20)     3852 2023-07-17 20:28:19.048396 gunicorn-21.0.0/PKG-INFO
+-rw-r--r--   0 benoitc    (501) staff       (20)     1988 2023-07-17 19:03:36.000000 gunicorn-21.0.0/README.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6969 2023-07-17 19:03:36.000000 gunicorn-21.0.0/THANKS
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.016334 gunicorn-21.0.0/docs/
+-rw-r--r--   0 benoitc    (501) staff       (20)     5791 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/Makefile
+-rw-r--r--   0 benoitc    (501) staff       (20)      288 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/README.rst
+-rwxr-xr-x   0 benoitc    (501) staff       (20)     3029 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/gunicorn_ext.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.016592 gunicorn-21.0.0/docs/logo/
+-rw-r--r--   0 benoitc    (501) staff       (20)    21550 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/logo/gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)    12798 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/logo/gunicorn.svg
+-rw-r--r--   0 benoitc    (501) staff       (20)     5109 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/make.bat
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.018512 gunicorn-21.0.0/docs/site/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/.nojekyll
+-rw-r--r--   0 benoitc    (501) staff       (20)       13 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/CNAME
+-rw-r--r--   0 benoitc    (501) staff       (20)      340 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/community.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      304 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/configuration.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      300 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/configure.html
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.018612 gunicorn-21.0.0/docs/site/css/
+-rw-r--r--   0 benoitc    (501) staff       (20)     6671 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/css/style.css
+-rw-r--r--   0 benoitc    (501) staff       (20)      343 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/deploy.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      342 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/deployment.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      297 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/design.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/faq.html
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.020586 gunicorn-21.0.0/docs/site/images/
+-rw-r--r--   0 benoitc    (501) staff       (20)    17551 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/about.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)      408 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/arrow.png
+-rw-r--r--   0 benoitc    (501) staff       (20)      611 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/banner-bg.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)    15593 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/community.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)    17566 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/documents.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)    15962 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/downloads.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     1771 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/favicon.png
+-rw-r--r--   0 benoitc    (501) staff       (20)      255 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/footer-arrow.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     2499 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/footer-logo.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)      335 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/greenbutton.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     1553 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)    21956 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/large_gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     3145 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/logo-bottom.png
+-rw-r--r--   0 benoitc    (501) staff       (20)    10238 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/logo.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     7343 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/logo.png
+-rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/redbutton.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)      440 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/separator.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     3450 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/title.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     2184 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/user1.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     7856 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/index.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      298 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/install.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      298 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/installation.html
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.020685 gunicorn-21.0.0/docs/site/js/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)     1479 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/js/main.js
+-rw-r--r--   0 benoitc    (501) staff       (20)      295 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/run.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     1990 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/sitemap.xml
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/tuning.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/usage.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     2088 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/sitemap_gen.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.023305 gunicorn-21.0.0/docs/source/
+-rw-r--r--   0 benoitc    (501) staff       (20)     6643 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2010-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2092 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2011-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     4184 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2012-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     3267 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2013-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6834 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2014-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     5702 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2015-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2911 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2016-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2100 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2017-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2956 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2018-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     4785 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2019-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)      112 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2020-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1905 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2021-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)      530 2023-07-17 20:14:25.000000 gunicorn-21.0.0/docs/source/2023-news.rst
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.023404 gunicorn-21.0.0/docs/source/_static/
+-rw-r--r--   0 benoitc    (501) staff       (20)    14398 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/_static/gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     1377 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/community.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1755 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/conf.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     3873 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/configure.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1927 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/custom.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)    12260 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/deploy.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6483 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/design.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     8672 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/faq.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1043 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/index.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     5551 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/install.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1325 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/instrumentation.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)      727 2023-07-17 20:14:25.000000 gunicorn-21.0.0/docs/source/news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6485 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/run.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)    36932 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/settings.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     5420 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/signals.rst
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.025797 gunicorn-21.0.0/examples/
+-rw-r--r--   0 benoitc    (501) staff       (20)      738 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/alt_spec.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      204 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/bad.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      108 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/boot_fail.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.025966 gunicorn-21.0.0/examples/deep/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/deep/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      659 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/deep/test.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      676 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/echo.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7621 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/example_config.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.027234 gunicorn-21.0.0/examples/frameworks/
+-rw-r--r--   0 benoitc    (501) staff       (20)      198 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/cherryapp.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.027336 gunicorn-21.0.0/examples/frameworks/django/
+-rw-r--r--   0 benoitc    (501) staff       (20)       60 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/README
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.027432 gunicorn-21.0.0/examples/frameworks/django/testing/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      244 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/manage.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.027820 gunicorn-21.0.0/examples/frameworks/django/testing/testing/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/__init__.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.027924 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/__init__.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.028472 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      627 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/middleware.py
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/models.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.028675 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/templates/
+-rw-r--r--   0 benoitc    (501) staff       (20)      759 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      471 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/templates/home.html
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      509 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/tests.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      133 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/urls.py
+-rwxr-xr-x   0 benoitc    (501) staff       (20)     1548 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/views.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5730 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/settings.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/urls.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1359 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/wsgi.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      291 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/flask_sendfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      147 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/flaskapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      501 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/flaskapp_aiohttp_wsgi.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      338 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/pyramidapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      150 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        9 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements_cherryapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        6 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements_flaskapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        8 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements_pyramidapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)       10 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements_tornadoapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        7 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements_webpyapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      873 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/tornadoapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      197 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/webpyapp.py
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      215 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/gunicorn_rc
+-rw-r--r--   0 benoitc    (501) staff       (20)       13 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/hello.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      448 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/log_app.ini
+-rw-r--r--   0 benoitc    (501) staff       (20)      372 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/log_app.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      841 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/logging.conf
+-rw-r--r--   0 benoitc    (501) staff       (20)      737 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/longpoll.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1470 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/multiapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      993 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/multidomainapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1980 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/nginx.conf
+-rw-r--r--   0 benoitc    (501) staff       (20)      403 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/read_django_settings.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1015 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/readline_app.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      584 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/sendfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1257 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/server.crt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1679 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/server.key
+-rw-r--r--   0 benoitc    (501) staff       (20)      604 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/slowclient.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1339 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/standalone_app.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      182 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/supervisor.conf
+-rw-r--r--   0 benoitc    (501) staff       (20)      659 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/test.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      620 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/timeout.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.028963 gunicorn-21.0.0/examples/websocket/
+-rw-r--r--   0 benoitc    (501) staff       (20)    15684 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/websocket/gevent_websocket.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1320 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/websocket/websocket.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    15729 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/websocket/websocket.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1020 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/when_ready.conf.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.030196 gunicorn-21.0.0/gunicorn/
+-rw-r--r--   0 benoitc    (501) staff       (20)      279 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      171 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/__main__.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.031323 gunicorn-21.0.0/gunicorn/app/
+-rw-r--r--   0 benoitc    (501) staff       (20)      127 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/app/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7400 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/app/base.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2038 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/app/pasterapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1926 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/app/wsgiapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    21509 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/arbiter.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    63419 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/config.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2293 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/debug.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      919 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/errors.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    15303 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/glogging.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.031999 gunicorn-21.0.0/gunicorn/http/
+-rw-r--r--   0 benoitc    (501) staff       (20)      277 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7296 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/body.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2850 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/errors.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    11958 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/message.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1364 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/parser.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1943 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/unreader.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    12366 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/wsgi.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.032179 gunicorn-21.0.0/gunicorn/instrument/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/instrument/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4690 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/instrument/statsd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2367 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/pidfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     3791 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/reloader.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6887 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/sock.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2520 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/systemd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    19104 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/util.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.033039 gunicorn-21.0.0/gunicorn/workers/
+-rw-r--r--   0 benoitc    (501) staff       (20)      594 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     9197 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/base.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5681 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/base_async.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6091 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/geventlet.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5800 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/ggevent.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    12585 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/gthread.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5854 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/gtornado.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7272 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/sync.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1651 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/workertmp.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.030921 gunicorn-21.0.0/gunicorn.egg-info/
+-rw-r--r--   0 benoitc    (501) staff       (20)     3852 2023-07-17 20:28:18.000000 gunicorn-21.0.0/gunicorn.egg-info/PKG-INFO
+-rw-r--r--   0 benoitc    (501) staff       (20)     9249 2023-07-17 20:28:19.000000 gunicorn-21.0.0/gunicorn.egg-info/SOURCES.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        1 2023-07-17 20:28:18.000000 gunicorn-21.0.0/gunicorn.egg-info/dependency_links.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      113 2023-07-17 20:28:18.000000 gunicorn-21.0.0/gunicorn.egg-info/entry_points.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        1 2023-07-17 20:27:30.000000 gunicorn-21.0.0/gunicorn.egg-info/not-zip-safe
+-rw-r--r--   0 benoitc    (501) staff       (20)      173 2023-07-17 20:28:18.000000 gunicorn-21.0.0/gunicorn.egg-info/requires.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        9 2023-07-17 20:28:18.000000 gunicorn-21.0.0/gunicorn.egg-info/top_level.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)       50 2023-07-17 19:03:36.000000 gunicorn-21.0.0/requirements_dev.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)       56 2023-07-17 19:20:23.000000 gunicorn-21.0.0/requirements_test.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      203 2023-07-17 20:28:19.048669 gunicorn-21.0.0/setup.cfg
+-rw-r--r--   0 benoitc    (501) staff       (20)     3555 2023-07-17 19:03:36.000000 gunicorn-21.0.0/setup.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.034618 gunicorn-21.0.0/tests/
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.035095 gunicorn-21.0.0/tests/config/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/config/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       88 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/config/test_cfg.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       24 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/config/test_cfg_alt.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       23 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/config/test_cfg_with_wsgi_app.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.014457 gunicorn-21.0.0/tests/requests/
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.041274 gunicorn-21.0.0/tests/requests/invalid/
+-rw-r--r--   0 benoitc    (501) staff       (20)       29 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/001.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       64 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/001.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       21 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/002.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/002.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       30 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/003.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       84 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/003.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       25 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/004.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       80 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/004.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       41 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/005.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       78 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/005.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4122 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/006.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       77 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/006.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     8358 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/007.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/007.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    12418 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/008.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/008.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1829 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/009.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/009.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       44 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/010.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/010.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/011.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/011.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/012.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/012.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       49 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/013.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/013.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       78 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/014.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       72 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/014.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       88 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/015.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       72 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/015.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       33 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/016.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       82 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/016.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     8222 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/017.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      134 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/017.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       48 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/018.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/018.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       82 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/019.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      172 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/019.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       69 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/020.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      130 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/020.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       90 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/021.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/021.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/022.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/022.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       52 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/023.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/023.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/024.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/024.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       37 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/pp_01.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      161 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/pp_01.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       53 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/pp_02.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      161 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/pp_02.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.047965 gunicorn-21.0.0/tests/requests/valid/
+-rw-r--r--   0 benoitc    (501) staff       (20)      149 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/001.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      275 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/001.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      168 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/002.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      296 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/002.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      394 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/003.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/003.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       57 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/004.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      164 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/004.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       62 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/005.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      153 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/005.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/006.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      142 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/006.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       61 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/007.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      167 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/007.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       73 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/008.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      178 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/008.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      137 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/009.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      264 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/009.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      134 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/010.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      218 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/010.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      125 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/011.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      196 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/011.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      166 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/012.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      285 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/012.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      159 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/013.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      192 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/013.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       46 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/014.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      137 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/014.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       98 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/015.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      226 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/015.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2234 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/016.http
+-rw-r--r--   0 benoitc    (501) staff       (20)     2376 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/016.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       91 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/017.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      207 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/017.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       58 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/018.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      258 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/018.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       58 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/019.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      119 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/019.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/020.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      171 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/020.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       80 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/021.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      142 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/021.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       85 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/022.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      286 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/022.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      155 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/023.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      335 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/023.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    16408 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/024.http
+-rw-r--r--   0 benoitc    (501) staff       (20)    16639 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/024.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      364 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/025.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      476 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/025.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     8233 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/026.http
+-rw-r--r--   0 benoitc    (501) staff       (20)     8463 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/026.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       30 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/027.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      130 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/027.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       68 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/028.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      261 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/028.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      129 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/029.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      278 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/029.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      129 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/030.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      278 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/030.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     9909 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/099.http
+-rw-r--r--   0 benoitc    (501) staff       (20)     9135 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/099.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       41 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/100.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      131 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/100.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      199 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/pp_01.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      359 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/pp_01.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      361 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/pp_02.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      639 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/pp_02.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1745 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/support.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1614 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/t.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6110 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_arbiter.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    14360 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_config.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6853 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_http.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      597 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_invalid_requests.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     3140 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_logger.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1522 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_pidfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1851 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_reload.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1875 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_sock.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2013 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_ssl.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4818 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_statsd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2049 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_systemd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4367 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_util.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      608 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_valid_requests.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     9434 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/treq.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.048242 gunicorn-21.0.0/tests/workers/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/workers/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      192 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/workers/test_geventlet.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      190 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/workers/test_ggevent.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gunicorn-20.1.0/gunicorn.egg-info/SOURCES.txt` & `gunicorn-21.0.0/gunicorn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 docs/source/2015-news.rst
 docs/source/2016-news.rst
 docs/source/2017-news.rst
 docs/source/2018-news.rst
 docs/source/2019-news.rst
 docs/source/2020-news.rst
 docs/source/2021-news.rst
+docs/source/2023-news.rst
 docs/source/community.rst
 docs/source/conf.py
 docs/source/configure.rst
 docs/source/custom.rst
 docs/source/deploy.rst
 docs/source/design.rst
 docs/source/faq.rst
@@ -237,14 +238,20 @@
 tests/requests/invalid/018.py
 tests/requests/invalid/019.http
 tests/requests/invalid/019.py
 tests/requests/invalid/020.http
 tests/requests/invalid/020.py
 tests/requests/invalid/021.http
 tests/requests/invalid/021.py
+tests/requests/invalid/022.http
+tests/requests/invalid/022.py
+tests/requests/invalid/023.http
+tests/requests/invalid/023.py
+tests/requests/invalid/024.http
+tests/requests/invalid/024.py
 tests/requests/invalid/pp_01.http
 tests/requests/invalid/pp_01.py
 tests/requests/invalid/pp_02.http
 tests/requests/invalid/pp_02.py
 tests/requests/valid/001.http
 tests/requests/valid/001.py
 tests/requests/valid/002.http
```

### Comparing `gunicorn-20.1.0/LICENSE` & `gunicorn-21.0.0/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-2009-2018 (c) Benoît Chesneau <benoitc@e-engura.org>
+2009-2023 (c) Benoît Chesneau <benoitc@gunicorn.org>
 2009-2015 (c) Paul J. Davis <paul.joseph.davis@gmail.com>
 
 Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation
 files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `gunicorn-20.1.0/tests/test_invalid_requests.py` & `gunicorn-21.0.0/tests/test_invalid_requests.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/support.py` & `gunicorn-21.0.0/tests/support.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/test_statsd.py` & `gunicorn-21.0.0/tests/test_statsd.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,26 @@
     logger.debug("No impact on logging")
     logger.critical("No impact on logging")
     logger.error("No impact on logging")
     logger.warning("No impact on logging")
     logger.exception("No impact on logging")
 
 
+def test_statsd_host_initialization():
+    c = Config()
+    c.set('statsd_host', 'unix:test.sock')
+    logger = Statsd(c)
+    logger.info("Can be initialized and used with a UDS socket")
+
+    # Can be initialized and used with a UDP address
+    c.set('statsd_host', 'host:8080')
+    logger = Statsd(c)
+    logger.info("Can be initialized and used with a UDP socket")
+
+
 def test_dogstatsd_tags():
     c = Config()
     tags = 'yucatan,libertine:rhubarb'
     c.set('dogstatsd_tags', tags)
     logger = Statsd(c)
     logger.sock = MockSocket(False)
     logger.info("Twill", extra={"mtype": "gauge", "metric": "barb.westerly",
```

### Comparing `gunicorn-20.1.0/tests/test_pidfile.py` & `gunicorn-21.0.0/tests/test_pidfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -
 #
 # This file is part of gunicorn released under the MIT license.
 # See the NOTICE for more information.
 
 import errno
-import unittest.mock as mock
+from unittest import mock
 
 import gunicorn.pidfile
 
 
 def builtin(name):
     return 'builtins.{}'.format(name)
```

### Comparing `gunicorn-20.1.0/tests/test_systemd.py` & `gunicorn-21.0.0/tests/test_systemd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -
 #
 # This file is part of gunicorn released under the MIT license.
 # See the NOTICE for more information.
 
 from contextlib import contextmanager
 import os
-import unittest.mock as mock
+from unittest import mock
 
 import pytest
 
 from gunicorn import systemd
 
 
 @contextmanager
```

### Comparing `gunicorn-20.1.0/tests/test_util.py` & `gunicorn-21.0.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/valid/026.http` & `gunicorn-21.0.0/tests/requests/valid/026.http`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/valid/026.py` & `gunicorn-21.0.0/tests/requests/valid/026.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/valid/016.py` & `gunicorn-21.0.0/tests/requests/valid/016.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/valid/016.http` & `gunicorn-21.0.0/tests/requests/valid/016.http`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/valid/099.http` & `gunicorn-21.0.0/tests/requests/valid/099.http`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/valid/003.py` & `gunicorn-21.0.0/tests/requests/valid/003.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/valid/024.py` & `gunicorn-21.0.0/tests/requests/valid/024.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/valid/pp_02.py` & `gunicorn-21.0.0/tests/requests/valid/pp_02.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/valid/024.http` & `gunicorn-21.0.0/tests/requests/valid/024.http`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/valid/099.py` & `gunicorn-21.0.0/tests/requests/valid/099.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/invalid/006.http` & `gunicorn-21.0.0/tests/requests/invalid/006.http`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/invalid/007.http` & `gunicorn-21.0.0/tests/requests/invalid/007.http`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/invalid/017.http` & `gunicorn-21.0.0/tests/requests/invalid/017.http`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/invalid/008.http` & `gunicorn-21.0.0/tests/requests/invalid/008.http`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/requests/invalid/009.http` & `gunicorn-21.0.0/tests/requests/invalid/009.http`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/test_arbiter.py` & `gunicorn-21.0.0/tests/test_arbiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -
 #
 # This file is part of gunicorn released under the MIT license.
 # See the NOTICE for more information.
 
 import os
-import unittest.mock as mock
+from unittest import mock
 
 import gunicorn.app.base
 import gunicorn.arbiter
 from gunicorn.config import ReusePort
 
 
 class DummyApplication(gunicorn.app.base.BaseApplication):
```

### Comparing `gunicorn-20.1.0/tests/treq.py` & `gunicorn-21.0.0/tests/treq.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/test_ssl.py` & `gunicorn-21.0.0/tests/test_ssl.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # This file is part of gunicorn released under the MIT license.
 # See the NOTICE for more information.
 
 import pytest
 
 from gunicorn.config import (
-    KeyFile, CertFile, SSLVersion, CACerts, SuppressRaggedEOFs,
+    KeyFile, CertFile, CACerts, SuppressRaggedEOFs,
     DoHandshakeOnConnect, Setting, Ciphers,
 )
 
 ssl = pytest.importorskip('ssl')
 
 
 def test_keyfile():
@@ -28,22 +28,14 @@
     assert issubclass(CertFile, Setting)
     assert CertFile.name == 'certfile'
     assert CertFile.section == 'SSL'
     assert CertFile.cli == ['--certfile']
     assert CertFile.default is None
 
 
-def test_ssl_version():
-    assert issubclass(SSLVersion, Setting)
-    assert SSLVersion.name == 'ssl_version'
-    assert SSLVersion.section == 'SSL'
-    assert SSLVersion.cli == ['--ssl-version']
-    assert SSLVersion.default == ssl.PROTOCOL_SSLv23
-
-
 def test_cacerts():
     assert issubclass(CACerts, Setting)
     assert CACerts.name == 'ca_certs'
     assert CACerts.section == 'SSL'
     assert CACerts.cli == ['--ca-certs']
     assert CACerts.meta == 'FILE'
     assert CACerts.default is None
```

### Comparing `gunicorn-20.1.0/tests/test_http.py` & `gunicorn-21.0.0/tests/test_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- encoding: utf-8 -*-
 
 import io
 import t
 import pytest
-import unittest.mock as mock
+from unittest import mock
 
 from gunicorn import util
 from gunicorn.http.body import Body, LengthReader, EOFReader
 from gunicorn.http.wsgi import Response
 from gunicorn.http.unreader import Unreader, IterUnreader, SocketUnreader
 from gunicorn.http.errors import InvalidHeader, InvalidHeaderName
```

### Comparing `gunicorn-20.1.0/tests/test_sock.py` & `gunicorn-21.0.0/tests/test_sock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -
 #
 # This file is part of gunicorn released under the MIT license.
 # See the NOTICE for more information.
 
-import unittest.mock as mock
+from unittest import mock
 
 from gunicorn import sock
 
 
 @mock.patch('os.stat')
 def test_create_sockets_unix_bytes(stat):
     conf = mock.Mock(address=[b'127.0.0.1:8000'])
```

### Comparing `gunicorn-20.1.0/tests/test_valid_requests.py` & `gunicorn-21.0.0/tests/test_valid_requests.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/test_config.py` & `gunicorn-21.0.0/tests/test_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -314,14 +314,38 @@
     def nworkers_changed_3(server, new_value, old_value):
         return 3
 
     c.set("nworkers_changed", nworkers_changed_3)
     assert c.nworkers_changed(1, 2, 3) == 3
 
 
+def test_statsd_host():
+    c = config.Config()
+    assert c.statsd_host is None
+    c.set("statsd_host", "localhost")
+    assert c.statsd_host == ("localhost", 8125)
+    c.set("statsd_host", "statsd:7777")
+    assert c.statsd_host == ("statsd", 7777)
+    c.set("statsd_host", "unix:///path/to.sock")
+    assert c.statsd_host == "/path/to.sock"
+    pytest.raises(TypeError, c.set, "statsd_host", 666)
+    pytest.raises(TypeError, c.set, "statsd_host", "host:string")
+
+
+def test_statsd_host_with_unix_as_hostname():
+    # This is a regression test for major release 20. After this release
+    # we should consider modifying the behavior of util.parse_address to
+    # simplify gunicorn's code
+    c = config.Config()
+    c.set("statsd_host", "unix:7777")
+    assert c.statsd_host == ("unix", 7777)
+    c.set("statsd_host", "unix://some.socket")
+    assert c.statsd_host == "some.socket"
+
+
 def test_statsd_changes_logger():
     c = config.Config()
     assert c.logger_class == glogging.Logger
     c.set('statsd_host', 'localhost:12345')
     assert c.logger_class == statsd.Statsd
 
 
@@ -425,49 +449,14 @@
     cmdline = ["prog_name"]
     cmdline.extend(options)
     with AltArgs(cmdline):
         app = NoConfigApp()
     assert app.cfg.umask == expected
 
 
-@pytest.mark.parametrize("options, expected", [
-    (["--ssl-version", "SSLv23"], 2),
-    (["--ssl-version", "TLSv1"], 3),
-    (["--ssl-version", "2"], 2),
-    (["--ssl-version", "3"], 3),
-])
-def test_ssl_version_named_constants_python3(options, expected):
-    _test_ssl_version(options, expected)
-
-
-@pytest.mark.skipif(sys.version_info < (3, 6),
-    reason="requires python3.6+")
-@pytest.mark.parametrize("options, expected", [
-    (["--ssl-version", "TLS"], 2),
-    (["--ssl-version", "TLSv1_1"], 4),
-    (["--ssl-version", "TLSv1_2"], 5),
-    (["--ssl-version", "TLS_SERVER"], 17),
-])
-def test_ssl_version_named_constants_python36(options, expected):
-    _test_ssl_version(options, expected)
-
-
-@pytest.mark.parametrize("ssl_version", [
-    "FOO",
-    "-99",
-    "99991234"
-])
-def test_ssl_version_bad(ssl_version):
-    c = config.Config()
-    with pytest.raises(ValueError) as exc:
-        c.set("ssl_version", ssl_version)
-    assert 'Valid options' in str(exc.value)
-    assert "TLSv" in str(exc.value)
-
-
 def _test_ssl_version(options, expected):
     cmdline = ["prog_name"]
     cmdline.extend(options)
     with AltArgs(cmdline):
         app = NoConfigApp()
     assert app.cfg.ssl_version == expected
```

### Comparing `gunicorn-20.1.0/tests/test_reload.py` & `gunicorn-21.0.0/tests/test_reload.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/t.py` & `gunicorn-21.0.0/tests/t.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/tests/test_logger.py` & `gunicorn-21.0.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/gunicorn/pidfile.py` & `gunicorn-21.0.0/gunicorn/pidfile.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/gunicorn/reloader.py` & `gunicorn-21.0.0/gunicorn/reloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 COMPILED_EXT_RE = re.compile(r'py[co]$')
 
 
 class Reloader(threading.Thread):
     def __init__(self, extra_files=None, interval=1, callback=None):
         super().__init__()
-        self.setDaemon(True)
+        self.daemon = True
         self._extra_files = set(extra_files or ())
         self._interval = interval
         self._callback = callback
 
     def add_extra_file(self, filename):
         self._extra_files.add(filename)
 
@@ -70,15 +70,15 @@
         event_mask = (inotify.constants.IN_CREATE | inotify.constants.IN_DELETE
                       | inotify.constants.IN_DELETE_SELF | inotify.constants.IN_MODIFY
                       | inotify.constants.IN_MOVE_SELF | inotify.constants.IN_MOVED_FROM
                       | inotify.constants.IN_MOVED_TO)
 
         def __init__(self, extra_files=None, callback=None):
             super().__init__()
-            self.setDaemon(True)
+            self.daemon = True
             self._callback = callback
             self._dirs = set()
             self._watcher = Inotify()
 
             for extra_file in extra_files:
                 self.add_extra_file(extra_file)
 
@@ -114,15 +114,15 @@
                 filename = event[3]
 
                 self._callback(filename)
 
 else:
 
     class InotifyReloader(object):
-        def __init__(self, callback=None):
+        def __init__(self, extra_files=None, callback=None):
             raise ImportError('You must have the inotify module installed to '
                               'use the inotify reloader')
 
 
 preferred_reloader = InotifyReloader if has_inotify else Reloader
 
 reloader_engines = {
```

### Comparing `gunicorn-20.1.0/gunicorn/config.py` & `gunicorn-21.0.0/gunicorn/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     @property
     def worker_class_str(self):
         uri = self.settings['worker_class'].get()
 
         # are we using a threaded worker?
         is_sync = uri.endswith('SyncWorker') or uri == 'sync'
         if is_sync and self.threads > 1:
-            return "threads"
+            return "gthread"
         return uri
 
     @property
     def worker_class(self):
         uri = self.settings['worker_class'].get()
 
         # are we using a threaded worker?
@@ -360,33 +360,17 @@
         val = int(val)
     if val < 0:
         raise ValueError("Value must be positive: %s" % val)
     return val
 
 
 def validate_ssl_version(val):
-    ssl_versions = {}
-    for protocol in [p for p in dir(ssl) if p.startswith("PROTOCOL_")]:
-        ssl_versions[protocol[9:]] = getattr(ssl, protocol)
-    if val in ssl_versions:
-        # string matching PROTOCOL_...
-        return ssl_versions[val]
-
-    try:
-        intval = validate_pos_int(val)
-        if intval in ssl_versions.values():
-            # positive int matching a protocol int constant
-            return intval
-    except (ValueError, TypeError):
-        # negative integer or not an integer
-        # drop this in favour of the more descriptive ValueError below
-        pass
-
-    raise ValueError("Invalid ssl_version: %s. Valid options: %s"
-                     % (val, ', '.join(ssl_versions)))
+    if val != SSLVersion.default:
+        sys.stderr.write("Warning: option `ssl_version` is deprecated and it is ignored. Use ssl_context instead.\n")
+    return val
 
 
 def validate_string(val):
     if val is None:
         return None
     if not isinstance(val, str):
         raise TypeError("Not a string: %s" % val)
@@ -444,15 +428,15 @@
             try:
                 mod = __import__(mod_name, fromlist=[obj_name])
                 val = getattr(mod, obj_name)
             except ImportError as e:
                 raise TypeError(str(e))
             except AttributeError:
                 raise TypeError("Can not load '%s' from '%s'"
-                    "" % (obj_name, mod_name))
+                                "" % (obj_name, mod_name))
         if not callable(val):
             raise TypeError("Value is not callable: %s" % val)
         if arity != -1 and arity != util.get_arity(val):
             raise TypeError("Value must have an arity of: %s" % arity)
         return val
     return _validate_callable
 
@@ -510,23 +494,33 @@
     # test if the path exists
     if not os.path.exists(path):
         raise ConfigError("can't chdir to %r" % val)
 
     return path
 
 
-def validate_hostport(val):
+def validate_statsd_address(val):
     val = validate_string(val)
     if val is None:
         return None
-    elements = val.split(":")
-    if len(elements) == 2:
-        return (elements[0], int(elements[1]))
-    else:
-        raise TypeError("Value must consist of: hostname:port")
+
+    # As of major release 20, util.parse_address would recognize unix:PORT
+    # as a UDS address, breaking backwards compatibility. We defend against
+    # that regression here (this is also unit-tested).
+    # Feel free to remove in the next major release.
+    unix_hostname_regression = re.match(r'^unix:(\d+)$', val)
+    if unix_hostname_regression:
+        return ('unix', int(unix_hostname_regression.group(1)))
+
+    try:
+        address = util.parse_address(val, default_port='8125')
+    except RuntimeError:
+        raise TypeError("Value must be one of ('host:port', 'unix://PATH')")
+
+    return address
 
 
 def validate_reload_engine(val):
     if val not in reloader_engines:
         raise ConfigError("Invalid reload_engine: %r" % val)
 
     return val
@@ -544,41 +538,43 @@
     name = "config"
     section = "Config File"
     cli = ["-c", "--config"]
     meta = "CONFIG"
     validator = validate_string
     default = "./gunicorn.conf.py"
     desc = """\
-        The Gunicorn config file.
+        :ref:`The Gunicorn config file<configuration_file>`.
 
         A string of the form ``PATH``, ``file:PATH``, or ``python:MODULE_NAME``.
 
         Only has an effect when specified on the command line or as part of an
         application specific configuration.
 
         By default, a file named ``gunicorn.conf.py`` will be read from the same
         directory where gunicorn is being run.
 
         .. versionchanged:: 19.4
            Loading the config from a Python module requires the ``python:``
            prefix.
         """
 
+
 class WSGIApp(Setting):
     name = "wsgi_app"
     section = "Config File"
     meta = "STRING"
     validator = validate_string
     default = None
     desc = """\
         A WSGI application path in pattern ``$(MODULE_NAME):$(VARIABLE_NAME)``.
 
         .. versionadded:: 20.1.0
         """
 
+
 class Bind(Setting):
     name = "bind"
     action = "append"
     section = "Server Socket"
     cli = ["-b", "--bind"]
     meta = "ADDRESS"
     validator = validate_list_string
@@ -720,15 +716,15 @@
     meta = "INT"
     validator = validate_pos_int
     type = int
     default = 1000
     desc = """\
         The maximum number of simultaneous clients.
 
-        This setting only affects the Eventlet and Gevent worker types.
+        This setting only affects the ``gthread``, ``eventlet`` and ``gevent`` worker types.
         """
 
 
 class MaxRequests(Setting):
     name = "max_requests"
     section = "Worker Processes"
     cli = ["--max-requests"]
@@ -1050,14 +1046,15 @@
 
 class Chdir(Setting):
     name = "chdir"
     section = "Server Mechanics"
     cli = ["--chdir"]
     validator = validate_chdir
     default = util.getcwd()
+    default_doc = "``'.'``"
     desc = """\
         Change directory to specified directory before loading apps.
         """
 
 
 class Daemon(Setting):
     name = "daemon"
@@ -1141,14 +1138,15 @@
 class User(Setting):
     name = "user"
     section = "Server Mechanics"
     cli = ["-u", "--user"]
     meta = "USER"
     validator = validate_user
     default = os.geteuid()
+    default_doc = "``os.geteuid()``"
     desc = """\
         Switch worker processes to run as this user.
 
         A valid user id (as an integer) or the name of a user that can be
         retrieved with a call to ``pwd.getpwnam(value)`` or ``None`` to not
         change the worker process user.
         """
@@ -1157,14 +1155,15 @@
 class Group(Setting):
     name = "group"
     section = "Server Mechanics"
     cli = ["-g", "--group"]
     meta = "GROUP"
     validator = validate_group
     default = os.getegid()
+    default_doc = "``os.getegid()``"
     desc = """\
         Switch worker process to run as this group.
 
         A valid group id (as an integer) or the name of a user that can be
         retrieved with a call to ``pwd.getgrnam(value)`` or ``None`` to not
         change the worker processes group.
         """
@@ -1232,18 +1231,24 @@
         "X-FORWARDED-PROTOCOL": "ssl",
         "X-FORWARDED-PROTO": "https",
         "X-FORWARDED-SSL": "on"
     }
     desc = """\
 
         A dictionary containing headers and values that the front-end proxy
-        uses to indicate HTTPS requests. These tell Gunicorn to set
+        uses to indicate HTTPS requests. If the source IP is permitted by
+        ``forwarded-allow-ips`` (below), *and* at least one request header matches
+        a key-value pair listed in this dictionary, then Gunicorn will set
         ``wsgi.url_scheme`` to ``https``, so your application can tell that the
         request is secure.
 
+        If the other headers listed in this dictionary are not present in the request, they will be ignored,
+        but if the other headers are present and do not match the provided values, then
+        the request will fail to parse. See the note below for more detailed examples of this behaviour.
+
         The dictionary should map upper-case header names to exact string
         values. The value comparisons are case-sensitive, unlike the header
         names, so make sure they're exactly what your front-end proxy sends
         when handling HTTPS requests.
 
         It is important that your front-end proxy configuration ensures that
         the headers defined here can not be passed directly from the client.
@@ -1263,14 +1268,79 @@
 
         Set to ``*`` to disable checking of Front-end IPs (useful for setups
         where you don't know in advance the IP address of Front-end, but
         you still trust the environment).
 
         By default, the value of the ``FORWARDED_ALLOW_IPS`` environment
         variable. If it is not defined, the default is ``"127.0.0.1"``.
+
+        .. note::
+
+            The interplay between the request headers, the value of ``forwarded_allow_ips``, and the value of
+            ``secure_scheme_headers`` is complex. Various scenarios are documented below to further elaborate.
+            In each case, we have a request from the remote address 134.213.44.18, and the default value of
+            ``secure_scheme_headers``:
+
+            .. code::
+
+                secure_scheme_headers = {
+                    'X-FORWARDED-PROTOCOL': 'ssl',
+                    'X-FORWARDED-PROTO': 'https',
+                    'X-FORWARDED-SSL': 'on'
+                }
+
+
+            .. list-table::
+                :header-rows: 1
+                :align: center
+                :widths: auto
+
+                * - ``forwarded-allow-ips``
+                  - Secure Request Headers
+                  - Result
+                  - Explanation
+                * - .. code::
+
+                        ["127.0.0.1"]
+                  - .. code::
+
+                        X-Forwarded-Proto: https
+                  - .. code::
+
+                        wsgi.url_scheme = "http"
+                  - IP address was not allowed
+                * - .. code::
+
+                        "*"
+                  - <none>
+                  - .. code::
+
+                        wsgi.url_scheme = "http"
+                  - IP address allowed, but no secure headers provided
+                * - .. code::
+
+                        "*"
+                  - .. code::
+
+                        X-Forwarded-Proto: https
+                  - .. code::
+
+                        wsgi.url_scheme = "https"
+                  - IP address allowed, one request header matched
+                * - .. code::
+
+                        ["134.213.44.18"]
+                  - .. code::
+
+                        X-Forwarded-Ssl: on
+                        X-Forwarded-Proto: http
+                  - ``InvalidSchemeHeaders()`` raised
+                  - IP address allowed, but the two secure headers disagreed on if HTTPS was used
+
+
         """
 
 
 class AccessLog(Setting):
     name = "accesslog"
     section = "Logging"
     cli = ["--access-logfile"]
@@ -1430,23 +1500,43 @@
     name = "logconfig_dict"
     section = "Logging"
     validator = validate_dict
     default = {}
     desc = """\
     The log config dictionary to use, using the standard Python
     logging module's dictionary configuration format. This option
-    takes precedence over the :ref:`logconfig` option, which uses the
-    older file configuration format.
+    takes precedence over the :ref:`logconfig` and :ref:`logConfigJson` options,
+    which uses the older file configuration format and JSON
+    respectively.
 
     Format: https://docs.python.org/3/library/logging.config.html#logging.config.dictConfig
 
+    For more context you can look at the default configuration dictionary for logging,
+    which can be found at ``gunicorn.glogging.CONFIG_DEFAULTS``.
+
     .. versionadded:: 19.8
     """
 
 
+class LogConfigJson(Setting):
+    name = "logconfig_json"
+    section = "Logging"
+    cli = ["--log-config-json"]
+    meta = "FILE"
+    validator = validate_string
+    default = None
+    desc = """\
+    The log config to read config from a JSON file
+
+    Format: https://docs.python.org/3/library/logging.config.html#logging.config.jsonConfig
+
+    .. versionadded:: 20.0
+    """
+
+
 class SyslogTo(Setting):
     name = "syslog_addr"
     section = "Logging"
     cli = ["--log-syslog-to"]
     meta = "SYSLOG_ADDR"
     validator = validate_string
 
@@ -1536,21 +1626,27 @@
 # statsD monitoring
 class StatsdHost(Setting):
     name = "statsd_host"
     section = "Logging"
     cli = ["--statsd-host"]
     meta = "STATSD_ADDR"
     default = None
-    validator = validate_hostport
+    validator = validate_statsd_address
     desc = """\
-    ``host:port`` of the statsd server to log to.
+    The address of the StatsD server to log to.
+
+    Address is a string of the form:
+
+    * ``unix://PATH`` : for a unix domain socket.
+    * ``HOST:PORT`` : for a network address
 
     .. versionadded:: 19.1
     """
 
+
 # Datadog Statsd (dogstatsd) tags. https://docs.datadoghq.com/developers/dogstatsd/
 class DogstatsdTags(Setting):
     name = "dogstatsd_tags"
     section = "Logging"
     cli = ["--dogstatsd-tags"]
     meta = "DOGSTATSD_TAGS"
     default = ""
@@ -1558,14 +1654,15 @@
     desc = """\
     A comma-delimited list of datadog statsd (dogstatsd) tags to append to
     statsd metrics.
 
     .. versionadded:: 20
     """
 
+
 class StatsdPrefix(Setting):
     name = "statsd_prefix"
     section = "Logging"
     cli = ["--statsd-prefix"]
     meta = "STATSD_PREFIX"
     default = ""
     validator = validate_string
@@ -1795,15 +1892,15 @@
 class PreRequest(Setting):
     name = "pre_request"
     section = "Server Hooks"
     validator = validate_callable(2)
     type = callable
 
     def pre_request(worker, req):
-        worker.log.debug("%s %s" % (req.method, req.path))
+        worker.log.debug("%s %s", req.method, req.path)
     default = staticmethod(pre_request)
     desc = """\
         Called just before a worker processes the request.
 
         The callable needs to accept two instance variables for the Worker and
         the Request.
         """
@@ -1894,14 +1991,49 @@
     desc = """\
         Called just before exiting Gunicorn.
 
         The callable needs to accept a single instance variable for the Arbiter.
         """
 
 
+class NewSSLContext(Setting):
+    name = "ssl_context"
+    section = "Server Hooks"
+    validator = validate_callable(2)
+    type = callable
+
+    def ssl_context(config, default_ssl_context_factory):
+        return default_ssl_context_factory()
+
+    default = staticmethod(ssl_context)
+    desc = """\
+        Called when SSLContext is needed.
+
+        Allows customizing SSL context.
+
+        The callable needs to accept an instance variable for the Config and
+        a factory function that returns default SSLContext which is initialized
+        with certificates, private key, cert_reqs, and ciphers according to
+        config and can be further customized by the callable.
+        The callable needs to return SSLContext object.
+
+        Following example shows a configuration file that sets the minimum TLS version to 1.3:
+
+        .. code-block:: python
+
+            def ssl_context(conf, default_ssl_context_factory):
+                import ssl
+                context = default_ssl_context_factory()
+                context.minimum_version = ssl.TLSVersion.TLSv1_3
+                return context
+
+        .. versionadded:: 20.2
+        """
+
+
 class ProxyProtocol(Setting):
     name = "proxy_protocol"
     section = "Server Mechanics"
     cli = ["--proxy-protocol"]
     validator = validate_bool
     default = False
     action = "store_true"
@@ -1970,25 +2102,20 @@
     validator = validate_ssl_version
 
     if hasattr(ssl, "PROTOCOL_TLS"):
         default = ssl.PROTOCOL_TLS
     else:
         default = ssl.PROTOCOL_SSLv23
 
-    desc = """\
-    SSL version to use (see stdlib ssl module's)
-
-    .. versionchanged:: 20.0.1
-       The default value has been changed from ``ssl.PROTOCOL_SSLv23`` to
-       ``ssl.PROTOCOL_TLS`` when Python >= 3.6 .
-
-    """
     default = ssl.PROTOCOL_SSLv23
     desc = """\
-    SSL version to use.
+    SSL version to use (see stdlib ssl module's).
+
+    .. deprecated:: 20.2
+       The option is deprecated and it is currently ignored. Use :ref:`ssl-context` instead.
 
     ============= ============
     --ssl-version Description
     ============= ============
     SSLv3         SSLv3 is not-secure and is strongly discouraged.
     SSLv23        Alias for TLS. Deprecated in Python 3.6, use TLS.
     TLS           Negotiate highest possible version between client/server.
@@ -2003,25 +2130,36 @@
 
     .. versionchanged:: 19.7
        The default value has been changed from ``ssl.PROTOCOL_TLSv1`` to
        ``ssl.PROTOCOL_SSLv23``.
     .. versionchanged:: 20.0
        This setting now accepts string names based on ``ssl.PROTOCOL_``
        constants.
+    .. versionchanged:: 20.0.1
+       The default value has been changed from ``ssl.PROTOCOL_SSLv23`` to
+       ``ssl.PROTOCOL_TLS`` when Python >= 3.6 .
     """
 
 
 class CertReqs(Setting):
     name = "cert_reqs"
     section = "SSL"
     cli = ["--cert-reqs"]
     validator = validate_pos_int
     default = ssl.CERT_NONE
     desc = """\
     Whether client certificate is required (see stdlib ssl module's)
+
+    ===========  ===========================
+    --cert-reqs      Description
+    ===========  ===========================
+    `0`          no client veirifcation
+    `1`          ssl.CERT_OPTIONAL
+    `2`          ssl.CERT_REQUIRED
+    ===========  ===========================
     """
 
 
 class CACerts(Setting):
     name = "ca_certs"
     section = "SSL"
     cli = ["--ca-certs"]
```

### Comparing `gunicorn-20.1.0/gunicorn/app/wsgiapp.py` & `gunicorn-21.0.0/gunicorn/app/wsgiapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/gunicorn/app/pasterapp.py` & `gunicorn-21.0.0/gunicorn/app/pasterapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/gunicorn/app/base.py` & `gunicorn-21.0.0/gunicorn/app/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,19 @@
                 sys.exit(1)
             sys.exit(0)
 
         if self.cfg.spew:
             debug.spew()
 
         if self.cfg.daemon:
+            if os.environ.get('NOTIFY_SOCKET'):
+                msg = "Warning: you shouldn't specify `daemon = True`" \
+                      " when launching by systemd with `Type = notify`"
+                print(msg, file=sys.stderr, flush=True)
+
             util.daemonize(self.cfg.enable_stdio_inheritance)
 
         # set python paths
         if self.cfg.pythonpath:
             paths = self.cfg.pythonpath.split(",")
             for path in paths:
                 pythonpath = os.path.abspath(path)
```

### Comparing `gunicorn-20.1.0/gunicorn/instrument/statsd.py` & `gunicorn-21.0.0/gunicorn/instrument/statsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,25 @@
 HISTOGRAM_TYPE = "histogram"
 
 
 class Statsd(Logger):
     """statsD-based instrumentation, that passes as a logger
     """
     def __init__(self, cfg):
-        """host, port: statsD server
-        """
         Logger.__init__(self, cfg)
         self.prefix = sub(r"^(.+[^.]+)\.*$", "\\g<1>.", cfg.statsd_prefix)
+
+        if isinstance(cfg.statsd_host, str):
+            address_family = socket.AF_UNIX
+        else:
+            address_family = socket.AF_INET
+
         try:
-            host, port = cfg.statsd_host
-            self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-            self.sock.connect((host, int(port)))
+            self.sock = socket.socket(address_family, socket.SOCK_DGRAM)
+            self.sock.connect(cfg.statsd_host)
         except Exception:
             self.sock = None
 
         self.dogstatsd_tags = cfg.dogstatsd_tags
 
     # Log errors and warnings
     def critical(self, msg, *args, **kwargs):
```

### Comparing `gunicorn-20.1.0/gunicorn/util.py` & `gunicorn-21.0.0/gunicorn/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 import socket
 import sys
 import textwrap
 import time
 import traceback
 import warnings
 
-import pkg_resources
+try:
+    import importlib.metadata as importlib_metadata
+except ImportError:
+    import importlib_metadata
 
 from gunicorn.errors import AppImportError
 from gunicorn.workers import SUPPORTED_WORKERS
 import urllib.parse
 
 REDIRECT_TO = getattr(os, 'devnull', '/dev/null')
 
@@ -50,29 +53,38 @@
     def _setproctitle(title):
         setproctitle("gunicorn: %s" % title)
 except ImportError:
     def _setproctitle(title):
         pass
 
 
+def load_entry_point(distribution, group, name):
+    dist_obj = importlib_metadata.distribution(distribution)
+    eps = [ep for ep in dist_obj.entry_points
+           if ep.group == group and ep.name == name]
+    if not eps:
+        raise ImportError("Entry point %r not found" % ((group, name),))
+    return eps[0].load()
+
+
 def load_class(uri, default="gunicorn.workers.sync.SyncWorker",
                section="gunicorn.workers"):
     if inspect.isclass(uri):
         return uri
     if uri.startswith("egg:"):
         # uses entry points
         entry_str = uri.split("egg:")[1]
         try:
             dist, name = entry_str.rsplit("#", 1)
         except ValueError:
             dist = entry_str
             name = default
 
         try:
-            return pkg_resources.load_entry_point(dist, section, name)
+            return load_entry_point(dist, section, name)
         except Exception:
             exc = traceback.format_exc()
             msg = "class uri %r invalid or not found: \n\n[%s]"
             raise RuntimeError(msg % (uri, exc))
     else:
         components = uri.split('.')
         if len(components) == 1:
@@ -81,27 +93,27 @@
                     uri = uri[1:]
 
                 if uri in SUPPORTED_WORKERS:
                     components = SUPPORTED_WORKERS[uri].split(".")
                     break
 
                 try:
-                    return pkg_resources.load_entry_point(
+                    return load_entry_point(
                         "gunicorn", section, uri
                     )
                 except Exception:
                     exc = traceback.format_exc()
                     msg = "class uri %r invalid or not found: \n\n[%s]"
                     raise RuntimeError(msg % (uri, exc))
 
         klass = components.pop(-1)
 
         try:
             mod = importlib.import_module('.'.join(components))
-        except:
+        except Exception:
             exc = traceback.format_exc()
             msg = "class uri %r invalid or not found: \n\n[%s]"
             raise RuntimeError(msg % (uri, exc))
         return getattr(mod, klass)
 
 
 positionals = (
@@ -141,15 +153,15 @@
         gid = abs(gid) & 0x7FFFFFFF
 
         if initgroups:
             os.initgroups(username, gid)
         elif gid != os.getgid():
             os.setgid(gid)
 
-    if uid:
+    if uid and uid != os.getuid():
         os.setuid(uid)
 
 
 def chown(path, uid, gid):
     os.chown(path, uid, gid)
 
 
@@ -456,15 +468,15 @@
 def is_hoppish(header):
     return header.lower().strip() in hop_headers
 
 
 def daemonize(enable_stdio_inheritance=False):
     """\
     Standard daemonization of a process.
-    http://www.svbug.com/documentation/comp.unix.programmer-FAQ/faq_2.html#SEC16
+    http://www.faqs.org/faqs/unix-faq/programmer/faq/ section 1.7
     """
     if 'GUNICORN_FD' not in os.environ:
         if os.fork():
             os._exit(0)
         os.setsid()
 
         if os.fork():
@@ -482,15 +494,18 @@
             # Remap all of stdin, stdout and stderr on to
             # /dev/null. The expectation is that users have
             # specified the --error-log option.
 
             closerange(0, 3)
 
             fd_null = os.open(REDIRECT_TO, os.O_RDWR)
+            # PEP 446, make fd for /dev/null inheritable
+            os.set_inheritable(fd_null, True)
 
+            # expect fd_null to be always 0 here, but in-case not ...
             if fd_null != 0:
                 os.dup2(fd_null, 0)
 
             os.dup2(fd_null, 1)
             os.dup2(fd_null, 2)
 
         else:
@@ -543,20 +558,20 @@
 def seed():
     try:
         random.seed(os.urandom(64))
     except NotImplementedError:
         random.seed('%s.%s' % (time.time(), os.getpid()))
 
 
-def check_is_writeable(path):
+def check_is_writable(path):
     try:
-        f = open(path, 'a')
+        with open(path, 'a') as f:
+            f.close()
     except IOError as e:
         raise RuntimeError("Error: '%s' isn't writable [%r]" % (path, e))
-    f.close()
 
 
 def to_bytestring(value, encoding="utf8"):
     """Converts a string argument to a byte string"""
     if isinstance(value, bytes):
         return value
     if not isinstance(value, str):
```

### Comparing `gunicorn-20.1.0/gunicorn/systemd.py` & `gunicorn-21.0.0/gunicorn/systemd.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,24 +54,23 @@
     If the unset_environment parameter is True, sd_notify() will unset
     the $NOTIFY_SOCKET environment variable before returning (regardless of
     whether the function call itself succeeded or not). Further calls to
     sd_notify() will then fail, but the variable is no longer inherited by
     child processes.
     """
 
-
     addr = os.environ.get('NOTIFY_SOCKET')
     if addr is None:
         # not run in a service, just a noop
         return
     try:
         sock = socket.socket(socket.AF_UNIX, socket.SOCK_DGRAM | socket.SOCK_CLOEXEC)
         if addr[0] == '@':
             addr = '\0' + addr[1:]
         sock.connect(addr)
         sock.sendall(state.encode('utf-8'))
-    except:
+    except Exception:
         logger.debug("Exception while invoking sd_notify()", exc_info=True)
     finally:
         if unset_environment:
             os.environ.pop('NOTIFY_SOCKET')
         sock.close()
```

### Comparing `gunicorn-20.1.0/gunicorn/sock.py` & `gunicorn-21.0.0/gunicorn/sock.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # This file is part of gunicorn released under the MIT license.
 # See the NOTICE for more information.
 
 import errno
 import os
 import socket
+import ssl
 import stat
 import sys
 import time
 
 from gunicorn import util
 
 
@@ -35,15 +36,15 @@
 
     def __getattr__(self, name):
         return getattr(self.sock, name)
 
     def set_options(self, sock, bound=False):
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         if (self.conf.reuse_port
-            and hasattr(socket, 'SO_REUSEPORT')):  # pragma: no cover
+                and hasattr(socket, 'SO_REUSEPORT')):  # pragma: no cover
             try:
                 sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
             except socket.error as err:
                 if err.errno not in (errno.ENOPROTOOPT, errno.EINVAL):
                     raise
         if not bound:
             self.bind(sock)
@@ -206,7 +207,26 @@
 
 def close_sockets(listeners, unlink=True):
     for sock in listeners:
         sock_name = sock.getsockname()
         sock.close()
         if unlink and _sock_type(sock_name) is UnixSocket:
             os.unlink(sock_name)
+
+
+def ssl_context(conf):
+    def default_ssl_context_factory():
+        context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH, cafile=conf.ca_certs)
+        context.load_cert_chain(certfile=conf.certfile, keyfile=conf.keyfile)
+        context.verify_mode = conf.cert_reqs
+        if conf.ciphers:
+            context.set_ciphers(conf.ciphers)
+        return context
+
+    return conf.ssl_context(conf, default_ssl_context_factory)
+
+
+def ssl_wrap_socket(sock, conf):
+    return ssl_context(conf).wrap_socket(sock,
+                                         server_side=True,
+                                         suppress_ragged_eofs=conf.suppress_ragged_eofs,
+                                         do_handshake_on_connect=conf.do_handshake_on_connect)
```

### Comparing `gunicorn-20.1.0/gunicorn/http/body.py` & `gunicorn-21.0.0/gunicorn/http/body.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self, req, unreader):
         self.req = req
         self.parser = self.parse_chunked(unreader)
         self.buf = io.BytesIO()
 
     def read(self, size):
         if not isinstance(size, int):
-            raise TypeError("size must be an integral type")
+            raise TypeError("size must be an integer type")
         if size < 0:
             raise ValueError("Size must be positive.")
         if size == 0:
             return b""
 
         if self.parser:
             while self.buf.tell() < size:
```

### Comparing `gunicorn-20.1.0/gunicorn/http/message.py` & `gunicorn-21.0.0/gunicorn/http/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,24 +27,25 @@
 
 
 class Message(object):
     def __init__(self, cfg, unreader, peer_addr):
         self.cfg = cfg
         self.unreader = unreader
         self.peer_addr = peer_addr
+        self.remote_addr = peer_addr
         self.version = None
         self.headers = []
         self.trailers = []
         self.body = None
         self.scheme = "https" if cfg.is_ssl else "http"
 
         # set headers limits
         self.limit_request_fields = cfg.limit_request_fields
         if (self.limit_request_fields <= 0
-            or self.limit_request_fields > MAX_HEADERS):
+                or self.limit_request_fields > MAX_HEADERS):
             self.limit_request_fields = MAX_HEADERS
         self.limit_request_field_size = cfg.limit_request_field_size
         if self.limit_request_field_size < 0:
             self.limit_request_field_size = DEFAULT_MAX_HEADERFIELD_SIZE
 
         # set max header buffer size
         max_header_field_size = self.limit_request_field_size or DEFAULT_MAX_HEADERFIELD_SIZE
@@ -66,15 +67,15 @@
         lines = [bytes_to_str(line) + "\r\n" for line in data.split(b"\r\n")]
 
         # handle scheme headers
         scheme_header = False
         secure_scheme_headers = {}
         if ('*' in cfg.forwarded_allow_ips or
             not isinstance(self.peer_addr, tuple)
-            or self.peer_addr[0] in cfg.forwarded_allow_ips):
+                or self.peer_addr[0] in cfg.forwarded_allow_ips):
             secure_scheme_headers = cfg.secure_scheme_headers
 
         # Parse headers into key/value pairs paying attention
         # to continuation lines.
         while lines:
             if len(headers) >= self.limit_request_fields:
                 raise LimitRequestHeaders("limit request headers fields")
@@ -134,15 +135,18 @@
                 if value.lower() == "chunked":
                     chunked = True
 
         if chunked:
             self.body = Body(ChunkedReader(self, self.unreader))
         elif content_length is not None:
             try:
-                content_length = int(content_length)
+                if str(content_length).isnumeric():
+                    content_length = int(content_length)
+                else:
+                    raise InvalidHeader("CONTENT-LENGTH", req=self)
             except ValueError:
                 raise InvalidHeader("CONTENT-LENGTH", req=self)
 
             if content_length < 0:
                 raise InvalidHeader("CONTENT-LENGTH", req=self)
 
             self.body = Body(LengthReader(self.unreader, content_length))
@@ -168,15 +172,15 @@
         self.path = None
         self.query = None
         self.fragment = None
 
         # get max request line size
         self.limit_request_line = cfg.limit_request_line
         if (self.limit_request_line < 0
-            or self.limit_request_line >= MAX_REQUEST_LINE):
+                or self.limit_request_line >= MAX_REQUEST_LINE):
             self.limit_request_line = MAX_REQUEST_LINE
 
         self.req_number = req_number
         self.proxy_protocol_info = None
         super().__init__(cfg, unreader, peer_addr)
 
     def get_data(self, unreader, buf, stop=False):
@@ -271,15 +275,15 @@
 
         return True
 
     def proxy_protocol_access_check(self):
         # check in allow list
         if ("*" not in self.cfg.proxy_allow_ips and
             isinstance(self.peer_addr, tuple) and
-            self.peer_addr[0] not in self.cfg.proxy_allow_ips):
+                self.peer_addr[0] not in self.cfg.proxy_allow_ips):
             raise ForbiddenProxyRequest(self.peer_addr[0])
 
     def parse_proxy_protocol(self, line):
         bits = line.split()
 
         if len(bits) != 6:
             raise InvalidProxyLine(line)
```

### Comparing `gunicorn-20.1.0/gunicorn/http/unreader.py` & `gunicorn-21.0.0/gunicorn/http/unreader.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/gunicorn/http/parser.py` & `gunicorn-21.0.0/gunicorn/http/parser.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/gunicorn/http/errors.py` & `gunicorn-21.0.0/gunicorn/http/errors.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/gunicorn/http/wsgi.py` & `gunicorn-21.0.0/gunicorn/http/wsgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 import re
 import sys
 
 from gunicorn.http.message import HEADER_RE
 from gunicorn.http.errors import InvalidHeader, InvalidHeaderName
 from gunicorn import SERVER_SOFTWARE, SERVER
-import gunicorn.util as util
+from gunicorn import util
 
 # Send files in at most 1GB blocks as some operating systems can have problems
 # with sending files in blocks over 2GB.
 BLKSIZE = 0x3FFFFFFF
 
 HEADER_VALUE_RE = re.compile(r'[\x00-\x1F\x7F]')
 
@@ -367,16 +367,16 @@
             return False
 
         self.send_headers()
 
         if self.is_chunked():
             chunk_size = "%X\r\n" % nbytes
             self.sock.sendall(chunk_size.encode('utf-8'))
-
-        self.sock.sendfile(respiter.filelike, count=nbytes)
+        if nbytes > 0:
+            self.sock.sendfile(respiter.filelike, offset=offset, count=nbytes)
 
         if self.is_chunked():
             self.sock.sendall(b"\r\n")
 
         os.lseek(fileno, offset, os.SEEK_SET)
 
         return True
```

### Comparing `gunicorn-20.1.0/gunicorn/debug.py` & `gunicorn-21.0.0/gunicorn/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     def __call__(self, frame, event, arg):
         if event == 'line':
             lineno = frame.f_lineno
             if '__file__' in frame.f_globals:
                 filename = frame.f_globals['__file__']
                 if (filename.endswith('.pyc') or
-                    filename.endswith('.pyo')):
+                        filename.endswith('.pyo')):
                     filename = filename[:-1]
                 name = frame.f_globals['__name__']
                 line = linecache.getline(filename, lineno)
             else:
                 name = '[unknown]'
                 try:
                     src = inspect.getsourcelines(frame)
```

### Comparing `gunicorn-20.1.0/gunicorn/arbiter.py` & `gunicorn-21.0.0/gunicorn/arbiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             elif self.master_pid:
                 fds = []
                 for fd in os.environ.pop('GUNICORN_FD').split(','):
                     fds.append(int(fd))
 
             self.LISTENERS = sock.create_sockets(self.cfg, self.log, fds)
 
-        listeners_str = ",".join([str(l) for l in self.LISTENERS])
+        listeners_str = ",".join([str(lnr) for lnr in self.LISTENERS])
         self.log.debug("Arbiter booted")
         self.log.info("Listening at: %s (%s)", listeners_str, self.pid)
         self.log.info("Using worker: %s", self.cfg.worker_class_str)
         systemd.sd_notify("READY=1\nSTATUS=Gunicorn arbiter booted", self.log)
 
         # check worker class requirements
         if hasattr(self.worker_class, "check_config"):
@@ -226,16 +226,16 @@
         except (StopIteration, KeyboardInterrupt):
             self.halt()
         except HaltServer as inst:
             self.halt(reason=inst.reason, exit_status=inst.exit_status)
         except SystemExit:
             raise
         except Exception:
-            self.log.info("Unhandled exception in main loop",
-                          exc_info=True)
+            self.log.error("Unhandled exception in main loop",
+                           exc_info=True)
             self.stop(False)
             if self.pidfile is not None:
                 self.pidfile.unlink()
             sys.exit(-1)
 
     def handle_chld(self, sig, frame):
         "SIGCHLD handling"
@@ -336,17 +336,20 @@
         except IOError as e:
             if e.errno not in [errno.EAGAIN, errno.EINTR]:
                 raise
 
     def halt(self, reason=None, exit_status=0):
         """ halt arbiter """
         self.stop()
-        self.log.info("Shutting down: %s", self.master_name)
+
+        log_func = self.log.info if exit_status == 0 else self.log.error
+        log_func("Shutting down: %s", self.master_name)
         if reason is not None:
-            self.log.info("Reason: %s", reason)
+            log_func("Reason: %s", reason)
+
         if self.pidfile is not None:
             self.pidfile.unlink()
         self.cfg.on_exit(self)
         sys.exit(exit_status)
 
     def sleep(self):
         """\
@@ -417,15 +420,15 @@
         environ['GUNICORN_PID'] = str(master_pid)
 
         if self.systemd:
             environ['LISTEN_PID'] = str(os.getpid())
             environ['LISTEN_FDS'] = str(len(self.LISTENERS))
         else:
             environ['GUNICORN_FD'] = ','.join(
-                str(l.fileno()) for l in self.LISTENERS)
+                str(lnr.fileno()) for lnr in self.LISTENERS)
 
         os.chdir(self.START_CTX['cwd'])
 
         # exec the process using the original environment
         os.execvpe(self.START_CTX[0], self.START_CTX['args'], environ)
 
     def reload(self):
@@ -450,19 +453,19 @@
 
         # reopen log files
         self.log.reopen_files()
 
         # do we need to change listener ?
         if old_address != self.cfg.address:
             # close all listeners
-            for l in self.LISTENERS:
-                l.close()
+            for lnr in self.LISTENERS:
+                lnr.close()
             # init new listeners
             self.LISTENERS = sock.create_sockets(self.cfg, self.log)
-            listeners_str = ",".join([str(l) for l in self.LISTENERS])
+            listeners_str = ",".join([str(lnr) for lnr in self.LISTENERS])
             self.log.info("Listening at: %s", listeners_str)
 
         # do some actions on reload
         self.cfg.on_reload(self)
 
         # unlink pidfile
         if self.pidfile is not None:
@@ -516,26 +519,43 @@
                 if self.reexec_pid == wpid:
                     self.reexec_pid = 0
                 else:
                     # A worker was terminated. If the termination reason was
                     # that it could not boot, we'll shut it down to avoid
                     # infinite start/stop cycles.
                     exitcode = status >> 8
+                    if exitcode != 0:
+                        self.log.error('Worker (pid:%s) exited with code %s', wpid, exitcode)
                     if exitcode == self.WORKER_BOOT_ERROR:
                         reason = "Worker failed to boot."
                         raise HaltServer(reason, self.WORKER_BOOT_ERROR)
                     if exitcode == self.APP_LOAD_ERROR:
                         reason = "App failed to load."
                         raise HaltServer(reason, self.APP_LOAD_ERROR)
-                    if os.WIFSIGNALED(status):
-                        self.log.warning(
-                            "Worker with pid %s was terminated due to signal %s",
-                            wpid,
-                            os.WTERMSIG(status)
-                        )
+
+                    if exitcode > 0:
+                        # If the exit code of the worker is greater than 0,
+                        # let the user know.
+                        self.log.error("Worker (pid:%s) exited with code %s.",
+                                       wpid, exitcode)
+                    elif status > 0:
+                        # If the exit code of the worker is 0 and the status
+                        # is greater than 0, then it was most likely killed
+                        # via a signal.
+                        try:
+                            sig_name = signal.Signals(status).name
+                        except ValueError:
+                            sig_name = "code {}".format(status)
+                        msg = "Worker (pid:{}) was sent {}!".format(
+                            wpid, sig_name)
+
+                        # Additional hint for SIGKILL
+                        if status == signal.SIGKILL:
+                            msg += " Perhaps out of memory?"
+                        self.log.error(msg)
 
                     worker = self.WORKERS.pop(wpid, None)
                     if not worker:
                         continue
                     worker.tmp.close()
                     self.cfg.child_exit(self, worker)
         except OSError as e:
```

### Comparing `gunicorn-20.1.0/gunicorn/workers/sync.py` & `gunicorn-21.0.0/gunicorn/workers/sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 import errno
 import os
 import select
 import socket
 import ssl
 import sys
 
-import gunicorn.http as http
-import gunicorn.http.wsgi as wsgi
-import gunicorn.util as util
-import gunicorn.workers.base as base
+from gunicorn import http
+from gunicorn.http import wsgi
+from gunicorn import sock
+from gunicorn import util
+from gunicorn.workers import base
 
 
 class StopWaiting(Exception):
     """ exception raised to stop waiting for a connection """
 
 
 class SyncWorker(base.Worker):
@@ -124,17 +125,15 @@
         else:
             self.run_for_one(timeout)
 
     def handle(self, listener, client, addr):
         req = None
         try:
             if self.cfg.is_ssl:
-                client = ssl.wrap_socket(client, server_side=True,
-                                         **self.cfg.ssl_options)
-
+                client = sock.ssl_wrap_socket(client, self.cfg)
             parser = http.RequestParser(self.cfg, client, addr)
             req = next(parser)
             self.handle_request(listener, req, client, addr)
         except http.errors.NoMoreData as e:
             self.log.debug("Ignored premature client disconnection. %s", e)
         except StopIteration as e:
             self.log.debug("Closing connection. %s", e)
@@ -180,17 +179,17 @@
             try:
                 if isinstance(respiter, environ['wsgi.file_wrapper']):
                     resp.write_file(respiter)
                 else:
                     for item in respiter:
                         resp.write(item)
                 resp.close()
+            finally:
                 request_time = datetime.now() - request_start
                 self.log.access(resp, req, environ, request_time)
-            finally:
                 if hasattr(respiter, "close"):
                     respiter.close()
         except EnvironmentError:
             # pass to next try-except level
             util.reraise(*sys.exc_info())
         except Exception:
             if resp and resp.headers_sent:
```

### Comparing `gunicorn-20.1.0/gunicorn/workers/base_async.py` & `gunicorn-21.0.0/gunicorn/workers/base_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 from datetime import datetime
 import errno
 import socket
 import ssl
 import sys
 
-import gunicorn.http as http
-import gunicorn.http.wsgi as wsgi
-import gunicorn.util as util
-import gunicorn.workers.base as base
+from gunicorn import http
+from gunicorn.http import wsgi
+from gunicorn import util
+from gunicorn.workers import base
 
 ALREADY_HANDLED = object()
 
 
 class AsyncWorker(base.Worker):
 
     def __init__(self, *args, **kwargs):
@@ -111,17 +111,17 @@
             try:
                 if isinstance(respiter, environ['wsgi.file_wrapper']):
                     resp.write_file(respiter)
                 else:
                     for item in respiter:
                         resp.write(item)
                 resp.close()
+            finally:
                 request_time = datetime.now() - request_start
                 self.log.access(resp, req, environ, request_time)
-            finally:
                 if hasattr(respiter, "close"):
                     respiter.close()
             if resp.should_close():
                 raise StopIteration()
         except StopIteration:
             raise
         except EnvironmentError:
```

### Comparing `gunicorn-20.1.0/gunicorn/workers/gtornado.py` & `gunicorn-21.0.0/gunicorn/workers/gtornado.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -
 #
 # This file is part of gunicorn released under the MIT license.
 # See the NOTICE for more information.
 
-import copy
 import os
 import sys
 
 try:
     import tornado
 except ImportError:
     raise RuntimeError("You need tornado installed to use this worker.")
 import tornado.web
 import tornado.httpserver
 from tornado.ioloop import IOLoop, PeriodicCallback
 from tornado.wsgi import WSGIContainer
 from gunicorn.workers.base import Worker
 from gunicorn import __version__ as gversion
+from gunicorn.sock import ssl_context
 
 
 # Tornado 5.0 updated its IOLoop, and the `io_loop` arguments to many
 # Tornado functions have been removed in Tornado 5.0. Also, they no
 # longer store PeriodCallbacks in ioloop._callbacks. Instead we store
 # them on our side, and use stop() on them when stopping the worker.
 # See https://www.tornadoweb.org/en/stable/releases/v5.0.0.html#backwards-compatibility-notes
@@ -104,17 +104,18 @@
         # Assume the app is a WSGI callable if its not an
         # instance of tornado.web.Application or is an
         # instance of tornado.wsgi.WSGIApplication
         app = self.wsgi
 
         if tornado.version_info[0] < 6:
             if not isinstance(app, tornado.web.Application) or \
-            isinstance(app, tornado.wsgi.WSGIApplication):
+                    isinstance(app, tornado.wsgi.WSGIApplication):
                 app = WSGIContainer(app)
-        elif not isinstance(app, WSGIContainer):
+        elif not isinstance(app, WSGIContainer) and \
+                not isinstance(app, tornado.web.Application):
             app = WSGIContainer(app)
 
         # Monkey-patching HTTPConnection.finish to count the
         # number of requests being handled by Tornado. This
         # will help gunicorn shutdown the worker if max_requests
         # is exceeded.
         httpserver = sys.modules["tornado.httpserver"]
@@ -135,24 +136,19 @@
                 def on_close(instance, server_conn):
                     self.handle_request()
                     super(_HTTPServer, instance).on_close(server_conn)
 
             server_class = _HTTPServer
 
         if self.cfg.is_ssl:
-            _ssl_opt = copy.deepcopy(self.cfg.ssl_options)
-            # tornado refuses initialization if ssl_options contains following
-            # options
-            del _ssl_opt["do_handshake_on_connect"]
-            del _ssl_opt["suppress_ragged_eofs"]
             if TORNADO5:
-                server = server_class(app, ssl_options=_ssl_opt)
+                server = server_class(app, ssl_options=ssl_context(self.cfg))
             else:
                 server = server_class(app, io_loop=self.ioloop,
-                                      ssl_options=_ssl_opt)
+                                      ssl_options=ssl_context(self.cfg))
         else:
             if TORNADO5:
                 server = server_class(app)
             else:
                 server = server_class(app, io_loop=self.ioloop)
 
         self.server = server
```

### Comparing `gunicorn-20.1.0/gunicorn/workers/__init__.py` & `gunicorn-21.0.0/gunicorn/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/gunicorn/workers/geventlet.py` & `gunicorn-21.0.0/gunicorn/workers/geventlet.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,30 @@
 import sys
 
 try:
     import eventlet
 except ImportError:
     raise RuntimeError("eventlet worker requires eventlet 0.24.1 or higher")
 else:
-    from pkg_resources import parse_version
+    from packaging.version import parse as parse_version
     if parse_version(eventlet.__version__) < parse_version('0.24.1'):
         raise RuntimeError("eventlet worker requires eventlet 0.24.1 or higher")
 
 from eventlet import hubs, greenthread
 from eventlet.greenio import GreenSocket
-from eventlet.wsgi import ALREADY_HANDLED as EVENTLET_ALREADY_HANDLED
+import eventlet.wsgi
 import greenlet
 
 from gunicorn.workers.base_async import AsyncWorker
+from gunicorn.sock import ssl_wrap_socket
+
+# ALREADY_HANDLED is removed in 0.30.3+ now it's `WSGI_LOCAL.already_handled: bool`
+# https://github.com/eventlet/eventlet/pull/544
+EVENTLET_WSGI_LOCAL = getattr(eventlet.wsgi, "WSGI_LOCAL", None)
+EVENTLET_ALREADY_HANDLED = getattr(eventlet.wsgi, "ALREADY_HANDLED", None)
 
 
 def _eventlet_socket_sendfile(self, file, offset=0, count=None):
     # Based on the implementation in gevent which in turn is slightly
     # modified from the standard library implementation.
     if self.gettimeout() == 0:
         raise ValueError("non-blocking sockets are not supported")
@@ -57,15 +63,14 @@
                         break
         return total_sent
     finally:
         if total_sent > 0 and hasattr(file, 'seek'):
             file.seek(offset + total_sent)
 
 
-
 def _eventlet_serve(sock, handle, concurrency):
     """
     Serve requests forever.
 
     This code is nearly identical to ``eventlet.convenience.serve`` except
     that it attempts to join the pool at the end, which allows for gunicorn
     graceful shutdowns.
@@ -121,14 +126,18 @@
 
     def patch(self):
         hubs.use_hub()
         eventlet.monkey_patch()
         patch_sendfile()
 
     def is_already_handled(self, respiter):
+        # eventlet >= 0.30.3
+        if getattr(EVENTLET_WSGI_LOCAL, "already_handled", None):
+            raise StopIteration()
+        # eventlet < 0.30.3
         if respiter == EVENTLET_ALREADY_HANDLED:
             raise StopIteration()
         return super().is_already_handled(respiter)
 
     def init_process(self):
         self.patch()
         super().init_process()
@@ -140,17 +149,15 @@
         eventlet.spawn(super().handle_usr1, sig, frame)
 
     def timeout_ctx(self):
         return eventlet.Timeout(self.cfg.keepalive or None, False)
 
     def handle(self, listener, client, addr):
         if self.cfg.is_ssl:
-            client = eventlet.wrap_ssl(client, server_side=True,
-                                       **self.cfg.ssl_options)
-
+            client = ssl_wrap_socket(client, self.cfg)
         super().handle(listener, client, addr)
 
     def run(self):
         acceptors = []
         for sock in self.sockets:
             gsock = GreenSocket(sock)
             gsock.setblocking(1)
@@ -162,14 +169,15 @@
             eventlet.sleep(0.0)
 
         while self.alive:
             self.notify()
             eventlet.sleep(1.0)
 
         self.notify()
+        t = None
         try:
             with eventlet.Timeout(self.cfg.graceful_timeout) as t:
                 for a in acceptors:
                     a.kill(eventlet.StopServe())
                 for a in acceptors:
                     a.wait()
         except eventlet.Timeout as te:
```

### Comparing `gunicorn-20.1.0/gunicorn/workers/workertmp.py` & `gunicorn-21.0.0/gunicorn/workers/workertmp.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         os.umask(old_umask)
 
         # change the owner and group of the file if the worker will run as
         # a different user or group, so that the worker can modify the file
         if cfg.uid != os.geteuid() or cfg.gid != os.getegid():
             util.chown(name, cfg.uid, cfg.gid)
 
-        # unlink the file so we don't leak tempory files
+        # unlink the file so we don't leak temporary files
         try:
             if not IS_CYGWIN:
                 util.unlink(name)
             # In Python 3.8, open() emits RuntimeWarning if buffering=1 for binary mode.
             # Because we never write to this file, pass 0 to switch buffering off.
             self._tmp = os.fdopen(fd, 'w+b', 0)
         except Exception:
```

### Comparing `gunicorn-20.1.0/gunicorn/workers/ggevent.py` & `gunicorn-21.0.0/gunicorn/workers/ggevent.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 import time
 
 try:
     import gevent
 except ImportError:
     raise RuntimeError("gevent worker requires gevent 1.4 or higher")
 else:
-    from pkg_resources import parse_version
+    from packaging.version import parse as parse_version
     if parse_version(gevent.__version__) < parse_version('1.4'):
         raise RuntimeError("gevent worker requires gevent 1.4 or higher")
 
 from gevent.pool import Pool
 from gevent.server import StreamServer
 from gevent import hub, monkey, socket, pywsgi
 
 import gunicorn
 from gunicorn.http.wsgi import base_environ
+from gunicorn.sock import ssl_context
 from gunicorn.workers.base_async import AsyncWorker
 
 VERSION = "gevent/%s gunicorn/%s" % (gevent.__version__, gunicorn.__version__)
 
 
 class GeventWorker(AsyncWorker):
 
@@ -37,15 +38,15 @@
     def patch(self):
         monkey.patch_all()
 
         # patch sockets
         sockets = []
         for s in self.sockets:
             sockets.append(socket.socket(s.FAMILY, socket.SOCK_STREAM,
-                fileno=s.sock.fileno()))
+                                         fileno=s.sock.fileno()))
         self.sockets = sockets
 
     def notify(self):
         super().notify()
         if self.ppid != os.getppid():
             self.log.info("Parent changed, shutting down: %s", self)
             sys.exit(0)
@@ -54,15 +55,15 @@
         return gevent.Timeout(self.cfg.keepalive, False)
 
     def run(self):
         servers = []
         ssl_args = {}
 
         if self.cfg.is_ssl:
-            ssl_args = dict(server_side=True, **self.cfg.ssl_options)
+            ssl_args = {"ssl_context": ssl_context(self.cfg)}
 
         for s in self.sockets:
             s.setblocking(1)
             pool = Pool(self.worker_connections)
             if self.server_class is not None:
                 environ = base_environ(self.cfg)
                 environ.update({
@@ -106,15 +107,15 @@
                 if not accepting:
                     return
 
                 self.notify()
                 gevent.sleep(1.0)
 
             # Force kill all active the handlers
-            self.log.warning("Worker graceful timeout (pid:%s)" % self.pid)
+            self.log.warning("Worker graceful timeout (pid:%s)", self.pid)
             for server in servers:
                 server.stop(timeout=1)
         except Exception:
             pass
 
     def handle(self, listener, client, addr):
         # Connected socket timeout defaults to socket.getdefaulttimeout().
```

### Comparing `gunicorn-20.1.0/gunicorn/workers/gthread.py` & `gunicorn-21.0.0/gunicorn/workers/gthread.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # A threaded worker accepts connections in the main loop, accepted
 # connections are added to the thread pool as a connection job.
 # Keepalive connections are put back in the loop waiting for an event.
 # If no event happen after the keep alive timeout, the connection is
 # closed.
 # pylint: disable=no-else-break
 
-import concurrent.futures as futures
+from concurrent import futures
 import errno
 import os
 import selectors
 import socket
 import ssl
 import sys
 import time
@@ -23,38 +23,41 @@
 from datetime import datetime
 from functools import partial
 from threading import RLock
 
 from . import base
 from .. import http
 from .. import util
+from .. import sock
 from ..http import wsgi
 
 
 class TConn(object):
 
     def __init__(self, cfg, sock, client, server):
         self.cfg = cfg
         self.sock = sock
         self.client = client
         self.server = server
 
         self.timeout = None
         self.parser = None
+        self.initialized = False
 
         # set the socket to non blocking
         self.sock.setblocking(False)
 
     def init(self):
+        self.initialized = True
         self.sock.setblocking(True)
+
         if self.parser is None:
             # wrap the socket if needed
             if self.cfg.is_ssl:
-                self.sock = ssl.wrap_socket(self.sock, server_side=True,
-                                            **self.cfg.ssl_options)
+                self.sock = sock.ssl_wrap_socket(self.sock, self.cfg)
 
             # initialize the parser
             self.parser = http.RequestParser(self.cfg, self.sock, self.client)
 
     def set_timeout(self):
         # set the timeout
         self.timeout = time.time() + self.cfg.keepalive
@@ -115,32 +118,40 @@
         self._wrap_future(fs, conn)
 
     def accept(self, server, listener):
         try:
             sock, client = listener.accept()
             # initialize the connection object
             conn = TConn(self.cfg, sock, client, server)
+            # set timeout to ensure it will not be in the loop too long
+            conn.set_timeout()
+
             self.nr_conns += 1
-            # enqueue the job
-            self.enqueue_req(conn)
+            # wait until socket is readable
+            with self._lock:
+                self._keep.append(conn)
+                self.poller.register(conn.sock, selectors.EVENT_READ,
+                                     partial(self.on_client_socket_readable, conn))
         except EnvironmentError as e:
             if e.errno not in (errno.EAGAIN, errno.ECONNABORTED,
                                errno.EWOULDBLOCK):
                 raise
 
-    def reuse_connection(self, conn, client):
+    def on_client_socket_readable(self, conn, client):
         with self._lock:
             # unregister the client from the poller
             self.poller.unregister(client)
-            # remove the connection from keepalive
-            try:
-                self._keep.remove(conn)
-            except ValueError:
-                # race condition
-                return
+
+            if conn.initialized:
+                # remove the connection from keepalive
+                try:
+                    self._keep.remove(conn)
+                except ValueError:
+                    # race condition
+                    return
 
         # submit the connection to a worker
         self.enqueue_req(conn)
 
     def murder_keepalived(self):
         now = time.time()
         while True:
@@ -245,15 +256,15 @@
                 # register the connection
                 conn.set_timeout()
                 with self._lock:
                     self._keep.append(conn)
 
                     # add the socket to the event loop
                     self.poller.register(conn.sock, selectors.EVENT_READ,
-                                         partial(self.reuse_connection, conn))
+                                         partial(self.on_client_socket_readable, conn))
             else:
                 self.nr_conns -= 1
                 conn.close()
         except Exception:
             # an exception happened, make sure to close the
             # socket.
             self.nr_conns -= 1
@@ -325,17 +336,17 @@
                 if isinstance(respiter, environ['wsgi.file_wrapper']):
                     resp.write_file(respiter)
                 else:
                     for item in respiter:
                         resp.write(item)
 
                 resp.close()
+            finally:
                 request_time = datetime.now() - request_start
                 self.log.access(resp, req, environ, request_time)
-            finally:
                 if hasattr(respiter, "close"):
                     respiter.close()
 
             if resp.should_close():
                 self.log.debug("Closing connection.")
                 return False
         except EnvironmentError:
```

### Comparing `gunicorn-20.1.0/gunicorn/workers/base.py` & `gunicorn-21.0.0/gunicorn/workers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,30 +226,32 @@
             elif isinstance(exc, (InvalidHeaderName, InvalidHeader,)):
                 mesg = "%s" % str(exc)
                 if not req and hasattr(exc, "req"):
                     req = exc.req  # for access log
             elif isinstance(exc, LimitRequestLine):
                 mesg = "%s" % str(exc)
             elif isinstance(exc, LimitRequestHeaders):
+                reason = "Request Header Fields Too Large"
                 mesg = "Error parsing headers: '%s'" % str(exc)
+                status_int = 431
             elif isinstance(exc, InvalidProxyLine):
                 mesg = "'%s'" % str(exc)
             elif isinstance(exc, ForbiddenProxyRequest):
                 reason = "Forbidden"
                 mesg = "Request forbidden"
                 status_int = 403
             elif isinstance(exc, InvalidSchemeHeaders):
                 mesg = "%s" % str(exc)
             elif isinstance(exc, SSLError):
                 reason = "Forbidden"
                 mesg = "'%s'" % str(exc)
                 status_int = 403
 
             msg = "Invalid request from ip={ip}: {error}"
-            self.log.debug(msg.format(ip=addr[0], error=str(exc)))
+            self.log.warning(msg.format(ip=addr[0], error=str(exc)))
         else:
             if hasattr(req, "uri"):
                 self.log.exception("Error handling request %s", req.uri)
             status_int = 500
             reason = "Internal Server Error"
             mesg = ""
```

### Comparing `gunicorn-20.1.0/gunicorn/errors.py` & `gunicorn-21.0.0/gunicorn/errors.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/gunicorn/glogging.py` & `gunicorn-21.0.0/gunicorn/glogging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -
 #
 # This file is part of gunicorn released under the MIT license.
 # See the NOTICE for more information.
 
 import base64
 import binascii
+import json
 import time
 import logging
 logging.Logger.manager.emittedNoHandlerWarning = 1  # noqa
 from logging.config import dictConfig
 from logging.config import fileConfig
 import os
 import socket
@@ -40,61 +41,59 @@
     "local3": 19,
     "local4": 20,
     "local5": 21,
     "local6": 22,
     "local7": 23
 }
 
+CONFIG_DEFAULTS = {
+    "version": 1,
+    "disable_existing_loggers": False,
+    "root": {"level": "INFO", "handlers": ["console"]},
+    "loggers": {
+        "gunicorn.error": {
+            "level": "INFO",
+            "handlers": ["error_console"],
+            "propagate": True,
+            "qualname": "gunicorn.error"
+        },
 
-CONFIG_DEFAULTS = dict(
-        version=1,
-        disable_existing_loggers=False,
-
-        root={"level": "INFO", "handlers": ["console"]},
-        loggers={
-            "gunicorn.error": {
-                "level": "INFO",
-                "handlers": ["error_console"],
-                "propagate": True,
-                "qualname": "gunicorn.error"
-            },
-
-            "gunicorn.access": {
-                "level": "INFO",
-                "handlers": ["console"],
-                "propagate": True,
-                "qualname": "gunicorn.access"
-            }
+        "gunicorn.access": {
+            "level": "INFO",
+            "handlers": ["console"],
+            "propagate": True,
+            "qualname": "gunicorn.access"
+        }
+    },
+    "handlers": {
+        "console": {
+            "class": "logging.StreamHandler",
+            "formatter": "generic",
+            "stream": "ext://sys.stdout"
         },
-        handlers={
-            "console": {
-                "class": "logging.StreamHandler",
-                "formatter": "generic",
-                "stream": "ext://sys.stdout"
-            },
-            "error_console": {
-                "class": "logging.StreamHandler",
-                "formatter": "generic",
-                "stream": "ext://sys.stderr"
-            },
+        "error_console": {
+            "class": "logging.StreamHandler",
+            "formatter": "generic",
+            "stream": "ext://sys.stderr"
         },
-        formatters={
-            "generic": {
-                "format": "%(asctime)s [%(process)d] [%(levelname)s] %(message)s",
-                "datefmt": "[%Y-%m-%d %H:%M:%S %z]",
-                "class": "logging.Formatter"
-            }
+    },
+    "formatters": {
+        "generic": {
+            "format": "%(asctime)s [%(process)d] [%(levelname)s] %(message)s",
+            "datefmt": "[%Y-%m-%d %H:%M:%S %z]",
+            "class": "logging.Formatter"
         }
-)
+    }
+}
 
 
 def loggers():
     """ get list of all loggers """
     root = logging.root
-    existing = root.manager.loggerDict.keys()
+    existing = list(root.manager.loggerDict.keys())
     return [logging.getLogger(name) for name in existing]
 
 
 class SafeAtoms(dict):
 
     def __init__(self, atoms):
         dict.__init__(self)
@@ -236,14 +235,29 @@
             except (
                     AttributeError,
                     ImportError,
                     ValueError,
                     TypeError
             ) as exc:
                 raise RuntimeError(str(exc))
+        elif cfg.logconfig_json:
+            config = CONFIG_DEFAULTS.copy()
+            if os.path.exists(cfg.logconfig_json):
+                try:
+                    config_json = json.load(open(cfg.logconfig_json))
+                    config.update(config_json)
+                    dictConfig(config)
+                except (
+                    json.JSONDecodeError,
+                    AttributeError,
+                    ImportError,
+                    ValueError,
+                    TypeError
+                ) as exc:
+                    raise RuntimeError(str(exc))
         elif cfg.logconfig:
             if os.path.exists(cfg.logconfig):
                 defaults = CONFIG_DEFAULTS.copy()
                 defaults['__file__'] = cfg.logconfig
                 defaults['here'] = os.path.dirname(cfg.logconfig)
                 fileConfig(cfg.logconfig, defaults=defaults,
                            disable_existing_loggers=False)
@@ -271,15 +285,15 @@
 
     def log(self, lvl, msg, *args, **kwargs):
         if isinstance(lvl, str):
             lvl = self.LOG_LEVELS.get(lvl.lower(), logging.INFO)
         self.error_log.log(lvl, msg, *args, **kwargs)
 
     def atoms(self, resp, req, environ, request_time):
-        """ Gets atoms for log formating.
+        """ Gets atoms for log formatting.
         """
         status = resp.status
         if isinstance(status, str):
             status = status.split(None, 1)[0]
         atoms = {
             'h': environ.get('REMOTE_ADDR', '-'),
             'l': '-',
@@ -295,15 +309,15 @@
             'H': environ.get('SERVER_PROTOCOL'),
             'b': getattr(resp, 'sent', None) is not None and str(resp.sent) or '-',
             'B': getattr(resp, 'sent', None),
             'f': environ.get('HTTP_REFERER', '-'),
             'a': environ.get('HTTP_USER_AGENT', '-'),
             'T': request_time.seconds,
             'D': (request_time.seconds * 1000000) + request_time.microseconds,
-            'M': (request_time.seconds * 1000) + int(request_time.microseconds/1000),
+            'M': (request_time.seconds * 1000) + int(request_time.microseconds / 1000),
             'L': "%d.%06d" % (request_time.seconds, request_time.microseconds),
             'p': "<%s>" % os.getpid()
         }
 
         # add request headers
         if hasattr(req, 'headers'):
             req_headers = req.headers
@@ -330,15 +344,15 @@
 
     def access(self, resp, req, environ, request_time):
         """ See http://httpd.apache.org/docs/2.0/logs.html#combined
         for format details
         """
 
         if not (self.cfg.accesslog or self.cfg.logconfig or
-           self.cfg.logconfig_dict or
+           self.cfg.logconfig_dict or self.cfg.logconfig_json or
            (self.cfg.syslog and not self.cfg.disable_redirect_access_to_syslog)):
             return
 
         # wrap atoms:
         # - make sure atoms will be test case insensitively
         # - if atom doesn't exist replace it by '-'
         safe_atoms = self.atoms_wrapper_class(
@@ -399,15 +413,15 @@
         if h:
             log.handlers.remove(h)
 
         if output is not None:
             if output == "-":
                 h = logging.StreamHandler(stream)
             else:
-                util.check_is_writeable(output)
+                util.check_is_writable(output)
                 h = logging.FileHandler(output)
                 # make sure the user can reopen the file
                 try:
                     os.chown(h.baseFilename, self.cfg.user, self.cfg.group)
                 except OSError:
                     # it's probably OK there, we assume the user has given
                     # /dev/null as a parameter.
@@ -433,15 +447,15 @@
             raise RuntimeError("unknown facility name")
 
         # parse syslog address
         socktype, addr = parse_syslog_address(cfg.syslog_addr)
 
         # finally setup the syslog handler
         h = logging.handlers.SysLogHandler(address=addr,
-                facility=facility, socktype=socktype)
+                                           facility=facility, socktype=socktype)
 
         h.setFormatter(fmt)
         h._gunicorn = True
         log.addHandler(h)
 
     def _get_user(self, environ):
         user = None
@@ -450,15 +464,11 @@
             auth = http_auth.split(" ", 1)
             if len(auth) == 2:
                 try:
                     # b64decode doesn't accept unicode in Python < 3.3
                     # so we need to convert it to a byte string
                     auth = base64.b64decode(auth[1].strip().encode('utf-8'))
                     # b64decode returns a byte string
-                    auth = auth.decode('utf-8')
-                    auth = auth.split(":", 1)
+                    user = auth.split(b":", 1)[0].decode("UTF-8")
                 except (TypeError, binascii.Error, UnicodeDecodeError) as exc:
                     self.debug("Couldn't get username: %s", exc)
-                    return user
-                if len(auth) == 2:
-                    user = auth[0]
         return user
```

### Comparing `gunicorn-20.1.0/docs/Makefile` & `gunicorn-21.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/install.rst` & `gunicorn-21.0.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/settings.rst` & `gunicorn-21.0.0/docs/source/settings.rst`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ``config``
 ~~~~~~~~~~
 
 **Command line:** ``-c CONFIG`` or ``--config CONFIG``
 
 **Default:** ``'./gunicorn.conf.py'``
 
-The Gunicorn config file.
+:ref:`The Gunicorn config file<configuration_file>`.
 
 A string of the form ``PATH``, ``file:PATH``, or ``python:MODULE_NAME``.
 
 Only has an effect when specified on the command line or as part of an
 application specific configuration.
 
 By default, a file named ``gunicorn.conf.py`` will be read from the same
@@ -306,35 +306,51 @@
 file format.
 
 .. _logconfig-dict:
 
 ``logconfig_dict``
 ~~~~~~~~~~~~~~~~~~
 
-**Command line:** ``--log-config-dict``
-
 **Default:** ``{}``
 
 The log config dictionary to use, using the standard Python
 logging module's dictionary configuration format. This option
-takes precedence over the :ref:`logconfig` option, which uses the
-older file configuration format.
+takes precedence over the :ref:`logconfig` and :ref:`logConfigJson` options,
+which uses the older file configuration format and JSON
+respectively.
 
 Format: https://docs.python.org/3/library/logging.config.html#logging.config.dictConfig
 
+For more context you can look at the default configuration dictionary for logging, which can be found at ``gunicorn.glogging.CONFIG_DEFAULTS``.
+
 .. versionadded:: 19.8
 
+.. _logconfig-json:
+
+``logconfig_json``
+~~~~~~~~~~~~~~~~~~
+
+**Command line:** ``--log-config-json FILE``
+
+**Default:** ``None``
+
+The log config to read config from a JSON file
+
+Format: https://docs.python.org/3/library/logging.config.html#logging.config.jsonConfig
+
+.. versionadded:: 20.0
+
 .. _syslog-addr:
 
 ``syslog_addr``
 ~~~~~~~~~~~~~~~
 
 **Command line:** ``--log-syslog-to SYSLOG_ADDR``
 
-**Default:** ``'unix:///var/run/syslog'``
+**Default:** ``'udp://localhost:514'``
 
 Address to send syslog messages.
 
 Address is a string of the form:
 
 * ``unix://PATH#TYPE`` : for unix domain socket. ``TYPE`` can be ``stream``
   for the stream driver or ``dgram`` for the dgram driver.
@@ -403,15 +419,20 @@
 ``statsd_host``
 ~~~~~~~~~~~~~~~
 
 **Command line:** ``--statsd-host STATSD_ADDR``
 
 **Default:** ``None``
 
-``host:port`` of the statsd server to log to.
+The address of the StatsD server to log to.
+
+Address is a string of the form:
+
+* ``unix://PATH`` : for a unix domain socket.
+* ``HOST:PORT`` : for a network address
 
 .. versionadded:: 19.1
 
 .. _dogstatsd-tags:
 
 ``dogstatsd_tags``
 ~~~~~~~~~~~~~~~~~~
@@ -499,15 +520,18 @@
 ``ssl_version``
 ~~~~~~~~~~~~~~~
 
 **Command line:** ``--ssl-version``
 
 **Default:** ``<_SSLMethod.PROTOCOL_TLS: 2>``
 
-SSL version to use.
+SSL version to use (see stdlib ssl module's).
+
+.. deprecated:: 20.2
+   The option is deprecated and it is currently ignored. Use :ref:`ssl-context` instead.
 
 ============= ============
 --ssl-version Description
 ============= ============
 SSLv3         SSLv3 is not-secure and is strongly discouraged.
 SSLv23        Alias for TLS. Deprecated in Python 3.6, use TLS.
 TLS           Negotiate highest possible version between client/server.
@@ -522,26 +546,37 @@
 
 .. versionchanged:: 19.7
    The default value has been changed from ``ssl.PROTOCOL_TLSv1`` to
    ``ssl.PROTOCOL_SSLv23``.
 .. versionchanged:: 20.0
    This setting now accepts string names based on ``ssl.PROTOCOL_``
    constants.
+.. versionchanged:: 20.0.1
+   The default value has been changed from ``ssl.PROTOCOL_SSLv23`` to
+   ``ssl.PROTOCOL_TLS`` when Python >= 3.6 .
 
 .. _cert-reqs:
 
 ``cert_reqs``
 ~~~~~~~~~~~~~
 
 **Command line:** ``--cert-reqs``
 
 **Default:** ``<VerifyMode.CERT_NONE: 0>``
 
 Whether client certificate is required (see stdlib ssl module's)
 
+===========  ===========================
+--cert-reqs      Description
+===========  ===========================
+`0`          no client veirifcation
+`1`          ssl.CERT_OPTIONAL
+`2`          ssl.CERT_REQUIRED
+===========  ===========================
+
 .. _ca-certs:
 
 ``ca_certs``
 ~~~~~~~~~~~~
 
 **Command line:** ``--ca-certs FILE``
 
@@ -814,15 +849,15 @@
 ~~~~~~~~~~~~~~~
 
 **Default:** 
 
 .. code-block:: python
 
         def pre_request(worker, req):
-            worker.log.debug("%s %s" % (req.method, req.path))
+            worker.log.debug("%s %s", req.method, req.path)
 
 Called just before a worker processes the request.
 
 The callable needs to accept two instance variables for the Worker and
 the Request.
 
 .. _post-request:
@@ -910,14 +945,48 @@
         def on_exit(server):
             pass
 
 Called just before exiting Gunicorn.
 
 The callable needs to accept a single instance variable for the Arbiter.
 
+.. _ssl-context:
+
+``ssl_context``
+~~~~~~~~~~~~~~~
+
+**Default:** 
+
+.. code-block:: python
+
+        def ssl_context(config, default_ssl_context_factory):
+            return default_ssl_context_factory()
+
+Called when SSLContext is needed.
+
+Allows customizing SSL context.
+
+The callable needs to accept an instance variable for the Config and
+a factory function that returns default SSLContext which is initialized
+with certificates, private key, cert_reqs, and ciphers according to
+config and can be further customized by the callable.
+The callable needs to return SSLContext object.
+
+Following example shows a configuration file that sets the minimum TLS version to 1.3:
+
+.. code-block:: python
+
+    def ssl_context(conf, default_ssl_context_factory):
+        import ssl
+        context = default_ssl_context_factory()
+        context.minimum_version = ssl.TLSVersion.TLSv1_3
+        return context
+
+.. versionadded:: 20.2
+
 Server Mechanics
 ----------------
 
 .. _preload-app:
 
 ``preload_app``
 ~~~~~~~~~~~~~~~
@@ -970,15 +1039,15 @@
 .. _chdir:
 
 ``chdir``
 ~~~~~~~~~
 
 **Command line:** ``--chdir``
 
-**Default:** ``'/Users/chainz/Documents/Projects/gunicorn/docs'``
+**Default:** ``'.'``
 
 Change directory to specified directory before loading apps.
 
 .. _daemon:
 
 ``daemon``
 ~~~~~~~~~~
@@ -1054,30 +1123,30 @@
 .. _user:
 
 ``user``
 ~~~~~~~~
 
 **Command line:** ``-u USER`` or ``--user USER``
 
-**Default:** ``501``
+**Default:** ``os.geteuid()``
 
 Switch worker processes to run as this user.
 
 A valid user id (as an integer) or the name of a user that can be
 retrieved with a call to ``pwd.getpwnam(value)`` or ``None`` to not
 change the worker process user.
 
 .. _group:
 
 ``group``
 ~~~~~~~~~
 
 **Command line:** ``-g GROUP`` or ``--group GROUP``
 
-**Default:** ``20``
+**Default:** ``os.getegid()``
 
 Switch worker process to run as this group.
 
 A valid group id (as an integer) or the name of a user that can be
 retrieved with a call to ``pwd.getgrnam(value)`` or ``None`` to not
 change the worker processes group.
 
@@ -1133,18 +1202,24 @@
 
 ``secure_scheme_headers``
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 **Default:** ``{'X-FORWARDED-PROTOCOL': 'ssl', 'X-FORWARDED-PROTO': 'https', 'X-FORWARDED-SSL': 'on'}``
 
 A dictionary containing headers and values that the front-end proxy
-uses to indicate HTTPS requests. These tell Gunicorn to set
+uses to indicate HTTPS requests. If the source IP is permitted by
+``forwarded-allow-ips`` (below), *and* at least one request header matches
+a key-value pair listed in this dictionary, then Gunicorn will set
 ``wsgi.url_scheme`` to ``https``, so your application can tell that the
 request is secure.
 
+If the other headers listed in this dictionary are not present in the request, they will be ignored,
+but if the other headers are present and do not match the provided values, then
+the request will fail to parse. See the note below for more detailed examples of this behaviour.
+
 The dictionary should map upper-case header names to exact string
 values. The value comparisons are case-sensitive, unlike the header
 names, so make sure they're exactly what your front-end proxy sends
 when handling HTTPS requests.
 
 It is important that your front-end proxy configuration ensures that
 the headers defined here can not be passed directly from the client.
@@ -1164,14 +1239,77 @@
 Set to ``*`` to disable checking of Front-end IPs (useful for setups
 where you don't know in advance the IP address of Front-end, but
 you still trust the environment).
 
 By default, the value of the ``FORWARDED_ALLOW_IPS`` environment
 variable. If it is not defined, the default is ``"127.0.0.1"``.
 
+.. note::
+
+    The interplay between the request headers, the value of ``forwarded_allow_ips``, and the value of
+    ``secure_scheme_headers`` is complex. Various scenarios are documented below to further elaborate.
+    In each case, we have a request from the remote address 134.213.44.18, and the default value of
+    ``secure_scheme_headers``:
+
+    .. code::
+
+        secure_scheme_headers = {
+            'X-FORWARDED-PROTOCOL': 'ssl',
+            'X-FORWARDED-PROTO': 'https',
+            'X-FORWARDED-SSL': 'on'
+        }
+
+
+    .. list-table::
+        :header-rows: 1
+        :align: center
+        :widths: auto
+
+        * - ``forwarded-allow-ips``
+          - Secure Request Headers
+          - Result
+          - Explanation
+        * - .. code::
+
+                ["127.0.0.1"]
+          - .. code::
+
+                X-Forwarded-Proto: https
+          - .. code::
+
+                wsgi.url_scheme = "http"
+          - IP address was not allowed
+        * - .. code::
+
+                "*"
+          - <none>
+          - .. code::
+
+                wsgi.url_scheme = "http"
+          - IP address allowed, but no secure headers provided
+        * - .. code::
+
+                "*"
+          - .. code::
+
+                X-Forwarded-Proto: https
+          - .. code::
+
+                wsgi.url_scheme = "https"
+          - IP address allowed, one request header matched
+        * - .. code::
+
+                ["134.213.44.18"]
+          - .. code::
+
+                X-Forwarded-Ssl: on
+                X-Forwarded-Proto: http
+          - ``InvalidSchemeHeaders()`` raised
+          - IP address allowed, but the two secure headers disagreed on if HTTPS was used
+
 .. _pythonpath:
 
 ``pythonpath``
 ~~~~~~~~~~~~~~
 
 **Command line:** ``--pythonpath STRING``
 
@@ -1336,16 +1474,17 @@
 
 The number of worker processes for handling requests.
 
 A positive integer generally in the ``2-4 x $(NUM_CORES)`` range.
 You'll want to vary this a bit to find the best for your particular
 application's work load.
 
-By default, the value of the ``WEB_CONCURRENCY`` environment variable.
-If it is not defined, the default is ``1``.
+By default, the value of the ``WEB_CONCURRENCY`` environment variable,
+which is set by some Platform-as-a-Service providers such as Heroku. If
+it is not defined, the default is ``1``.
 
 .. _worker-class:
 
 ``worker_class``
 ~~~~~~~~~~~~~~~~
 
 **Command line:** ``-k STRING`` or ``--worker-class STRING``
@@ -1409,15 +1548,15 @@
 
 **Command line:** ``--worker-connections INT``
 
 **Default:** ``1000``
 
 The maximum number of simultaneous clients.
 
-This setting only affects the Eventlet and Gevent worker types.
+This setting only affects the ``gthread``, ``eventlet`` and ``gevent`` worker types.
 
 .. _max-requests:
 
 ``max_requests``
 ~~~~~~~~~~~~~~~~
 
 **Command line:** ``--max-requests INT``
```

### Comparing `gunicorn-20.1.0/docs/source/custom.rst` & `gunicorn-21.0.0/docs/source/custom.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/index.rst` & `gunicorn-21.0.0/docs/source/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ======================
 
 .. image:: _static/gunicorn.png
 
 :Website: http://gunicorn.org
 :Source code: https://github.com/benoitc/gunicorn
 :Issue tracker: https://github.com/benoitc/gunicorn/issues
-:IRC: ``#gunicorn`` on Freenode
+:IRC: ``#gunicorn`` on Libera Chat
 :Usage questions: https://github.com/benoitc/gunicorn/issues
 
 Gunicorn 'Green Unicorn' is a Python WSGI HTTP Server for UNIX. It's a pre-fork
 worker model ported from Ruby's Unicorn project. The Gunicorn server is broadly
 compatible with various web frameworks, simply implemented, light on server
 resources, and fairly speedy.
```

### Comparing `gunicorn-20.1.0/docs/source/2018-news.rst` & `gunicorn-21.0.0/docs/source/2018-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/2019-news.rst` & `gunicorn-21.0.0/docs/source/2019-news.rst`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 - Fixed setting max_requests
 - Bump minimum Eventlet and Gevent versions to 0.24 and 1.4
 - Use Python default SSL cipher list by default
 - handle `wsgi.input_terminated` extension
 - Simplify Paste Deployment documentation
 - Fix root logging: root and logger are same level.
 - Fixed typo in ssl_version documentation
-- Documented  systemd deployement unit examples
+- Documented  systemd deployment unit examples
 - Added systemd sd_notify support
 - Fixed typo in gthread.py
 - Added `tornado <https://www.tornadoweb.org/>`_ 5 and  6 support
 - Declare our setuptools dependency
 - Added support to `--bind` to open file descriptors
 - Document how to serve WSGI app modules from Gunicorn
 - Provide guidance on X-Forwarded-For access log in documentation
```

### Comparing `gunicorn-20.1.0/docs/source/news.rst` & `gunicorn-21.0.0/docs/source/2021-news.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,54 @@
-=========
-Changelog
-=========
+================
+Changelog - 2021
+================
+
+.. note::
+
+   Please see :doc:`news` for the latest changes
 
 20.1.0 - 2021-02-12
 ===================
 
 - document WEB_CONCURRENCY is set by, at least, Heroku
-- capture peername from accept: Avoid calls to getpeername by capturing the peer name returned by accept
+- capture peername from accept: Avoid calls to getpeername by capturing the peer name returned by
+  accept
 - log a warning when a worker was terminated due to a signal
 - fix tornado usage with latest versions of Django 
 - add support for python -m gunicorn
 - fix systemd socket activation example
-- allows to set wsgi application in configg file using ``wsgi_app``
-- document ``--timeout = 0``
+- allows to set wsgi application in configg file using `wsgi_app`
+- document `--timeout = 0`
 - always close a connection when the number of requests exceeds the max requests
 - Disable keepalive during graceful shutdown
 - kill tasks in the gthread workers during upgrade
 - fix latency in gevent worker when accepting new requests
 - fix file watcher: handle errors when new worker reboot and ensure the list of files is kept
 - document the default name and path of the configuration file
 - document how variable impact configuration
-- document the ``$PORT`` environment variable
+- document the `$PORT` environment variable
 - added milliseconds option to request_time in access_log
 - added PIP requirements to be used for example
 - remove version from the Server header
-- fix sendfile: use ``socket.sendfile`` instead of ``os.sendfile``
-- reloader: use  absolute path to prevent empty to prevent0 ``InotifyError`` when a file 
+- fix sendfile: use `socket.sendfile` instead of `os.sendfile`
+- reloader: use  absolute path to prevent empty to prevent0 `InotifyError` when a file 
   is added to the working directory
 - Add --print-config option to print the resolved settings at startup.
-- remove the ``--log-dict-config`` CLI flag because it never had a working format
-  (the ``logconfig_dict`` setting in configuration files continues to work)
+- remove the `--log-dict-config` CLI flag because it never had a working format
+  (the `logconfig_dict` setting in configuration files continues to work)
+
 
 ** Breaking changes **
 
 - minimum version is Python 3.5
 - remove version from the Server header 
 
+** Documentation **
+
+
+
 ** Others **
 
 - miscellaneous changes in the code base to be a better citizen with Python 3
 - remove dead code
 - fix documentation generation
 
-
-History
-=======
-
-.. toctree::
-   :titlesonly:
-
-   2020-news
-   2019-news
-   2018-news
-   2017-news
-   2016-news
-   2015-news
-   2014-news
-   2013-news
-   2012-news
-   2011-news
-   2010-news
-
```

### Comparing `gunicorn-20.1.0/docs/source/design.rst` & `gunicorn-21.0.0/docs/source/design.rst`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,23 @@
 For full greenlet support applications might need to be adapted.
 When using, e.g., Gevent_ and Psycopg_ it makes sense to ensure psycogreen_ is
 installed and `setup <http://www.gevent.org/api/gevent.monkey.html#plugins>`_.
 
 Other applications might not be compatible at all as they, e.g., rely on
 the original unpatched behavior.
 
+Gthread Workers
+---------------
+
+The worker `gthread` is a threaded worker. It accepts connections in the
+main loop. Accepted connections are added to the thread pool as a
+connection job. On keepalive connections are put back in the loop
+waiting for an event. If no event happens after the keepalive timeout,
+the connection is closed.
+
 Tornado Workers
 ---------------
 
 There's also a Tornado worker class. It can be used to write applications using
 the Tornado framework. Although the Tornado workers are capable of serving a
 WSGI application, this is not a recommended configuration.
 
@@ -64,20 +73,14 @@
 .. _asyncio-workers:
 
 AsyncIO Workers
 ---------------
 
 These workers are compatible with Python 3.
 
-The worker `gthread` is a threaded worker. It accepts connections in the
-main loop, accepted connections are added to the thread pool as a
-connection job. On keepalive connections are put back in the loop
-waiting for an event. If no event happen after the keep alive timeout,
-the connection is closed.
-
 You can port also your application to use aiohttp_'s ``web.Application`` API and use the
 ``aiohttp.worker.GunicornWebWorker`` worker.
 
 Choosing a Worker Type
 ======================
 
 The default synchronous workers assume that your application is resource-bound
@@ -147,8 +150,8 @@
 .. _Greenlets: https://github.com/python-greenlet/greenlet
 .. _Eventlet: http://eventlet.net/
 .. _Gevent: http://www.gevent.org/
 .. _Hey: https://github.com/rakyll/hey
 .. _aiohttp: https://docs.aiohttp.org/en/stable/deployment.html#nginx-gunicorn
 .. _`example`: https://github.com/benoitc/gunicorn/blob/master/examples/frameworks/flaskapp_aiohttp_wsgi.py
 .. _Psycopg: http://initd.org/psycopg/
-.. _psycogreen: https://bitbucket.org/dvarrazzo/psycogreen
+.. _psycogreen: https://github.com/psycopg/psycogreen/
```

### Comparing `gunicorn-20.1.0/docs/source/signals.rst` & `gunicorn-21.0.0/docs/source/signals.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/2012-news.rst` & `gunicorn-21.0.0/docs/source/2012-news.rst`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 - more fixes in django settings resolutions
 - fix gevent.core import
 - fix keepalive=0 in eventlet worker
 - fix handle_error display with the unix worker
 - fix tornado.wsgi.WSGIApplication calling error
 
 - **breaking change**: take the control on graceful reload back.
-  graceful can't be overrided anymore using the on_reload function.
+  graceful can't be overridden anymore using the on_reload function.
 
 0.14.3 / 2012-05-15
 -------------------
 
 - improvement: performance of http.body.Body.readline()
 - improvement: log HTTP errors in access log like Apache
 - improvement: display traceback when the worker fails to boot
```

### Comparing `gunicorn-20.1.0/docs/source/2013-news.rst` & `gunicorn-21.0.0/docs/source/2013-news.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,26 +34,26 @@
 - fix graceful timeout with the Eventlet worker
 - fix: don't raise an error when closing the socket if already closed
 - fix: fix --settings parameter for django application and try to find
   the django settings when using the ``gunicorn`` command.
 - fix: give the initial global_conf to paster application
 - fix: fix 'Expect: 100-continue' support on Python 3
 
-New versionning:
+New versioning:
 ++++++++++++++++
 
-With this release, the versionning of Gunicorn is changing. Gunicorn is
+With this release, the versioning of Gunicorn is changing. Gunicorn is
 stable since a long time and there is no point to release a "1.0" now.
 It should have been done since a long time. 0.17 really meant it was the
 17th stable version. From the beginning we have only 2 kind of
 releases:
 
 major release: releases with major changes or huge features added
 services releases: fixes and minor features added So from now we will
-apply the following versionning ``<major>.<service>``. For example ``17.5`` is a
+apply the following versioning ``<major>.<service>``. For example ``17.5`` is a
 service release.
 
 0.17.4 / 2013-04-24
 -------------------
 
 - fix unix socket address parsing
```

### Comparing `gunicorn-20.1.0/docs/source/conf.py` & `gunicorn-21.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/2015-news.rst` & `gunicorn-21.0.0/docs/source/2015-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/2014-news.rst` & `gunicorn-21.0.0/docs/source/2014-news.rst`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 - fix: don't install the worker if python < 3.3
 - fix :issue:`822`: Support UNIX sockets in gaiohttp worker
 
 
 Async worker
 ++++++++++++
 
-- fix :issue:`790`: StopIteration shouldn't be catched at this level.
+- fix :issue:`790`: StopIteration shouldn't be caught at this level.
 
 
 Logging
 +++++++
 
 - add statsd logging handler fix :issue:`748`
 
@@ -176,15 +176,15 @@
   the arguments of the command line. It allows you to :ref:`embed gunicorn in
   your own application <custom>`.
 - improve: set wsgi.multithread to True for async workers
 - fix logging: make sure to redirect wsgi.errors when needed
 - add: syslog logging can now be done to a unix socket
 - fix logging: don't try to redirect stdout/stderr to the logfile.
 - fix logging: don't propagate log
-- improve logging: file option can be overriden by the gunicorn options
+- improve logging: file option can be overridden by the gunicorn options
   `--error-logfile` and `--access-logfile` if they are given.
 - fix: don't override SERVER_* by the Host header
 - fix: handle_error
 - add more option to configure SSL
 - fix: sendfile with SSL
 - add: worker_int callback (to react on SIGTERM)
 - fix: don't depend on entry point for internal classes, now absolute
```

### Comparing `gunicorn-20.1.0/docs/source/deploy.rst` & `gunicorn-21.0.0/docs/source/deploy.rst`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,30 @@
       proxy_redirect off;
       proxy_buffering off;
 
       proxy_pass http://app_server;
   }
   ...
 
+If you want to ignore aborted requests like health check of Load Balancer, some
+of which close the connection without waiting for a response, you need to turn
+on `ignoring client abort`_.
+
+To ignore aborted requests, you only need to add
+``proxy_ignore_client_abort on;`` to your ``location`` block::
+
+    ...
+    proxy_ignore_client_abort on;
+    ...
+
+.. note::
+    The default value of ``proxy_ignore_client_abort`` is ``off``. Error code
+    499 may appear in Nginx log and ``Ignoring EPIPE`` may appear in Gunicorn
+    log if loglevel is set to ``debug``.
+
 It is recommended to pass protocol information to Gunicorn. Many web
 frameworks use this information to generate URLs. Without this
 information, the application may mistakenly generate 'http' URLs in
 'https' responses, leading to mixed content warnings or broken
 applications. To configure Nginx to pass an appropriate header, add
 a ``proxy_set_header`` directive to your ``location`` block::
 
@@ -212,15 +228,15 @@
 Systemd
 -------
 
 A tool that is starting to be common on linux systems is Systemd_. It is a
 system services manager that allows for strict process management, resources
 and permissions control.
 
-Below are configurations files and instructions for using systemd to create
+Below are configuration files and instructions for using systemd to create
 a unix socket for incoming Gunicorn requests.  Systemd will listen on this
 socket and start gunicorn automatically in response to traffic.  Later in
 this section are instructions for configuring Nginx to forward web traffic
 to the newly created unix socket:
 
 **/etc/systemd/system/gunicorn.service**::
 
@@ -353,7 +369,8 @@
 .. _Supervisor: http://supervisord.org/
 .. _`simple configuration`: https://github.com/benoitc/gunicorn/blob/master/examples/supervisor.conf
 .. _`configuration documentation`: http://docs.gunicorn.org/en/latest/settings.html#logging
 .. _`logging configuration file`: https://github.com/benoitc/gunicorn/blob/master/examples/logging.conf
 .. _Virtualenv: https://pypi.python.org/pypi/virtualenv
 .. _Systemd: https://www.freedesktop.org/wiki/Software/systemd/
 .. _Gaffer: https://gaffer.readthedocs.io/
+.. _`ignoring client abort`: http://nginx.org/en/docs/http/ngx_http_proxy_module.html#proxy_ignore_client_abort
```

### Comparing `gunicorn-20.1.0/docs/source/community.rst` & `gunicorn-21.0.0/docs/source/community.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 for 3 different purposes:
 
   * `Bug tracker <https://github.com/benoitc/gunicorn/projects/2>`_ : to check latest bug 
   * `Forum <https://github.com/benoitc/gunicorn/projects/4>`_ : Stackoverflow-style questions about Gunicorn usage
   * `Mailing list <https://github.com/benoitc/gunicorn/projects/3>`_ : Discussion of Gunicorn development, new features
     and project management.  
 
-Project maintenance guidelines are avaible on the `wiki <https://github.com/benoitc/gunicorn/wiki/Project-management>`_
+Project maintenance guidelines are available on the `wiki <https://github.com/benoitc/gunicorn/wiki/Project-management>`_
 .
 
 IRC
 ===
 
 The Gunicorn channel is on the `Freenode <http://freenode.net/>`_ IRC
 network. You can chat with other on `#gunicorn channel
```

### Comparing `gunicorn-20.1.0/docs/source/_static/gunicorn.png` & `gunicorn-21.0.0/docs/source/_static/gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/2011-news.rst` & `gunicorn-21.0.0/docs/source/2011-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/2010-news.rst` & `gunicorn-21.0.0/docs/source/2010-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/instrumentation.rst` & `gunicorn-21.0.0/docs/source/instrumentation.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/run.rst` & `gunicorn-21.0.0/docs/source/run.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/configure.rst` & `gunicorn-21.0.0/docs/source/configure.rst`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 usual::
 
     $ gunicorn -h
 
 There is also a ``--version`` flag available to the command line scripts that
 isn't mentioned in the list of :ref:`settings <settings>`.
 
+.. _configuration_file:
 
 Configuration File
 ==================
 
 The configuration file should be a valid Python source file with a **python
 extension** (e.g. `gunicorn.conf.py`). It only needs to be readable from the
 file system. More specifically, it does not have to be on the module path
```

### Comparing `gunicorn-20.1.0/docs/source/2016-news.rst` & `gunicorn-21.0.0/docs/source/2016-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/2017-news.rst` & `gunicorn-21.0.0/docs/source/2017-news.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/source/faq.rst` & `gunicorn-21.0.0/docs/source/faq.rst`

 * *Files 4% similar despite different names*

```diff
@@ -125,17 +125,21 @@
 How can I increase the maximum number of file descriptors?
 ----------------------------------------------------------
 
 One of the first settings that usually needs to be bumped is the maximum number
 of open file descriptors for a given process. For the confused out there,
 remember that Unices treat sockets as files.
 
-::
+.. warning:: ``sudo ulimit`` may not work
+
+Considering non-privileged users are not able to relax the limit, you should
+firstly switch to root user, increase the limit, then run gunicorn. Using ``sudo
+ulimit`` would not take effect.
 
-    $ sudo ulimit -n 2048
+Try systemd's service unit file, or an initscript which runs as root.
 
 How can I increase the maximum socket backlog?
 ----------------------------------------------
 
 Listening sockets have an associated queue of incoming connections that are
 waiting to be accepted. If you happen to have a stampede of clients that fill
 up this queue new connections will eventually start getting dropped.
@@ -212,15 +216,15 @@
 A sometimes subtle problem to debug is when a worker process is killed and there
 is little logging information about what happened.
 
 If you use a reverse proxy like NGINX you might see 502 returned to a client.
 
 In the gunicorn logs you might simply see ``[35] [INFO] Booting worker with pid: 35``
 
-It's completely normal for workers to be killed and startup, for example due to
+It's completely normal for workers to be stop and start, for example due to
 max-requests setting. Ordinarily gunicorn will capture any signals and log something.
 
 This particular failure case is usually due to a SIGKILL being received, as it's
 not possible to catch this signal silence is usually a common side effect! A common
 cause of SIGKILL is when OOM killer terminates a process due to low memory condition.
 
 This is increasingly common in container deployments where memory limits are enforced
```

### Comparing `gunicorn-20.1.0/docs/sitemap_gen.py` & `gunicorn-21.0.0/docs/sitemap_gen.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/gunicorn_ext.py` & `gunicorn-21.0.0/docs/gunicorn_ext.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 
     with open(settings_file, 'w') as settings:
         settings.write(HEAD)
         settings.write(''.join(ret))
 
 
 def fmt_setting(s):
-    if callable(s.default):
+    if hasattr(s, "default_doc"):
+        val = s.default_doc
+    elif callable(s.default):
         val = inspect.getsource(s.default)
         val = "\n".join("    %s" % line for line in val.splitlines())
         val = "\n\n.. code-block:: python\n\n" + val
     elif s.default == '':
         val = "``''``"
     else:
         val = "``%r``" % s.default
```

### Comparing `gunicorn-20.1.0/docs/make.bat` & `gunicorn-21.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/logo/gunicorn.png` & `gunicorn-21.0.0/docs/logo/gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/logo/gunicorn.svg` & `gunicorn-21.0.0/docs/logo/gunicorn.svg`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/index.html` & `gunicorn-21.0.0/docs/site/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 </head>
 <body>
   <div class="logo-wrapper">
     <div class="logo-div">
       <div class="latest">
         Latest version: <strong><a
-            href="https://docs.gunicorn.org/en/stable/">20.0.4</a></strong>
+            href="https://docs.gunicorn.org/en/stable/">20.1.0</a></strong>
       </div>
 
       <div class="logo"><img src="images/logo.jpg" ></div>
     </div>
   </div>
   <div class="banner-wrapper">
     <div class="banner">
@@ -114,19 +114,19 @@
         <h1>Project Management</h1>
         <p><strong>Gunicorn</strong> uses <a href="https://github.com/benoitc/gunicorn/projects">GitHub for the project management</a>. GitHub issues are used for 3 different purposes:</p>
         <ul>
           <li><a href="https://github.com/benoitc/gunicorn/projects/2">Bug tracker</a></li>
           <li><a href="https://github.com/benoitc/gunicorn/projects/4">Forum</a></li>
           <li><a href="https://github.com/benoitc/gunicorn/projects/3">Mailing list</a>
         </ul>
-        <p>Project maintenance guidelines are avaible on the <a href="https://github.com/benoitc/gunicorn/wiki/Project-management">wiki</a></p>
+        <p>Project maintenance guidelines are available on the <a href="https://github.com/benoitc/gunicorn/wiki/Project-management">wiki</a></p>
         
-        <h1>Irc</h1>
-        <p>The Gunicorn channel is on the <a href="http://freenode.net/">Freenode</a> IRC
-          network. You can chat with the community on the <a href="http://webchat.freenode.net/?channels=gunicorn">#gunicorn channel</a>.</p>
+        <h1>IRC</h1>
+        <p>The Gunicorn channel is on the <a href="https://libera.chat/">Libera Chat</a> IRC
+          network. You can chat with the community on the <a href="https://web.libera.chat/?channels=#gunicorn">#gunicorn channel</a>.</p>
 
         <h1>Issue Tracking</h1>
         <p>Bug reports, enhancement requests and tasks generally go in the <a  href="http://github.com/benoitc/gunicorn/issues">Github
           issue tracker</a>.</p>
 
         <h1>Security Issues</h1>
         <p>The security mailing list is a place to report security issues. Only
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 
 
 
-Latest version: 20.0.4
+Latest version: 20.1.0
 [images/logo.jpg]
 [images/title.png]
 ****** Gunicorn 'Green Unicorn' is a Python WSGI HTTP Server for UNIX. It's a
 pre-fork worker model. The Gunicorn server is broadly compatible with various
 web frameworks, simply implemented, light on server resources, and fairly
 speedy. ******
 View_source Download
@@ -57,17 +57,17 @@
 Read the full documentation at docs.gunicorn.org
 ****** Project Management ******
 Gunicorn uses GitHub_for_the_project_management. GitHub issues are used for 3
 different purposes:
     * Bug_tracker
     * Forum
     * Mailing_list
-Project maintenance guidelines are avaible on the wiki
-****** Irc ******
-The Gunicorn channel is on the Freenode IRC network. You can chat with the
+Project maintenance guidelines are available on the wiki
+****** IRC ******
+The Gunicorn channel is on the Libera_Chat IRC network. You can chat with the
 community on the #gunicorn_channel.
 ****** Issue Tracking ******
 Bug reports, enhancement requests and tasks generally go in the Github_issue
 tracker.
 ****** Security Issues ******
 The security mailing list is a place to report security issues. Only developers
 are subscribed to it. To post a message to the list use the address
```

### Comparing `gunicorn-20.1.0/docs/site/css/style.css` & `gunicorn-21.0.0/docs/site/css/style.css`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/title.png` & `gunicorn-21.0.0/docs/site/images/title.png`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/community.jpg` & `gunicorn-21.0.0/docs/site/images/community.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/downloads.jpg` & `gunicorn-21.0.0/docs/site/images/downloads.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/redbutton.jpg` & `gunicorn-21.0.0/docs/site/images/redbutton.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/documents.jpg` & `gunicorn-21.0.0/docs/site/images/documents.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/favicon.png` & `gunicorn-21.0.0/docs/site/images/favicon.png`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/user1.jpg` & `gunicorn-21.0.0/docs/site/images/user1.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/logo.jpg` & `gunicorn-21.0.0/docs/site/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/logo.png` & `gunicorn-21.0.0/docs/site/images/logo.png`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/gunicorn.png` & `gunicorn-21.0.0/docs/site/images/gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/logo-bottom.png` & `gunicorn-21.0.0/docs/site/images/logo-bottom.png`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/banner-bg.jpg` & `gunicorn-21.0.0/docs/site/images/banner-bg.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/about.jpg` & `gunicorn-21.0.0/docs/site/images/about.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/footer-logo.jpg` & `gunicorn-21.0.0/docs/site/images/footer-logo.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/images/large_gunicorn.png` & `gunicorn-21.0.0/docs/site/images/large_gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/js/main.js` & `gunicorn-21.0.0/docs/site/js/main.js`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/docs/site/sitemap.xml` & `gunicorn-21.0.0/docs/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/NOTICE` & `gunicorn-21.0.0/NOTICE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Gunicorn
 
-2009-2018 (c) Benoît Chesneau <benoitc@e-engura.org>
+2009-2023 (c) Benoît Chesneau <benoitc@gunicorn.org>
 2009-2015 (c) Paul J. Davis <paul.joseph.davis@gmail.com>
 
 Gunicorn is released under the MIT license. See the LICENSE
 file for the complete license.
 
 gunicorn.logging_config
 -----------------------
@@ -82,8 +82,8 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 
 util/unlink.py
 --------------
 
-backport frop python3 Lib/test/support.py
+backport from python3 Lib/test/support.py
```

### Comparing `gunicorn-20.1.0/setup.py` & `gunicorn-21.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: Implementation :: CPython',
     'Programming Language :: Python :: Implementation :: PyPy',
     'Topic :: Internet',
     'Topic :: Utilities',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet :: WWW/HTTP',
@@ -65,19 +67,16 @@
     def run_tests(self):
         import pytest
         errno = pytest.main(self.test_args)
         sys.exit(errno)
 
 
 install_requires = [
-    # We depend on functioning pkg_resources.working_set.add_entry() and
-    # pkg_resources.load_entry_point(). These both work as of 3.0 which
-    # is the first version to support Python 3.4 which we require as a
-    # floor.
-    'setuptools>=3.0',
+    'importlib_metadata; python_version<"3.8"',
+    'packaging',
 ]
 
 extras_require = {
     'gevent':  ['gevent>=1.4.0'],
     'eventlet': ['eventlet>=0.24.1'],
     'tornado': ['tornado>=0.2'],
     'gthread': [],
@@ -87,15 +86,15 @@
 setup(
     name='gunicorn',
     version=__version__,
 
     description='WSGI HTTP Server for UNIX',
     long_description=long_description,
     author='Benoit Chesneau',
-    author_email='benoitc@e-engura.com',
+    author_email='benoitc@gunicorn.org',
     license='MIT',
     url='https://gunicorn.org',
     project_urls={
         'Documentation': 'https://docs.gunicorn.org',
         'Homepage': 'https://gunicorn.org',
         'Issue tracker': 'https://github.com/benoitc/gunicorn/issues',
         'Source code': 'https://github.com/benoitc/gunicorn',
```

### Comparing `gunicorn-20.1.0/examples/multidomainapp.py` & `gunicorn-21.0.0/examples/multidomainapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/websocket/gevent_websocket.py` & `gunicorn-21.0.0/examples/websocket/gevent_websocket.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/websocket/websocket.html` & `gunicorn-21.0.0/examples/websocket/websocket.html`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/websocket/websocket.py` & `gunicorn-21.0.0/examples/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/server.key` & `gunicorn-21.0.0/examples/server.key`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/sendfile.py` & `gunicorn-21.0.0/examples/sendfile.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/timeout.py` & `gunicorn-21.0.0/examples/timeout.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/alt_spec.py` & `gunicorn-21.0.0/examples/alt_spec.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/deep/test.py` & `gunicorn-21.0.0/examples/deep/test.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/test.py` & `gunicorn-21.0.0/examples/test.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/logging.conf` & `gunicorn-21.0.0/examples/logging.conf`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/server.crt` & `gunicorn-21.0.0/examples/server.crt`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/longpoll.py` & `gunicorn-21.0.0/examples/longpoll.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/multiapp.py` & `gunicorn-21.0.0/examples/multiapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/standalone_app.py` & `gunicorn-21.0.0/examples/standalone_app.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/when_ready.conf.py` & `gunicorn-21.0.0/examples/when_ready.conf.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/readline_app.py` & `gunicorn-21.0.0/examples/readline_app.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/slowclient.py` & `gunicorn-21.0.0/examples/slowclient.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/nginx.conf` & `gunicorn-21.0.0/examples/nginx.conf`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/frameworks/tornadoapp.py` & `gunicorn-21.0.0/examples/frameworks/tornadoapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/frameworks/django/testing/testing/settings.py` & `gunicorn-21.0.0/examples/frameworks/django/testing/testing/settings.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/frameworks/django/testing/testing/urls.py` & `gunicorn-21.0.0/examples/frameworks/django/testing/testing/urls.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html` & `gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/middleware.py` & `gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/middleware.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/frameworks/django/testing/testing/apps/someapp/views.py` & `gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/views.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/frameworks/django/testing/testing/wsgi.py` & `gunicorn-21.0.0/examples/frameworks/django/testing/testing/wsgi.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/echo.py` & `gunicorn-21.0.0/examples/echo.py`

 * *Files identical despite different names*

### Comparing `gunicorn-20.1.0/examples/example_config.py` & `gunicorn-21.0.0/examples/example_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -210,7 +210,31 @@
                 lineno, name))
             if line:
                 code.append("  %s" % (line.strip()))
     worker.log.debug("\n".join(code))
 
 def worker_abort(worker):
     worker.log.info("worker received SIGABRT signal")
+
+def ssl_context(conf, default_ssl_context_factory):
+    import ssl
+
+    # The default SSLContext returned by the factory function is initialized
+    # with the TLS parameters from config, including TLS certificates and other
+    # parameters.
+    context = default_ssl_context_factory()
+
+    # The SSLContext can be further customized, for example by enforcing
+    # minimum TLS version.
+    context.minimum_version = ssl.TLSVersion.TLSv1_3
+
+    # Server can also return different server certificate depending which
+    # hostname the client uses. Requires Python 3.7 or later.
+    def sni_callback(socket, server_hostname, context):
+        if server_hostname == "foo.127.0.0.1.nip.io":
+            new_context = default_ssl_context_factory()
+            new_context.load_cert_chain(certfile="foo.pem", keyfile="foo-key.pem")
+            socket.context = new_context
+
+    context.sni_callback = sni_callback
+
+    return context
```

### Comparing `gunicorn-20.1.0/THANKS` & `gunicorn-21.0.0/THANKS`

 * *Files 6% similar despite different names*

```diff
@@ -18,31 +18,34 @@
 Anand Chitipothu <anandology@gmail.com>
 Andreas Stührk <andy-python@hammerhartes.de>
 Andrew Burdo <zeezooz@gmail.com>
 Andrew Svetlov <andrew.svetlov@gmail.com>
 Anil V <avaitla16@gmail.com>
 Antoine Girard <antoine.girard.dev@gmail.com>
 Anton Vlasenko <antares.spica@gmail.com>
+Artur Kruchinin <arturkruchinin@gmail.com>
 Bartosz Oler <bartosz@bzimage.us>
 Ben Cochran <bcochran@gmail.com>
 Ben Oswald <ben.oswald@root-space.de>
 Benjamin Gilbert <bgilbert@backtick.net>
+Benny Mei <meibenny@gmail.com>
 Benoit Chesneau <bchesneau@gmail.com>
 Berker Peksag <berker.peksag@gmail.com>
 bninja <andrew@poundpay.com>
 Bob Hagemann <bob+code@twilio.com>
 Bobby Beckmann <bobby@macs-MacBook-Pro.local>
 Brett Randall <javabrett@gmail.com>
 Brian Rosner <brosner@gmail.com>
 Bruno Bigras <bigras.bruno@gmail.com>
 Caleb Brown <git@calebbrown.id.au>
 Chris Adams <chris@improbable.org>
 Chris Forbes <chrisf@ijw.co.nz>
 Chris Lamb <lamby@debian.org>
 Chris Streeter <chris@chrisstreeter.com>
+Christian Clauss <cclauss@me.com>
 Christoph Heer <Christoph.Heer@gmail.com>
 Christos Stavrakakis <cstavr@grnet.gr>
 CMGS <ilskdw@mspil.edu.cn>
 Curt Micol <asenchi@asenchi.com>
 Dan Callaghan <dcallagh@redhat.com>
 Dan Sully <daniel-github@electricrain.com>
 Daniel Quinn <code@danielquinn.org>
@@ -99,20 +102,22 @@
 Kevin Littlejohn <kevin@littlejohn.id.au>
 Kevin Luikens <kluikens@gmail.com>
 Kirill Zaborsky <qrilka@gmail.com>
 Konstantin Kapustin <sirkonst@gmail.com>
 kracekumar <kracethekingmaker@gmail.com>
 Kristian Glass <git@doismellburning.co.uk>
 Kristian Øllegaard <kristian.ollegaard@divio.ch>
+Krystian <chrisjozwik@outlook.com>
 Krzysztof Urbaniak <urban@fail.pl>
 Kyle Kelley <rgbkrk@gmail.com>
 Kyle Mulka <repalviglator@yahoo.com>
 Lars Hansson <romabysen@gmail.com>
 Leonardo Santagada <santagada@gmail.com>
 Levi Gross <levi@levigross.com>
+licunlong <shenxiaogll@163.com>
 Łukasz Kucharski <lkucharski@leon.pl>
 Mahmoud Hashemi <mahmoudrhashemi@gmail.com>
 Malthe Borch <mborch@gmail.com>
 Marc Abramowitz <marc@marc-abramowitz.com>
 Marc Abramowitz <msabramo@gmail.com>
 Mark Adams <mark@markadams.me>
 Matt Behrens <askedrelic@gmail.com>
@@ -149,26 +154,29 @@
 Randall Leeds <randall@meebo-inc.com>
 Raphaël Slinckx <rslinckx@gmail.com>
 Rhys Powell <rhys@rhyspowell.com>
 Rik <rvachterberg@gmail.com>
 Ronan Amicel <ronan.amicel@gmail.com>
 Ryan Peck <ryan@rypeck.com>
 Saeed Gharedaghi <saeed.ghx68@gmail.com>
+Samuel Matos <samypr100@users.noreply.github.com>
 Sergey Rublev <narma.nsk@gmail.com>
 Shane Reustle <me@shanereustle.com>
 shouse-cars <shouse@cars.com>
 sib <andrew.sibley@gmail.com>
 Simon Lundmark <simon.lundmark@gmail.com>
 Stephane Wirtel <stephane@wirtel.be>
 Stephen DiCato <Locker537@gmail.com>
 Stephen Holsapple <sholsapp@gmail.com>
 Steven Cummings <estebistec@gmail.com>
 Sébastien Fievet <zyegfryed@gmail.com>
+Tal Einat <532281+taleinat@users.noreply.github.com>
 Talha Malik <talham7391@hotmail.com>
 TedWantsMore <TedWantsMore@gmx.com>
+Teko012 <112829523+Teko012@users.noreply.github.com>
 Thomas Grainger <tagrain@gmail.com>
 Thomas Steinacher <tom@eggdrop.ch>
 Travis Cline <travis.cline@gmail.com>
 Travis Swicegood <development@domain51.com>
 Trey Long <trey@ktrl.com>
 W. Trevor King <wking@tremily.us>
 Wojtek <wojtek@monodev.com>
```

