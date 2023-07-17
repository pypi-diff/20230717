# Comparing `tmp/gunicorn-21.0.0.tar.gz` & `tmp/gunicorn-21.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunicorn-21.0.0.tar", last modified: Mon Jul 17 20:28:19 2023, max compression
+gzip compressed data, was "gunicorn-21.0.1.tar", last modified: Mon Jul 17 21:22:35 2023, max compression
```

## Comparing `gunicorn-21.0.0.tar` & `gunicorn-21.0.1.tar`

### file list

```diff
@@ -1,357 +1,485 @@
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.048336 gunicorn-21.0.0/
--rwxr-xr-x   0 benoitc    (501) staff       (20)      267 2023-07-17 19:03:36.000000 gunicorn-21.0.0/.gitignore
--rw-r--r--   0 benoitc    (501) staff       (20)     1136 2023-07-17 19:03:36.000000 gunicorn-21.0.0/LICENSE
--rw-r--r--   0 benoitc    (501) staff       (20)      324 2023-07-17 19:03:36.000000 gunicorn-21.0.0/MANIFEST.in
--rw-r--r--   0 benoitc    (501) staff       (20)     3777 2023-07-17 19:03:36.000000 gunicorn-21.0.0/NOTICE
--rw-r--r--   0 benoitc    (501) staff       (20)     3852 2023-07-17 20:28:19.048396 gunicorn-21.0.0/PKG-INFO
--rw-r--r--   0 benoitc    (501) staff       (20)     1988 2023-07-17 19:03:36.000000 gunicorn-21.0.0/README.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6969 2023-07-17 19:03:36.000000 gunicorn-21.0.0/THANKS
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.016334 gunicorn-21.0.0/docs/
--rw-r--r--   0 benoitc    (501) staff       (20)     5791 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/Makefile
--rw-r--r--   0 benoitc    (501) staff       (20)      288 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/README.rst
--rwxr-xr-x   0 benoitc    (501) staff       (20)     3029 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/gunicorn_ext.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.016592 gunicorn-21.0.0/docs/logo/
--rw-r--r--   0 benoitc    (501) staff       (20)    21550 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/logo/gunicorn.png
--rw-r--r--   0 benoitc    (501) staff       (20)    12798 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/logo/gunicorn.svg
--rw-r--r--   0 benoitc    (501) staff       (20)     5109 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/make.bat
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.018512 gunicorn-21.0.0/docs/site/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/.nojekyll
--rw-r--r--   0 benoitc    (501) staff       (20)       13 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/CNAME
--rw-r--r--   0 benoitc    (501) staff       (20)      340 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/community.html
--rw-r--r--   0 benoitc    (501) staff       (20)      304 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/configuration.html
--rw-r--r--   0 benoitc    (501) staff       (20)      300 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/configure.html
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.018612 gunicorn-21.0.0/docs/site/css/
--rw-r--r--   0 benoitc    (501) staff       (20)     6671 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/css/style.css
--rw-r--r--   0 benoitc    (501) staff       (20)      343 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/deploy.html
--rw-r--r--   0 benoitc    (501) staff       (20)      342 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/deployment.html
--rw-r--r--   0 benoitc    (501) staff       (20)      297 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/design.html
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/faq.html
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.020586 gunicorn-21.0.0/docs/site/images/
--rw-r--r--   0 benoitc    (501) staff       (20)    17551 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/about.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)      408 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/arrow.png
--rw-r--r--   0 benoitc    (501) staff       (20)      611 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/banner-bg.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)    15593 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/community.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)    17566 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/documents.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)    15962 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/downloads.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     1771 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/favicon.png
--rw-r--r--   0 benoitc    (501) staff       (20)      255 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/footer-arrow.png
--rw-r--r--   0 benoitc    (501) staff       (20)     2499 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/footer-logo.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)      335 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/greenbutton.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     1553 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/gunicorn.png
--rw-r--r--   0 benoitc    (501) staff       (20)    21956 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/large_gunicorn.png
--rw-r--r--   0 benoitc    (501) staff       (20)     3145 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/logo-bottom.png
--rw-r--r--   0 benoitc    (501) staff       (20)    10238 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/logo.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     7343 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/logo.png
--rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/redbutton.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)      440 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/separator.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     3450 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/title.png
--rw-r--r--   0 benoitc    (501) staff       (20)     2184 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/images/user1.jpg
--rw-r--r--   0 benoitc    (501) staff       (20)     7856 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/index.html
--rw-r--r--   0 benoitc    (501) staff       (20)      298 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/install.html
--rw-r--r--   0 benoitc    (501) staff       (20)      298 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/installation.html
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.020685 gunicorn-21.0.0/docs/site/js/
--rwxr-xr-x   0 benoitc    (501) staff       (20)     1479 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/js/main.js
--rw-r--r--   0 benoitc    (501) staff       (20)      295 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/news.html
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/run.html
--rw-r--r--   0 benoitc    (501) staff       (20)     1990 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/sitemap.xml
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/tuning.html
--rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/site/usage.html
--rw-r--r--   0 benoitc    (501) staff       (20)     2088 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/sitemap_gen.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.023305 gunicorn-21.0.0/docs/source/
--rw-r--r--   0 benoitc    (501) staff       (20)     6643 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2010-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2092 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2011-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     4184 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2012-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     3267 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2013-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6834 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2014-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     5702 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2015-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2911 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2016-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2100 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2017-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     2956 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2018-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     4785 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2019-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)      112 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2020-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1905 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/2021-news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)      530 2023-07-17 20:14:25.000000 gunicorn-21.0.0/docs/source/2023-news.rst
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.023404 gunicorn-21.0.0/docs/source/_static/
--rw-r--r--   0 benoitc    (501) staff       (20)    14398 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/_static/gunicorn.png
--rw-r--r--   0 benoitc    (501) staff       (20)     1377 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/community.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1755 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/conf.py
--rw-r--r--   0 benoitc    (501) staff       (20)     3873 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/configure.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1927 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/custom.rst
--rw-r--r--   0 benoitc    (501) staff       (20)    12260 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/deploy.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6483 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/design.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     8672 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/faq.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1043 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/index.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     5551 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/install.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     1325 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/instrumentation.rst
--rw-r--r--   0 benoitc    (501) staff       (20)      727 2023-07-17 20:14:25.000000 gunicorn-21.0.0/docs/source/news.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     6485 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/run.rst
--rw-r--r--   0 benoitc    (501) staff       (20)    36932 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/settings.rst
--rw-r--r--   0 benoitc    (501) staff       (20)     5420 2023-07-17 19:03:36.000000 gunicorn-21.0.0/docs/source/signals.rst
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.025797 gunicorn-21.0.0/examples/
--rw-r--r--   0 benoitc    (501) staff       (20)      738 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/alt_spec.py
--rw-r--r--   0 benoitc    (501) staff       (20)      204 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/bad.py
--rw-r--r--   0 benoitc    (501) staff       (20)      108 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/boot_fail.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.025966 gunicorn-21.0.0/examples/deep/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/deep/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)      659 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/deep/test.py
--rw-r--r--   0 benoitc    (501) staff       (20)      676 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/echo.py
--rw-r--r--   0 benoitc    (501) staff       (20)     7621 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/example_config.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.027234 gunicorn-21.0.0/examples/frameworks/
--rw-r--r--   0 benoitc    (501) staff       (20)      198 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/cherryapp.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.027336 gunicorn-21.0.0/examples/frameworks/django/
--rw-r--r--   0 benoitc    (501) staff       (20)       60 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/README
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.027432 gunicorn-21.0.0/examples/frameworks/django/testing/
--rwxr-xr-x   0 benoitc    (501) staff       (20)      244 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/manage.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.027820 gunicorn-21.0.0/examples/frameworks/django/testing/testing/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/__init__.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.027924 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/__init__.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.028472 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/
--rwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)      627 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/middleware.py
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/models.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.028675 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/templates/
--rw-r--r--   0 benoitc    (501) staff       (20)      759 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html
--rw-r--r--   0 benoitc    (501) staff       (20)      471 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/templates/home.html
--rwxr-xr-x   0 benoitc    (501) staff       (20)      509 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/tests.py
--rw-r--r--   0 benoitc    (501) staff       (20)      133 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/urls.py
--rwxr-xr-x   0 benoitc    (501) staff       (20)     1548 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/views.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5730 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/settings.py
--rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/urls.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1359 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/django/testing/testing/wsgi.py
--rw-r--r--   0 benoitc    (501) staff       (20)      291 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/flask_sendfile.py
--rw-r--r--   0 benoitc    (501) staff       (20)      147 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/flaskapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)      501 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/flaskapp_aiohttp_wsgi.py
--rw-r--r--   0 benoitc    (501) staff       (20)      338 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/pyramidapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)      150 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        9 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements_cherryapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        6 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements_flaskapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        8 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements_pyramidapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)       10 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements_tornadoapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        7 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/requirements_webpyapp.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      873 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/tornadoapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)      197 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/frameworks/webpyapp.py
--rwxr-xr-x   0 benoitc    (501) staff       (20)      215 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/gunicorn_rc
--rw-r--r--   0 benoitc    (501) staff       (20)       13 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/hello.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      448 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/log_app.ini
--rw-r--r--   0 benoitc    (501) staff       (20)      372 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/log_app.py
--rw-r--r--   0 benoitc    (501) staff       (20)      841 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/logging.conf
--rw-r--r--   0 benoitc    (501) staff       (20)      737 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/longpoll.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1470 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/multiapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)      993 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/multidomainapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1980 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/nginx.conf
--rw-r--r--   0 benoitc    (501) staff       (20)      403 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/read_django_settings.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1015 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/readline_app.py
--rw-r--r--   0 benoitc    (501) staff       (20)      584 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/sendfile.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1257 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/server.crt
--rw-r--r--   0 benoitc    (501) staff       (20)     1679 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/server.key
--rw-r--r--   0 benoitc    (501) staff       (20)      604 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/slowclient.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1339 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/standalone_app.py
--rw-r--r--   0 benoitc    (501) staff       (20)      182 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/supervisor.conf
--rw-r--r--   0 benoitc    (501) staff       (20)      659 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/test.py
--rw-r--r--   0 benoitc    (501) staff       (20)      620 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/timeout.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.028963 gunicorn-21.0.0/examples/websocket/
--rw-r--r--   0 benoitc    (501) staff       (20)    15684 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/websocket/gevent_websocket.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1320 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/websocket/websocket.html
--rw-r--r--   0 benoitc    (501) staff       (20)    15729 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/websocket/websocket.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1020 2023-07-17 19:03:36.000000 gunicorn-21.0.0/examples/when_ready.conf.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.030196 gunicorn-21.0.0/gunicorn/
--rw-r--r--   0 benoitc    (501) staff       (20)      279 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)      171 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/__main__.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.031323 gunicorn-21.0.0/gunicorn/app/
--rw-r--r--   0 benoitc    (501) staff       (20)      127 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/app/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     7400 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/app/base.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2038 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/app/pasterapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1926 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/app/wsgiapp.py
--rw-r--r--   0 benoitc    (501) staff       (20)    21509 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/arbiter.py
--rw-r--r--   0 benoitc    (501) staff       (20)    63419 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/config.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2293 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/debug.py
--rw-r--r--   0 benoitc    (501) staff       (20)      919 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/errors.py
--rw-r--r--   0 benoitc    (501) staff       (20)    15303 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/glogging.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.031999 gunicorn-21.0.0/gunicorn/http/
--rw-r--r--   0 benoitc    (501) staff       (20)      277 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     7296 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/body.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2850 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/errors.py
--rw-r--r--   0 benoitc    (501) staff       (20)    11958 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/message.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1364 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/parser.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1943 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/unreader.py
--rw-r--r--   0 benoitc    (501) staff       (20)    12366 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/http/wsgi.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.032179 gunicorn-21.0.0/gunicorn/instrument/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/instrument/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4690 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/instrument/statsd.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2367 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/pidfile.py
--rw-r--r--   0 benoitc    (501) staff       (20)     3791 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/reloader.py
--rw-r--r--   0 benoitc    (501) staff       (20)     6887 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/sock.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2520 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/systemd.py
--rw-r--r--   0 benoitc    (501) staff       (20)    19104 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/util.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.033039 gunicorn-21.0.0/gunicorn/workers/
--rw-r--r--   0 benoitc    (501) staff       (20)      594 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)     9197 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/base.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5681 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/base_async.py
--rw-r--r--   0 benoitc    (501) staff       (20)     6091 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/geventlet.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5800 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/ggevent.py
--rw-r--r--   0 benoitc    (501) staff       (20)    12585 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/gthread.py
--rw-r--r--   0 benoitc    (501) staff       (20)     5854 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/gtornado.py
--rw-r--r--   0 benoitc    (501) staff       (20)     7272 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/sync.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1651 2023-07-17 19:03:36.000000 gunicorn-21.0.0/gunicorn/workers/workertmp.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.030921 gunicorn-21.0.0/gunicorn.egg-info/
--rw-r--r--   0 benoitc    (501) staff       (20)     3852 2023-07-17 20:28:18.000000 gunicorn-21.0.0/gunicorn.egg-info/PKG-INFO
--rw-r--r--   0 benoitc    (501) staff       (20)     9249 2023-07-17 20:28:19.000000 gunicorn-21.0.0/gunicorn.egg-info/SOURCES.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        1 2023-07-17 20:28:18.000000 gunicorn-21.0.0/gunicorn.egg-info/dependency_links.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      113 2023-07-17 20:28:18.000000 gunicorn-21.0.0/gunicorn.egg-info/entry_points.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        1 2023-07-17 20:27:30.000000 gunicorn-21.0.0/gunicorn.egg-info/not-zip-safe
--rw-r--r--   0 benoitc    (501) staff       (20)      173 2023-07-17 20:28:18.000000 gunicorn-21.0.0/gunicorn.egg-info/requires.txt
--rw-r--r--   0 benoitc    (501) staff       (20)        9 2023-07-17 20:28:18.000000 gunicorn-21.0.0/gunicorn.egg-info/top_level.txt
--rw-r--r--   0 benoitc    (501) staff       (20)       50 2023-07-17 19:03:36.000000 gunicorn-21.0.0/requirements_dev.txt
--rw-r--r--   0 benoitc    (501) staff       (20)       56 2023-07-17 19:20:23.000000 gunicorn-21.0.0/requirements_test.txt
--rw-r--r--   0 benoitc    (501) staff       (20)      203 2023-07-17 20:28:19.048669 gunicorn-21.0.0/setup.cfg
--rw-r--r--   0 benoitc    (501) staff       (20)     3555 2023-07-17 19:03:36.000000 gunicorn-21.0.0/setup.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.034618 gunicorn-21.0.0/tests/
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.035095 gunicorn-21.0.0/tests/config/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/config/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)       88 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/config/test_cfg.py
--rw-r--r--   0 benoitc    (501) staff       (20)       24 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/config/test_cfg_alt.py
--rw-r--r--   0 benoitc    (501) staff       (20)       23 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/config/test_cfg_with_wsgi_app.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.014457 gunicorn-21.0.0/tests/requests/
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.041274 gunicorn-21.0.0/tests/requests/invalid/
--rw-r--r--   0 benoitc    (501) staff       (20)       29 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/001.http
--rw-r--r--   0 benoitc    (501) staff       (20)       64 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/001.py
--rw-r--r--   0 benoitc    (501) staff       (20)       21 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/002.http
--rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/002.py
--rw-r--r--   0 benoitc    (501) staff       (20)       30 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/003.http
--rw-r--r--   0 benoitc    (501) staff       (20)       84 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/003.py
--rw-r--r--   0 benoitc    (501) staff       (20)       25 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/004.http
--rw-r--r--   0 benoitc    (501) staff       (20)       80 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/004.py
--rw-r--r--   0 benoitc    (501) staff       (20)       41 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/005.http
--rw-r--r--   0 benoitc    (501) staff       (20)       78 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/005.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4122 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/006.http
--rw-r--r--   0 benoitc    (501) staff       (20)       77 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/006.py
--rw-r--r--   0 benoitc    (501) staff       (20)     8358 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/007.http
--rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/007.py
--rw-r--r--   0 benoitc    (501) staff       (20)    12418 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/008.http
--rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/008.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1829 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/009.http
--rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/009.py
--rw-r--r--   0 benoitc    (501) staff       (20)       44 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/010.http
--rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/010.py
--rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/011.http
--rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/011.py
--rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/012.http
--rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/012.py
--rw-r--r--   0 benoitc    (501) staff       (20)       49 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/013.http
--rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/013.py
--rw-r--r--   0 benoitc    (501) staff       (20)       78 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/014.http
--rw-r--r--   0 benoitc    (501) staff       (20)       72 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/014.py
--rw-r--r--   0 benoitc    (501) staff       (20)       88 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/015.http
--rw-r--r--   0 benoitc    (501) staff       (20)       72 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/015.py
--rw-r--r--   0 benoitc    (501) staff       (20)       33 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/016.http
--rw-r--r--   0 benoitc    (501) staff       (20)       82 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/016.py
--rw-r--r--   0 benoitc    (501) staff       (20)     8222 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/017.http
--rw-r--r--   0 benoitc    (501) staff       (20)      134 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/017.py
--rw-r--r--   0 benoitc    (501) staff       (20)       48 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/018.http
--rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/018.py
--rw-r--r--   0 benoitc    (501) staff       (20)       82 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/019.http
--rw-r--r--   0 benoitc    (501) staff       (20)      172 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/019.py
--rw-r--r--   0 benoitc    (501) staff       (20)       69 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/020.http
--rw-r--r--   0 benoitc    (501) staff       (20)      130 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/020.py
--rw-r--r--   0 benoitc    (501) staff       (20)       90 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/021.http
--rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/021.py
--rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/022.http
--rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/022.py
--rw-r--r--   0 benoitc    (501) staff       (20)       52 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/023.http
--rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/023.py
--rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/024.http
--rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/024.py
--rw-r--r--   0 benoitc    (501) staff       (20)       37 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/pp_01.http
--rw-r--r--   0 benoitc    (501) staff       (20)      161 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/pp_01.py
--rw-r--r--   0 benoitc    (501) staff       (20)       53 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/pp_02.http
--rw-r--r--   0 benoitc    (501) staff       (20)      161 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/invalid/pp_02.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.047965 gunicorn-21.0.0/tests/requests/valid/
--rw-r--r--   0 benoitc    (501) staff       (20)      149 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/001.http
--rw-r--r--   0 benoitc    (501) staff       (20)      275 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/001.py
--rw-r--r--   0 benoitc    (501) staff       (20)      168 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/002.http
--rw-r--r--   0 benoitc    (501) staff       (20)      296 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/002.py
--rw-r--r--   0 benoitc    (501) staff       (20)      394 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/003.http
--rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/003.py
--rw-r--r--   0 benoitc    (501) staff       (20)       57 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/004.http
--rw-r--r--   0 benoitc    (501) staff       (20)      164 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/004.py
--rw-r--r--   0 benoitc    (501) staff       (20)       62 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/005.http
--rw-r--r--   0 benoitc    (501) staff       (20)      153 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/005.py
--rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/006.http
--rw-r--r--   0 benoitc    (501) staff       (20)      142 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/006.py
--rw-r--r--   0 benoitc    (501) staff       (20)       61 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/007.http
--rw-r--r--   0 benoitc    (501) staff       (20)      167 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/007.py
--rw-r--r--   0 benoitc    (501) staff       (20)       73 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/008.http
--rw-r--r--   0 benoitc    (501) staff       (20)      178 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/008.py
--rw-r--r--   0 benoitc    (501) staff       (20)      137 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/009.http
--rw-r--r--   0 benoitc    (501) staff       (20)      264 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/009.py
--rw-r--r--   0 benoitc    (501) staff       (20)      134 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/010.http
--rw-r--r--   0 benoitc    (501) staff       (20)      218 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/010.py
--rw-r--r--   0 benoitc    (501) staff       (20)      125 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/011.http
--rw-r--r--   0 benoitc    (501) staff       (20)      196 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/011.py
--rw-r--r--   0 benoitc    (501) staff       (20)      166 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/012.http
--rw-r--r--   0 benoitc    (501) staff       (20)      285 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/012.py
--rw-r--r--   0 benoitc    (501) staff       (20)      159 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/013.http
--rw-r--r--   0 benoitc    (501) staff       (20)      192 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/013.py
--rw-r--r--   0 benoitc    (501) staff       (20)       46 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/014.http
--rw-r--r--   0 benoitc    (501) staff       (20)      137 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/014.py
--rw-r--r--   0 benoitc    (501) staff       (20)       98 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/015.http
--rw-r--r--   0 benoitc    (501) staff       (20)      226 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/015.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2234 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/016.http
--rw-r--r--   0 benoitc    (501) staff       (20)     2376 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/016.py
--rw-r--r--   0 benoitc    (501) staff       (20)       91 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/017.http
--rw-r--r--   0 benoitc    (501) staff       (20)      207 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/017.py
--rw-r--r--   0 benoitc    (501) staff       (20)       58 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/018.http
--rw-r--r--   0 benoitc    (501) staff       (20)      258 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/018.py
--rw-r--r--   0 benoitc    (501) staff       (20)       58 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/019.http
--rw-r--r--   0 benoitc    (501) staff       (20)      119 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/019.py
--rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/020.http
--rw-r--r--   0 benoitc    (501) staff       (20)      171 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/020.py
--rw-r--r--   0 benoitc    (501) staff       (20)       80 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/021.http
--rw-r--r--   0 benoitc    (501) staff       (20)      142 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/021.py
--rw-r--r--   0 benoitc    (501) staff       (20)       85 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/022.http
--rw-r--r--   0 benoitc    (501) staff       (20)      286 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/022.py
--rw-r--r--   0 benoitc    (501) staff       (20)      155 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/023.http
--rw-r--r--   0 benoitc    (501) staff       (20)      335 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/023.py
--rw-r--r--   0 benoitc    (501) staff       (20)    16408 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/024.http
--rw-r--r--   0 benoitc    (501) staff       (20)    16639 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/024.py
--rw-r--r--   0 benoitc    (501) staff       (20)      364 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/025.http
--rw-r--r--   0 benoitc    (501) staff       (20)      476 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/025.py
--rw-r--r--   0 benoitc    (501) staff       (20)     8233 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/026.http
--rw-r--r--   0 benoitc    (501) staff       (20)     8463 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/026.py
--rw-r--r--   0 benoitc    (501) staff       (20)       30 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/027.http
--rw-r--r--   0 benoitc    (501) staff       (20)      130 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/027.py
--rw-r--r--   0 benoitc    (501) staff       (20)       68 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/028.http
--rw-r--r--   0 benoitc    (501) staff       (20)      261 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/028.py
--rw-r--r--   0 benoitc    (501) staff       (20)      129 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/029.http
--rw-r--r--   0 benoitc    (501) staff       (20)      278 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/029.py
--rw-r--r--   0 benoitc    (501) staff       (20)      129 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/030.http
--rw-r--r--   0 benoitc    (501) staff       (20)      278 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/030.py
--rw-r--r--   0 benoitc    (501) staff       (20)     9909 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/099.http
--rw-r--r--   0 benoitc    (501) staff       (20)     9135 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/099.py
--rw-r--r--   0 benoitc    (501) staff       (20)       41 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/100.http
--rw-r--r--   0 benoitc    (501) staff       (20)      131 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/100.py
--rw-r--r--   0 benoitc    (501) staff       (20)      199 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/pp_01.http
--rw-r--r--   0 benoitc    (501) staff       (20)      359 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/pp_01.py
--rw-r--r--   0 benoitc    (501) staff       (20)      361 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/pp_02.http
--rw-r--r--   0 benoitc    (501) staff       (20)      639 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/requests/valid/pp_02.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1745 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/support.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1614 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/t.py
--rw-r--r--   0 benoitc    (501) staff       (20)     6110 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_arbiter.py
--rw-r--r--   0 benoitc    (501) staff       (20)    14360 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_config.py
--rw-r--r--   0 benoitc    (501) staff       (20)     6853 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_http.py
--rw-r--r--   0 benoitc    (501) staff       (20)      597 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_invalid_requests.py
--rw-r--r--   0 benoitc    (501) staff       (20)     3140 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_logger.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1522 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_pidfile.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1851 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_reload.py
--rw-r--r--   0 benoitc    (501) staff       (20)     1875 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_sock.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2013 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_ssl.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4818 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_statsd.py
--rw-r--r--   0 benoitc    (501) staff       (20)     2049 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_systemd.py
--rw-r--r--   0 benoitc    (501) staff       (20)     4367 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_util.py
--rw-r--r--   0 benoitc    (501) staff       (20)      608 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/test_valid_requests.py
--rw-r--r--   0 benoitc    (501) staff       (20)     9434 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/treq.py
-drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 20:28:19.048242 gunicorn-21.0.0/tests/workers/
--rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/workers/__init__.py
--rw-r--r--   0 benoitc    (501) staff       (20)      192 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/workers/test_geventlet.py
--rw-r--r--   0 benoitc    (501) staff       (20)      190 2023-07-17 19:03:36.000000 gunicorn-21.0.0/tests/workers/test_ggevent.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.593168 gunicorn-21.0.1/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      267 2023-07-17 19:03:36.000000 gunicorn-21.0.1/.gitignore
+-rw-r--r--   0 benoitc    (501) staff       (20)     1136 2023-07-17 19:03:36.000000 gunicorn-21.0.1/LICENSE
+-rw-r--r--   0 benoitc    (501) staff       (20)      324 2023-07-17 19:03:36.000000 gunicorn-21.0.1/MANIFEST.in
+-rw-r--r--   0 benoitc    (501) staff       (20)     3777 2023-07-17 19:03:36.000000 gunicorn-21.0.1/NOTICE
+-rw-r--r--   0 benoitc    (501) staff       (20)     3852 2023-07-17 21:22:35.593265 gunicorn-21.0.1/PKG-INFO
+-rw-r--r--   0 benoitc    (501) staff       (20)     1988 2023-07-17 19:03:36.000000 gunicorn-21.0.1/README.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6969 2023-07-17 19:03:36.000000 gunicorn-21.0.1/THANKS
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.508619 gunicorn-21.0.1/docs/
+-rw-r--r--   0 benoitc    (501) staff       (20)     5791 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/Makefile
+-rw-r--r--   0 benoitc    (501) staff       (20)      288 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/README.rst
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.504287 gunicorn-21.0.1/docs/build/
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.516257 gunicorn-21.0.1/docs/build/doctrees/
+-rw-r--r--   0 benoitc    (501) staff       (20)    43583 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2010-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    15287 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2011-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    27991 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2012-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    19851 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2013-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    48784 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2014-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    51800 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2015-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    25377 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2016-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    17557 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2017-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    29568 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2018-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    33177 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2019-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)     2984 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2020-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    13095 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2021-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)     5292 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/2023-news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    11251 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/community.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    17815 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/configure.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    10993 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/custom.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    54089 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/deploy.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    25657 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/design.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)  1267881 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/environment.pickle
+-rw-r--r--   0 benoitc    (501) staff       (20)    35498 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/faq.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)     8337 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/index.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    27785 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/install.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)     9613 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/instrumentation.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)     6075 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/news.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    31793 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/run.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)   261405 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/settings.doctree
+-rw-r--r--   0 benoitc    (501) staff       (20)    24042 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/doctrees/signals.doctree
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.522564 gunicorn-21.0.1/docs/build/html/
+-rw-r--r--   0 benoitc    (501) staff       (20)      230 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/.buildinfo
+-rw-r--r--   0 benoitc    (501) staff       (20)    19422 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2010-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    10972 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2011-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    15120 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2012-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    13036 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2013-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    20800 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2014-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    23465 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2015-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    15406 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2016-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    12213 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2017-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    17042 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2018-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    14935 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2019-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     7097 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2020-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     9650 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2021-news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     7724 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/2023-news.html
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.522748 gunicorn-21.0.1/docs/build/html/_images/
+-rw-r--r--   0 benoitc    (501) staff       (20)    14398 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_images/gunicorn.png
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.528028 gunicorn-21.0.1/docs/build/html/_sources/
+-rw-r--r--   0 benoitc    (501) staff       (20)     6643 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2010-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     2092 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2011-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     4184 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2012-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     3267 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2013-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     6834 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2014-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     5702 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2015-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     2911 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2016-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     2100 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2017-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     2956 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2018-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     4785 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2019-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      112 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2020-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1905 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/2021-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      530 2023-07-17 20:14:25.000000 gunicorn-21.0.1/docs/build/html/_sources/2023-news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1377 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/community.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     3873 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/configure.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1927 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/custom.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)    12260 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/deploy.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     6483 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/design.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     8672 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/faq.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1043 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     5551 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/install.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1325 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/instrumentation.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      727 2023-07-17 20:14:25.000000 gunicorn-21.0.1/docs/build/html/_sources/news.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     6485 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/run.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)    36935 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/_sources/settings.rst.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)     5420 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_sources/signals.rst.txt
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.529554 gunicorn-21.0.1/docs/build/html/_static/
+-rw-r--r--   0 benoitc    (501) staff       (20)    14813 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/_static/basic.css
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.529797 gunicorn-21.0.1/docs/build/html/_static/css/
+-rw-r--r--   0 benoitc    (501) staff       (20)     3229 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/badge_only.css
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.547736 gunicorn-21.0.1/docs/build/html/_static/css/fonts/
+-rw-r--r--   0 benoitc    (501) staff       (20)    87624 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)    67312 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)    86288 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)    66444 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   165742 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 benoitc    (501) staff       (20)   444379 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 benoitc    (501) staff       (20)   165548 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 benoitc    (501) staff       (20)    98024 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)    77160 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   323344 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)   193308 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   309728 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)   184912 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   328412 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)   195704 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   309192 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 benoitc    (501) staff       (20)   182708 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 benoitc    (501) staff       (20)   135314 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/css/theme.css
+-rw-r--r--   0 benoitc    (501) staff       (20)     4472 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/doctools.js
+-rw-r--r--   0 benoitc    (501) staff       (20)      421 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 benoitc    (501) staff       (20)      286 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/file.png
+-rw-r--r--   0 benoitc    (501) staff       (20)    14398 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/build/html/_static/gunicorn.png
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.548614 gunicorn-21.0.1/docs/build/html/_static/js/
+-rw-r--r--   0 benoitc    (501) staff       (20)      934 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     4370 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     2734 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     5023 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/js/theme.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     4758 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/_static/language_data.js
+-rw-r--r--   0 benoitc    (501) staff       (20)       90 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/minus.png
+-rw-r--r--   0 benoitc    (501) staff       (20)       90 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/plus.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     4846 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/_static/pygments.css
+-rw-r--r--   0 benoitc    (501) staff       (20)    18215 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     4712 2023-07-17 19:08:28.000000 gunicorn-21.0.1/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 benoitc    (501) staff       (20)     7909 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/build/html/community.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    12328 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/configure.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    14413 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/custom.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    40350 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/deploy.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    14905 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/design.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    26212 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/faq.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     4623 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/genindex.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    13234 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/index.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    18129 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/install.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     7694 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/instrumentation.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     8954 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     1679 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/objects.inv
+-rw-r--r--   0 benoitc    (501) staff       (20)    20340 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/run.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     4713 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/search.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    61641 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/searchindex.js
+-rw-r--r--   0 benoitc    (501) staff       (20)   116855 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/settings.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    25507 2023-07-17 21:13:37.000000 gunicorn-21.0.1/docs/build/html/signals.html
+-rwxr-xr-x   0 benoitc    (501) staff       (20)     3029 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/gunicorn_ext.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.549333 gunicorn-21.0.1/docs/logo/
+-rw-r--r--   0 benoitc    (501) staff       (20)    21550 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/logo/gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)    12798 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/logo/gunicorn.svg
+-rw-r--r--   0 benoitc    (501) staff       (20)     5109 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/make.bat
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.551656 gunicorn-21.0.1/docs/site/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/.nojekyll
+-rw-r--r--   0 benoitc    (501) staff       (20)       13 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/CNAME
+-rw-r--r--   0 benoitc    (501) staff       (20)      340 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/community.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      304 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/configuration.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      300 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/configure.html
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.551790 gunicorn-21.0.1/docs/site/css/
+-rw-r--r--   0 benoitc    (501) staff       (20)     6671 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/css/style.css
+-rw-r--r--   0 benoitc    (501) staff       (20)      343 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/deploy.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      342 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/deployment.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      297 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/design.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/faq.html
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.554244 gunicorn-21.0.1/docs/site/images/
+-rw-r--r--   0 benoitc    (501) staff       (20)    17551 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/about.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)      408 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/arrow.png
+-rw-r--r--   0 benoitc    (501) staff       (20)      611 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/banner-bg.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)    15593 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/community.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)    17566 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/documents.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)    15962 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/downloads.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     1771 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/favicon.png
+-rw-r--r--   0 benoitc    (501) staff       (20)      255 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/footer-arrow.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     2499 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/footer-logo.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)      335 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/greenbutton.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     1553 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)    21956 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/large_gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     3145 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/logo-bottom.png
+-rw-r--r--   0 benoitc    (501) staff       (20)    10238 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/logo.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     7343 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/logo.png
+-rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/redbutton.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)      440 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/separator.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     3450 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/title.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     2184 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/images/user1.jpg
+-rw-r--r--   0 benoitc    (501) staff       (20)     7856 2023-07-17 21:18:12.000000 gunicorn-21.0.1/docs/site/index.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      298 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/install.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      298 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/installation.html
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.554377 gunicorn-21.0.1/docs/site/js/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)     1479 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/js/main.js
+-rw-r--r--   0 benoitc    (501) staff       (20)      295 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/news.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/run.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     1990 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/sitemap.xml
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/tuning.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      294 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/site/usage.html
+-rw-r--r--   0 benoitc    (501) staff       (20)     2088 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/sitemap_gen.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.559121 gunicorn-21.0.1/docs/source/
+-rw-r--r--   0 benoitc    (501) staff       (20)     6643 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2010-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2092 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2011-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     4184 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2012-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     3267 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2013-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6834 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2014-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     5702 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2015-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2911 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2016-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2100 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2017-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     2956 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2018-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     4785 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2019-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)      112 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2020-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1905 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/2021-news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)      598 2023-07-17 21:19:00.000000 gunicorn-21.0.1/docs/source/2023-news.rst
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.559286 gunicorn-21.0.1/docs/source/_static/
+-rw-r--r--   0 benoitc    (501) staff       (20)    14398 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/_static/gunicorn.png
+-rw-r--r--   0 benoitc    (501) staff       (20)     1377 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/community.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1755 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/conf.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     3873 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/configure.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1927 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/custom.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)    12260 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/deploy.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6483 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/design.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     8672 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/faq.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1043 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/index.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     5551 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/install.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     1325 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/instrumentation.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)      795 2023-07-17 21:19:19.000000 gunicorn-21.0.1/docs/source/news.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     6485 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/run.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)    36935 2023-07-17 21:13:36.000000 gunicorn-21.0.1/docs/source/settings.rst
+-rw-r--r--   0 benoitc    (501) staff       (20)     5420 2023-07-17 19:03:36.000000 gunicorn-21.0.1/docs/source/signals.rst
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.562582 gunicorn-21.0.1/examples/
+-rw-r--r--   0 benoitc    (501) staff       (20)      738 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/alt_spec.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      204 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/bad.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      108 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/boot_fail.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.562800 gunicorn-21.0.1/examples/deep/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/deep/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      659 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/deep/test.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      676 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/echo.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7621 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/example_config.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.564568 gunicorn-21.0.1/examples/frameworks/
+-rw-r--r--   0 benoitc    (501) staff       (20)      198 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/cherryapp.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.564701 gunicorn-21.0.1/examples/frameworks/django/
+-rw-r--r--   0 benoitc    (501) staff       (20)       60 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/README
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.564836 gunicorn-21.0.1/examples/frameworks/django/testing/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      244 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/manage.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.565360 gunicorn-21.0.1/examples/frameworks/django/testing/testing/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/__init__.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.565496 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/__init__.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.566248 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/
+-rwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      627 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/middleware.py
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/models.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.566551 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/templates/
+-rw-r--r--   0 benoitc    (501) staff       (20)      759 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html
+-rw-r--r--   0 benoitc    (501) staff       (20)      471 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/templates/home.html
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      509 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/tests.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      133 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/urls.py
+-rwxr-xr-x   0 benoitc    (501) staff       (20)     1548 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/views.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5730 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/settings.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/urls.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1359 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/django/testing/testing/wsgi.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      291 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/flask_sendfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      147 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/flaskapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      501 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/flaskapp_aiohttp_wsgi.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      338 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/pyramidapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      150 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/requirements.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        9 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/requirements_cherryapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        6 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/requirements_flaskapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        8 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/requirements_pyramidapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)       10 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/requirements_tornadoapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        7 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/requirements_webpyapp.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      873 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/tornadoapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      197 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/frameworks/webpyapp.py
+-rwxr-xr-x   0 benoitc    (501) staff       (20)      215 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/gunicorn_rc
+-rw-r--r--   0 benoitc    (501) staff       (20)       13 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/hello.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      448 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/log_app.ini
+-rw-r--r--   0 benoitc    (501) staff       (20)      372 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/log_app.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      841 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/logging.conf
+-rw-r--r--   0 benoitc    (501) staff       (20)      737 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/longpoll.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1470 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/multiapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      993 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/multidomainapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1980 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/nginx.conf
+-rw-r--r--   0 benoitc    (501) staff       (20)      403 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/read_django_settings.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1015 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/readline_app.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      584 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/sendfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1257 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/server.crt
+-rw-r--r--   0 benoitc    (501) staff       (20)     1679 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/server.key
+-rw-r--r--   0 benoitc    (501) staff       (20)      604 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/slowclient.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1339 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/standalone_app.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      182 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/supervisor.conf
+-rw-r--r--   0 benoitc    (501) staff       (20)      659 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/test.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      620 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/timeout.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.567044 gunicorn-21.0.1/examples/websocket/
+-rw-r--r--   0 benoitc    (501) staff       (20)    15684 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/websocket/gevent_websocket.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1320 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/websocket/websocket.html
+-rw-r--r--   0 benoitc    (501) staff       (20)    15729 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/websocket/websocket.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1020 2023-07-17 19:03:36.000000 gunicorn-21.0.1/examples/when_ready.conf.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.568721 gunicorn-21.0.1/gunicorn/
+-rw-r--r--   0 benoitc    (501) staff       (20)      279 2023-07-17 21:17:21.000000 gunicorn-21.0.1/gunicorn/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      171 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/__main__.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.570070 gunicorn-21.0.1/gunicorn/app/
+-rw-r--r--   0 benoitc    (501) staff       (20)      127 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/app/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7400 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/app/base.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2038 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/app/pasterapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1926 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/app/wsgiapp.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    21509 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/arbiter.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    63419 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/config.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2293 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/debug.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      919 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/errors.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    15303 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/glogging.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.570948 gunicorn-21.0.1/gunicorn/http/
+-rw-r--r--   0 benoitc    (501) staff       (20)      277 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/http/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7296 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/http/body.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2850 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/http/errors.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    11958 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/http/message.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1364 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/http/parser.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1943 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/http/unreader.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    12366 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/http/wsgi.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.571191 gunicorn-21.0.1/gunicorn/instrument/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/instrument/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4690 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/instrument/statsd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2367 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/pidfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     3791 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/reloader.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6887 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/sock.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2520 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/systemd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    19127 2023-07-17 21:06:48.000000 gunicorn-21.0.1/gunicorn/util.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.572452 gunicorn-21.0.1/gunicorn/workers/
+-rw-r--r--   0 benoitc    (501) staff       (20)      594 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/workers/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     9197 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/workers/base.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5681 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/workers/base_async.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6091 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/workers/geventlet.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5800 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/workers/ggevent.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    12585 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/workers/gthread.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     5854 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/workers/gtornado.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     7272 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/workers/sync.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1651 2023-07-17 19:03:36.000000 gunicorn-21.0.1/gunicorn/workers/workertmp.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.569540 gunicorn-21.0.1/gunicorn.egg-info/
+-rw-r--r--   0 benoitc    (501) staff       (20)     3852 2023-07-17 21:22:35.000000 gunicorn-21.0.1/gunicorn.egg-info/PKG-INFO
+-rw-r--r--   0 benoitc    (501) staff       (20)    13924 2023-07-17 21:22:35.000000 gunicorn-21.0.1/gunicorn.egg-info/SOURCES.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        1 2023-07-17 21:22:35.000000 gunicorn-21.0.1/gunicorn.egg-info/dependency_links.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      113 2023-07-17 21:22:35.000000 gunicorn-21.0.1/gunicorn.egg-info/entry_points.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        1 2023-07-17 20:27:30.000000 gunicorn-21.0.1/gunicorn.egg-info/not-zip-safe
+-rw-r--r--   0 benoitc    (501) staff       (20)      173 2023-07-17 21:22:35.000000 gunicorn-21.0.1/gunicorn.egg-info/requires.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)        9 2023-07-17 21:22:35.000000 gunicorn-21.0.1/gunicorn.egg-info/top_level.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)       50 2023-07-17 19:03:36.000000 gunicorn-21.0.1/requirements_dev.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)       56 2023-07-17 20:45:55.000000 gunicorn-21.0.1/requirements_test.txt
+-rw-r--r--   0 benoitc    (501) staff       (20)      203 2023-07-17 21:22:35.593629 gunicorn-21.0.1/setup.cfg
+-rw-r--r--   0 benoitc    (501) staff       (20)     3555 2023-07-17 19:03:36.000000 gunicorn-21.0.1/setup.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.575012 gunicorn-21.0.1/tests/
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.575466 gunicorn-21.0.1/tests/config/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/config/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       88 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/config/test_cfg.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       24 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/config/test_cfg_alt.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       23 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/config/test_cfg_with_wsgi_app.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.506274 gunicorn-21.0.1/tests/requests/
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.583149 gunicorn-21.0.1/tests/requests/invalid/
+-rw-r--r--   0 benoitc    (501) staff       (20)       29 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/001.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       64 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/001.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       21 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/002.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/002.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       30 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/003.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       84 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/003.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       25 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/004.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       80 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/004.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       41 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/005.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       78 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/005.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4122 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/006.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       77 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/006.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     8358 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/007.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/007.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    12418 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/008.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/008.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1829 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/009.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       83 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/009.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       44 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/010.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/010.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/011.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/011.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      169 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/012.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/012.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       49 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/013.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      174 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/013.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       78 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/014.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       72 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/014.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       88 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/015.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       72 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/015.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       33 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/016.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       82 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/016.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     8222 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/017.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      134 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/017.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       48 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/018.http
+-rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/018.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       82 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/019.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      172 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/019.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       69 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/020.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      130 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/020.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       90 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/021.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/021.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/022.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/022.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       52 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/023.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/023.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/024.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      122 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/024.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       37 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/pp_01.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      161 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/pp_01.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       53 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/pp_02.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      161 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/invalid/pp_02.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.592599 gunicorn-21.0.1/tests/requests/valid/
+-rw-r--r--   0 benoitc    (501) staff       (20)      149 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/001.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      275 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/001.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      168 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/002.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      296 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/002.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      394 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/003.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      577 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/003.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       57 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/004.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      164 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/004.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       62 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/005.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      153 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/005.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       51 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/006.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      142 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/006.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       61 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/007.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      167 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/007.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       73 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/008.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      178 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/008.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      137 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/009.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      264 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/009.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      134 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/010.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      218 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/010.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      125 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/011.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      196 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/011.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      166 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/012.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      285 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/012.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      159 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/013.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      192 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/013.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       46 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/014.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      137 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/014.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       98 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/015.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      226 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/015.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2234 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/016.http
+-rw-r--r--   0 benoitc    (501) staff       (20)     2376 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/016.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       91 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/017.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      207 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/017.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       58 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/018.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      258 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/018.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       58 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/019.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      119 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/019.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       81 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/020.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      171 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/020.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       80 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/021.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      142 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/021.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       85 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/022.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      286 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/022.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      155 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/023.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      335 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/023.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    16408 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/024.http
+-rw-r--r--   0 benoitc    (501) staff       (20)    16639 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/024.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      364 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/025.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      476 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/025.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     8233 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/026.http
+-rw-r--r--   0 benoitc    (501) staff       (20)     8463 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/026.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       30 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/027.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      130 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/027.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       68 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/028.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      261 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/028.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      129 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/029.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      278 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/029.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      129 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/030.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      278 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/030.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     9909 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/099.http
+-rw-r--r--   0 benoitc    (501) staff       (20)     9135 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/099.py
+-rw-r--r--   0 benoitc    (501) staff       (20)       41 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/100.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      131 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/100.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      199 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/pp_01.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      359 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/pp_01.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      361 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/pp_02.http
+-rw-r--r--   0 benoitc    (501) staff       (20)      639 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/requests/valid/pp_02.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1745 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/support.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1614 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/t.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6110 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_arbiter.py
+-rw-r--r--   0 benoitc    (501) staff       (20)    14360 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_config.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     6853 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_http.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      597 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_invalid_requests.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     3140 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_logger.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1522 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_pidfile.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1851 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_reload.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     1875 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_sock.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2013 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_ssl.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4818 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_statsd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     2049 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_systemd.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     4367 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_util.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      608 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/test_valid_requests.py
+-rw-r--r--   0 benoitc    (501) staff       (20)     9434 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/treq.py
+drwxr-xr-x   0 benoitc    (501) staff       (20)        0 2023-07-17 21:22:35.593006 gunicorn-21.0.1/tests/workers/
+-rw-r--r--   0 benoitc    (501) staff       (20)        0 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/workers/__init__.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      192 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/workers/test_geventlet.py
+-rw-r--r--   0 benoitc    (501) staff       (20)      190 2023-07-17 19:03:36.000000 gunicorn-21.0.1/tests/workers/test_ggevent.py
```

### Comparing `gunicorn-21.0.0/LICENSE` & `gunicorn-21.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/NOTICE` & `gunicorn-21.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/PKG-INFO` & `gunicorn-21.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunicorn
-Version: 21.0.0
+Version: 21.0.1
 Summary: WSGI HTTP Server for UNIX
 Home-page: https://gunicorn.org
 Author: Benoit Chesneau
 Author-email: benoitc@gunicorn.org
 License: MIT
 Project-URL: Documentation, https://docs.gunicorn.org
 Project-URL: Homepage, https://gunicorn.org
```

### Comparing `gunicorn-21.0.0/README.rst` & `gunicorn-21.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/THANKS` & `gunicorn-21.0.1/THANKS`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/Makefile` & `gunicorn-21.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/gunicorn_ext.py` & `gunicorn-21.0.1/docs/gunicorn_ext.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/logo/gunicorn.png` & `gunicorn-21.0.1/docs/logo/gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/logo/gunicorn.svg` & `gunicorn-21.0.1/docs/logo/gunicorn.svg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/make.bat` & `gunicorn-21.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/css/style.css` & `gunicorn-21.0.1/docs/site/css/style.css`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/about.jpg` & `gunicorn-21.0.1/docs/site/images/about.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/banner-bg.jpg` & `gunicorn-21.0.1/docs/site/images/banner-bg.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/community.jpg` & `gunicorn-21.0.1/docs/site/images/community.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/documents.jpg` & `gunicorn-21.0.1/docs/site/images/documents.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/downloads.jpg` & `gunicorn-21.0.1/docs/site/images/downloads.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/favicon.png` & `gunicorn-21.0.1/docs/site/images/favicon.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/footer-logo.jpg` & `gunicorn-21.0.1/docs/site/images/footer-logo.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/gunicorn.png` & `gunicorn-21.0.1/docs/site/images/gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/large_gunicorn.png` & `gunicorn-21.0.1/docs/site/images/large_gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/logo-bottom.png` & `gunicorn-21.0.1/docs/site/images/logo-bottom.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/logo.jpg` & `gunicorn-21.0.1/docs/site/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/logo.png` & `gunicorn-21.0.1/docs/site/images/logo.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/redbutton.jpg` & `gunicorn-21.0.1/docs/site/images/redbutton.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/title.png` & `gunicorn-21.0.1/docs/site/images/title.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/images/user1.jpg` & `gunicorn-21.0.1/docs/site/images/user1.jpg`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/index.html` & `gunicorn-21.0.1/docs/site/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 </head>
 <body>
   <div class="logo-wrapper">
     <div class="logo-div">
       <div class="latest">
         Latest version: <strong><a
-            href="https://docs.gunicorn.org/en/stable/">20.1.0</a></strong>
+            href="https://docs.gunicorn.org/en/stable/">21.0.1</a></strong>
       </div>
 
       <div class="logo"><img src="images/logo.jpg" ></div>
     </div>
   </div>
   <div class="banner-wrapper">
     <div class="banner">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 
 
 
-Latest version: 20.1.0
+Latest version: 21.0.1
 [images/logo.jpg]
 [images/title.png]
 ****** Gunicorn 'Green Unicorn' is a Python WSGI HTTP Server for UNIX. It's a
 pre-fork worker model. The Gunicorn server is broadly compatible with various
 web frameworks, simply implemented, light on server resources, and fairly
 speedy. ******
 View_source Download
```

### Comparing `gunicorn-21.0.0/docs/site/js/main.js` & `gunicorn-21.0.1/docs/site/js/main.js`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/site/sitemap.xml` & `gunicorn-21.0.1/docs/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/sitemap_gen.py` & `gunicorn-21.0.1/docs/sitemap_gen.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2010-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2010-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2011-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2011-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2012-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2012-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2013-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2013-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2014-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2014-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2015-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2015-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2016-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2016-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2017-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2017-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2018-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2018-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2019-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2019-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2021-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2021-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/2023-news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/2023-news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/_static/gunicorn.png` & `gunicorn-21.0.1/docs/build/html/_images/gunicorn.png`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/community.rst` & `gunicorn-21.0.1/docs/build/html/_sources/community.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/conf.py` & `gunicorn-21.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/configure.rst` & `gunicorn-21.0.1/docs/build/html/_sources/configure.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/custom.rst` & `gunicorn-21.0.1/docs/build/html/_sources/custom.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/deploy.rst` & `gunicorn-21.0.1/docs/build/html/_sources/deploy.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/design.rst` & `gunicorn-21.0.1/docs/build/html/_sources/design.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/faq.rst` & `gunicorn-21.0.1/docs/build/html/_sources/faq.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/index.rst` & `gunicorn-21.0.1/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/install.rst` & `gunicorn-21.0.1/docs/build/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/instrumentation.rst` & `gunicorn-21.0.1/docs/build/html/_sources/instrumentation.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/news.rst` & `gunicorn-21.0.1/docs/build/html/_sources/news.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/run.rst` & `gunicorn-21.0.1/docs/build/html/_sources/run.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/docs/source/settings.rst` & `gunicorn-21.0.1/docs/build/html/_sources/settings.rst.txt`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,16 @@
 logging module's dictionary configuration format. This option
 takes precedence over the :ref:`logconfig` and :ref:`logConfigJson` options,
 which uses the older file configuration format and JSON
 respectively.
 
 Format: https://docs.python.org/3/library/logging.config.html#logging.config.dictConfig
 
-For more context you can look at the default configuration dictionary for logging, which can be found at ``gunicorn.glogging.CONFIG_DEFAULTS``.
+For more context you can look at the default configuration dictionary for logging,
+which can be found at ``gunicorn.glogging.CONFIG_DEFAULTS``.
 
 .. versionadded:: 19.8
 
 .. _logconfig-json:
 
 ``logconfig_json``
 ~~~~~~~~~~~~~~~~~~
@@ -342,15 +343,15 @@
 .. _syslog-addr:
 
 ``syslog_addr``
 ~~~~~~~~~~~~~~~
 
 **Command line:** ``--log-syslog-to SYSLOG_ADDR``
 
-**Default:** ``'udp://localhost:514'``
+**Default:** ``'unix:///var/run/syslog'``
 
 Address to send syslog messages.
 
 Address is a string of the form:
 
 * ``unix://PATH#TYPE`` : for unix domain socket. ``TYPE`` can be ``stream``
   for the stream driver or ``dgram`` for the dgram driver.
```

### Comparing `gunicorn-21.0.0/docs/source/signals.rst` & `gunicorn-21.0.1/docs/build/html/_sources/signals.rst.txt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/alt_spec.py` & `gunicorn-21.0.1/examples/alt_spec.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/deep/test.py` & `gunicorn-21.0.1/examples/deep/test.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/echo.py` & `gunicorn-21.0.1/examples/echo.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/example_config.py` & `gunicorn-21.0.1/examples/example_config.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/middleware.py` & `gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/middleware.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html` & `gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/templates/base.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/frameworks/django/testing/testing/apps/someapp/views.py` & `gunicorn-21.0.1/examples/frameworks/django/testing/testing/apps/someapp/views.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/frameworks/django/testing/testing/settings.py` & `gunicorn-21.0.1/examples/frameworks/django/testing/testing/settings.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/frameworks/django/testing/testing/urls.py` & `gunicorn-21.0.1/examples/frameworks/django/testing/testing/urls.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/frameworks/django/testing/testing/wsgi.py` & `gunicorn-21.0.1/examples/frameworks/django/testing/testing/wsgi.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/frameworks/tornadoapp.py` & `gunicorn-21.0.1/examples/frameworks/tornadoapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/logging.conf` & `gunicorn-21.0.1/examples/logging.conf`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/longpoll.py` & `gunicorn-21.0.1/examples/longpoll.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/multiapp.py` & `gunicorn-21.0.1/examples/multiapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/multidomainapp.py` & `gunicorn-21.0.1/examples/multidomainapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/nginx.conf` & `gunicorn-21.0.1/examples/nginx.conf`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/readline_app.py` & `gunicorn-21.0.1/examples/readline_app.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/sendfile.py` & `gunicorn-21.0.1/examples/sendfile.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/server.crt` & `gunicorn-21.0.1/examples/server.crt`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/server.key` & `gunicorn-21.0.1/examples/server.key`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/slowclient.py` & `gunicorn-21.0.1/examples/slowclient.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/standalone_app.py` & `gunicorn-21.0.1/examples/standalone_app.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/test.py` & `gunicorn-21.0.1/examples/test.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/timeout.py` & `gunicorn-21.0.1/examples/timeout.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/websocket/gevent_websocket.py` & `gunicorn-21.0.1/examples/websocket/gevent_websocket.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/websocket/websocket.html` & `gunicorn-21.0.1/examples/websocket/websocket.html`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/websocket/websocket.py` & `gunicorn-21.0.1/examples/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/examples/when_ready.conf.py` & `gunicorn-21.0.1/examples/when_ready.conf.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/app/base.py` & `gunicorn-21.0.1/gunicorn/app/base.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/app/pasterapp.py` & `gunicorn-21.0.1/gunicorn/app/pasterapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/app/wsgiapp.py` & `gunicorn-21.0.1/gunicorn/app/wsgiapp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/arbiter.py` & `gunicorn-21.0.1/gunicorn/arbiter.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/config.py` & `gunicorn-21.0.1/gunicorn/config.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/debug.py` & `gunicorn-21.0.1/gunicorn/debug.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/errors.py` & `gunicorn-21.0.1/gunicorn/errors.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/glogging.py` & `gunicorn-21.0.1/gunicorn/glogging.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/http/body.py` & `gunicorn-21.0.1/gunicorn/http/body.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/http/errors.py` & `gunicorn-21.0.1/gunicorn/http/errors.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/http/message.py` & `gunicorn-21.0.1/gunicorn/http/message.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/http/parser.py` & `gunicorn-21.0.1/gunicorn/http/parser.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/http/unreader.py` & `gunicorn-21.0.1/gunicorn/http/unreader.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/http/wsgi.py` & `gunicorn-21.0.1/gunicorn/http/wsgi.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/instrument/statsd.py` & `gunicorn-21.0.1/gunicorn/instrument/statsd.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/pidfile.py` & `gunicorn-21.0.1/gunicorn/pidfile.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/reloader.py` & `gunicorn-21.0.1/gunicorn/reloader.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/sock.py` & `gunicorn-21.0.1/gunicorn/sock.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/systemd.py` & `gunicorn-21.0.1/gunicorn/systemd.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/util.py` & `gunicorn-21.0.1/gunicorn/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import textwrap
 import time
 import traceback
 import warnings
 
 try:
     import importlib.metadata as importlib_metadata
-except ImportError:
+except (ModuleNotFoundError, ImportError):
     import importlib_metadata
 
 from gunicorn.errors import AppImportError
 from gunicorn.workers import SUPPORTED_WORKERS
 import urllib.parse
 
 REDIRECT_TO = getattr(os, 'devnull', '/dev/null')
```

### Comparing `gunicorn-21.0.0/gunicorn/workers/__init__.py` & `gunicorn-21.0.1/gunicorn/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/workers/base.py` & `gunicorn-21.0.1/gunicorn/workers/base.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/workers/base_async.py` & `gunicorn-21.0.1/gunicorn/workers/base_async.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/workers/geventlet.py` & `gunicorn-21.0.1/gunicorn/workers/geventlet.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/workers/ggevent.py` & `gunicorn-21.0.1/gunicorn/workers/ggevent.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/workers/gthread.py` & `gunicorn-21.0.1/gunicorn/workers/gthread.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/workers/gtornado.py` & `gunicorn-21.0.1/gunicorn/workers/gtornado.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/workers/sync.py` & `gunicorn-21.0.1/gunicorn/workers/sync.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn/workers/workertmp.py` & `gunicorn-21.0.1/gunicorn/workers/workertmp.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/gunicorn.egg-info/PKG-INFO` & `gunicorn-21.0.1/gunicorn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gunicorn
-Version: 21.0.0
+Version: 21.0.1
 Summary: WSGI HTTP Server for UNIX
 Home-page: https://gunicorn.org
 Author: Benoit Chesneau
 Author-email: benoitc@gunicorn.org
 License: MIT
 Project-URL: Documentation, https://docs.gunicorn.org
 Project-URL: Homepage, https://gunicorn.org
```

### Comparing `gunicorn-21.0.0/setup.py` & `gunicorn-21.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/invalid/006.http` & `gunicorn-21.0.1/tests/requests/invalid/006.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/invalid/007.http` & `gunicorn-21.0.1/tests/requests/invalid/007.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/invalid/008.http` & `gunicorn-21.0.1/tests/requests/invalid/008.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/invalid/009.http` & `gunicorn-21.0.1/tests/requests/invalid/009.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/invalid/017.http` & `gunicorn-21.0.1/tests/requests/invalid/017.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/valid/003.py` & `gunicorn-21.0.1/tests/requests/valid/003.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/valid/016.http` & `gunicorn-21.0.1/tests/requests/valid/016.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/valid/016.py` & `gunicorn-21.0.1/tests/requests/valid/016.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/valid/024.http` & `gunicorn-21.0.1/tests/requests/valid/024.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/valid/024.py` & `gunicorn-21.0.1/tests/requests/valid/024.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/valid/026.http` & `gunicorn-21.0.1/tests/requests/valid/026.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/valid/026.py` & `gunicorn-21.0.1/tests/requests/valid/026.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/valid/099.http` & `gunicorn-21.0.1/tests/requests/valid/099.http`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/valid/099.py` & `gunicorn-21.0.1/tests/requests/valid/099.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/requests/valid/pp_02.py` & `gunicorn-21.0.1/tests/requests/valid/pp_02.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/support.py` & `gunicorn-21.0.1/tests/support.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/t.py` & `gunicorn-21.0.1/tests/t.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_arbiter.py` & `gunicorn-21.0.1/tests/test_arbiter.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_config.py` & `gunicorn-21.0.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_http.py` & `gunicorn-21.0.1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_invalid_requests.py` & `gunicorn-21.0.1/tests/test_invalid_requests.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_logger.py` & `gunicorn-21.0.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_pidfile.py` & `gunicorn-21.0.1/tests/test_pidfile.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_reload.py` & `gunicorn-21.0.1/tests/test_reload.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_sock.py` & `gunicorn-21.0.1/tests/test_sock.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_ssl.py` & `gunicorn-21.0.1/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_statsd.py` & `gunicorn-21.0.1/tests/test_statsd.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_systemd.py` & `gunicorn-21.0.1/tests/test_systemd.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_util.py` & `gunicorn-21.0.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/test_valid_requests.py` & `gunicorn-21.0.1/tests/test_valid_requests.py`

 * *Files identical despite different names*

### Comparing `gunicorn-21.0.0/tests/treq.py` & `gunicorn-21.0.1/tests/treq.py`

 * *Files identical despite different names*

