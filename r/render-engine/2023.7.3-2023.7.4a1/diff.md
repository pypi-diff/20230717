# Comparing `tmp/render_engine-2023.7.3.tar.gz` & `tmp/render_engine-2023.7.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine-2023.7.3.tar", last modified: Sat Jul 15 15:16:07 2023, max compression
+gzip compressed data, was "render_engine-2023.7.4a1.tar", last modified: Sun Jul 16 23:43:16 2023, max compression
```

## Comparing `render_engine-2023.7.3.tar` & `render_engine-2023.7.4a1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-15 15:15:45.000000 render_engine-2023.7.3/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-15 15:15:45.000000 render_engine-2023.7.3/Contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-15 15:16:07.074638 render_engine-2023.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-15 15:15:45.000000 render_engine-2023.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-15 15:15:45.000000 render_engine-2023.7.3/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.062637 render_engine-2023.7.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.066638 render_engine-2023.7.3/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.066638 render_engine-2023.7.3/docs/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/assets/create-app-help.png
--rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/assets/render-engine-init-help.png
--rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/assets/render-engine-init.png
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/collection.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.066638 render_engine-2023.7.3/docs/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/contributing/pages.md
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/custom_collections.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/feeds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.066638 render_engine-2023.7.3/docs/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/building-your-site.md
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/creating-a-collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/creating-a-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/creating-your-app.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/getting-started/layout.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/hookspecs.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/page.md
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/parsers.md
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/site.md
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/docs/templates.md
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-15 15:15:45.000000 render_engine-2023.7.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-15 15:15:45.000000 render_engine-2023.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-15 15:15:45.000000 render_engine-2023.7.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 15:16:07.074638 render_engine-2023.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.066638 render_engine-2023.7.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.070638 render_engine-2023.7.3/src/render_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.070638 render_engine-2023.7.3/src/render_engine/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/README_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/base_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.070638 render_engine-2023.7.3/src/render_engine/parsers/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/parsers/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/src/render_engine/render_engine_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/base_collection_path.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/create_app_py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/rss2.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/rss2.0_items.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/sitemap.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/render_engine_templates/sitemap_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-15 15:15:45.000000 render_engine-2023.7.3/src/render_engine/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.070638 render_engine-2023.7.3/src/render_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 15:16:07.000000 render_engine-2023.7.3/src/render_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/create_app_check_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/create_app_check_file_no_site_vars.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/tests/site_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/tests/site_test/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/site_test/blog/test_blog_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/site_test/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:07.074638 render_engine-2023.7.3/tests/site_test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/site_test/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_parser_markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-15 15:15:45.000000 render_engine-2023.7.3/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.183571 render_engine-2023.7.4a1/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.183571 render_engine-2023.7.4a1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.187571 render_engine-2023.7.4a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.187571 render_engine-2023.7.4a1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.187571 render_engine-2023.7.4a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.187571 render_engine-2023.7.4a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/Contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.187571 render_engine-2023.7.4a1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.191571 render_engine-2023.7.4a1/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.195571 render_engine-2023.7.4a1/docs/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/assets/create-app-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/assets/render-engine-init-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/assets/render-engine-init.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/collection.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.195571 render_engine-2023.7.4a1/docs/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/contributing/pages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/custom_collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/feeds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.195571 render_engine-2023.7.4a1/docs/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/building-your-site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/creating-a-collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/creating-a-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/creating-your-app.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/getting-started/layout.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/hookspecs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/docs/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.195571 render_engine-2023.7.4a1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.203571 render_engine-2023.7.4a1/src/render_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.203571 render_engine-2023.7.4a1/src/render_engine/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/README_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/base_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.207571 render_engine-2023.7.4a1/src/render_engine/parsers/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/parsers/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.211571 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/base_collection_path.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/create_app_py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/rss2.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/rss2.0_items.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/sitemap.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/render_engine_templates/sitemap_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/src/render_engine/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.203571 render_engine-2023.7.4a1/src/render_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 23:43:16.000000 render_engine-2023.7.4a1/src/render_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/create_app_check_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/create_app_check_file_no_site_vars.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/tests/site_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/tests/site_test/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/site_test/blog/test_blog_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/site_test/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 23:43:16.215571 render_engine-2023.7.4a1/tests/site_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/site_test/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_parser_markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-16 23:43:01.000000 render_engine-2023.7.4a1/tests/test_site.py
```

### Comparing `render_engine-2023.7.3/.chglog/CHANGELOG.tpl.md` & `render_engine-2023.7.4a1/.chglog/CHANGELOG.tpl.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 {{ if .Versions -}}
 <a name="unreleased"></a>
 ## [Unreleased]
 
 {{ if .Unreleased.CommitGroups -}}
 {{ range .Unreleased.CommitGroups -}}
+### {{ .Title }}
 {{ range .Commits -}}
-- {{ .Header }}
+- {{ if .Scope }}**{{ .Scope }}:** {{ end }}{{ .Subject }}
 {{ end }}
 {{ end -}}
 {{ end -}}
 {{ end -}}
 
 {{ range .Versions }}
 <a name="{{ .Tag.Name }}"></a>
 ## {{ if .Tag.Previous }}[{{ .Tag.Name }}]{{ else }}{{ .Tag.Name }}{{ end }} - {{ datetime "2006-01-02" .Tag.Date }}
 {{ range .CommitGroups -}}
+### {{ .Title }}
 {{ range .Commits -}}
-- {{ .Header }}
+- {{ if .Scope }}**{{ .Scope }}:** {{ end }}{{ .Subject }}
 {{ end }}
 {{ end -}}
 
 {{- if .RevertCommits -}}
 ### Reverts
 {{ range .RevertCommits -}}
 - {{ .Revert.Header }}
```

### Comparing `render_engine-2023.7.3/.devcontainer/devcontainer.json` & `render_engine-2023.7.4a1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/.github/CODE_OF_CONDUCT.md` & `render_engine-2023.7.4a1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/.github/CONTRIBUTION.md` & `render_engine-2023.7.4a1/.github/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/.github/FUNDING.yml` & `render_engine-2023.7.4a1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/.github/LICENSE` & `render_engine-2023.7.4a1/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/.github/dependabot.yml` & `render_engine-2023.7.4a1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/.github/workflows/publish.yml` & `render_engine-2023.7.4a1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/.gitignore` & `render_engine-2023.7.4a1/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/PKG-INFO` & `render_engine-2023.7.4a1/src/render_engine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: render_engine
-Version: 2023.7.3
+Name: render-engine
+Version: 2023.7.4a1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.7.3/README.md` & `render_engine-2023.7.4a1/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/changelog.md` & `render_engine-2023.7.4a1/changelog.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,67 @@
 <a name="unreleased"></a>
 ## [Unreleased]
 
 
+<a name="2023.7.3"></a>
+## [2023.7.3] - 2023-07-15
+### Pull Requests
+- Merge pull request [#214](https://github.com/kjaymiller/render_engine/issues/214) from kjaymiller:jm-update-requirements
+- Merge pull request [#213](https://github.com/kjaymiller/render_engine/issues/213) from kjaymiller/kjaymiller/issue210
+- Merge pull request [#212](https://github.com/kjaymiller/render_engine/issues/212) from kjaymiller/kjaymiller/issue210
+
+
+<a name="2023.7.1a1"></a>
+## [2023.7.1a1] - 2023-07-02
+
+<a name="2023.7.2a1"></a>
+## [2023.7.2a1] - 2023-07-02
+### Pull Requests
+- Merge pull request [#211](https://github.com/kjaymiller/render_engine/issues/211) from kjaymiller:2023.7.1-create-post-render-content
+
+
+<a name="2023.7.1"></a>
+## [2023.7.1] - 2023-06-15
+### Pull Requests
+- Merge pull request [#204](https://github.com/kjaymiller/render_engine/issues/204) from kjaymiller/jm-makes-feed-public
+- Merge pull request [#203](https://github.com/kjaymiller/render_engine/issues/203) from kjaymiller/jm-makes-feed-public
+
+
+<a name="2023.6.2b1"></a>
+## [2023.6.2b1] - 2023-06-15
+### Pull Requests
+- Merge pull request [#202](https://github.com/kjaymiller/render_engine/issues/202) from kjaymiller:kjaymiller/issue180
+
+
+<a name="2023.6.1"></a>
+## [2023.6.1] - 2023-06-01
+
+<a name="2023.5.2a2"></a>
+## [2023.5.2a2] - 2023-05-18
+### Pull Requests
+- Merge pull request [#193](https://github.com/kjaymiller/render_engine/issues/193) from kjaymiller/dependabot/pip/typer-0.9.0
+
+
+<a name="2023.5.2a1"></a>
+## [2023.5.2a1] - 2023-05-15
+
 <a name="2023.5.1"></a>
 ## [2023.5.1] - 2023-05-08
 
 <a name="2023.5.1a2"></a>
 ## [2023.5.1a2] - 2023-05-08
 
 <a name="2023.5.1a1"></a>
 ## [2023.5.1a1] - 2023-05-08
+### Pencil
+- Fixes settings typo
+
+### Tractor
+- Fixes Getting Started link
 
-<a name="v-2023.5.1a1"></a>
-## [v-2023.5.1a1] - 2023-05-08
 ### Pull Requests
 - Merge pull request [#187](https://github.com/kjaymiller/render_engine/issues/187) from kjaymiller:dependabot/pip/platformdirs-3.5.0
 - Merge pull request [#189](https://github.com/kjaymiller/render_engine/issues/189) from kjaymiller:dependabot/pip/ruff-0.0.265
 - Merge pull request [#188](https://github.com/kjaymiller/render_engine/issues/188) from kjaymiller:dependabot/pip/urllib3-2.0.2
 - Merge pull request [#190](https://github.com/kjaymiller/render_engine/issues/190) from kjaymiller:dependabot/pip/rich-13.3.5
 - Merge pull request [#191](https://github.com/kjaymiller/render_engine/issues/191) from kjaymiller:dependabot/pip/mkdocs-1.4.3
 - Merge pull request [#185](https://github.com/kjaymiller/render_engine/issues/185) from kjaymiller/kjaymiller/issue146
@@ -151,19 +196,26 @@
 - Merge pull request [#54](https://github.com/kjaymiller/render_engine/issues/54) from jonafato/fix-docs-requirements
 - Merge pull request [#53](https://github.com/kjaymiller/render_engine/issues/53) from jonafato/missing-pages-broken-links
 - Merge pull request [#50](https://github.com/kjaymiller/render_engine/issues/50) from kjaymiller/adds-tox
 - Merge pull request [#41](https://github.com/kjaymiller/render_engine/issues/41) from jonafato/fix-tests
 - Merge pull request [#40](https://github.com/kjaymiller/render_engine/issues/40) from jonafato/test-in-ci
 
 
-[Unreleased]: https://github.com/kjaymiller/render_engine/compare/2023.5.1...HEAD
+[Unreleased]: https://github.com/kjaymiller/render_engine/compare/2023.7.3...HEAD
+[2023.7.3]: https://github.com/kjaymiller/render_engine/compare/2023.7.1a1...2023.7.3
+[2023.7.1a1]: https://github.com/kjaymiller/render_engine/compare/2023.7.2a1...2023.7.1a1
+[2023.7.2a1]: https://github.com/kjaymiller/render_engine/compare/2023.7.1...2023.7.2a1
+[2023.7.1]: https://github.com/kjaymiller/render_engine/compare/2023.6.2b1...2023.7.1
+[2023.6.2b1]: https://github.com/kjaymiller/render_engine/compare/2023.6.1...2023.6.2b1
+[2023.6.1]: https://github.com/kjaymiller/render_engine/compare/2023.5.2a2...2023.6.1
+[2023.5.2a2]: https://github.com/kjaymiller/render_engine/compare/2023.5.2a1...2023.5.2a2
+[2023.5.2a1]: https://github.com/kjaymiller/render_engine/compare/2023.5.1...2023.5.2a1
 [2023.5.1]: https://github.com/kjaymiller/render_engine/compare/2023.5.1a2...2023.5.1
 [2023.5.1a2]: https://github.com/kjaymiller/render_engine/compare/2023.5.1a1...2023.5.1a2
-[2023.5.1a1]: https://github.com/kjaymiller/render_engine/compare/v-2023.5.1a1...2023.5.1a1
-[v-2023.5.1a1]: https://github.com/kjaymiller/render_engine/compare/2023.4.2a1...v-2023.5.1a1
+[2023.5.1a1]: https://github.com/kjaymiller/render_engine/compare/2023.4.2a1...2023.5.1a1
 [2023.4.2a1]: https://github.com/kjaymiller/render_engine/compare/2023.4.1a5...2023.4.2a1
 [2023.4.1a5]: https://github.com/kjaymiller/render_engine/compare/2023.4.1a4...2023.4.1a5
 [2023.4.1a4]: https://github.com/kjaymiller/render_engine/compare/2023.4.1a3...2023.4.1a4
 [2023.4.1a3]: https://github.com/kjaymiller/render_engine/compare/2023.4.1a2...2023.4.1a3
 [2023.4.1a2]: https://github.com/kjaymiller/render_engine/compare/2023.4.1a1...2023.4.1a2
 [2023.4.1a1]: https://github.com/kjaymiller/render_engine/compare/2023.3.1b13...2023.4.1a1
 [2023.3.1b13]: https://github.com/kjaymiller/render_engine/compare/2023.3.1b14...2023.3.1b13
```

### Comparing `render_engine-2023.7.3/docs/docs/archive.md` & `render_engine-2023.7.4a1/docs/docs/archive.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/assets/create-app-help.png` & `render_engine-2023.7.4a1/docs/docs/assets/create-app-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/assets/render-engine-init-help.png` & `render_engine-2023.7.4a1/docs/docs/assets/render-engine-init-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/assets/render-engine-init.png` & `render_engine-2023.7.4a1/docs/docs/assets/render-engine-init.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/cli.md` & `render_engine-2023.7.4a1/docs/docs/cli.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/contributing/pages.md` & `render_engine-2023.7.4a1/docs/docs/contributing/pages.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/custom_collections.md` & `render_engine-2023.7.4a1/docs/docs/custom_collections.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/getting-started/building-your-site.md` & `render_engine-2023.7.4a1/docs/docs/getting-started/building-your-site.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/getting-started/creating-a-collection.md` & `render_engine-2023.7.4a1/docs/docs/getting-started/creating-a-collection.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/getting-started/creating-a-page.md` & `render_engine-2023.7.4a1/docs/docs/getting-started/creating-a-page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/getting-started/installation.md` & `render_engine-2023.7.4a1/docs/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/getting-started/layout.md` & `render_engine-2023.7.4a1/docs/docs/getting-started/layout.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/index.md` & `render_engine-2023.7.4a1/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/page.md` & `render_engine-2023.7.4a1/docs/docs/page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/parsers.md` & `render_engine-2023.7.4a1/docs/docs/parsers.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/plugins.md` & `render_engine-2023.7.4a1/docs/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/docs/templates.md` & `render_engine-2023.7.4a1/docs/docs/templates.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/docs/mkdocs.yml` & `render_engine-2023.7.4a1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/pyproject.toml` & `render_engine-2023.7.4a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/requirements.txt` & `render_engine-2023.7.4a1/requirements.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/.DS_Store` & `render_engine-2023.7.4a1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/.DS_Store` & `render_engine-2023.7.4a1/src/render_engine/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/_base_object.py` & `render_engine-2023.7.4a1/src/render_engine/_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/archive.py` & `render_engine-2023.7.4a1/src/render_engine/archive.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/blog.py` & `render_engine-2023.7.4a1/src/render_engine/blog.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/cli.py` & `render_engine-2023.7.4a1/src/render_engine/cli.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/collection.py` & `render_engine-2023.7.4a1/src/render_engine/collection.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/engine.py` & `render_engine-2023.7.4a1/src/render_engine/engine.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/feeds.py` & `render_engine-2023.7.4a1/src/render_engine/feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/hookspecs.py` & `render_engine-2023.7.4a1/src/render_engine/hookspecs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing
+
 import pluggy
 
 _PROJECT_NAME = "render_engine"
 hook_impl = pluggy.HookimplMarker(project_name=_PROJECT_NAME)
 hook_spec = pluggy.HookspecMarker(project_name=_PROJECT_NAME)
 
 
@@ -15,34 +17,56 @@
     return pm
 
 
 class SiteSpecs:
     """Plugin hook specifications for the Site class"""
 
     @hook_spec
-    def pre_build_site(self, site: "Site") -> None:
+    def pre_build_site(
+        self,
+        site: "Site",
+        settings: dict[str, typing.Any],
+    ) -> None:
         """Steps Prior to Building the site"""
 
-
     @hook_spec
-    def post_build_site(self, site: "Site") -> None:
+    def post_build_site(
+        self,
+        site: "Site",
+        settings: dict[str, typing.Any],
+    ) -> None:
         """Build After Building the site"""
 
     @hook_spec
-    def render_content(page: "page"):
+    def render_content(
+        self,
+        page: "page",
+        settings: dict[str, typing.Any],
+    ) -> None:
         """
         Augments the content of the page before it is rendered as output.
         """
 
     @hook_spec
-    def post_render_content(page : "page"):
+    def post_render_content(
+        self,
+        page : "page",
+        settings: dict[str: typing.Any]):
         """
         Augments the content of the page before it is rendered as output.
         """
 
     @hook_spec
-    def pre_build_collection(self, collection: "Collection") -> None:
+    def pre_build_collection(
+        self,
+        collection: "Collection",
+        settings: dict[str, typing.Any],
+    ) -> None:
         """Steps Prior to Building the collection"""
 
     @hook_spec
-    def post_build_collection(self, site: "Site") -> None:
+    def post_build_collection(
+        self,
+        site: "Site",
+        settings: dict[str, typing.Any],
+    ) -> None:
         """Build After Building the collection"""
```

### Comparing `render_engine-2023.7.3/src/render_engine/links.py` & `render_engine-2023.7.4a1/src/render_engine/links.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/page.py` & `render_engine-2023.7.4a1/src/render_engine/page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/parsers/.DS_Store` & `render_engine-2023.7.4a1/src/render_engine/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/parsers/README_TEMPLATE.md` & `render_engine-2023.7.4a1/src/render_engine/parsers/README_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/parsers/base_parsers.py` & `render_engine-2023.7.4a1/src/render_engine/parsers/base_parsers.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/parsers/markdown/README.md` & `render_engine-2023.7.4a1/src/render_engine/parsers/markdown/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/plugins.py` & `render_engine-2023.7.4a1/src/render_engine/plugins.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/render_engine_templates/create_app_py.txt` & `render_engine-2023.7.4a1/src/render_engine/render_engine_templates/create_app_py.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/render_engine_templates/index.html` & `render_engine-2023.7.4a1/src/render_engine/render_engine_templates/index.html`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/render_engine_templates/rss2.0.xml` & `render_engine-2023.7.4a1/src/render_engine/render_engine_templates/rss2.0.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.7.4a1/src/render_engine/render_engine_templates/rss2.0_items.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/src/render_engine/site.py` & `render_engine-2023.7.4a1/src/render_engine/site.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,18 @@
         _Collection = Collection()
         plugins = [*self.plugins, *getattr(_Collection, "plugins", [])]
         
         for plugin in getattr(_Collection, 'ignore_plugins', []):
             plugins.remove(plugin)
         _Collection.register_plugins(plugins)
 
-        self._pm.hook.pre_build_collection(collection=_Collection) #type: ignore
+        self._pm.hook.pre_build_collection(
+            collection=_Collection,
+            settings=self.site_settings.get('plugins', {}),
+        ) #type: ignore
         self.route_list[_Collection._slug] = _Collection
         return _Collection
 
     def page(self, Page: Page) -> Page:
         """
         Add the page to the route list to be rendered later.
         Also remaps `title` in case the user wants to use it in the template rendering.
@@ -195,15 +198,18 @@
 
         You can choose to call it manually in your file or use the CLI command [`render-engine build`][src.render_engine.cli.build]
         """
 
         with Progress() as progress:
 
             pre_build_task = progress.add_task("Loading Pre-Build Plugins", total=1)
-            self._pm.hook.pre_build_site(site=self)
+            self._pm.hook.pre_build_site(
+                site=self,
+                settings=self.site_settings.get('plugins', {})
+                ) #type: ignore
 
             # Parse Route List
             task_add_route = progress.add_task(
                 "[blue]Adding Routes", total=len(self.route_list)
             )
 
             if pathlib.Path(self.static_path).exists():
@@ -213,23 +219,26 @@
 
             for slug, entry in self.route_list.items():
                 progress.update(
                     task_add_route, description=f"[blue]Adding[gold]Route: [blue]{slug}"
                 )
                 if isinstance(entry, Page):
                     if getattr(entry, "collection", None):
-                        self._pm.hook.render_content(Page=entry)
+                        self._pm.hook.render_content(Page=entry, settings=self.site_settings.get('plugins', None))
                     for route in entry.routes:
                         progress.update(
                             task_add_route,
                             description=f"[blue]Adding[gold]Route: [blue]{entry._slug}",
                         )
                         self._render_output(route, entry)
 
                 if isinstance(entry, Collection):
                     if self.partial:
                         self._render_partial_collection(entry)
                     else:
                         self._render_full_collection(entry)
             progress.add_task("Loading Post-Build Plugins", total=1)
-            self._pm.hook.post_build_site(site=self)
+            self._pm.hook.post_build_site(
+                site=self,
+                settings=self.site_settings.get('plugins', {}),
+            )
             progress.update(pre_build_task, advance=1)
```

### Comparing `render_engine-2023.7.3/src/render_engine.egg-info/PKG-INFO` & `render_engine-2023.7.4a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: render-engine
-Version: 2023.7.3
+Name: render_engine
+Version: 2023.7.4a1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.7.3/src/render_engine.egg-info/SOURCES.txt` & `render_engine-2023.7.4a1/src/render_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/tests/conftest.py` & `render_engine-2023.7.4a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/tests/create_app_check_file.txt` & `render_engine-2023.7.4a1/tests/create_app_check_file.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/tests/test_base_object.py` & `render_engine-2023.7.4a1/tests/test_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/tests/test_base_parser.py` & `render_engine-2023.7.4a1/tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/tests/test_collections.py` & `render_engine-2023.7.4a1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/tests/test_create_app.py` & `render_engine-2023.7.4a1/tests/test_create_app.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/tests/test_feeds.py` & `render_engine-2023.7.4a1/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/tests/test_page.py` & `render_engine-2023.7.4a1/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.7.3/tests/test_plugins.py` & `render_engine-2023.7.4a1/tests/test_plugins.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+import typing
+import logging
 import pytest
 from render_engine.hookspecs import hook_impl
 from render_engine.page import Page
 from render_engine.site import Site
 from render_engine.collection import Collection
 
 
 class FakePlugin:
     """Clean the output folder before rendering"""
 
     @hook_impl
-    def pre_build_site(site: type[Site]):
+    def pre_build_site(
+        site: type[Site],
+        settings: dict[str, typing.Any]|None,
+        ):
         """Clean the output folder before rendering"""
-        pass
+        if settings:
+            logging.info(settings['FakePlugin']['test'])
+        else:
+            print(settings)
+            raise ValueError("FAIL")
 
 @pytest.fixture
 def site():
     class TestSite(Site):
         plugins = [
             FakePlugin,
         ]
@@ -69,8 +78,33 @@
     class testCollection(Collection):
         ignore_plugins = [
             FakePlugin,
         ]
     
     assert site.route_list['testcollection']._pm.list_name_plugin() == []
 
+    
+
+def test_plugin_settings_from_site(caplog):
+    """Check that the plugin settings are passed from the site to the plugin"""
+    
+    class testSite(Site):
+        plugins = [
+            FakePlugin,
+        ]
+        site_settings = {
+            "plugins": {
+                "FakePlugin": {
+                    "test": "Testing the plugin settings"
+                }
+            }
+        }
+
+    
+    site = testSite()
+    with caplog.at_level(logging.INFO):
+        site._pm.hook.pre_build_site(
+            site=site,
+            settings=site.site_settings['plugins']
+        )
+    assert 'Testing the plugin settings' in caplog.text
```

### Comparing `render_engine-2023.7.3/tests/test_site.py` & `render_engine-2023.7.4a1/tests/test_site.py`

 * *Files identical despite different names*

