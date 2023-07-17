# Comparing `tmp/opensafely-1.9.1.tar.gz` & `tmp/opensafely-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opensafely-1.9.1.tar", last modified: Fri Jul 23 16:07:40 2021, max compression
+gzip compressed data, was "dist/opensafely-1.9.2.tar", last modified: Wed Aug  4 08:43:28 2021, max compression
```

## Comparing `opensafely-1.9.1.tar` & `opensafely-1.9.2.tar`

### file list

```diff
@@ -1,202 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)      664 2021-07-23 16:07:38.000000 opensafely-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-07-23 16:07:38.000000 opensafely-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-07-23 16:07:40.000000 opensafely-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-07-23 16:07:38.000000 opensafely-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-23 16:07:39.000000 opensafely-1.9.1/opensafely/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/certifi/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/certifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/certifi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)   263774 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/certifi/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/certifi/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/chardet/
--rw-r--r--   0 runner    (1001) docker     (121)     3271 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31254 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/big5freq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/big5prober.py
--rw-r--r--   0 runner    (1001) docker     (121)     9411 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/chardistribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     3839 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0 runner    (1001) docker     (121)     5110 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/charsetprober.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/chardet/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0 runner    (1001) docker     (121)     3590 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/cp949prober.py
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     3950 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/escprober.py
--rw-r--r--   0 runner    (1001) docker     (121)    10510 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/escsm.py
--rw-r--r--   0 runner    (1001) docker     (121)     3749 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/eucjpprober.py
--rw-r--r--   0 runner    (1001) docker     (121)    13546 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/euckrfreq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/euckrprober.py
--rw-r--r--   0 runner    (1001) docker     (121)    31621 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/euctwfreq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1747 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/euctwprober.py
--rw-r--r--   0 runner    (1001) docker     (121)    20715 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/gb2312freq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/gb2312prober.py
--rw-r--r--   0 runner    (1001) docker     (121)    13838 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/hebrewprober.py
--rw-r--r--   0 runner    (1001) docker     (121)    25777 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/jisfreq.py
--rw-r--r--   0 runner    (1001) docker     (121)    19643 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/jpcntx.py
--rw-r--r--   0 runner    (1001) docker     (121)   105704 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)    99578 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)    98783 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)   102505 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)   131187 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)   103319 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/langthaimodel.py
--rw-r--r--   0 runner    (1001) docker     (121)    95953 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5370 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/latin1prober.py
--rw-r--r--   0 runner    (1001) docker     (121)     3413 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0 runner    (1001) docker     (121)    25481 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/mbcssm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/chardet/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19474 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/metadata/languages.py
--rw-r--r--   0 runner    (1001) docker     (121)     6136 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0 runner    (1001) docker     (121)     4309 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0 runner    (1001) docker     (121)     3774 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/sjisprober.py
--rw-r--r--   0 runner    (1001) docker     (121)    12503 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/universaldetector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/utf8prober.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/chardet/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/idna/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/idna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3299 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/idna/codec.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/idna/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    11951 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/idna/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    42350 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/idna/idnadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/idna/intranges.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/idna/package_data.py
--rw-r--r--   0 runner    (1001) docker     (121)   202084 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/idna/uts46data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3159 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/add_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     4903 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    13900 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/create_or_update_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7756 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/database.py
--rw-r--r--   0 runner    (1001) docker     (121)    12144 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/docker_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/extract_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)    12376 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/job.py
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/kill_job.py
--rw-r--r--   0 runner    (1001) docker     (121)    20234 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/local_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     4817 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    25557 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/manage_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6572 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    18545 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/record_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/retry_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     9071 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/schema.sql
--rw-r--r--   0 runner    (1001) docker     (121)     2238 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      996 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3983 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/jobrunner/system_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/requests/
--rw-r--r--   0 runner    (1001) docker     (121)     4205 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/_internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    21667 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/adapters.py
--rw-r--r--   0 runner    (1001) docker     (121)     6496 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    10207 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/certs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    18430 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/help.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)    34408 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/packages.py
--rw-r--r--   0 runner    (1001) docker     (121)    30137 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4188 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3005 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/structures.py
--rw-r--r--   0 runner    (1001) docker     (121)    30529 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/anchor.py
--rw-r--r--   0 runner    (1001) docker     (121)    36226 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     7545 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     8442 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/composer.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/configobjwalker.py
--rw-r--r--   0 runner    (1001) docker     (121)    69741 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/constructor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6620 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/cyaml.py
--rw-r--r--   0 runner    (1001) docker     (121)     6680 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/dumper.py
--rw-r--r--   0 runner    (1001) docker     (121)    65610 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/emitter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9541 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     4099 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)    59033 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     3801 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)    33635 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    10746 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    43904 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/representer.py
--rw-r--r--   0 runner    (1001) docker     (121)    15603 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/scalarbool.py
--rw-r--r--   0 runner    (1001) docker     (121)     4300 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/scalarfloat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4338 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/scalarint.py
--rw-r--r--   0 runner    (1001) docker     (121)     4343 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/scalarstring.py
--rw-r--r--   0 runner    (1001) docker     (121)    72441 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/scanner.py
--rw-r--r--   0 runner    (1001) docker     (121)     8461 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (121)     7757 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     6004 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10811 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    18748 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    37133 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      957 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17656 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)    13908 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (121)    11048 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (121)    16802 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (121)    34286 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (121)     7097 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (121)     8217 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8579 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     2440 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (121)    32536 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/packages/six.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/packages/ssl_match_hostname/
--rw-r--r--   0 runner    (1001) docker     (121)      757 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5679 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-r--r--   0 runner    (1001) docker     (121)    19763 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (121)     5985 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (121)    28203 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4929 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     4123 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     3510 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (121)    21396 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (121)    16288 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (121)     6946 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0 runner    (1001) docker     (121)    10003 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (121)    13988 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (121)     5404 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/_vendor/urllib3/util/wait.py
--rw-r--r--   0 runner    (1001) docker     (121)     8083 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/codelists.py
--rw-r--r--   0 runner    (1001) docker     (121)     3714 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/pull.py
--rw-r--r--   0 runner    (1001) docker     (121)     3432 2021-07-23 16:07:38.000000 opensafely-1.9.1/opensafely/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7437 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-07-23 16:07:40.000000 opensafely-1.9.1/opensafely.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-23 16:07:40.000000 opensafely-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      699 2021-07-23 16:07:38.000000 opensafely-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2021-08-04 08:43:18.000000 opensafely-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-08-04 08:43:18.000000 opensafely-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2021-08-04 08:43:28.000000 opensafely-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2021-08-04 08:43:18.000000 opensafely-1.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-08-04 08:43:26.000000 opensafely-1.9.2/opensafely/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/certifi/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/certifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/certifi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   263774 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/certifi/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (121)     2322 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/certifi/core.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/chardet/
+-rw-r--r--   0 runner    (1001) docker     (121)     3271 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31254 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/big5freq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1757 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/big5prober.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9411 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/chardistribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3839 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5110 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/charsetprober.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/chardet/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2768 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3590 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1855 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/cp949prober.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1661 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3950 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/escprober.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10510 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/escsm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3749 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13546 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/euckrprober.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31621 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1747 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/euctwprober.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20715 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13838 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25777 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/jisfreq.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19643 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/jpcntx.py
+-rw-r--r--   0 runner    (1001) docker     (121)   105704 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    99578 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    98783 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)   102505 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)   131187 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)   103319 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    95953 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5370 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/latin1prober.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3413 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2012 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25481 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/mbcssm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/chardet/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19474 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6136 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4309 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3774 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/sjisprober.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12503 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/universaldetector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2766 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/utf8prober.py
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/chardet/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/idna/
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/idna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3299 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/idna/codec.py
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/idna/compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11951 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/idna/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42350 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/idna/idnadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1749 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/idna/intranges.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/idna/package_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)   202084 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/idna/uts46data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3159 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/add_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5200 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11822 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/create_or_update_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7756 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12144 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1341 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/docker_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/extract_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12376 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2399 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/github_validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2205 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/kill_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20565 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/local_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5869 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25557 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/manage_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6572 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1402 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21969 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/project.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/record_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2589 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/retry_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9403 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (121)     2238 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1336 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3983 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4007 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/jobrunner/system_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/requests/
+-rw-r--r--   0 runner    (1001) docker     (121)     4205 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/_internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21667 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6496 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10207 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/certs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1806 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18430 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3180 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3606 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/help.py
+-rw-r--r--   0 runner    (1001) docker     (121)      757 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34408 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/packages.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30137 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4188 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3005 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/structures.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30529 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/
+-rw-r--r--   0 runner    (1001) docker     (121)     1770 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36226 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/comments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7545 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8442 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/composer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/configobjwalker.py
+-rw-r--r--   0 runner    (1001) docker     (121)    69741 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6620 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/cyaml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6680 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65610 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9541 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4099 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3043 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)    59033 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3801 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33635 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10746 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43904 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/representer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15603 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1431 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/scalarbool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4300 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/scalarfloat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4338 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/scalarint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4343 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/scalarstring.py
+-rw-r--r--   0 runner    (1001) docker     (121)    72441 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8461 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1762 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7757 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6004 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (121)     2763 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10811 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18748 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37133 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17656 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13908 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11048 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4160 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16802 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34286 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7097 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8217 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8579 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2440 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1417 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32536 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/packages/six.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/packages/ssl_match_hostname/
+-rw-r--r--   0 runner    (1001) docker     (121)      757 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5679 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19763 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5985 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28203 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4929 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4123 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3510 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21396 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16288 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6946 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10003 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13988 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5404 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/_vendor/urllib3/util/wait.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8083 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/codelists.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3714 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/pull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3432 2021-08-04 08:43:18.000000 opensafely-1.9.2/opensafely/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7487 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2021-08-04 08:43:28.000000 opensafely-1.9.2/opensafely.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-04 08:43:28.000000 opensafely-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2021-08-04 08:43:18.000000 opensafely-1.9.2/setup.py
```

### Comparing `opensafely-1.9.1/LICENSE` & `opensafely-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/README.md` & `opensafely-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/__init__.py` & `opensafely-1.9.2/opensafely/__init__.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/certifi/cacert.pem` & `opensafely-1.9.2/opensafely/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/certifi/core.py` & `opensafely-1.9.2/opensafely/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/__init__.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/big5freq.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/big5prober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/chardistribution.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/charsetgroupprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/charsetprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/cli/chardetect.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/codingstatemachine.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/compat.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/cp949prober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/enums.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/escprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/escsm.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/eucjpprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/euckrfreq.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/euckrprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/euctwfreq.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/euctwprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/gb2312freq.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/gb2312prober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/hebrewprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/jisfreq.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/jpcntx.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/langbulgarianmodel.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/langgreekmodel.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/langhebrewmodel.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/langhungarianmodel.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/langrussianmodel.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/langthaimodel.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/langturkishmodel.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/latin1prober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/mbcharsetprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/mbcsgroupprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/mbcssm.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/metadata/languages.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/sbcharsetprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/sbcsgroupprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/sjisprober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/universaldetector.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/chardet/utf8prober.py` & `opensafely-1.9.2/opensafely/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/idna/codec.py` & `opensafely-1.9.2/opensafely/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/idna/core.py` & `opensafely-1.9.2/opensafely/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/idna/idnadata.py` & `opensafely-1.9.2/opensafely/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/idna/intranges.py` & `opensafely-1.9.2/opensafely/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/idna/uts46data.py` & `opensafely-1.9.2/opensafely/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/add_job.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/add_job.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/config.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 truthy = ("true", "1", "yes")
 
 if os.environ.get("USING_DUMMY_DATA_BACKEND", "false").lower().strip() in truthy:
     USING_DUMMY_DATA_BACKEND = True
 else:
     USING_DUMMY_DATA_BACKEND = BACKEND == "expectations"
 
-ALLOWED_IMAGES = {"cohortextractor", "stata-mp", "r", "jupyter", "python"}
+ALLOWED_IMAGES = {"cohortextractor", "cohortextractor-v2", "stata-mp", "r", "jupyter", "python"}
 
 DOCKER_REGISTRY = "ghcr.io/opensafely-core"
 
 DATABASE_URLS = {
     "full": os.environ.get("FULL_DATABASE_URL"),
     "slice": os.environ.get("SLICE_DATABASE_URL"),
     "dummy": os.environ.get("DUMMY_DATABASE_URL"),
@@ -89,14 +89,20 @@
         raise ConfigException(
             f"PRESTO_TLS_CERT_PATH={cert_path}, but file does not exist"
         )
 
 
 MAX_WORKERS = int(os.environ.get("MAX_WORKERS") or max(cpu_count() - 1, 1))
 
+# This is a crude mechanism for preventing a single large JobRequest with lots
+# of associated Jobs from hogging all the resources. We want this configurable
+# because it's useful to be able to disable this during tests and when running
+# locally
+RANDOMISE_JOB_ORDER = True
+
 # See `local_run.py` for more detail
 LOCAL_RUN_MODE = False
 
 # Automatically delete containers and volumes after they have been used
 CLEAN_UP_DOCKER_OBJECTS = True
 
 # See `manage_jobs.ensure_overwritable` for more detail
```

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/create_or_update_jobs.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/create_or_update_jobs.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,33 +4,36 @@
 It handles all logic connected with creating or updating Jobs in response to
 JobRequests. This includes fetching the code with git, validating the project
 and doing the necessary dependency resolution.
 """
 import logging
 from pathlib import Path
 import re
-from urllib.parse import urlparse
 import time
 
 from . import config
 from .database import (
     transaction,
     insert,
     exists_where,
     find_where,
     count_where,
     update_where,
 )
 from .git import (
     read_file_from_repo,
     get_sha_from_remote_ref,
-    commit_reachable_from_ref,
     GitError,
     GitFileNotFoundError,
 )
+from .github_validators import (
+    validate_branch_and_commit,
+    validate_repo_url,
+    GithubValidationError,
+)
 from .project import (
     parse_and_validate_project_file,
     get_action_specification,
     get_all_actions,
     assert_valid_actions,
     ProjectValidationError,
     RUN_ALL_COMMAND,
@@ -60,15 +63,20 @@
     displayed to the user.
     """
     if not related_jobs_exist(job_request):
         try:
             log.info(f"Handling new JobRequest:\n{job_request}")
             new_job_count = create_jobs(job_request)
             log.info(f"Created {new_job_count} new jobs")
-        except (GitError, ProjectValidationError, JobRequestError) as e:
+        except (
+            GitError,
+            GithubValidationError,
+            ProjectValidationError,
+            JobRequestError,
+        ) as e:
             log.info(f"JobRequest failed:\n{e}")
             create_failed_job(job_request, e)
         except Exception:
             log.exception("Uncaught error while creating jobs")
             create_failed_job(job_request, JobRequestError("Internal error"))
     else:
         if job_request.cancelled_actions:
@@ -259,61 +267,14 @@
         # As this involves talking to the remote git server we only do it at
         # the end once all other checks have passed
         validate_branch_and_commit(
             job_request.repo_url, job_request.commit, job_request.branch
         )
 
 
-def validate_repo_url(repo_url, allowed_gitub_orgs):
-    parsed_url = urlparse(repo_url)
-    if parsed_url.scheme != "https" or parsed_url.netloc != "github.com":
-        raise JobRequestError("Repository URLs must start https://github.com")
-    path = parsed_url.path.strip("/").split("/")
-    if not path or path[0] not in allowed_gitub_orgs:
-        raise JobRequestError(
-            f"Repositories must belong to one of the following Github "
-            f"organisations: {' '.join(allowed_gitub_orgs)}"
-        )
-    expected_url = f"https://github.com/{'/'.join(path[:2])}"
-    if repo_url.rstrip("/") != expected_url or len(path) != 2:
-        raise JobRequestError(
-            "Repository URL was not of the expected format: "
-            "https://github.com/[organisation]/[project-name]"
-        )
-
-
-def validate_branch_and_commit(repo_url, commit, branch):
-    """
-    Due to the way Github works, anyone who can open a pull request against a
-    repository can make a commit appear to be "in" that repository, even if
-    they do not have write access to it.
-
-    For example, someone created this PR against the Linux kernel:
-    https://github.com/torvalds/linux/pull/437
-
-    And even though this will never be merged, it still appears as a commit in
-    that repo:
-    https://github.com/torvalds/linux/commit/2793ae1df012c7c3f13ea5c0f0adb99017999c3b
-
-    If we are enforcing that only code from certain organisations can be run
-    then we need to check that any commits supplied have been made by someone
-    with write access to the repository, which means we need to check they
-    belong to a branch or tag in the repository.
-    """
-    if not branch:
-        raise JobRequestError("A branch name must be supplied")
-    # A further wrinkle is that each PR gets an associated ref within the repo
-    # of the form `pull/PR_NUMBER/head`. So we enforce that the branch name
-    # must be a "plain vanilla" branch name with no slashes.
-    if "/" in branch:
-        raise JobRequestError(f"Branch name must not contain slashes: {branch}")
-    if not commit_reachable_from_ref(repo_url, commit, branch):
-        raise JobRequestError(f"Could not find commit on branch '{branch}': {commit}")
-
-
 def create_failed_job(job_request, exception):
     """
     Sometimes we want to say to the job-server (and the user): your JobRequest
     was broken so we weren't able to create any jobs for it. But the only way
     for the job-runner to communicate back to the job-server is by creating a
     job. So this function creates a single job with the special action name
     "__error__", which starts in the FAILED state and whose status_message
```

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/database.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/database.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/docker.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/docker.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/docker_stats.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/docker_stats.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/extract_stats.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/extract_stats.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/git.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/git.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/job.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/job.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/kill_job.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/kill_job.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/local_run.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/local_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import shutil
 import string
 import subprocess
 import sys
 import tempfile
 import textwrap
 
-from .run import main as run_main, JobError
+from .run import main as run_main
 from . import config
 from . import docker
 from .database import find_where
 from .manage_jobs import METADATA_DIR
 from .models import JobRequest, Job, State, StatusCode
 from .create_or_update_jobs import (
     create_jobs,
@@ -192,14 +192,16 @@
     clean_up_docker_objects=True,
     log_format=LOCAL_RUN_FORMAT,
     format_output_for_github=False,
 ):
     # Configure
     docker.LABEL = docker_label
     config.LOCAL_RUN_MODE = True
+    # It's more helpful in this context to have things consistent
+    config.RANDOMISE_JOB_ORDER = False
     config.HIGH_PRIVACY_WORKSPACES_DIR = project_dir.parent
     # Append a random value so that multiple runs in the same process will each
     # get their own unique in-memory database. This is only really relevant
     # during testing.
     config.DATABASE_FILE = f":memory:{random.randrange(sys.maxsize)}"
     config.JOB_LOG_DIR = temp_log_dir
     config.BACKEND = "expectations"
@@ -294,22 +296,22 @@
         stream=sys.stdout,
     )
 
     # Wrap all the log output inside an expandable block when running inside
     # Github Actions
     if format_output_for_github:
         print(f"::group::Job Runner Logs {ANSI.Grey}(click to view){ANSI.Reset}")
+
     # Run everything
+    exit_condition = (
+        no_jobs_remaining if continue_on_error else job_failed_or_none_remaining
+    )
     try:
-        run_main(
-            exit_when_done=True,
-            shuffle_jobs=False,
-            raise_on_failure=not continue_on_error,
-        )
-    except (JobError, KeyboardInterrupt):
+        run_main(exit_callback=exit_condition)
+    except KeyboardInterrupt:
         pass
     finally:
         if format_output_for_github:
             print("::endgroup::")
 
     final_jobs = find_where(Job, state__in=[State.FAILED, State.SUCCEEDED])
     # Always show failed jobs last, otherwise show in order run
@@ -372,14 +374,24 @@
                 print(textwrap.indent(logs, "     "))
         print()
 
     success_flag = all(job.state == State.SUCCEEDED for job in final_jobs)
     return success_flag
 
 
+def no_jobs_remaining(active_jobs):
+    return len(active_jobs) == 0
+
+
+def job_failed_or_none_remaining(active_jobs):
+    if any(job.state == State.FAILED for job in active_jobs):
+        return True
+    return len(active_jobs) == 0
+
+
 # Copied from test/conftest.py to avoid a more complex dependency tree
 def delete_docker_entities(entity, label, ignore_errors=False):
     ls_args = [
         "docker",
         entity,
         "ls",
         "--all" if entity == "container" else None,
```

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/log_utils.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/log_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,66 +2,68 @@
 This sets up some basic logging configuration (log to stderr with a default log
 level of INFO) with some job-runner specific tweaks. In particular it supports
 automatically including the currently executing Job or JobRequest in the log
 output. It also includes the stderr output from any failed attempts to shell
 out to external processes.
 """
 import contextlib
-import datetime
 import logging
+import logging.handlers
 import os
 import subprocess
 import sys
 import threading
 import time
 
 
 DEFAULT_FORMAT = "{asctime} {message} {tags}"
 
 
-def formatting_filter(record):
-    """Ensure various record attribute are always available for formatting."""
-
-    # ensure this are always available for static formatting
-    record.action = ""
-
-    tags = {}
-    ctx = set_log_context.current_context
-    job = getattr(record, "job", None) or ctx.get("job")
-    req = getattr(record, "job_request", None) or ctx.get("job_request")
-
-    status_code = getattr(record, "status_code", None)
-    if status_code:
-        tags["status"] = record.status_code
-
-    if job:
-        # preserve short action for local run formatting
-        record.action = job.action + ": "
-        if "status" not in tags and job.status_code:
-            tags["status"] = job.status_code
-        tags["project"] = job.project
-        tags["action"] = job.action
-        tags["id"] = job.id
-
-    if req:
-        tags["req"] = req.id
-
-    record.tags = " ".join(f"{k}={v}" for k, v in tags.items())
-
-    return True
-
-
 def configure_logging(fmt=DEFAULT_FORMAT, stream=None, status_codes_to_ignore=None):
     formatter = JobRunnerFormatter(fmt, style="{")
     handler = logging.StreamHandler(stream=stream)
     handler.setFormatter(formatter)
     if status_codes_to_ignore:
         handler.addFilter(IgnoreStatusCodes(status_codes_to_ignore))
     handler.addFilter(formatting_filter)
-    logging.basicConfig(level=os.environ.get("LOGLEVEL", "INFO"), handlers=[handler])
+
+    log_level = os.environ.get("LOGLEVEL", "INFO")
+    handlers = [handler]
+
+    # Support a separate log file at level DEBUG, while leaving the default
+    # logs untouched. DEBUG logging can be extremely noisy and so we want a way
+    # to capture these that doesn't pollute the primary logs.
+    debug_log_file = os.environ.get("DEBUG_LOG_FILE")
+    if debug_log_file:
+        debug_handler = logging.handlers.TimedRotatingFileHandler(
+            debug_log_file,
+            encoding="utf-8",
+            delay=True,
+            # Rotate daily, keeping 14 days of backups
+            when="D",
+            interval=1,
+            backupCount=14,
+            utc=True,
+        )
+        debug_handler.setFormatter(formatter)
+        debug_handler.addFilter(formatting_filter)
+        debug_handler.setLevel("DEBUG")
+        handlers.append(debug_handler)
+        # Set the default handler to the originally specified log level and
+        # then increase the base log level to DEBUG
+        handler.setLevel(log_level)
+        log_level = "DEBUG"
+
+    logging.basicConfig(level=log_level, handlers=handlers)
+
+    if debug_log_file:
+        logging.getLogger(__name__).info(f"Writing DEBUG logs to '{debug_log_file}'")
+
+    # We attach a custom handler for uncaught exceptions to display error
+    # output from failed subprocesses
     sys.excepthook = show_subprocess_stderr
 
 
 class JobRunnerFormatter(logging.Formatter):
 
     converter = time.gmtime  # utc rather than local
     default_msec_format = "%s.%03dZ"  # s/,/. and append Z
@@ -78,27 +80,43 @@
             if stderr:
                 if isinstance(stderr, bytes):
                     stderr = stderr.decode("utf-8", "ignore")
                 message = f"{message}\n\nstderr:\n\n{stderr}"
         return message
 
 
-def show_subprocess_stderr(typ, value, traceback):
-    """
-    This applies the same CalledProcessError formatting as in `formatException`
-    above but to uncaught exceptions
-    """
-    sys.__excepthook__(typ, value, traceback)
-    if isinstance(value, subprocess.CalledProcessError):
-        stderr = value.stderr
-        if stderr:
-            if isinstance(stderr, bytes):
-                stderr = stderr.decode("utf-8", "ignore")
-            print("\nstderr:\n", file=sys.stderr)
-            print(stderr, file=sys.stderr)
+def formatting_filter(record):
+    """Ensure various record attribute are always available for formatting."""
+
+    ctx = set_log_context.current_context
+    job = getattr(record, "job", None) or ctx.get("job")
+    req = getattr(record, "job_request", None) or ctx.get("job_request")
+
+    status_code = getattr(record, "status_code", None)
+    if job and not status_code:
+        status_code = job.status_code
+
+    tags = {}
+
+    if status_code:
+        tags["status"] = status_code
+    if job:
+        tags["project"] = job.project
+        tags["action"] = job.action
+        tags["id"] = job.id
+    if req:
+        tags["req"] = req.id
+
+    record.tags = " ".join(f"{k}={v}" for k, v in tags.items())
+
+    # The `action` attribute is only used by format string in "local_run" mode
+    # but we make sure it's always available
+    record.action = f"{job.action}: " if job else ""
+
+    return True
 
 
 class IgnoreStatusCodes:
     """
     Skip log lines which have certain status codes
     """
 
@@ -139,14 +157,24 @@
         self.context_stack.append(self.current_context)
         self.current_context = dict(self.current_context, **kwargs)
         try:
             yield
         finally:
             self.current_context = self.context_stack.pop()
 
-    def filter(self, record):
-        if hasattr(record, "status_code"):
-            return record.status_code not in self.status_codes_to_ignore
-        return True
+
+def show_subprocess_stderr(typ, value, traceback):
+    """
+    This applies the same CalledProcessError formatting as in `JobRunnerFormatter`
+    above but to uncaught exceptions
+    """
+    sys.__excepthook__(typ, value, traceback)
+    if isinstance(value, subprocess.CalledProcessError):
+        stderr = value.stderr
+        if stderr:
+            if isinstance(stderr, bytes):
+                stderr = stderr.decode("utf-8", "ignore")
+            print("\nstderr:\n", file=sys.stderr)
+            print(stderr, file=sys.stderr)
 
 
 set_log_context = SetLogContext()
```

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/manage_jobs.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/manage_jobs.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/models.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/models.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/path_utils.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/path_utils.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/project.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/project.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 import shlex
 from types import SimpleNamespace
 
 from opensafely._vendor.ruamel.yaml import YAML
 from opensafely._vendor.ruamel.yaml.error import YAMLError, YAMLStreamError, YAMLWarning, YAMLFutureWarning
 
 from . import config, git
+from .github_validators import (
+    validate_branch_and_commit,
+    validate_repo_url,
+    GithubValidationError,
+)
 
 
 # The magic action name which means "run every action"
 RUN_ALL_COMMAND = "run_all"
 
 # The version of `project.yaml` where each feature was introduced
 FEATURE_FLAGS_BY_VERSION = {"UNIQUE_OUTPUT_PATH": 2, "EXPECTATIONS_POPULATION": 3}
@@ -61,14 +66,21 @@
     run: str
     needs: list
     outputs: dict
     repo_url: str
     commit: str
 
 
+@dataclasses.dataclass
+class ReusableAction:
+    repo_url: str
+    commit: str
+    action_file: bytes
+
+
 def parse_yaml_file(yaml_file):
     try:
         # We're using the pure-Python version here as we don't care about speed
         # and this gives better error messages (and consistent behaviour
         # cross-platform)
         return YAML(typ="safe", pure=True).load(yaml_file)
         # ruamel doesn't have a nice exception hierarchy so we have to catch
@@ -111,68 +123,120 @@
         The action's representation as a dict. If `action` resolves to a reusable
         action, then it is rewritten to point to the reusable action and a copy is
         returned. If not, then `action` is returned unchanged.
 
     Raises:
         ReusableActionError: An error occurred when accessing the reusable action.
     """
-    # This avoids a circular import and is much less invasive than either moving the
-    # imports or importing `project` within `create_or_update_jobs`.
-    from .create_or_update_jobs import (
-        JobRequestError,
-        validate_branch_and_commit,
-        validate_repo_url,
-    )
-
     run_args = shlex.split(action["run"])
     image, tag = run_args[0].split(":")
 
     if image in config.ALLOWED_IMAGES:
         # This isn't a reusable action.
         return action
 
-    # This is a reusable action.
+    reusable_action = fetch_reusable_action(action_id, image, tag)
+    new_action = apply_reusable_action(action_id, action, reusable_action)
+    return new_action
+
+
+def fetch_reusable_action(action_id, image, tag):
+    """
+    Fetch all metadata from git needed to apply a reusable action
+
+    Args:
+        action_id: The action's ID as a string. This is the action's key in
+            project.yaml. It is used to raise errors with more informative messages.
+        image: The name of the reusable action
+        tag: The specified version of the reusable action
+
+    Returns:
+        ReusableAction object, wrapping the repo_url, commit and the contents
+        of the `action.yaml` file
+
+    Raises:
+        ReusableActionError: An error occurred when accessing the reusable action.
+    """
     repo_url = f"{config.ACTIONS_GITHUB_ORG_URL}/{image}"
     try:
         validate_repo_url(repo_url, [config.ACTIONS_GITHUB_ORG])
-    except JobRequestError as e:
+    except GithubValidationError as e:
         raise ReusableActionError(*e.args)  # This keeps the function signature clean
 
     try:
         # If there's a problem, then it relates to the repository. Maybe the study
         # developer made an error; maybe the reusable action developer made an error.
-        commit_sha = git.get_sha_from_remote_ref(repo_url, tag)
+        commit = git.get_sha_from_remote_ref(repo_url, tag)
     except git.GitError:
         raise ReusableActionError(
             f"Cannot resolve '{action_id}' to a repository at '{repo_url}'"
         )
 
     try:
-        validate_branch_and_commit(repo_url, commit_sha, "main")
-    except JobRequestError as e:
+        validate_branch_and_commit(repo_url, commit, "main")
+    except GithubValidationError as e:
         raise ReusableActionError(*e.args)
 
     try:
         # If there's a problem, then it relates to the reusable action. The study
         # developer didn't make an error; the reusable action developer did.
-        action_file = git.read_file_from_repo(repo_url, commit_sha, "action.yaml")
-        action_config = parse_yaml_file(action_file)
+        action_file = git.read_file_from_repo(repo_url, commit, "action.yaml")
+    except git.GitError:
+        raise ReusableActionError(
+            f"There is a problem with the reusable action required by '{action_id}'"
+        )
+
+    return ReusableAction(repo_url=repo_url, commit=commit, action_file=action_file)
+
+
+def apply_reusable_action(action_id, action, reusable_action):
+    """
+    Rewrite an `action` dict to run the code specifed by the supplied
+    `ReusableAction` instance.
+
+    Args:
+        action_id: The action's ID as a string. This is the action's key in
+            project.yaml. It is used to raise errors with more informative messages.
+        action: The action's representation as a dict. This is the action's value in
+            project.yaml.
+        reusable_action: A ReusableAction instance
+
+    Returns:
+        The modified action's representation as a dict.
+
+    Raises:
+        ReusableActionError: An error occurred when accessing the reusable action.
+    """
+    try:
+        # If there's a problem, then it relates to the reusable action. The study
+        # developer didn't make an error; the reusable action developer did.
+        action_config = parse_yaml_file(reusable_action.action_file)
         assert "run" in action_config
-    except (git.GitError, ProjectYAMLError, AssertionError):
+        action_run_args = shlex.split(action_config["run"])
+        action_image, action_tag = action_run_args[0].split(":")
+        if action_image not in config.ALLOWED_IMAGES:
+            raise ProjectValidationError(f"Unrecognised runtime: {action_image}")
+        is_generate_cohort, _ = is_generate_cohort_command(action_run_args)
+        if is_generate_cohort:
+            raise ProjectValidationError(
+                "Re-usable actions cannot invoke cohortextractor"
+            )
+    except (ProjectYAMLError, AssertionError, ProjectValidationError):
         raise ReusableActionError(
             f"There is a problem with the reusable action required by '{action_id}'"
         )
 
     # ["action:tag", "arg", ...] -> ["runtime:tag binary entrypoint", "arg", ...]
+    run_args = shlex.split(action["run"])
     run_args[0] = action_config["run"]
 
     new_action = action.copy()
     new_action["run"] = " ".join(run_args)
-    new_action["repo_url"] = repo_url
-    new_action["commit"] = commit_sha
+    new_action["repo_url"] = reusable_action.repo_url
+    new_action["commit"] = reusable_action.commit
     return new_action
 
 
 def make_yaml_error_more_helpful(exc):
     """
     ruamel produces quite helpful error messages but they refer to the file as
     `<byte_string>` (which will be confusing for users) and they also include
@@ -218,15 +282,16 @@
     else:
         project["expectations"] = {}
         project["expectations"]["population_size"] = 1000
 
     project_actions = project["actions"]
 
     for action_id, action_config in project_actions.items():
-        if is_generate_cohort_command(shlex.split(action_config["run"])):
+        is_generate_cohort, _ = is_generate_cohort_command(shlex.split(action_config["run"]))
+        if is_generate_cohort:
             if len(action_config["outputs"]) != 1:
                 raise ProjectValidationError(
                     f"A `generate_cohort` action must have exactly one output; {action_id} had {len(action_config['outputs'])}",
                 )
 
         # Check a `generate_cohort` command only generates a single output
         # Check outputs are permitted
@@ -309,44 +374,57 @@
             f"Action '{action_id}' not found in project.yaml", project
         )
     run_command = action_spec["run"]
     if "config" in action_spec:
         run_command = add_config_to_run_command(run_command, action_spec["config"])
     run_args = shlex.split(run_command)
 
-    # Specical case handling for the `cohortextractor generate_cohort` command
-    if is_generate_cohort_command(run_args):
-        # Set the size of the dummy data population, if that's what were
-        # generating.  Possibly this should be moved to the study definition
-        # anyway, which would make this unnecessary.
-        if config.USING_DUMMY_DATA_BACKEND:
-            if "dummy_data_file" in action_spec:
-                run_command += f" --dummy-data-file={action_spec['dummy_data_file']}"
+    # Special case handling for the `cohortextractor generate_cohort` command
+    is_generate_cohort, version = is_generate_cohort_command(run_args)
+    if is_generate_cohort:
+        if version == 1:
+            # Set the size of the dummy data population, if that's what we're
+            # generating.  Possibly this should be moved to the study definition
+            # anyway, which would make this unnecessary.
+            if config.USING_DUMMY_DATA_BACKEND:
+                if "dummy_data_file" in action_spec:
+                    run_command += f" --dummy-data-file={action_spec['dummy_data_file']}"
+                else:
+                    size = int(project["expectations"]["population_size"])
+                    run_command += f" --expectations-population={size}"
+            # Automatically configure the cohortextractor to produce output in the
+            # directory the `outputs` spec is expecting. Longer term I'd like to
+            # just make it an error if the directories don't match, rather than
+            # silently fixing it. (We can use the project versioning system to
+            # ensure this doesn't break existing studies.)
+            output_dirs = get_output_dirs(action_spec["outputs"])
+            if len(output_dirs) != 1:
+                # If we detect multiple output directories but the command
+                # explicitly specifies an output directory then we assume the user
+                # knows what they're doing and don't attempt to modify the output
+                # directory or throw an error
+                if not args_include(run_args, "--output-dir"):
+                    raise ProjectValidationError(
+                        f"generate_cohort command should produce output in only one "
+                        f"directory, found {len(output_dirs)}:\n"
+                        + "\n".join([f" - {d}/" for d in output_dirs])
+                    )
             else:
-                size = int(project["expectations"]["population_size"])
-                run_command += f" --expectations-population={size}"
-        # Automatically configure the cohortextractor to produce output in the
-        # directory the `outputs` spec is expecting. Longer term I'd like to
-        # just make it an error if the directories don't match, rather than
-        # silently fixing it. (We can use the project versioning system to
-        # ensure this doesn't break existing studies.)
-        output_dirs = get_output_dirs(action_spec["outputs"])
-        if len(output_dirs) != 1:
-            # If we detect multiple output directories but the command
-            # explicitly specifies an output directory then we assume the user
-            # knows what they're doing and don't attempt to modify the output
-            # directory or throw an error
-            if not args_include(run_args, "--output-dir"):
-                raise ProjectValidationError(
-                    f"generate_cohort command should produce output in only one "
-                    f"directory, found {len(output_dirs)}:\n"
-                    + "\n".join([f" - {d}/" for d in output_dirs])
-                )
+                run_command += f" --output-dir={output_dirs[0]}"
         else:
-            run_command += f" --output-dir={output_dirs[0]}"
+            # cohortextractor Version 2 expects all command line arguments to be specified in the run command
+            assert version == 2, version
+            if config.USING_DUMMY_DATA_BACKEND and "--dummy-data-file" not in run_command:
+                raise ProjectValidationError("--dummy-data-file is required for a local run")
+
+            # There is one and only one output file in the outputs spec (verified in validate_project_and_set_defaults())
+            output_file = next(output_file for output in action_spec["outputs"].values() for output_file in output.values())
+            if output_file not in run_command:
+                raise ProjectValidationError("--output in run command and outputs must match")
+
     return ActionSpecifiction(
         run=run_command,
         needs=action_spec.get("needs", []),
         outputs=action_spec["outputs"],
         # If action_spec (a dict) represents a reusable action, then it will have the
         # following keys. If not, then it won't.
         repo_url=action_spec.get("repo_url"),
@@ -368,21 +446,20 @@
 def is_generate_cohort_command(args):
     """
     The `cohortextractor generate_cohort` command gets special treatment in
     various places (e.g. it's the only command which gets access to the
     database) so it's helpful to have a single function for identifying it
     """
     assert not isinstance(args, str)
-    if (
-        len(args) > 1
-        and args[0].startswith("cohortextractor:")
-        and args[1] == "generate_cohort"
-    ):
-        return True
-    return False
+    if len(args) > 1:
+        if args[0].startswith("cohortextractor:") and args[1] == "generate_cohort":
+            return True, 1
+        if args[0].startswith("cohortextractor-v2:"):
+            return True, 2
+    return False, None
 
 
 def args_include(args, target_arg):
     return any(arg == target_arg or arg.startswith(f"{target_arg}=") for arg in args)
 
 
 def get_all_actions(project):
```

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/record_stats.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/record_stats.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/retry_job.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/retry_job.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/run.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,43 +22,41 @@
     kill_job,
 )
 
 
 log = logging.getLogger(__name__)
 
 
-def main(exit_when_done=False, raise_on_failure=False, shuffle_jobs=True):
+def main(exit_callback=lambda _: False):
     log.info("jobrunner.run loop started")
     while True:
-        active_jobs = handle_jobs(
-            raise_on_failure=raise_on_failure, shuffle_jobs=shuffle_jobs
-        )
-        if exit_when_done and len(active_jobs) == 0:
+        active_jobs = handle_jobs()
+        if exit_callback(active_jobs):
             break
         time.sleep(config.JOB_LOOP_INTERVAL)
 
 
-def handle_jobs(raise_on_failure=False, shuffle_jobs=True):
+def handle_jobs():
+    log.debug("Querying database for active jobs")
     active_jobs = find_where(Job, state__in=[State.PENDING, State.RUNNING])
+    log.debug("Done query")
     # Randomising the job order is a crude but effective way to ensure that a
     # single large job request doesn't hog all the workers. We make this
     # optional as, when running locally, having jobs run in a predictable order
     # is preferable
-    if shuffle_jobs:
+    if config.RANDOMISE_JOB_ORDER:
         random.shuffle(active_jobs)
     for job in active_jobs:
         # `set_log_context` ensures that all log messages triggered anywhere
         # further down the stack will have `job` set on them
         with set_log_context(job=job):
             if job.state == State.PENDING:
                 handle_pending_job(job)
             elif job.state == State.RUNNING:
                 handle_running_job(job)
-        if raise_on_failure and job.state == State.FAILED:
-            raise JobError("Job failed")
     return active_jobs
 
 
 def handle_pending_job(job):
     if job.cancelled:
         # Mark the job as running and then immediately invoke
         # `handle_running_job` to deal with the cancellation. This slightly
@@ -99,15 +97,18 @@
 
 
 def handle_running_job(job):
     if job.cancelled:
         log.info("Cancellation requested, killing job")
         kill_job(job)
 
-    if job_still_running(job):
+    log.debug("Checking job running state")
+    is_running = job_still_running(job)
+    log.debug("Check done")
+    if is_running:
         set_message(job, "Running")
     else:
         try:
             set_message(job, "Finished, checking status and extracting outputs")
             job = finalise_job(job)
             # We expect the job to be transitioned into its final state at this
             # point
@@ -132,15 +133,19 @@
             cleanup_job(job)
 
 
 def get_states_of_awaited_jobs(job):
     job_ids = job.wait_for_job_ids
     if not job_ids:
         return []
-    return select_values(Job, "state", id__in=job_ids)
+
+    log.debug("Querying database for state of dependencies")
+    states = select_values(Job, "state", id__in=job_ids)
+    log.debug("Done query")
+    return states
 
 
 def mark_job_as_failed(job, error, code=None):
     if isinstance(error, str):
         message = error
     else:
         message = f"{type(error).__name__}: {error}"
@@ -159,39 +164,43 @@
     # database exactly as is with the exception of setting the completed at
     # timestamp
     assert job.state in [State.SUCCEEDED, State.FAILED]
     if job.state == State.FAILED and job.cancelled:
         job.status_message = "Cancelled by user"
         job.status_code = StatusCode.CANCELLED_BY_USER
     job.completed_at = int(time.time())
+    log.debug("Updating full job record")
     update(job)
+    log.debug("Update done")
     log.info(job.status_message, extra={"status_code": job.status_code})
 
 
 def set_state(job, state, message, code=None):
     timestamp = int(time.time())
     if state == State.RUNNING:
         job.started_at = timestamp
     elif state == State.FAILED or state == State.SUCCEEDED:
         job.completed_at = timestamp
     job.state = state
     job.status_message = message
     job.status_code = code
     job.updated_at = timestamp
+    log.debug("Updating job status and timestamps")
     update(
         job,
         update_fields=[
             "state",
             "status_message",
             "status_code",
             "updated_at",
             "started_at",
             "completed_at",
         ],
     )
+    log.debug("Update done")
     log.info(job.status_message, extra={"status_code": job.status_code})
 
 
 def set_message(job, message, code=None):
     timestamp = int(time.time())
     # If message has changed then update and log
     if job.status_message != message:
@@ -201,25 +210,29 @@
         update(job, update_fields=["status_message", "status_code", "updated_at"])
         log.info(job.status_message, extra={"status_code": job.status_code})
     # If the status message hasn't changed then we only update the timestamp
     # once a minute. This gives the user some confidence that the job is still
     # active without writing to the database every single time we poll
     elif timestamp - job.updated_at >= 60:
         job.updated_at = timestamp
+        log.debug("Updating job timestamp")
         update(job, update_fields=["updated_at"])
+        log.debug("Update done")
         # For long running jobs we don't want to fill the logs up with "Job X
         # is still running" messages, but it is useful to have semi-regular
         # confirmations in the logs that it is still running. The below will
         # log approximately once every 10 minutes.
         if datetime.datetime.fromtimestamp(timestamp).minute % 10 == 0:
             log.info(job.status_message, extra={"status_code": job.status_code})
 
 
 def get_reason_job_not_started(job):
+    log.debug("Querying for running jobs")
     running_jobs = find_where(Job, state=State.RUNNING)
+    log.debug("Query done")
     used_resources = sum(
         get_job_resource_weight(running_job) for running_job in running_jobs
     )
     required_resources = get_job_resource_weight(job)
     if used_resources + required_resources > config.MAX_WORKERS:
         if required_resources > 1:
             return "Waiting on available workers for resource intensive job"
```

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/schema.sql` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/schema.sql`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/service.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/service.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/string_utils.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/string_utils.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/subprocess_utils.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/sync.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/sync.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/jobrunner/system_stats.py` & `opensafely-1.9.2/opensafely/_vendor/jobrunner/system_stats.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/__init__.py` & `opensafely-1.9.2/opensafely/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/_internal_utils.py` & `opensafely-1.9.2/opensafely/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/adapters.py` & `opensafely-1.9.2/opensafely/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/api.py` & `opensafely-1.9.2/opensafely/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/auth.py` & `opensafely-1.9.2/opensafely/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/compat.py` & `opensafely-1.9.2/opensafely/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/cookies.py` & `opensafely-1.9.2/opensafely/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/exceptions.py` & `opensafely-1.9.2/opensafely/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/help.py` & `opensafely-1.9.2/opensafely/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/hooks.py` & `opensafely-1.9.2/opensafely/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/models.py` & `opensafely-1.9.2/opensafely/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/packages.py` & `opensafely-1.9.2/opensafely/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/sessions.py` & `opensafely-1.9.2/opensafely/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/status_codes.py` & `opensafely-1.9.2/opensafely/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/structures.py` & `opensafely-1.9.2/opensafely/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/requests/utils.py` & `opensafely-1.9.2/opensafely/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/__init__.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/anchor.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/anchor.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/comments.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/comments.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/compat.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/compat.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/composer.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/constructor.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/cyaml.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/dumper.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/emitter.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/error.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/error.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/events.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/events.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/loader.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/main.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/main.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/nodes.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/parser.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/reader.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/representer.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/resolver.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/scalarbool.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/scalarbool.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/scalarfloat.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/scalarfloat.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/scalarint.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/scalarint.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/scalarstring.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/scalarstring.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/scanner.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/serializer.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/timestamp.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/timestamp.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/tokens.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/ruamel/yaml/util.py` & `opensafely-1.9.2/opensafely/_vendor/ruamel/yaml/util.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/__init__.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/_collections.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/connection.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/connectionpool.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/_appengine_environ.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/_securetransport/bindings.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/_securetransport/low_level.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/appengine.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/ntlmpool.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/pyopenssl.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/securetransport.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/contrib/socks.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/exceptions.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/fields.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/filepost.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/packages/backports/makefile.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/packages/six.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/packages/ssl_match_hostname/__init__.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/packages/ssl_match_hostname/__init__.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/poolmanager.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/request.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/response.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/util/__init__.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/util/connection.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/util/proxy.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/util/request.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/util/response.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/util/retry.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/util/ssl_.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/util/ssltransport.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/util/timeout.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/util/url.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/_vendor/urllib3/util/wait.py` & `opensafely-1.9.2/opensafely/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/codelists.py` & `opensafely-1.9.2/opensafely/codelists.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/pull.py` & `opensafely-1.9.2/opensafely/pull.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely/upgrade.py` & `opensafely-1.9.2/opensafely/upgrade.py`

 * *Files identical despite different names*

### Comparing `opensafely-1.9.1/opensafely.egg-info/SOURCES.txt` & `opensafely-1.9.2/opensafely.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 opensafely/_vendor/jobrunner/config.py
 opensafely/_vendor/jobrunner/create_or_update_jobs.py
 opensafely/_vendor/jobrunner/database.py
 opensafely/_vendor/jobrunner/docker.py
 opensafely/_vendor/jobrunner/docker_stats.py
 opensafely/_vendor/jobrunner/extract_stats.py
 opensafely/_vendor/jobrunner/git.py
+opensafely/_vendor/jobrunner/github_validators.py
 opensafely/_vendor/jobrunner/job.py
 opensafely/_vendor/jobrunner/kill_job.py
 opensafely/_vendor/jobrunner/local_run.py
 opensafely/_vendor/jobrunner/log_utils.py
 opensafely/_vendor/jobrunner/manage_jobs.py
 opensafely/_vendor/jobrunner/models.py
 opensafely/_vendor/jobrunner/path_utils.py
```

### Comparing `opensafely-1.9.1/setup.py` & `opensafely-1.9.2/setup.py`

 * *Files identical despite different names*

