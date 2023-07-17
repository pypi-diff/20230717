# Comparing `tmp/iceprod-2.7.0.tar.gz` & `tmp/iceprod-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceprod-2.7.0.tar", last modified: Mon Jul 10 16:31:13 2023, max compression
+gzip compressed data, was "iceprod-2.7.1.tar", last modified: Mon Jul 17 21:10:48 2023, max compression
```

## Comparing `iceprod-2.7.0.tar` & `iceprod-2.7.1.tar`

### file list

```diff
@@ -1,161 +1,162 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.980805 iceprod-2.7.0/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-07-10 16:31:10.000000 iceprod-2.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2634 2023-07-10 16:31:13.980805 iceprod-2.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1774 2023-07-10 16:31:10.000000 iceprod-2.7.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.944805 iceprod-2.7.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)    10083 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/basic_submit.py
--rwxr-xr-x   0 root         (0) root         (0)     1331 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_add_site_to_master.py
--rwxr-xr-x   0 root         (0) root         (0)     1408 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_debugger.py
--rwxr-xr-x   0 root         (0) root         (0)     1095 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_gridftp_proxy.py
--rwxr-xr-x   0 root         (0) root         (0)     1330 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_join_pool.py
--rwxr-xr-x   0 root         (0) root         (0)     3330 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_rest.py
--rwxr-xr-x   0 root         (0) root         (0)     4606 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_server.py
--rwxr-xr-x   0 root         (0) root         (0)     7147 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprodsh
--rwxr-xr-x   0 root         (0) root         (0)     3697 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/loader.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.948805 iceprod-2.7.0/iceprod/
--rw-r--r--   0 root         (0) root         (0)      625 2023-07-10 16:31:11.000000 iceprod-2.7.0/iceprod/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/client_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.952805 iceprod-2.7.0/iceprod/core/
--rw-r--r--   0 root         (0) root         (0)     2295 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5339 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/data_transfer.py
--rw-r--r--   0 root         (0) root         (0)    33372 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/dataclasses.py
--rw-r--r--   0 root         (0) root         (0)      591 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)    45616 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/exe.py
--rw-r--r--   0 root         (0) root         (0)     4147 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/exe_helper.py
--rw-r--r--   0 root         (0) root         (0)    18581 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/exe_json.py
--rw-r--r--   0 root         (0) root         (0)     4927 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/file_catalog.py
--rw-r--r--   0 root         (0) root         (0)    15648 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/functions.py
--rw-r--r--   0 root         (0) root         (0)    16121 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/gridftp.py
--rw-r--r--   0 root         (0) root         (0)    21592 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/i3exec.py
--rw-r--r--   0 root         (0) root         (0)     6108 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/jsonUtil.py
--rw-r--r--   0 root         (0) root         (0)     4035 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/logger.py
--rw-r--r--   0 root         (0) root         (0)    20137 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/parser.py
--rw-r--r--   0 root         (0) root         (0)    25463 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/pilot.py
--rw-r--r--   0 root         (0) root         (0)    30084 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/resources.py
--rw-r--r--   0 root         (0) root         (0)     1949 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/serialization.py
--rw-r--r--   0 root         (0) root         (0)      556 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.956805 iceprod-2.7.0/iceprod/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/credentials/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/credentials/__main__.py
--rw-r--r--   0 root         (0) root         (0)    19558 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/credentials/server.py
--rw-r--r--   0 root         (0) root         (0)     6689 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/credentials/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.956805 iceprod-2.7.0/iceprod/materialization/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/materialization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/materialization/__main__.py
--rw-r--r--   0 root         (0) root         (0)    13731 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/materialization/materialize.py
--rw-r--r--   0 root         (0) root         (0)    14142 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/materialization/server.py
--rw-r--r--   0 root         (0) root         (0)     3247 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/materialization/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.956805 iceprod-2.7.0/iceprod/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.956805 iceprod-2.7.0/iceprod/rest/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4892 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/auth.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/base_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.960805 iceprod-2.7.0/iceprod/rest/handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6059 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/auth.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/config.py
--rw-r--r--   0 root         (0) root         (0)    12602 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/datasets.py
--rw-r--r--   0 root         (0) root         (0)     3804 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/grids.py
--rw-r--r--   0 root         (0) root         (0)    10884 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/jobs.py
--rw-r--r--   0 root         (0) root         (0)    11679 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/logs.py
--rw-r--r--   0 root         (0) root         (0)     5706 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/pilots.py
--rw-r--r--   0 root         (0) root         (0)     7201 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/task_stats.py
--rw-r--r--   0 root         (0) root         (0)    39857 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/tasks.py
--rw-r--r--   0 root         (0) root         (0)     5278 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/server.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/roles_groups.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.964805 iceprod-2.7.0/iceprod/server/
--rw-r--r--   0 root         (0) root         (0)     7572 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8125 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/config.py
--rw-r--r--   0 root         (0) root         (0)     6025 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.940805 iceprod-2.7.0/iceprod/server/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.964805 iceprod-2.7.0/iceprod/server/data/etc/
--rw-r--r--   0 root         (0) root         (0)     1272 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/etc/config_defaults.json
--rw-r--r--   0 root         (0) root         (0)     1820 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/etc/iceprod_schema.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.972805 iceprod-2.7.0/iceprod/server/data/www/
--rw-r--r--   0 root         (0) root         (0)     8624 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/base.css
--rw-r--r--   0 root         (0) root         (0)    13205 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/chart.stackedarea.js
--rw-r--r--   0 root         (0) root         (0)      646 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/chosen-sprite.png
--rw-r--r--   0 root         (0) root         (0)      872 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/chosen-sprite@2x.png
--rw-r--r--   0 root         (0) root         (0)    26966 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/chosen.jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    10751 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/chosen.min.css
--rw-r--r--   0 root         (0) root         (0)      643 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/documentation.css
--rw-r--r--   0 root         (0) root         (0)     1591 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/documentation.js
--rw-r--r--   0 root         (0) root         (0)     1150 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/favicon.ico
--rw-r--r--   0 root         (0) root         (0)      211 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/favicon.png
--rw-r--r--   0 root         (0) root         (0)    13277 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/fetch.js
--rw-r--r--   0 root         (0) root         (0)     1493 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/json-rpc.js
--rw-r--r--   0 root         (0) root         (0)     8775 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/jsonlint.js
--rw-r--r--   0 root         (0) root         (0)    46933 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/jsviews.min.js
--rw-r--r--   0 root         (0) root         (0)     3842 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/logo_155x60.png
--rw-r--r--   0 root         (0) root         (0)    10659 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/rest.js
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/robots.txt
--rw-r--r--   0 root         (0) root         (0)     5218 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/submit.css
--rw-r--r--   0 root         (0) root         (0)    29484 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/submit.js
--rw-r--r--   0 root         (0) root         (0)     7716 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/util.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.976805 iceprod-2.7.0/iceprod/server/data/www_templates/
--rw-r--r--   0 root         (0) root         (0)      315 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/404.html
--rw-r--r--   0 root         (0) root         (0)     3124 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/base.html
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/dataset_browse.html
--rw-r--r--   0 root         (0) root         (0)     4467 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/dataset_detail.html
--rw-r--r--   0 root         (0) root         (0)     2659 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/groups.html
--rw-r--r--   0 root         (0) root         (0)     2285 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/job_browse.html
--rw-r--r--   0 root         (0) root         (0)     2255 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/job_detail.html
--rw-r--r--   0 root         (0) root         (0)      611 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/login.html
--rw-r--r--   0 root         (0) root         (0)      183 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/logout.html
--rw-r--r--   0 root         (0) root         (0)      352 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/main.html
--rw-r--r--   0 root         (0) root         (0)     6133 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/profile.html
--rw-r--r--   0 root         (0) root         (0)     2121 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/site.html
--rw-r--r--   0 root         (0) root         (0)     6626 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/submit.html
--rw-r--r--   0 root         (0) root         (0)     1790 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/task_browse.html
--rw-r--r--   0 root         (0) root         (0)     4893 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/task_detail.html
--rw-r--r--   0 root         (0) root         (0)      360 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/tasks.html
--rw-r--r--   0 root         (0) root         (0)     4547 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/dataset_prio.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/documentation.py
--rw-r--r--   0 root         (0) root         (0)     3501 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/globus.py
--rw-r--r--   0 root         (0) root         (0)    30407 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/grid.py
--rw-r--r--   0 root         (0) root         (0)     6785 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.976805 iceprod-2.7.0/iceprod/server/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8067 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/modules/queue.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/modules/schedule.py
--rw-r--r--   0 root         (0) root         (0)    30111 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/modules/website.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.980805 iceprod-2.7.0/iceprod/server/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11131 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/condor.py
--rw-r--r--   0 root         (0) root         (0)    47154 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/condor_direct.py
--rw-r--r--   0 root         (0) root         (0)     2463 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/condor_file_transfer.py
--rw-r--r--   0 root         (0) root         (0)    33448 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/sc_demo.py
--rw-r--r--   0 root         (0) root         (0)    10523 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/supercomp_cedar.py
--rw-r--r--   0 root         (0) root         (0)    22909 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/supercomp_graham.py
--rw-r--r--   0 root         (0) root         (0)    10177 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/priority.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.980805 iceprod-2.7.0/iceprod/server/scheduled_tasks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2927 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3846 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     3492 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_completion.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3444 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/job_completion.py
--rw-r--r--   0 root         (0) root         (0)     4904 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/job_temp_cleaning.py
--rw-r--r--   0 root         (0) root         (0)     2088 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/log_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     5274 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/non_active_tasks.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/pilot_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/pilot_monitor.py
--rw-r--r--   0 root         (0) root         (0)     5355 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/queue_tasks.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/removed_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/reset_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3896 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/update_task_priority.py
--rw-r--r--   0 root         (0) root         (0)     3638 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/server.py
--rw-r--r--   0 root         (0) root         (0)     8715 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/ssl_cert.py
--rw-r--r--   0 root         (0) root         (0)     1344 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/task_queue.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.948805 iceprod-2.7.0/iceprod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2634 2023-07-10 16:31:13.000000 iceprod-2.7.0/iceprod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4798 2023-07-10 16:31:13.000000 iceprod-2.7.0/iceprod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 16:31:13.000000 iceprod-2.7.0/iceprod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      368 2023-07-10 16:31:13.000000 iceprod-2.7.0/iceprod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 16:31:13.000000 iceprod-2.7.0/iceprod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2090 2023-07-10 16:31:13.980805 iceprod-2.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      224 2023-07-10 16:31:10.000000 iceprod-2.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.290387 iceprod-2.7.1/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-17 21:10:44.000000 iceprod-2.7.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-07-17 21:10:48.290387 iceprod-2.7.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-07-17 21:10:44.000000 iceprod-2.7.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.258387 iceprod-2.7.1/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    10083 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/basic_submit.py
+-rwxr-xr-x   0 root         (0) root         (0)     1331 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_add_site_to_master.py
+-rwxr-xr-x   0 root         (0) root         (0)     1408 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_debugger.py
+-rwxr-xr-x   0 root         (0) root         (0)     1095 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_gridftp_proxy.py
+-rwxr-xr-x   0 root         (0) root         (0)     1330 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_join_pool.py
+-rwxr-xr-x   0 root         (0) root         (0)     3330 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_rest.py
+-rwxr-xr-x   0 root         (0) root         (0)     4606 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprod_server.py
+-rwxr-xr-x   0 root         (0) root         (0)     7147 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/iceprodsh
+-rwxr-xr-x   0 root         (0) root         (0)     3697 2023-07-17 21:10:44.000000 iceprod-2.7.1/bin/loader.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.262387 iceprod-2.7.1/iceprod/
+-rw-r--r--   0 root         (0) root         (0)      625 2023-07-17 21:10:45.000000 iceprod-2.7.1/iceprod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/client_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.266387 iceprod-2.7.1/iceprod/core/
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/data_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    33372 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/dataclasses.py
+-rw-r--r--   0 root         (0) root         (0)      591 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)    45616 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/exe.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/exe_helper.py
+-rw-r--r--   0 root         (0) root         (0)    18581 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/exe_json.py
+-rw-r--r--   0 root         (0) root         (0)     4927 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/file_catalog.py
+-rw-r--r--   0 root         (0) root         (0)    15935 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/functions.py
+-rw-r--r--   0 root         (0) root         (0)    16121 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/gridftp.py
+-rw-r--r--   0 root         (0) root         (0)    21592 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/i3exec.py
+-rw-r--r--   0 root         (0) root         (0)     6108 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/jsonUtil.py
+-rw-r--r--   0 root         (0) root         (0)     4035 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/logger.py
+-rw-r--r--   0 root         (0) root         (0)    20137 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/parser.py
+-rw-r--r--   0 root         (0) root         (0)    25463 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/pilot.py
+-rw-r--r--   0 root         (0) root         (0)    30084 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/serialization.py
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/core/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.270387 iceprod-2.7.1/iceprod/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/credentials/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/credentials/client.py
+-rw-r--r--   0 root         (0) root         (0)    19558 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/credentials/server.py
+-rw-r--r--   0 root         (0) root         (0)     6689 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/credentials/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.270387 iceprod-2.7.1/iceprod/materialization/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/materialization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/materialization/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    13731 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/materialization/materialize.py
+-rw-r--r--   0 root         (0) root         (0)    14142 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/materialization/server.py
+-rw-r--r--   0 root         (0) root         (0)     3247 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/materialization/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.270387 iceprod-2.7.1/iceprod/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.270387 iceprod-2.7.1/iceprod/rest/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4892 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/base_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.274387 iceprod-2.7.1/iceprod/rest/handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/auth.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/config.py
+-rw-r--r--   0 root         (0) root         (0)    12602 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/datasets.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/grids.py
+-rw-r--r--   0 root         (0) root         (0)    10884 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/jobs.py
+-rw-r--r--   0 root         (0) root         (0)    11679 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/logs.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/pilots.py
+-rw-r--r--   0 root         (0) root         (0)     7201 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/task_stats.py
+-rw-r--r--   0 root         (0) root         (0)    39857 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/handlers/tasks.py
+-rw-r--r--   0 root         (0) root         (0)     5278 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/rest/server.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/roles_groups.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.278387 iceprod-2.7.1/iceprod/server/
+-rw-r--r--   0 root         (0) root         (0)     7572 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8125 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/config.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.254387 iceprod-2.7.1/iceprod/server/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.278387 iceprod-2.7.1/iceprod/server/data/etc/
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/etc/config_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/etc/iceprod_schema.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.282387 iceprod-2.7.1/iceprod/server/data/www/
+-rw-r--r--   0 root         (0) root         (0)     8624 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/base.css
+-rw-r--r--   0 root         (0) root         (0)    13205 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/chart.stackedarea.js
+-rw-r--r--   0 root         (0) root         (0)      646 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/chosen-sprite.png
+-rw-r--r--   0 root         (0) root         (0)      872 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/chosen-sprite@2x.png
+-rw-r--r--   0 root         (0) root         (0)    26966 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/chosen.jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    10751 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/chosen.min.css
+-rw-r--r--   0 root         (0) root         (0)      643 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/documentation.css
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/documentation.js
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/favicon.png
+-rw-r--r--   0 root         (0) root         (0)    13277 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/fetch.js
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/json-rpc.js
+-rw-r--r--   0 root         (0) root         (0)     8775 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/jsonlint.js
+-rw-r--r--   0 root         (0) root         (0)    46933 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/jsviews.min.js
+-rw-r--r--   0 root         (0) root         (0)     3842 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/logo_155x60.png
+-rw-r--r--   0 root         (0) root         (0)    10659 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/rest.js
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/robots.txt
+-rw-r--r--   0 root         (0) root         (0)     5218 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/submit.css
+-rw-r--r--   0 root         (0) root         (0)    29484 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/submit.js
+-rw-r--r--   0 root         (0) root         (0)     7716 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www/util.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.286387 iceprod-2.7.1/iceprod/server/data/www_templates/
+-rw-r--r--   0 root         (0) root         (0)      315 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/404.html
+-rw-r--r--   0 root         (0) root         (0)     3124 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/dataset_browse.html
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/dataset_detail.html
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/groups.html
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/job_browse.html
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/job_detail.html
+-rw-r--r--   0 root         (0) root         (0)      611 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/login.html
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/logout.html
+-rw-r--r--   0 root         (0) root         (0)      352 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/main.html
+-rw-r--r--   0 root         (0) root         (0)     6133 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/profile.html
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/site.html
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/submit.html
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/task_browse.html
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/task_detail.html
+-rw-r--r--   0 root         (0) root         (0)      360 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/data/www_templates/tasks.html
+-rw-r--r--   0 root         (0) root         (0)     4547 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/dataset_prio.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/documentation.py
+-rw-r--r--   0 root         (0) root         (0)     3501 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/globus.py
+-rw-r--r--   0 root         (0) root         (0)    30710 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/grid.py
+-rw-r--r--   0 root         (0) root         (0)     6785 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.286387 iceprod-2.7.1/iceprod/server/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8067 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/modules/queue.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/modules/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    30111 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/modules/website.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.286387 iceprod-2.7.1/iceprod/server/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11131 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/condor.py
+-rw-r--r--   0 root         (0) root         (0)    47259 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/condor_direct.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/condor_file_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    33448 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/sc_demo.py
+-rw-r--r--   0 root         (0) root         (0)    10523 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/supercomp_cedar.py
+-rw-r--r--   0 root         (0) root         (0)    22909 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/plugins/supercomp_graham.py
+-rw-r--r--   0 root         (0) root         (0)    10177 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/priority.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.290387 iceprod-2.7.1/iceprod/server/scheduled_tasks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3846 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_completion.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/job_completion.py
+-rw-r--r--   0 root         (0) root         (0)     4904 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/job_temp_cleaning.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/log_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     5274 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/non_active_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/pilot_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/pilot_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     5355 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/queue_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/removed_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/reset_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3896 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/scheduled_tasks/update_task_priority.py
+-rw-r--r--   0 root         (0) root         (0)     3638 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     8715 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/ssl_cert.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/task_queue.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-17 21:10:44.000000 iceprod-2.7.1/iceprod/server/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:10:48.262387 iceprod-2.7.1/iceprod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-07-17 21:10:48.000000 iceprod-2.7.1/iceprod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-07-17 21:10:48.000000 iceprod-2.7.1/iceprod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 21:10:48.000000 iceprod-2.7.1/iceprod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      368 2023-07-17 21:10:48.000000 iceprod-2.7.1/iceprod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 21:10:48.000000 iceprod-2.7.1/iceprod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-07-17 21:10:48.294387 iceprod-2.7.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      224 2023-07-17 21:10:44.000000 iceprod-2.7.1/setup.py
```

### Comparing `iceprod-2.7.0/LICENSE` & `iceprod-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/PKG-INFO` & `iceprod-2.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceprod
-Version: 2.7.0
+Version: 2.7.1
 Summary: IceCube dataset management system
 Home-page: https://github.com/WIPACrepo/iceprod
 Download-URL: https://pypi.org/project/iceprod/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/iceprod/issues
```

### Comparing `iceprod-2.7.0/README.rst` & `iceprod-2.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/bin/basic_submit.py` & `iceprod-2.7.1/bin/basic_submit.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/bin/iceprod_add_site_to_master.py` & `iceprod-2.7.1/bin/iceprod_add_site_to_master.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/bin/iceprod_debugger.py` & `iceprod-2.7.1/bin/iceprod_debugger.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/bin/iceprod_gridftp_proxy.py` & `iceprod-2.7.1/bin/iceprod_gridftp_proxy.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/bin/iceprod_join_pool.py` & `iceprod-2.7.1/bin/iceprod_join_pool.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/bin/iceprod_rest.py` & `iceprod-2.7.1/bin/iceprod_rest.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/bin/iceprod_server.py` & `iceprod-2.7.1/bin/iceprod_server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/bin/iceprodsh` & `iceprod-2.7.1/bin/iceprodsh`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/bin/loader.sh` & `iceprod-2.7.1/bin/loader.sh`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/__init__.py` & `iceprod-2.7.1/iceprod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.7.0"
+__version__ = "2.7.1"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `iceprod-2.7.0/iceprod/client_auth.py` & `iceprod-2.7.1/iceprod/client_auth.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/__init__.py` & `iceprod-2.7.1/iceprod/core/__init__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/data_transfer.py` & `iceprod-2.7.1/iceprod/core/data_transfer.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/dataclasses.py` & `iceprod-2.7.1/iceprod/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/defaults.py` & `iceprod-2.7.1/iceprod/core/defaults.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/exe.py` & `iceprod-2.7.1/iceprod/core/exe.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/exe_helper.py` & `iceprod-2.7.1/iceprod/core/exe_helper.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/exe_json.py` & `iceprod-2.7.1/iceprod/core/exe_json.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/file_catalog.py` & `iceprod-2.7.1/iceprod/core/file_catalog.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/functions.py` & `iceprod-2.7.1/iceprod/core/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,24 +411,29 @@
                             m = MultipartEncoder(
                                 fields={'field0': ('filename', f, 'text/plain')}
                             )
                             r = s.post(url, timeout=300, data=m,
                                        headers={'Content-Type': m.content_type})
                             r.raise_for_status()
                 if checksum:  # get checksum
-                    r = s.get(url, stream=True, timeout=300)
-                    try:
-                        with open(local+'.tmp', 'wb') as f:
-                            for chunk in r.iter_content(65536):
-                                f.write(chunk)
-                        r.raise_for_status()
-                        if sha512sum(local+'.tmp') != chksum:
+                    if 'ETAG' in r.headers:
+                        md5 = r.headers['ETAG'].strip('"\'')
+                        if md5sum(local) != md5:
                             raise Exception('http checksum error')
-                    finally:
-                        removedirs(local+'.tmp')
+                    else:
+                        r = s.get(url, stream=True, timeout=300)
+                        try:
+                            with open(local+'.tmp', 'wb') as f:
+                                for chunk in r.iter_content(65536):
+                                    f.write(chunk)
+                            r.raise_for_status()
+                            if sha512sum(local+'.tmp') != chksum:
+                                raise Exception('http checksum error')
+                        finally:
+                            removedirs(local+'.tmp')
         await asyncio.get_event_loop().run_in_executor(None, _d)
     elif url.startswith('file:'):
         # use copy command
         url = url[5:]
 
         def _c():
             if os.path.exists(url):
```

### Comparing `iceprod-2.7.0/iceprod/core/gridftp.py` & `iceprod-2.7.1/iceprod/core/gridftp.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/i3exec.py` & `iceprod-2.7.1/iceprod/core/i3exec.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/jsonUtil.py` & `iceprod-2.7.1/iceprod/core/jsonUtil.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/logger.py` & `iceprod-2.7.1/iceprod/core/logger.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/parser.py` & `iceprod-2.7.1/iceprod/core/parser.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/pilot.py` & `iceprod-2.7.1/iceprod/core/pilot.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/resources.py` & `iceprod-2.7.1/iceprod/core/resources.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/serialization.py` & `iceprod-2.7.1/iceprod/core/serialization.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/core/util.py` & `iceprod-2.7.1/iceprod/core/util.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/credentials/__main__.py` & `iceprod-2.7.1/iceprod/credentials/__main__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/credentials/server.py` & `iceprod-2.7.1/iceprod/credentials/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/credentials/service.py` & `iceprod-2.7.1/iceprod/credentials/service.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/materialization/__main__.py` & `iceprod-2.7.1/iceprod/materialization/__main__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/materialization/materialize.py` & `iceprod-2.7.1/iceprod/materialization/materialize.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/materialization/server.py` & `iceprod-2.7.1/iceprod/materialization/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/materialization/service.py` & `iceprod-2.7.1/iceprod/materialization/service.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/__main__.py` & `iceprod-2.7.1/iceprod/rest/__main__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/auth.py` & `iceprod-2.7.1/iceprod/rest/auth.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/base_handler.py` & `iceprod-2.7.1/iceprod/rest/base_handler.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/handlers/auth.py` & `iceprod-2.7.1/iceprod/rest/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/handlers/config.py` & `iceprod-2.7.1/iceprod/rest/handlers/config.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/handlers/datasets.py` & `iceprod-2.7.1/iceprod/rest/handlers/datasets.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/handlers/grids.py` & `iceprod-2.7.1/iceprod/rest/handlers/grids.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/handlers/jobs.py` & `iceprod-2.7.1/iceprod/rest/handlers/jobs.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/handlers/logs.py` & `iceprod-2.7.1/iceprod/rest/handlers/logs.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/handlers/pilots.py` & `iceprod-2.7.1/iceprod/rest/handlers/pilots.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/handlers/task_stats.py` & `iceprod-2.7.1/iceprod/rest/handlers/task_stats.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/handlers/tasks.py` & `iceprod-2.7.1/iceprod/rest/handlers/tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/rest/server.py` & `iceprod-2.7.1/iceprod/rest/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/s3.py` & `iceprod-2.7.1/iceprod/s3.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/__init__.py` & `iceprod-2.7.1/iceprod/server/__init__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/config.py` & `iceprod-2.7.1/iceprod/server/config.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/daemon.py` & `iceprod-2.7.1/iceprod/server/daemon.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/etc/config_defaults.json` & `iceprod-2.7.1/iceprod/server/data/etc/config_defaults.json`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/etc/iceprod_schema.json` & `iceprod-2.7.1/iceprod/server/data/etc/iceprod_schema.json`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/base.css` & `iceprod-2.7.1/iceprod/server/data/www/base.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/chart.stackedarea.js` & `iceprod-2.7.1/iceprod/server/data/www/chart.stackedarea.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/chosen-sprite.png` & `iceprod-2.7.1/iceprod/server/data/www/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/chosen-sprite@2x.png` & `iceprod-2.7.1/iceprod/server/data/www/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/chosen.jquery.min.js` & `iceprod-2.7.1/iceprod/server/data/www/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/chosen.min.css` & `iceprod-2.7.1/iceprod/server/data/www/chosen.min.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/documentation.css` & `iceprod-2.7.1/iceprod/server/data/www/documentation.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/documentation.js` & `iceprod-2.7.1/iceprod/server/data/www/documentation.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/favicon.ico` & `iceprod-2.7.1/iceprod/server/data/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/fetch.js` & `iceprod-2.7.1/iceprod/server/data/www/fetch.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/json-rpc.js` & `iceprod-2.7.1/iceprod/server/data/www/json-rpc.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/jsonlint.js` & `iceprod-2.7.1/iceprod/server/data/www/jsonlint.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/jsviews.min.js` & `iceprod-2.7.1/iceprod/server/data/www/jsviews.min.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/logo_155x60.png` & `iceprod-2.7.1/iceprod/server/data/www/logo_155x60.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/rest.js` & `iceprod-2.7.1/iceprod/server/data/www/rest.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/submit.css` & `iceprod-2.7.1/iceprod/server/data/www/submit.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/submit.js` & `iceprod-2.7.1/iceprod/server/data/www/submit.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www/util.js` & `iceprod-2.7.1/iceprod/server/data/www/util.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/base.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/base.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/dataset_browse.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/dataset_browse.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/dataset_detail.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/dataset_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/groups.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/groups.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/job_browse.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/job_browse.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/job_detail.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/job_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/login.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/login.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/profile.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/profile.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/site.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/site.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/submit.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/submit.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/task_browse.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/task_browse.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/data/www_templates/task_detail.html` & `iceprod-2.7.1/iceprod/server/data/www_templates/task_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/dataset_prio.py` & `iceprod-2.7.1/iceprod/server/dataset_prio.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/documentation.py` & `iceprod-2.7.1/iceprod/server/documentation.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/globus.py` & `iceprod-2.7.1/iceprod/server/globus.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/grid.py` & `iceprod-2.7.1/iceprod/server/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,15 +447,16 @@
                 queued_time = timedelta(seconds=self.queue_cfg['max_task_queued_time'])
             except Exception:
                 queued_time = timedelta(seconds=86400*2)
             try:
                 processing_time = timedelta(seconds=self.queue_cfg['max_task_processing_time'])
             except Exception:
                 processing_time = timedelta(seconds=86400*2)
-            expiration = (queued_time + processing_time).seconds
+            expiration = (queued_time + processing_time).total_seconds()
+            logger.info(f's3 cred expire time: {expiration}')
 
             def presign_s3(cfg):
                 new_data = []
                 for d in cfg.get('data', []):
                     for url in s3_creds:
                         if d['remote'].startswith(url):
                             logger.info('found data for cred: %s', url)
@@ -465,15 +466,19 @@
                                 bucket, key = path.split('/', 1)
                             if (not bucket) or bucket not in s3_creds[url]['buckets']:
                                 key = path
                                 bucket = urlparse(url).hostname.split('.', 1)[0]
                                 if bucket not in s3_creds[url]['buckets']:
                                     raise RuntimeError('bad s3 bucket')
 
+                            while key.startswith('/'):
+                                key = key[1:]
+
                             s = S3(url, s3_creds[url]['access_key'], s3_creds[url]['secret_key'], bucket=bucket)
+                            logger.info(f'S3 url={url} bucket={bucket} key={key}')
                             if d['movement'] == 'input':
                                 d['remote'] = s.get_presigned(key, expiration=expiration)
                                 new_data.append(d)
                             elif d['movement'] == 'output':
                                 d['remote'] = s.put_presigned(key, expiration=expiration)
                             elif d['movement'] == 'both':
                                 d['movement'] = 'input'
@@ -587,15 +592,15 @@
             config['options']['dataset_id'] = task['dataset_id']
         if 'dataset' in task:
             config['options']['dataset'] = task['dataset']
         config['options']['stillrunninginterval'] = self.queue_cfg['ping_interval']
         config['options']['debug'] = task['debug']
         config['options']['upload'] = 'logging'
         config['options']['gridspec'] = self.gridspec
-        if 'site_temp' in self.cfg['queue']:
+        if (not config['options'].get('site_temp','')) and 'site_temp' in self.cfg['queue']:
             config['options']['site_temp'] = self.cfg['queue']['site_temp']
         if ('download' in self.cfg and 'http_username' in self.cfg['download']
                 and self.cfg['download']['http_username']):
             config['options']['username'] = self.cfg['download']['http_username']
         if ('download' in self.cfg and 'http_password' in self.cfg['download']
                 and self.cfg['download']['http_password']):
             config['options']['password'] = self.cfg['download']['http_password']
```

### Comparing `iceprod-2.7.0/iceprod/server/module.py` & `iceprod-2.7.1/iceprod/server/module.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/modules/queue.py` & `iceprod-2.7.1/iceprod/server/modules/queue.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/modules/schedule.py` & `iceprod-2.7.1/iceprod/server/modules/schedule.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/modules/website.py` & `iceprod-2.7.1/iceprod/server/modules/website.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/plugins/condor.py` & `iceprod-2.7.1/iceprod/server/plugins/condor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/plugins/condor_direct.py` & `iceprod-2.7.1/iceprod/server/plugins/condor_direct.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,17 @@
                                 except Exception:
                                     pass
                         elif 'disk usage exceeded' in line:
                             resource_type = 'disk'
                         if resource_type:
                             if val:
                                 resources[resource_type] = val
-                            reason = f'Resource overusage for {resource_type}: {resources[resource_type]}'
+                            reason = f'Resource overusage for {resource_type}: '
+                            if resource_type in resources:
+                                reason += f'{resources[resource_type]}'
                             break
                     elif 'Transfer output files failure' in line:
                         reason = 'Failed to transfer output files'
                         break
                     elif 'Transfer input files failure' in line:
                         reason = 'Failed to transfer input files'
                         break
```

### Comparing `iceprod-2.7.0/iceprod/server/plugins/condor_file_transfer.py` & `iceprod-2.7.1/iceprod/server/plugins/condor_file_transfer.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/plugins/sc_demo.py` & `iceprod-2.7.1/iceprod/server/plugins/sc_demo.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/plugins/supercomp_cedar.py` & `iceprod-2.7.1/iceprod/server/plugins/supercomp_cedar.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/plugins/supercomp_graham.py` & `iceprod-2.7.1/iceprod/server/plugins/supercomp_graham.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/priority.py` & `iceprod-2.7.1/iceprod/server/priority.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_cleanup.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_completion.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_completion.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_monitor.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/dataset_monitor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/job_completion.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/job_completion.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/job_temp_cleaning.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/job_temp_cleaning.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/log_cleanup.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/log_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/non_active_tasks.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/non_active_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/pilot_cleanup.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/pilot_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/pilot_monitor.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/pilot_monitor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/queue_tasks.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/queue_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/removed_tasks.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/removed_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/reset_tasks.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/reset_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/scheduled_tasks/update_task_priority.py` & `iceprod-2.7.1/iceprod/server/scheduled_tasks/update_task_priority.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/server.py` & `iceprod-2.7.1/iceprod/server/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/ssl_cert.py` & `iceprod-2.7.1/iceprod/server/ssl_cert.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/task_queue.py` & `iceprod-2.7.1/iceprod/server/task_queue.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod/server/util.py` & `iceprod-2.7.1/iceprod/server/util.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.7.0/iceprod.egg-info/PKG-INFO` & `iceprod-2.7.1/iceprod.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceprod
-Version: 2.7.0
+Version: 2.7.1
 Summary: IceCube dataset management system
 Home-page: https://github.com/WIPACrepo/iceprod
 Download-URL: https://pypi.org/project/iceprod/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/iceprod/issues
```

### Comparing `iceprod-2.7.0/iceprod.egg-info/SOURCES.txt` & `iceprod-2.7.1/iceprod.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 iceprod/core/parser.py
 iceprod/core/pilot.py
 iceprod/core/resources.py
 iceprod/core/serialization.py
 iceprod/core/util.py
 iceprod/credentials/__init__.py
 iceprod/credentials/__main__.py
+iceprod/credentials/client.py
 iceprod/credentials/server.py
 iceprod/credentials/service.py
 iceprod/materialization/__init__.py
 iceprod/materialization/__main__.py
 iceprod/materialization/materialize.py
 iceprod/materialization/server.py
 iceprod/materialization/service.py
```

### Comparing `iceprod-2.7.0/setup.cfg` & `iceprod-2.7.1/setup.cfg`

 * *Files identical despite different names*

