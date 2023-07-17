# Comparing `tmp/ural-0.9.0.tar.gz` & `tmp/ural-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ural-0.9.0.tar", last modified: Thu Sep 12 14:48:18 2019, max compression
+gzip compressed data, was "dist/ural-1.0.0a1.tar", last modified: Mon Jul 17 11:03:20 2023, max compression
```

## Comparing `ural-0.9.0.tar` & `ural-1.0.0a1.tar`

### file list

```diff
@@ -1,35 +1,94 @@
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-09-12 14:48:18.000000 ural-0.9.0/
--rw-r--r--   0 Yomgui     (501) staff       (20)    11013 2019-09-12 14:48:18.000000 ural-0.9.0/PKG-INFO
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/
--rw-r--r--   0 Yomgui     (501) staff       (20)    11013 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/PKG-INFO
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2019-09-12 14:47:54.000000 ural-0.9.0/ural.egg-info/zip-safe
--rw-r--r--   0 Yomgui     (501) staff       (20)      627 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/SOURCES.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)       49 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/entry_points.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)       48 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/requires.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        5 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/top_level.txt
--rw-r--r--   0 Yomgui     (501) staff       (20)        1 2019-09-12 14:48:18.000000 ural-0.9.0/ural.egg-info/dependency_links.txt
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-09-12 14:48:18.000000 ural-0.9.0/ural/
--rw-r--r--   0 Yomgui     (501) staff       (20)     1569 2019-04-03 13:45:15.000000 ural-0.9.0/ural/normalized_lru_from_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      820 2019-04-17 12:03:58.000000 ural-0.9.0/ural/is_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      710 2018-12-13 17:12:14.000000 ural-0.9.0/ural/patterns.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      841 2018-12-14 10:39:22.000000 ural-0.9.0/ural/urls_from_html.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      690 2019-05-13 14:14:51.000000 ural-0.9.0/ural/__init__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      931 2018-12-13 17:12:14.000000 ural-0.9.0/ural/force_protocol.py
-drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2019-09-12 14:48:18.000000 ural-0.9.0/ural/cli/
--rw-r--r--   0 Yomgui     (501) staff       (20)      749 2019-04-17 12:17:03.000000 ural-0.9.0/ural/cli/domain.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1116 2019-01-12 17:44:10.000000 ural-0.9.0/ural/cli/normalize.py
--rw-r--r--   0 Yomgui     (501) staff       (20)        0 2019-01-12 17:44:10.000000 ural-0.9.0/ural/cli/__init__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1806 2019-02-21 10:04:26.000000 ural-0.9.0/ural/cli/join.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      423 2019-01-12 17:44:10.000000 ural-0.9.0/ural/cli/utils.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     4022 2019-04-17 12:18:34.000000 ural-0.9.0/ural/cli/__main__.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     2272 2019-09-12 14:44:13.000000 ural-0.9.0/ural/facebook.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     1538 2019-04-03 13:45:18.000000 ural-0.9.0/ural/lru_from_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      547 2018-11-12 15:03:34.000000 ural-0.9.0/ural/strip_protocol.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     6144 2019-06-25 15:30:43.000000 ural-0.9.0/ural/normalize_url.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      875 2019-05-13 14:14:55.000000 ural-0.9.0/ural/ensure_protocol.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      656 2018-12-14 10:39:37.000000 ural-0.9.0/ural/urls_from_text.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      566 2019-04-17 12:08:35.000000 ural-0.9.0/ural/get_domain_name.py
--rw-r--r--   0 Yomgui     (501) staff       (20)      930 2019-02-21 10:04:26.000000 ural-0.9.0/ural/lru_trie.py
--rw-r--r--   0 Yomgui     (501) staff       (20)     7944 2019-09-12 14:39:48.000000 ural-0.9.0/README.md
--rw-r--r--   0 Yomgui     (501) staff       (20)      889 2019-09-12 14:46:58.000000 ural-0.9.0/setup.py
--rw-r--r--   0 Yomgui     (501) staff       (20)       38 2019-09-12 14:48:18.000000 ural-0.9.0/setup.cfg
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-07-17 11:03:20.000000 ural-1.0.0a1/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    65115 2023-07-17 11:03:20.000000 ural-1.0.0a1/PKG-INFO
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/
+-rw-r--r--   0 Yomgui     (501) staff       (20)    65115 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/PKG-INFO
+-rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/zip-safe
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1872 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/SOURCES.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)       43 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/requires.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)        5 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/top_level.txt
+-rw-r--r--   0 Yomgui     (501) staff       (20)        1 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural.egg-info/dependency_links.txt
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural/
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural/lru/
+-rw-r--r--   0 Yomgui     (501) staff       (20)      966 2023-02-26 16:51:20.000000 ural-1.0.0a1/ural/lru/trie.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)      298 2023-02-26 16:51:20.000000 ural-1.0.0a1/ural/lru/stems.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1384 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/lru/conversion.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      637 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/lru/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      150 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/lru/conversion.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2816 2023-02-26 16:51:20.000000 ural-1.0.0a1/ural/lru/stems.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1970 2023-02-26 16:51:20.000000 ural-1.0.0a1/ural/lru/trie.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      478 2023-02-25 09:51:53.000000 ural-1.0.0a1/ural/lru/serialization.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      121 2023-02-25 16:45:24.000000 ural-1.0.0a1/ural/lru/serialization.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)   195604 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/tld_data.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      550 2023-02-25 16:32:31.000000 ural-1.0.0a1/ural/twitter.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2013 2023-07-15 07:16:51.000000 ural-1.0.0a1/ural/is_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)       88 2023-02-25 16:15:45.000000 ural-1.0.0a1/ural/should_resolve.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     9788 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/youtube.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3065 2023-07-15 11:26:13.000000 ural-1.0.0a1/ural/patterns.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      138 2023-02-25 15:39:15.000000 ural-1.0.0a1/ural/has_special_host.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1543 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/could_be_rss.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1508 2023-07-15 10:52:43.000000 ural-1.0.0a1/ural/format_url.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4857 2023-02-25 10:06:33.000000 ural-1.0.0a1/ural/is_typo_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1485 2023-07-15 10:51:13.000000 ural-1.0.0a1/ural/urls_from_html.py
+drwxr-xr-x   0 Yomgui     (501) staff       (20)        0 2023-07-17 11:03:20.000000 ural-1.0.0a1/ural/classes/
+-rw-r--r--   0 Yomgui     (501) staff       (20)     5238 2023-02-25 09:51:53.000000 ural-1.0.0a1/ural/classes/trie_dict.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      328 2023-02-25 20:51:29.000000 ural-1.0.0a1/ural/classes/hostname_trie_set.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)       44 2022-11-03 11:31:14.000000 ural-1.0.0a1/ural/classes/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1030 2023-02-25 16:43:56.000000 ural-1.0.0a1/ural/classes/trie_dict.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1468 2023-02-25 20:53:15.000000 ural-1.0.0a1/ural/classes/hostname_trie_set.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3857 2023-02-26 12:31:27.000000 ural-1.0.0a1/ural/classes/suffix_trie.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      446 2023-02-25 20:56:18.000000 ural-1.0.0a1/ural/classes/suffix_trie.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)      734 2023-02-25 09:51:53.000000 ural-1.0.0a1/ural/is_homepage.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3712 2023-03-11 16:28:18.000000 ural-1.0.0a1/ural/telegram.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      594 2023-02-26 20:00:25.000000 ural-1.0.0a1/ural/should_follow_href.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2341 2023-07-15 11:18:40.000000 ural-1.0.0a1/ural/infer_redirection.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2163 2023-02-25 14:40:59.000000 ural-1.0.0a1/ural/facebook.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)       93 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/could_be_rss.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1302 2023-07-15 13:15:05.000000 ural-1.0.0a1/ural/canonicalize_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      719 2023-02-25 15:37:43.000000 ural-1.0.0a1/ural/google.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1533 2023-07-15 12:38:29.000000 ural-1.0.0a1/ural/__init__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      742 2023-02-25 20:40:43.000000 ural-1.0.0a1/ural/get_hostname.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)       39 2023-02-25 16:14:40.000000 ural-1.0.0a1/ural/is_homepage.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3779 2023-03-11 16:28:18.000000 ural-1.0.0a1/ural/google.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      931 2023-02-25 09:51:53.000000 ural-1.0.0a1/ural/force_protocol.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      143 2023-02-25 20:43:43.000000 ural-1.0.0a1/ural/get_hostname.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)      631 2023-02-25 16:38:38.000000 ural-1.0.0a1/ural/youtube.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1030 2023-02-25 20:10:18.000000 ural-1.0.0a1/ural/should_resolve.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     2889 2023-07-15 13:25:42.000000 ural-1.0.0a1/ural/fingerprint_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1168 2023-07-15 13:13:06.000000 ural-1.0.0a1/ural/utils.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)      289 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/types.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)    11953 2023-03-11 16:28:18.000000 ural-1.0.0a1/ural/facebook.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      709 2023-02-26 19:32:09.000000 ural-1.0.0a1/ural/could_be_html.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      176 2023-02-25 16:17:21.000000 ural-1.0.0a1/ural/is_url.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)      599 2023-03-02 12:55:19.000000 ural-1.0.0a1/ural/instagram.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)       39 2023-02-25 16:16:15.000000 ural-1.0.0a1/ural/is_typo_url.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)      537 2019-10-04 20:55:44.000000 ural-1.0.0a1/ural/strip_protocol.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)       63 2023-02-25 14:00:44.000000 ural-1.0.0a1/ural/ensure_protocol.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     4146 2023-07-15 13:17:26.000000 ural-1.0.0a1/ural/utils.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3367 2023-03-11 16:28:18.000000 ural-1.0.0a1/ural/twitter.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)    11499 2023-07-17 11:00:36.000000 ural-1.0.0a1/ural/normalize_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)       99 2023-07-15 13:02:03.000000 ural-1.0.0a1/ural/canonicalize_url.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)    22337 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/is_shortened_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      592 2023-02-25 16:31:00.000000 ural-1.0.0a1/ural/telegram.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)       47 2023-02-26 19:56:28.000000 ural-1.0.0a1/ural/should_follow_href.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)      167 2023-07-15 10:23:50.000000 ural-1.0.0a1/ural/urls_from_html.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)      864 2023-02-25 10:12:21.000000 ural-1.0.0a1/ural/ensure_protocol.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3285 2023-03-11 16:28:18.000000 ural-1.0.0a1/ural/instagram.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      198 2023-02-25 20:18:35.000000 ural-1.0.0a1/ural/exceptions.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)       62 2023-02-25 14:00:50.000000 ural-1.0.0a1/ural/force_protocol.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1244 2023-07-13 18:30:25.000000 ural-1.0.0a1/ural/urls_from_text.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)       87 2023-02-26 17:47:23.000000 ural-1.0.0a1/ural/could_be_html.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)      908 2023-02-25 15:39:17.000000 ural-1.0.0a1/ural/has_special_host.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)      394 2023-02-26 17:08:42.000000 ural-1.0.0a1/ural/tld.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)       81 2023-02-25 14:43:13.000000 ural-1.0.0a1/ural/urls_from_text.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)       41 2023-02-25 16:22:37.000000 ural-1.0.0a1/ural/strip_protocol.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)      407 2023-02-25 20:05:32.000000 ural-1.0.0a1/ural/__main__.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     5438 2023-02-26 09:49:32.000000 ural-1.0.0a1/ural/tld.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3612 2023-07-15 10:51:43.000000 ural-1.0.0a1/ural/format_url.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     3090 2023-02-26 19:56:02.000000 ural-1.0.0a1/ural/data.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)     1481 2023-07-17 11:00:36.000000 ural-1.0.0a1/ural/normalize_url.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)      330 2023-07-15 13:26:15.000000 ural-1.0.0a1/ural/fingerprint_url.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)       90 2023-02-25 16:15:29.000000 ural-1.0.0a1/ural/is_shortened_url.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)       60 2023-02-25 15:42:33.000000 ural-1.0.0a1/ural/infer_redirection.pyi
+-rw-r--r--   0 Yomgui     (501) staff       (20)    50214 2023-07-17 11:01:14.000000 ural-1.0.0a1/README.md
+-rw-r--r--   0 Yomgui     (501) staff       (20)      908 2023-07-17 11:03:01.000000 ural-1.0.0a1/setup.py
+-rw-r--r--   0 Yomgui     (501) staff       (20)       38 2023-07-17 11:03:20.000000 ural-1.0.0a1/setup.cfg
```

### Comparing `ural-0.9.0/ural/strip_protocol.py` & `ural-1.0.0a1/ural/strip_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # =============================================================================
 # Ural URL Strip Protocol Function
 # =============================================================================
 #
 # A function removing the protocol from the given url.
 #
-import re
 from ural.patterns import PROTOCOL_RE
 
 
 def strip_protocol(url):
     """
     Function removing the protocol from the given url.
```

### Comparing `ural-0.9.0/ural/ensure_protocol.py` & `ural-1.0.0a1/ural/force_protocol.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # =============================================================================
-# Ural URL Ensure Protocol Function
+# Ural URL Force Protocol Function
 # =============================================================================
 #
-# A function checking if the url has a protocol, and adding one if there is none.
+# A function force-replacing the url protocol by the given one (and adding it if there is none).
 #
 import re
 
 from ural.patterns import PROTOCOL_RE
 
 
-def ensure_protocol(url, protocol='http'):
+def force_protocol(url, protocol="http"):
     """
-    Function checking if the url has a protocol, and adding the given one if there is none.
+    Function force-replacing the url protocol by the given one (and adding it if there is none).
 
     Args:
         url (str): Target URL as a string.
-        protocol (str): protocol to use if there is none in url. Is 'http' by default.
+        protocol (str): protocol wanted. Is 'http' by default.
 
     Returns:
         string: The protocol-equipped url.
 
     """
-    protocol = protocol.rstrip(':/')
+    protocol = protocol.rstrip(":/")
 
     if not PROTOCOL_RE.match(url):
-        url = protocol + '://' + url
-    elif url.startswith('//'):
-        url = protocol + ':' + url
+        url = protocol + "://" + url
+    elif url[:2] == "//":
+        url = protocol + ":" + url
+    else:
+        url = re.sub(PROTOCOL_RE, protocol + "://", url)
 
     return url
```

### Comparing `ural-0.9.0/setup.py` & `ural-1.0.0a1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from setuptools import setup, find_packages
 
-with open('./README.md', 'r') as f:
+with open("./README.md", "r") as f:
     long_description = f.read()
 
-setup(name='ural',
-      version='0.9.0',
-      description='A helper library full of URL-related heuristics.',
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      url='http://github.com/medialab/ural',
-      license='MIT',
-      author='Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou',
-      author_email='kropotkinepiotr@gmail.com',
-      keywords='url',
-      python_requires='>=2.7',
-      packages=find_packages(exclude=['test']),
-      package_data={'docs': ['README.md']},
-      install_requires=[
-        'phylactery>=0.2.2',
-        'pycountry>=18.12.8',
-        'tld>=0.9.3'
-      ],
-      entry_points={
-        'console_scripts': ['ural=ural.cli.__main__:main']
-      },
-      zip_safe=True)
+setup(
+    name="ural",
+    version="1.0.0-a1",
+    description="A helper library full of URL-related heuristics.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="http://github.com/medialab/ural",
+    license="MIT",
+    author="Guillaume Plique, Jules Farjas, Oubine Perrin, Benjamin Ooghe-Tabanou, Martin Delabre, Pauline Breteau, Jean Descamps, Béatrice Mazoyer, Amélie Pellé, Laura Miguel",
+    author_email="guillaume.plique@sciencespo.fr",
+    keywords="url",
+    python_requires=">=2.7",
+    packages=find_packages(exclude=["scripts", "test"]),
+    package_data={"docs": ["README.md"], "ural": ["*.pyi", "**/*.pyi"]},
+    install_requires=[],
+    extras_require={":python_version<'3.8'": ["typing_extensions"]},
+    zip_safe=True,
+)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

