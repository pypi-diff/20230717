# Comparing `tmp/render_engine-2023.7.4a1.tar.gz` & `tmp/render_engine-2023.7.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine-2023.7.4a1.tar", last modified: Sun Jul 16 23:43:16 2023, max compression
+gzip compressed data, was "render_engine-2023.7.4a2.tar", last modified: Mon Jul 17 16:40:31 2023, max compression
```

## Comparing `render_engine-2023.7.4a1.tar` & `render_engine-2023.7.4a2.tar`

### file list

```diff
@@ -1,126 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.183571 render_engine-2023.7.4a1/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.183571 render_engine-2023.7.4a1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.187571 render_engine-2023.7.4a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.187571 render_engine-2023.7.4a1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.187571 render_engine-2023.7.4a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.187571 render_engine-2023.7.4a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/Contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.187571 render_engine-2023.7.4a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.191571 render_engine-2023.7.4a1/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.195571 render_engine-2023.7.4a1/docs/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/assets/create-app-help.png
--rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/assets/render-engine-init-help.png
--rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/assets/render-engine-init.png
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/collection.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.195571 render_engine-2023.7.4a1/docs/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/contributing/pages.md
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/custom_collections.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/feeds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.195571 render_engine-2023.7.4a1/docs/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/building-your-site.md
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/creating-a-collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/creating-a-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/creating-your-app.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/layout.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/hookspecs.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/page.md
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/parsers.md
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/site.md
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/templates.md
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.195571 render_engine-2023.7.4a1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.203571 render_engine-2023.7.4a1/src/render_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.203571 render_engine-2023.7.4a1/src/render_engine/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/README_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/base_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.207571 render_engine-2023.7.4a1/src/render_engine/parsers/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.211571 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/base_collection_path.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/create_app_py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/rss2.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/rss2.0_items.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/sitemap.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/sitemap_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.203571 render_engine-2023.7.4a1/src/render_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/create_app_check_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/create_app_check_file_no_site_vars.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/tests/site_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/tests/site_test/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/site_test/blog/test_blog_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/site_test/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/tests/site_test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/site_test/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_parser_markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.358789 render_engine-2023.7.4a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.346789 render_engine-2023.7.4a2/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.346789 render_engine-2023.7.4a2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.346789 render_engine-2023.7.4a2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.github/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.github/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.346789 render_engine-2023.7.4a2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.350789 render_engine-2023.7.4a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.350789 render_engine-2023.7.4a2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/Contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-17 16:40:31.358789 render_engine-2023.7.4a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.350789 render_engine-2023.7.4a2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.350789 render_engine-2023.7.4a2/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.350789 render_engine-2023.7.4a2/docs/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/assets/create-app-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/assets/render-engine-init-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/assets/render-engine-init.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/collection.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.350789 render_engine-2023.7.4a2/docs/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/contributing/pages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/custom_collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/feeds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.350789 render_engine-2023.7.4a2/docs/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/getting-started/building-your-site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/getting-started/creating-a-collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/getting-started/creating-a-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/getting-started/creating-your-app.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/getting-started/layout.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/hookspecs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/docs/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:40:31.358789 render_engine-2023.7.4a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.350789 render_engine-2023.7.4a2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.354789 render_engine-2023.7.4a2/src/render_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.354789 render_engine-2023.7.4a2/src/render_engine/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/parsers/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/parsers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/parsers/README_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/parsers/base_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.354789 render_engine-2023.7.4a2/src/render_engine/parsers/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/parsers/markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/parsers/markdown/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.354789 render_engine-2023.7.4a2/src/render_engine/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/plugins/clean_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/plugins/site_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.358789 render_engine-2023.7.4a2/src/render_engine/render_engine_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/render_engine_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/render_engine_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/render_engine_templates/base_collection_path.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/render_engine_templates/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/render_engine_templates/create_app_py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/render_engine_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/render_engine_templates/rss2.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/render_engine_templates/rss2.0_items.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/render_engine_templates/sitemap.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/render_engine_templates/sitemap_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/src/render_engine/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.354789 render_engine-2023.7.4a2/src/render_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-17 16:40:31.000000 render_engine-2023.7.4a2/src/render_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-17 16:40:31.000000 render_engine-2023.7.4a2/src/render_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:40:31.000000 render_engine-2023.7.4a2/src/render_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-17 16:40:31.000000 render_engine-2023.7.4a2/src/render_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 16:40:31.000000 render_engine-2023.7.4a2/src/render_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 16:40:31.000000 render_engine-2023.7.4a2/src/render_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.358789 render_engine-2023.7.4a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/create_app_check_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/create_app_check_file_no_site_vars.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.358789 render_engine-2023.7.4a2/tests/site_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.358789 render_engine-2023.7.4a2/tests/site_test/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/site_test/blog/test_blog_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/site_test/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:40:31.358789 render_engine-2023.7.4a2/tests/site_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/site_test/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/test_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/test_parser_markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-17 16:40:12.000000 render_engine-2023.7.4a2/tests/test_site.py
```

### Comparing `render_engine-2023.7.4a1/.chglog/CHANGELOG.tpl.md` & `render_engine-2023.7.4a2/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/.chglog/config.yml` & `render_engine-2023.7.4a2/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/.devcontainer/devcontainer.json` & `render_engine-2023.7.4a2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/.github/CODE_OF_CONDUCT.md` & `render_engine-2023.7.4a2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/.github/CONTRIBUTION.md` & `render_engine-2023.7.4a2/.github/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/.github/FUNDING.yml` & `render_engine-2023.7.4a2/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/.github/LICENSE` & `render_engine-2023.7.4a2/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/.github/dependabot.yml` & `render_engine-2023.7.4a2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/.github/workflows/publish.yml` & `render_engine-2023.7.4a2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/.gitignore` & `render_engine-2023.7.4a2/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/PKG-INFO` & `render_engine-2023.7.4a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine
-Version: 2023.7.4a1
+Version: 2023.7.4a2
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.7.4a1/README.md` & `render_engine-2023.7.4a2/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/changelog.md` & `render_engine-2023.7.4a2/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 <a name="unreleased"></a>
 ## [Unreleased]
 
 
+<a name="2023.7.4a1"></a>
+## [2023.7.4a1] - 2023-07-16
+
 <a name="2023.7.3"></a>
 ## [2023.7.3] - 2023-07-15
 ### Pull Requests
 - Merge pull request [#214](https://github.com/kjaymiller/render_engine/issues/214) from kjaymiller:jm-update-requirements
 - Merge pull request [#213](https://github.com/kjaymiller/render_engine/issues/213) from kjaymiller/kjaymiller/issue210
 - Merge pull request [#212](https://github.com/kjaymiller/render_engine/issues/212) from kjaymiller/kjaymiller/issue210
 
@@ -196,15 +199,16 @@
 - Merge pull request [#54](https://github.com/kjaymiller/render_engine/issues/54) from jonafato/fix-docs-requirements
 - Merge pull request [#53](https://github.com/kjaymiller/render_engine/issues/53) from jonafato/missing-pages-broken-links
 - Merge pull request [#50](https://github.com/kjaymiller/render_engine/issues/50) from kjaymiller/adds-tox
 - Merge pull request [#41](https://github.com/kjaymiller/render_engine/issues/41) from jonafato/fix-tests
 - Merge pull request [#40](https://github.com/kjaymiller/render_engine/issues/40) from jonafato/test-in-ci
 
 
-[Unreleased]: https://github.com/kjaymiller/render_engine/compare/2023.7.3...HEAD
+[Unreleased]: https://github.com/kjaymiller/render_engine/compare/2023.7.4a1...HEAD
+[2023.7.4a1]: https://github.com/kjaymiller/render_engine/compare/2023.7.3...2023.7.4a1
 [2023.7.3]: https://github.com/kjaymiller/render_engine/compare/2023.7.1a1...2023.7.3
 [2023.7.1a1]: https://github.com/kjaymiller/render_engine/compare/2023.7.2a1...2023.7.1a1
 [2023.7.2a1]: https://github.com/kjaymiller/render_engine/compare/2023.7.1...2023.7.2a1
 [2023.7.1]: https://github.com/kjaymiller/render_engine/compare/2023.6.2b1...2023.7.1
 [2023.6.2b1]: https://github.com/kjaymiller/render_engine/compare/2023.6.1...2023.6.2b1
 [2023.6.1]: https://github.com/kjaymiller/render_engine/compare/2023.5.2a2...2023.6.1
 [2023.5.2a2]: https://github.com/kjaymiller/render_engine/compare/2023.5.2a1...2023.5.2a2
```

### Comparing `render_engine-2023.7.4a1/docs/docs/archive.md` & `render_engine-2023.7.4a2/docs/docs/archive.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/assets/create-app-help.png` & `render_engine-2023.7.4a2/docs/docs/assets/create-app-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/assets/render-engine-init-help.png` & `render_engine-2023.7.4a2/docs/docs/assets/render-engine-init-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/assets/render-engine-init.png` & `render_engine-2023.7.4a2/docs/docs/assets/render-engine-init.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/cli.md` & `render_engine-2023.7.4a2/docs/docs/cli.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/contributing/pages.md` & `render_engine-2023.7.4a2/docs/docs/contributing/pages.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/custom_collections.md` & `render_engine-2023.7.4a2/docs/docs/custom_collections.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/getting-started/building-your-site.md` & `render_engine-2023.7.4a2/docs/docs/getting-started/building-your-site.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/getting-started/creating-a-collection.md` & `render_engine-2023.7.4a2/docs/docs/getting-started/creating-a-collection.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/getting-started/creating-a-page.md` & `render_engine-2023.7.4a2/docs/docs/getting-started/creating-a-page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/getting-started/installation.md` & `render_engine-2023.7.4a2/docs/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/getting-started/layout.md` & `render_engine-2023.7.4a2/docs/docs/getting-started/layout.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/index.md` & `render_engine-2023.7.4a2/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/page.md` & `render_engine-2023.7.4a2/docs/docs/page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/parsers.md` & `render_engine-2023.7.4a2/docs/docs/parsers.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/plugins.md` & `render_engine-2023.7.4a2/docs/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/docs/templates.md` & `render_engine-2023.7.4a2/docs/docs/templates.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/docs/mkdocs.yml` & `render_engine-2023.7.4a2/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/pyproject.toml` & `render_engine-2023.7.4a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/requirements.txt` & `render_engine-2023.7.4a2/requirements.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/.DS_Store` & `render_engine-2023.7.4a2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/.DS_Store` & `render_engine-2023.7.4a2/src/render_engine/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/_base_object.py` & `render_engine-2023.7.4a2/src/render_engine/_base_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
         """
         base_dict ={
             **vars(self),
             "title": self._title,
             "slug": self._slug,
             "url": self.url_for(),
+            "path_name": self.path_name,
         }
 
         # Pull out template_vars
         if hasattr(self, "template_vars"):
             for key, value in self.template_vars.items():
                 base_dict[key] = value
```

### Comparing `render_engine-2023.7.4a1/src/render_engine/archive.py` & `render_engine-2023.7.4a2/src/render_engine/archive.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/blog.py` & `render_engine-2023.7.4a2/src/render_engine/blog.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/cli.py` & `render_engine-2023.7.4a2/src/render_engine/cli.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/collection.py` & `render_engine-2023.7.4a2/src/render_engine/collection.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/engine.py` & `render_engine-2023.7.4a2/src/render_engine/engine.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/feeds.py` & `render_engine-2023.7.4a2/src/render_engine/feeds.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 
 
 class RSSFeed(BasePage):
     """
     Creates an RSS feed [`Page`][render_engine.Page] Object.
 
     !!! Note
-        This is the base object type and should only contain the params identified by the standards defined in the [RSS 2.0 Specification](http://www.rssboard.org/rss-specification)
+        This is the base object type and should only contain the params identified
+        by the standards defined in the [RSS 2.0 Specification](http://www.rssboard.org/rss-specification)
 
     This is built using the built-in `rss2.0.xml` jinja template.
 
     !!! Note
-        Some browsers may not support the `rss` extension. If you are having issues with your feed, try changing the extension to `xml`.
+        Some browsers may not support the `rss` extension.
+        If you are having issues with your feed, try changing the extension to `xml`.
 
         ```python
         from render_engine import Site, RSSFeed
 
         class MyFeed(RSSFeed):
             extension = "xml"
 
@@ -30,8 +32,8 @@
         @site.collection
         class MyCollection(Collection):
             Feed = MyFeed
         ```
     """
 
     template = "rss2.0.xml"
-    extension: str = ".rss"
+    extension: str = ".rss"
```

### Comparing `render_engine-2023.7.4a1/src/render_engine/hookspecs.py` & `render_engine-2023.7.4a2/src/render_engine/hookspecs.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,22 @@
     for plugin in plugins:
         pm.register(plugin)
     return pm
 
 
 class SiteSpecs:
     """Plugin hook specifications for the Site class"""
+    default_settings: dict[str, typing.Any]
+    
+    @hook_spec
+    def add_default_settings(
+        self,
+        site: "Site",
+    ) -> None:
+        """Add default settings to the site"""
 
     @hook_spec
     def pre_build_site(
         self,
         site: "Site",
         settings: dict[str, typing.Any],
     ) -> None:
@@ -66,7 +74,12 @@
     @hook_spec
     def post_build_collection(
         self,
         site: "Site",
         settings: dict[str, typing.Any],
     ) -> None:
         """Build After Building the collection"""
+
+
+
+
+
```

### Comparing `render_engine-2023.7.4a1/src/render_engine/links.py` & `render_engine-2023.7.4a2/src/render_engine/links.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/page.py` & `render_engine-2023.7.4a2/src/render_engine/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Type, Callable
+from typing import Any, Callable
 
 import jinja2
 
 from ._base_object import BaseObject
 from .parsers.base_parsers import BasePageParser
 
 
@@ -130,25 +130,24 @@
             Defaults to `BasePageParser`.
         title: The title of the page. Defaults to the class name.
 
     """
 
     content: Any
     content_path: str | None
-    Parser: Type[BasePageParser] = BasePageParser
+    Parser: type[BasePageParser] = BasePageParser
     inherit_plugins: bool
     parser_extras: dict[str, Any] | None
     title: str
 
     def __init__(
         self,
         content_path: str | None = None,
         content: Any | None = None,
-        Parser: Type[BasePageParser] | None = None,
-        plugins: list[Callable] = [],
+        Parser: type[BasePageParser] | None = None,
     ) -> None:
 
         if Parser:
             self.Parser = Parser
 
         # Parse Content from the Content Path or the Content
         if content_path := (content_path or getattr(self, "content_path", None)):
```

### Comparing `render_engine-2023.7.4a1/src/render_engine/parsers/.DS_Store` & `render_engine-2023.7.4a2/src/render_engine/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/parsers/README_TEMPLATE.md` & `render_engine-2023.7.4a2/src/render_engine/parsers/README_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/parsers/base_parsers.py` & `render_engine-2023.7.4a2/src/render_engine/parsers/base_parsers.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/parsers/markdown/README.md` & `render_engine-2023.7.4a2/src/render_engine/parsers/markdown/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/render_engine_templates/create_app_py.txt` & `render_engine-2023.7.4a2/src/render_engine/render_engine_templates/create_app_py.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/render_engine_templates/index.html` & `render_engine-2023.7.4a2/src/render_engine/render_engine_templates/index.html`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/render_engine_templates/rss2.0.xml` & `render_engine-2023.7.4a2/src/render_engine/render_engine_templates/rss2.0.xml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0"?>
 <rss version="2.0" xmlns:atom="http://www.w3.org/2005/Atom">
   <channel>
     <title>{{SITE_TITLE}}-{{title}}</title>
     <link>{{SITE_URL}}</link>
     <description>{{description}}</description>
-    <atom:link href="{{SITE_URL}}" rel="self" type="application/rss+xml" />
+    <atom:link href="{{ path_name | to_absolute }}" rel="self" type="application/rss+xml" />
 
 {% if language is defined and language %}<language>{{language}}</language>{% endif %}
 {% if copyright is defined and copyright %}<copyright>{{copyright}}</copyright>{% endif %}
 {% if managing_editor is defined and managing_editor %}<managingEditor>{{managing_editor}}</managingEditor>{% endif %}
 {% if web_master is defined and web_master %}<webMaster>{{web_master}}</webMaster>{% endif %}
 {% if pub_date is defined and pub_date %}<pubDate>{{pub_date}}</pubDate>{% endif %}
 {% if last_build_date is defined and last_build_date %}<lastBuildDate>{{last_build_date}}</lastBuildDate>{% endif %}
```

### Comparing `render_engine-2023.7.4a1/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.7.4a2/src/render_engine/render_engine_templates/rss2.0_items.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/src/render_engine/site.py` & `render_engine-2023.7.4a2/src/render_engine/site.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import sys
+import typing
 import logging
 import pathlib
 import shutil
 from collections import defaultdict
 
 from jinja2 import Environment
 from rich.progress import Progress
 
 from .collection import Collection
 from .engine import engine
-from .hookspecs import register_plugins
 from .page import Page
+import pluggy
+from .hookspecs import _PROJECT_NAME, SiteSpecs
 
 class Site:
     """
     The site stores your pages and collections to be rendered.
 
     Attributes:
         engine: Jinja2 Environment used to render pages
@@ -27,38 +30,64 @@
             path for the static folder. This will get copied to the output folder.
         site_vars: 
             dictionary that will be passed into page template
         site_settings:
             settings that will be passed into pages and collections but not into templates
     """
 
+    _pm: pluggy.PluginManager
     output_path: str = "output"
     static_path: str = "static"
     partial: bool = False
     site_settings: dict = {
         "plugins": {}
     }
     site_vars: dict = {
         "SITE_TITLE": "Untitled Site",
         "SITE_URL": "http://localhost:8000/",
         "DATETIME_FORMAT": "%d %b %Y %H:%M %Z"
     }
-    plugins: list
     engine: Environment = engine
 
 
     def __init__(
         self,
-        plugins: list[str] = [],
     ) -> None:
         self.route_list = dict()
         self.subcollections = defaultdict(lambda: {"pages": []})
         self.engine.globals.update(self.site_vars)
-        self.plugins = [*plugins, *getattr(self, "plugins", [])]
-        self._pm = register_plugins(plugins=self.plugins)
+        
+        # Manage Plugins
+        self._pm = pluggy.PluginManager(project_name=_PROJECT_NAME)
+        self._pm.add_hookspecs(SiteSpecs)
+
+
+    def register_plugins(self, *plugins, **settings: dict[str, typing.Any]) -> None:
+        """Register plugins with the site
+        
+        parameters:
+            plugins: list of plugins to register
+            settings: settings to pass into the plugins
+                settings keys are the plugin names as strings.
+        """
+        
+        for plugin in plugins:
+            self._pm.register(plugin)        
+            self.site_settings['plugins'][plugin.__name__] = plugin.default_settings
+
+        self._pm.hook.add_default_settings(
+            site=self,
+            custom_settings=settings,
+        ) 
+        self.site_settings['plugins'].update(**settings)
+
+    @property
+    def plugins(self):
+        return self._pm.get_plugins()
+
 
     def collection(self, Collection: type[Collection]) -> Collection:
         """
         Add the collection to the route list to be rendered later.
 
         This is the primary way to add a collection to the site and 
         can either be called on an uninstantiated class or on the class definition as a decorator.
@@ -119,20 +148,21 @@
             pass
 
         site.page(About) # also works
         ```
         """
         page = Page()
         page.title = page._title # Expose _title to the user through `title`
-        
-        plugins = [*self.plugins, *getattr(page, "plugins", [])]
-        
+
+        # copy the plugin manager, removing any plugins that the page has ignored
+        page._pm = self._pm
+
         for plugin in getattr(page, 'ignore_plugins', []):
-            plugins.remove(plugin)
-        page.register_plugins(plugins)
+            page._pm.unregister(plugin)
+
         self.route_list[getattr(page, page._reference)] = page
 
     def _render_static(self) -> None:
         """Copies a Static Directory to the output folder"""
         shutil.copytree(
             self.static_path,
             pathlib.Path(self.output_path) / pathlib.Path(self.static_path).name,
```

### Comparing `render_engine-2023.7.4a1/src/render_engine.egg-info/PKG-INFO` & `render_engine-2023.7.4a2/src/render_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine
-Version: 2023.7.4a1
+Version: 2023.7.4a2
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.7.4a1/src/render_engine.egg-info/SOURCES.txt` & `render_engine-2023.7.4a2/src/render_engine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,29 +54,30 @@
 src/render_engine/cli.py
 src/render_engine/collection.py
 src/render_engine/engine.py
 src/render_engine/feeds.py
 src/render_engine/hookspecs.py
 src/render_engine/links.py
 src/render_engine/page.py
-src/render_engine/plugins.py
 src/render_engine/site.py
 src/render_engine.egg-info/PKG-INFO
 src/render_engine.egg-info/SOURCES.txt
 src/render_engine.egg-info/dependency_links.txt
 src/render_engine.egg-info/entry_points.txt
 src/render_engine.egg-info/requires.txt
 src/render_engine.egg-info/top_level.txt
 src/render_engine/parsers/.DS_Store
 src/render_engine/parsers/README.md
 src/render_engine/parsers/README_TEMPLATE.md
 src/render_engine/parsers/__init__.py
 src/render_engine/parsers/base_parsers.py
 src/render_engine/parsers/markdown/README.md
 src/render_engine/parsers/markdown/__init__.py
+src/render_engine/plugins/clean_output.py
+src/render_engine/plugins/site_map.py
 src/render_engine/render_engine_templates/__init__.py
 src/render_engine/render_engine_templates/base.html
 src/render_engine/render_engine_templates/base_collection_path.md
 src/render_engine/render_engine_templates/content.html
 src/render_engine/render_engine_templates/create_app_py.txt
 src/render_engine/render_engine_templates/index.html
 src/render_engine/render_engine_templates/rss2.0.xml
```

### Comparing `render_engine-2023.7.4a1/tests/conftest.py` & `render_engine-2023.7.4a2/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,15 +31,35 @@
 @pytest.fixture()
 def site(tmp_path):
     tmp_dir = tmp_path / "content"
     tmp_dir.mkdir()
     file = tmp_dir / "#"
     file.write_text("test")
     
+    site = Site()
 
+    @site.collection
     class TestCollection(Collection):
         pages = [Page(content_path=file)]
         Feed = RSSFeed
 
+    return site
+
+
+@pytest.fixture()
+def feed_test_site(tmp_path):
+    tmp_dir = tmp_path / "content"
+    tmp_dir.mkdir()
+    file = tmp_dir / "#"
+    file.write_text("test")
+    
     site = Site()
-    site.collection(TestCollection)
-    return site
+
+    @site.collection
+    class TestCollection(Collection):
+        pages = [Page(content_path=file)]
+        Feed = RSSFeed
+        routes = ['feed']
+
+    feed = site.route_list['testcollection'].feed
+    feed_content = feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
+    return feed_content
```

### Comparing `render_engine-2023.7.4a1/tests/create_app_check_file.txt` & `render_engine-2023.7.4a2/tests/create_app_check_file.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/tests/test_base_object.py` & `render_engine-2023.7.4a2/tests/test_base_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,22 +45,24 @@
 
     def test_base_object_to_dict(self):
         """Tests that the to_dict method returns a dict of the object's attributes"""
         assert self.test_object.to_dict() == {
             "title": "TestObject",
             "slug": "testobject",
             "url": None,
+            "path_name": "testobject.html",
         }
 
     def test_base_object_to_dict_with_template_vars(self):
         """Tests that the `to_dict` adds template_vars extracted method returns a dict of the object's attributes"""
         self.test_object.template_vars = {"test": "test"}
 
         assert self.test_object.to_dict() == {
             "title": "TestObject",
             "slug": "testobject",
             "url": None,
             "test": "test",
             'template_vars': {'test': 'test'},
+            "path_name": "testobject.html",
         }
 
         assert self.test_object.template_vars == {"test": "test"}
```

### Comparing `render_engine-2023.7.4a1/tests/test_base_parser.py` & `render_engine-2023.7.4a2/tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/tests/test_collections.py` & `render_engine-2023.7.4a2/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/tests/test_create_app.py` & `render_engine-2023.7.4a2/tests/test_create_app.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/tests/test_feeds.py` & `render_engine-2023.7.4a2/tests/test_feeds.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pluggy
 import pytest
 from jinja2 import StrictUndefined
 
 from render_engine.collection import Collection
 from render_engine.feeds import RSSFeed
 from render_engine.page import Page
+from render_engine.site import Site
 
 pm = pluggy.PluginManager("fake_test")
 
 
 def test_can_manually_set_slug():
     """Test that the feed slug can be set manually"""
 
@@ -25,49 +26,31 @@
     """Test that the feed path name is set correctly"""
 
     class feed(RSSFeed):
         pages = []
 
     assert feed().path_name == "feed.rss"
 
-def test_rss_feed_title_from_collection():
-    """Test that the feed title is set from the collection"""
+def test_rss_feed_title_from_collection(feed_test_site):
+    """
+    Test a Collection's title is used as the feed title if no title is provided.
+
+    In this case, the collection is named TestCollection.
+    """
+    assert "<title>Untitled Site-TestCollection</title>" in feed_test_site
 
-    class TestCollection(Collection):
-        feed_title = "Test Feed Title"
-        Feed = RSSFeed
-        pages = [Page()]
-
-    collection = TestCollection()
-
-    assert collection.feed.title == "Test Feed Title"
-
-
-def test_rss_feed_inherites_from_collection():
-    """Test that the feed title is set from the collection"""
-
-    class BasicCollection(Collection):
-        pages = [Page()]
-        archive_template = None
-        Feed = RSSFeed
-
-    collection = BasicCollection()
-
-    assert collection.feed.title == "BasicCollection"
-
-
-def test_rss_feed_item_url(site):
+def test_rss_feed_item_url(feed_test_site):
     """Test that the feed item url is set correctly"""
-    assert "<link>http://localhost:8000/page.html</link>" in site.route_list['testcollection'].feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
+    assert "<link>http://localhost:8000/page.html</link>" in feed_test_site
 
 
 
-def test_rss_feed_item_has_guid(site):
+def test_rss_feed_item_has_guid(feed_test_site):
     """Test that the feed item url is set correctly"""
-    assert '<guid isPermaLink="true">http://localhost:8000/page.html</guid>' in site.route_list['testcollection'].feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
+    assert '<guid isPermaLink="true">http://localhost:8000/page.html</guid>' in feed_test_site
 
 
 @pytest.mark.skip("Invalid Test")
 def test_rss_feed_template_with_strictundefined(engine, tmp_path):
     """Test that the RSS feed template works with the StrictUndefined undefined handler."""
     tmp_dir = tmp_path / "content"
     tmp_dir.mkdir()
@@ -89,15 +72,14 @@
     )
     assert "http://localhost:8000/page.html" in rendered_content
 
 
 def test_rss_feed_template_parses_date_correctly(engine):
     """Tests that a feed parses the page date in RFC2822 Format"""
 
-
     class TestPage(Page):
         date = datetime.datetime(2023, 4, 15, 0, 0, 0, tzinfo=datetime.timezone.utc)   # noqa: UP017
     class TestCollection(Collection):
         Feed = RSSFeed
         pages = [TestPage()]
 
     collection = TestCollection()
@@ -107,7 +89,11 @@
         SITE_TITLE="Test Site Title",
         SITE_URL="http://localhost:8000",
         title="Test Feed Title",
         description="Test Feed Description",
     )
 
     assert "Sat, 15 Apr 2023 00:00:00 +0000" in rendered_content
+
+def test_feed_atom_link(feed_test_site):
+    """Test that the feed atom link is set correctly"""
+    assert '<atom:link href="http://localhost:8000/testcollection.rss" rel="self" type="application/rss+xml" />' in feed_test_site
```

### Comparing `render_engine-2023.7.4a1/tests/test_page.py` & `render_engine-2023.7.4a2/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.4a1/tests/test_plugins.py` & `render_engine-2023.7.4a2/tests/test_plugins.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,62 +5,56 @@
 from render_engine.page import Page
 from render_engine.site import Site
 from render_engine.collection import Collection
 
 
 class FakePlugin:
     """Clean the output folder before rendering"""
+    default_settings = {
+        "test": "default",
+    }
 
     @hook_impl
     def pre_build_site(
         site: type[Site],
         settings: dict[str, typing.Any]|None,
         ):
-        """Clean the output folder before rendering"""
+        """Test Pre Build Site"""
         if settings:
             logging.info(settings['FakePlugin']['test'])
         else:
-            print(settings)
             raise ValueError("FAIL")
 
 @pytest.fixture
 def site():
-    class TestSite(Site):
-        plugins = [
-            FakePlugin,
-        ]
+    site = Site()
+    site.register_plugins(FakePlugin)
+    return site
 
-    return TestSite()
-
-def test_register_plugins(site: "TestSite"):
+def test_plugin_is_registered(site: Site):
     """Check that the plugin is registered"""
-    assert site._pm.list_name_plugin()[0][0] == 'FakePlugin' 
+    assert [site._pm.get_name(x) for x in site.plugins] == ['FakePlugin']
+
 
 def test_pages_in_collection_inherit_pugins():
     """Check that collection plugins are inherited by pages in the collection"""
 
     collection = Collection()
     collection.register_plugins([FakePlugin])
     page = collection.get_page()
     # Check that a plugin was registered in the page
     assert page._pm.list_name_plugin()[0][0] == 'FakePlugin' 
 
     # Check that the plugin is the same as the one in the collection
     assert page._pm.get_plugins() == collection._pm.get_plugins()
 
 
-def test_page_ignores_plugin():
+def test_page_ignores_plugin(site: Site):
     """Check that the plugin is not registered in the page if it is ignored"""
-    class testSite(Site):
-        plugins = [
-            FakePlugin,
-        ]
-
-    site = testSite()
-    
+       
     @site.page
     class testPage(Page):
         ignore_plugins = [
             FakePlugin,
         ]
     
     assert site.route_list['testpage']._pm.list_name_plugin() == []
@@ -80,31 +74,17 @@
             FakePlugin,
         ]
     
     assert site.route_list['testcollection']._pm.list_name_plugin() == []
 
     
 
-def test_plugin_settings_from_site(caplog):
+def test_plugin_settings_from_site(caplog, site: Site):
     """Check that the plugin settings are passed from the site to the plugin"""
-    
-    class testSite(Site):
-        plugins = [
-            FakePlugin,
-        ]
-        site_settings = {
-            "plugins": {
-                "FakePlugin": {
-                    "test": "Testing the plugin settings"
-                }
-            }
-        }
 
-    
-    site = testSite()
     with caplog.at_level(logging.INFO):
         site._pm.hook.pre_build_site(
             site=site,
             settings=site.site_settings['plugins']
         )
-    assert 'Testing the plugin settings' in caplog.text
+    assert 'default' in caplog.text
```

### Comparing `render_engine-2023.7.4a1/tests/test_site.py` & `render_engine-2023.7.4a2/tests/test_site.py`

 * *Files identical despite different names*

