# Comparing `tmp/docx-hitalent-0.8.50.tar.gz` & `tmp/docx-hitalent-0.8.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx-hitalent-0.8.50.tar", last modified: Tue Nov 22 07:19:39 2022, max compression
+gzip compressed data, was "docx-hitalent-0.8.51.tar", last modified: Mon Jul 17 05:08:46 2023, max compression
```

## Comparing `docx-hitalent-0.8.50.tar` & `docx-hitalent-0.8.51.tar`

### file list

```diff
@@ -1,520 +1,520 @@
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.285294 docx-hitalent-0.8.50/
--rw-r--r--   0 ghoul      (501) staff       (20)     8861 2022-11-22 02:12:45.000000 docx-hitalent-0.8.50/HISTORY.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     1104 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/LICENSE
--rw-r--r--   0 ghoul      (501) staff       (20)      200 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/MANIFEST.in
--rw-r--r--   0 ghoul      (501) staff       (20)    11505 2022-11-22 07:19:39.284687 docx-hitalent-0.8.50/PKG-INFO
--rw-r--r--   0 ghoul      (501) staff       (20)      382 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/README.rst
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.818582 docx-hitalent-0.8.50/docs/
--rw-r--r--   0 ghoul      (501) staff       (20)     5580 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/Makefile
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.819774 docx-hitalent-0.8.50/docs/_static/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/_static/.gitignore
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.823716 docx-hitalent-0.8.50/docs/_static/img/
--rw-r--r--   0 ghoul      (501) staff       (20)    77526 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/_static/img/example-docx-01.png
--rw-r--r--   0 ghoul      (501) staff       (20)    56762 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/_static/img/hdrftr-01.png
--rw-r--r--   0 ghoul      (501) staff       (20)    16218 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/_static/img/hdrftr-02.png
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.824501 docx-hitalent-0.8.50/docs/_templates/
--rw-r--r--   0 ghoul      (501) staff       (20)      299 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/_templates/sidebarlinks.html
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.788567 docx-hitalent-0.8.50/docs/_themes/
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.828834 docx-hitalent-0.8.50/docs/_themes/armstrong/
--rw-r--r--   0 ghoul      (501) staff       (20)     1164 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/_themes/armstrong/LICENSE
--rw-r--r--   0 ghoul      (501) staff       (20)     1661 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/_themes/armstrong/layout.html
--rw-r--r--   0 ghoul      (501) staff       (20)     1147 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/_themes/armstrong/rtd-themes.conf
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.829641 docx-hitalent-0.8.50/docs/_themes/armstrong/static/
--rw-r--r--   0 ghoul      (501) staff       (20)    16885 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/_themes/armstrong/static/rtd.css_t
--rw-r--r--   0 ghoul      (501) staff       (20)     1147 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/_themes/armstrong/theme.conf
--rw-r--r--   0 ghoul      (501) staff       (20)     1400 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/_themes/armstrong/theme.conf.orig
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.844145 docx-hitalent-0.8.50/docs/api/
--rw-r--r--   0 ghoul      (501) staff       (20)      255 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/dml.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     3363 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/document.rst
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.884419 docx-hitalent-0.8.50/docs/api/enum/
--rw-r--r--   0 ghoul      (501) staff       (20)      382 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/MsoColorType.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     1270 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/MsoThemeColorIndex.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      791 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdAlignParagraph.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     4567 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdBuiltinStyle.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      804 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdCellVerticalAlignment.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      692 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdColorIndex.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      771 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdLineSpacing.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      339 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdOrientation.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      336 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdRowAlignment.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      519 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdRowHeightRule.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      486 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdSectionStart.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      421 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdStyleType.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      434 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdTabAlignment.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      285 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdTabLeader.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      495 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdTableDirection.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     1334 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/WdUnderline.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      446 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/enum/index.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      565 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/section.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      206 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/settings.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      613 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/shape.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     1174 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/shared.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     1808 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/style.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      621 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/table.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      778 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/api/text.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    10904 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/conf.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.789959 docx-hitalent-0.8.50/docs/dev/
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.885021 docx-hitalent-0.8.50/docs/dev/analysis/
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.889429 docx-hitalent-0.8.50/docs/dev/analysis/features/
--rw-r--r--   0 ghoul      (501) staff       (20)     7557 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/coreprops.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    11261 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/header.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     2015 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/numbering.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    10642 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/sections.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    13252 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/settings.rst
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.892238 docx-hitalent-0.8.50/docs/dev/analysis/features/shapes/
--rw-r--r--   0 ghoul      (501) staff       (20)     1935 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/shapes/index.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     9428 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/shapes/picture.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     3459 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/shapes/shapes-inline-size.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     6584 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/shapes/shapes-inline.rst
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.896122 docx-hitalent-0.8.50/docs/dev/analysis/features/styles/
--rw-r--r--   0 ghoul      (501) staff       (20)     5471 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/styles/character-style.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    12771 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/styles/index.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     8560 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/styles/latent-styles.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     5508 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/styles/paragraph-style.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    13979 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/styles/style.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     8145 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/styles/styles.rst
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.900201 docx-hitalent-0.8.50/docs/dev/analysis/features/table/
--rw-r--r--   0 ghoul      (501) staff       (20)    20675 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/table/cell-merge.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     9218 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/table/index.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     8041 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/table/table-cell.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     7949 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/table/table-props.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     4150 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/table/table-row.rst
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.909563 docx-hitalent-0.8.50/docs/dev/analysis/features/text/
--rw-r--r--   0 ghoul      (501) staff       (20)     7581 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/text/breaks.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     9879 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/text/font-color.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     5902 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/text/font-highlight-color.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    18391 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/text/font.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      159 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/text/index.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    16282 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/text/paragraph-format.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     3094 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/text/run-content.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     9567 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/text/tab-stops.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     4247 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/features/text/underline.rst
--rw-r--r--   0 ghoul      (501) staff       (20)      576 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/index.rst
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.912532 docx-hitalent-0.8.50/docs/dev/analysis/schema/
--rw-r--r--   0 ghoul      (501) staff       (20)     7226 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/schema/ct_body.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     4659 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/schema/ct_document.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     6406 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/dev/analysis/schema/ct_p.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     3824 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/index.rst
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.918891 docx-hitalent-0.8.50/docs/user/
--rw-r--r--   0 ghoul      (501) staff       (20)     1287 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/user/api-concepts.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     3635 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/user/documents.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     6897 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/user/hdrftr.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     1031 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/user/install.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    11875 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/user/quickstart.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     3859 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/user/sections.rst
--rw-r--r--   0 ghoul      (501) staff       (20)     1477 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/user/shapes.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    12392 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/user/styles-understanding.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    13587 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/user/styles-using.rst
--rw-r--r--   0 ghoul      (501) staff       (20)    14125 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docs/user/text.rst
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.931392 docx-hitalent-0.8.50/docx/
--rw-r--r--   0 ghoul      (501) staff       (20)     1480 2022-11-22 02:12:45.000000 docx-hitalent-0.8.50/docx/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1242 2021-12-29 08:23:13.000000 docx-hitalent-0.8.50/docx/api.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2872 2022-01-22 07:43:55.000000 docx-hitalent-0.8.50/docx/blkcntnr.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1043 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/compat.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.932614 docx-hitalent-0.8.50/docx/dml/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/dml/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3978 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/dml/color.py
--rw-r--r--   0 ghoul      (501) staff       (20)     7497 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/document.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.937378 docx-hitalent-0.8.50/docx/enum/
--rw-r--r--   0 ghoul      (501) staff       (20)      343 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/enum/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)    11042 2022-10-08 03:28:45.000000 docx-hitalent-0.8.50/docx/enum/base.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3533 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/enum/dml.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2666 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/enum/section.py
--rw-r--r--   0 ghoul      (501) staff       (20)      475 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/enum/shape.py
--rw-r--r--   0 ghoul      (501) staff       (20)    12189 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/enum/style.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3929 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/enum/table.py
--rw-r--r--   0 ghoul      (501) staff       (20)    10810 2021-12-27 05:07:08.000000 docx-hitalent-0.8.50/docx/enum/text.py
--rw-r--r--   0 ghoul      (501) staff       (20)      503 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/exceptions.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.943389 docx-hitalent-0.8.50/docx/image/
--rw-r--r--   0 ghoul      (501) staff       (20)      754 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/image/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1512 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/image/bmp.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3471 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/image/constants.py
--rw-r--r--   0 ghoul      (501) staff       (20)      432 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/image/exceptions.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1260 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/image/gif.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3286 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/image/helpers.py
--rw-r--r--   0 ghoul      (501) staff       (20)     8029 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/image/image.py
--rw-r--r--   0 ghoul      (501) staff       (20)    16099 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/image/jpeg.py
--rw-r--r--   0 ghoul      (501) staff       (20)     8789 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/image/png.py
--rw-r--r--   0 ghoul      (501) staff       (20)    11140 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/image/tiff.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.950806 docx-hitalent-0.8.50/docx/opc/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1327 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/compat.py
--rw-r--r--   0 ghoul      (501) staff       (20)    20515 2021-12-29 08:23:13.000000 docx-hitalent-0.8.50/docx/opc/constants.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3246 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/coreprops.py
--rw-r--r--   0 ghoul      (501) staff       (20)      302 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/exceptions.py
--rw-r--r--   0 ghoul      (501) staff       (20)     8540 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/oxml.py
--rw-r--r--   0 ghoul      (501) staff       (20)     8510 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/package.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3880 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/packuri.py
--rw-r--r--   0 ghoul      (501) staff       (20)     8157 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/part.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.951390 docx-hitalent-0.8.50/docx/opc/parts/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/parts/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1664 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/parts/coreprops.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4370 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/phys_pkg.py
--rw-r--r--   0 ghoul      (501) staff       (20)    10311 2022-10-20 09:06:50.000000 docx-hitalent-0.8.50/docx/opc/pkgreader.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4524 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/pkgwriter.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5385 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/rel.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1453 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/shared.py
--rw-r--r--   0 ghoul      (501) staff       (20)      716 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/opc/spec.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.960018 docx-hitalent-0.8.50/docx/oxml/
--rw-r--r--   0 ghoul      (501) staff       (20)    11906 2022-10-09 09:15:37.000000 docx-hitalent-0.8.50/docx/oxml/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)    10278 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/oxml/coreprops.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2513 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/oxml/document.py
--rw-r--r--   0 ghoul      (501) staff       (20)      290 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/oxml/exceptions.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3969 2022-01-13 09:30:22.000000 docx-hitalent-0.8.50/docx/oxml/ns.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5265 2022-10-08 02:41:55.000000 docx-hitalent-0.8.50/docx/oxml/numbering.py
--rw-r--r--   0 ghoul      (501) staff       (20)    11463 2022-10-21 09:12:28.000000 docx-hitalent-0.8.50/docx/oxml/section.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3491 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/oxml/settings.py
--rw-r--r--   0 ghoul      (501) staff       (20)    12070 2022-10-08 02:37:34.000000 docx-hitalent-0.8.50/docx/oxml/shape.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1623 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/oxml/shared.py
--rw-r--r--   0 ghoul      (501) staff       (20)    12126 2022-10-08 01:57:26.000000 docx-hitalent-0.8.50/docx/oxml/simpletypes.py
--rw-r--r--   0 ghoul      (501) staff       (20)    11125 2022-01-21 07:38:50.000000 docx-hitalent-0.8.50/docx/oxml/styles.py
--rw-r--r--   0 ghoul      (501) staff       (20)    30495 2022-10-09 09:19:04.000000 docx-hitalent-0.8.50/docx/oxml/table.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.963952 docx-hitalent-0.8.50/docx/oxml/text/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/oxml/text/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)    10114 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/oxml/text/font.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2247 2022-01-22 07:41:15.000000 docx-hitalent-0.8.50/docx/oxml/text/paragraph.py
--rw-r--r--   0 ghoul      (501) staff       (20)    10767 2022-01-21 09:09:02.000000 docx-hitalent-0.8.50/docx/oxml/text/parfmt.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5088 2022-01-22 07:07:07.000000 docx-hitalent-0.8.50/docx/oxml/text/run.py
--rw-r--r--   0 ghoul      (501) staff       (20)    10050 2022-10-11 08:10:53.000000 docx-hitalent-0.8.50/docx/oxml/textbox.py
--rw-r--r--   0 ghoul      (501) staff       (20)    24645 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/oxml/xmlchemy.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3868 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/package.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.968391 docx-hitalent-0.8.50/docx/parts/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/parts/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5355 2022-08-05 07:07:54.000000 docx-hitalent-0.8.50/docx/parts/document.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1717 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/parts/hdrftr.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2668 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/parts/image.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2788 2022-10-08 01:57:26.000000 docx-hitalent-0.8.50/docx/parts/numbering.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1465 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/parts/settings.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3238 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/parts/story.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1428 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/parts/styles.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2315 2022-09-30 06:39:26.000000 docx-hitalent-0.8.50/docx/picture.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1215 2022-10-11 09:47:10.000000 docx-hitalent-0.8.50/docx/rect.py
--rw-r--r--   0 ghoul      (501) staff       (20)    16201 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/section.py
--rw-r--r--   0 ghoul      (501) staff       (20)      780 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/settings.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2811 2022-01-13 09:33:30.000000 docx-hitalent-0.8.50/docx/shape.py
--rw-r--r--   0 ghoul      (501) staff       (20)     6836 2022-09-22 06:55:10.000000 docx-hitalent-0.8.50/docx/shared.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.970327 docx-hitalent-0.8.50/docx/styles/
--rw-r--r--   0 ghoul      (501) staff       (20)     1500 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/styles/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     7549 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/styles/latent.py
--rw-r--r--   0 ghoul      (501) staff       (20)     7987 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/styles/style.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5637 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/styles/styles.py
--rw-r--r--   0 ghoul      (501) staff       (20)    18479 2022-11-22 02:10:56.000000 docx-hitalent-0.8.50/docx/table.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.973757 docx-hitalent-0.8.50/docx/templates/
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.974654 docx-hitalent-0.8.50/docx/templates/default-docx-template/
--rw-r--r--   0 ghoul      (501) staff       (20)     1782 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/[Content_Types].xml
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.975005 docx-hitalent-0.8.50/docx/templates/default-docx-template/_rels/
--rw-r--r--   0 ghoul      (501) staff       (20)      748 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/_rels/.rels
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.976137 docx-hitalent-0.8.50/docx/templates/default-docx-template/customXml/
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.976631 docx-hitalent-0.8.50/docx/templates/default-docx-template/customXml/_rels/
--rw-r--r--   0 ghoul      (501) staff       (20)      300 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/customXml/_rels/item1.xml.rels
--rw-r--r--   0 ghoul      (501) staff       (20)      262 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/customXml/item1.xml
--rw-r--r--   0 ghoul      (501) staff       (20)      354 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/customXml/itemProps1.xml
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.977868 docx-hitalent-0.8.50/docx/templates/default-docx-template/docProps/
--rw-r--r--   0 ghoul      (501) staff       (20)     1132 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/docProps/app.xml
--rw-r--r--   0 ghoul      (501) staff       (20)      753 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/docProps/core.xml
--rw-r--r--   0 ghoul      (501) staff       (20)     8324 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/docProps/thumbnail.jpeg
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.987043 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.988943 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/_rels/
--rw-r--r--   0 ghoul      (501) staff       (20)     1253 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/_rels/document.xml.rels
--rw-r--r--   0 ghoul      (501) staff       (20)     1594 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/document.xml
--rw-r--r--   0 ghoul      (501) staff       (20)     2811 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/fontTable.xml
--rw-r--r--   0 ghoul      (501) staff       (20)     6747 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/numbering.xml
--rw-r--r--   0 ghoul      (501) staff       (20)     2749 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/settings.xml
--rw-r--r--   0 ghoul      (501) staff       (20)   438677 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/styles.xml
--rw-r--r--   0 ghoul      (501) staff       (20)   438131 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/stylesWithEffects.xml
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.989640 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/theme/
--rw-r--r--   0 ghoul      (501) staff       (20)    10939 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/theme/theme1.xml
--rw-r--r--   0 ghoul      (501) staff       (20)      438 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-docx-template/word/webSettings.xml
--rw-r--r--   0 ghoul      (501) staff       (20)     1395 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-footer.xml
--rw-r--r--   0 ghoul      (501) staff       (20)     1395 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-header.xml
--rw-r--r--   0 ghoul      (501) staff       (20)     1640 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-settings.xml
--rw-r--r--   0 ghoul      (501) staff       (20)    15823 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default-styles.xml
--rw-r--r--   0 ghoul      (501) staff       (20)    38116 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/templates/default.docx
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.993100 docx-hitalent-0.8.50/docx/text/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/text/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)    12072 2022-01-21 09:41:56.000000 docx-hitalent-0.8.50/docx/text/font.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5737 2022-10-08 01:51:39.000000 docx-hitalent-0.8.50/docx/text/paragraph.py
--rw-r--r--   0 ghoul      (501) staff       (20)    10833 2022-09-22 07:58:07.000000 docx-hitalent-0.8.50/docx/text/parfmt.py
--rw-r--r--   0 ghoul      (501) staff       (20)     8035 2022-11-22 03:01:09.000000 docx-hitalent-0.8.50/docx/text/run.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4183 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/docx/text/tabstops.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2070 2022-11-22 07:19:35.000000 docx-hitalent-0.8.50/docx/textbox.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:38.996505 docx-hitalent-0.8.50/docx_hitalent.egg-info/
--rw-r--r--   0 ghoul      (501) staff       (20)    11505 2022-11-22 07:19:38.000000 docx-hitalent-0.8.50/docx_hitalent.egg-info/PKG-INFO
--rw-r--r--   0 ghoul      (501) staff       (20)    14393 2022-11-22 07:19:38.000000 docx-hitalent-0.8.50/docx_hitalent.egg-info/SOURCES.txt
--rw-r--r--   0 ghoul      (501) staff       (20)        1 2022-11-22 07:19:38.000000 docx-hitalent-0.8.50/docx_hitalent.egg-info/dependency_links.txt
--rw-r--r--   0 ghoul      (501) staff       (20)        1 2021-12-27 02:59:56.000000 docx-hitalent-0.8.50/docx_hitalent.egg-info/not-zip-safe
--rw-r--r--   0 ghoul      (501) staff       (20)       12 2022-11-22 07:19:38.000000 docx-hitalent-0.8.50/docx_hitalent.egg-info/requires.txt
--rw-r--r--   0 ghoul      (501) staff       (20)        5 2022-11-22 07:19:38.000000 docx-hitalent-0.8.50/docx_hitalent.egg-info/top_level.txt
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.051354 docx-hitalent-0.8.50/features/
--rw-r--r--   0 ghoul      (501) staff       (20)      476 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/api-open-document.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      407 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/blk-add-paragraph.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      378 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/blk-add-table.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      428 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/cel-add-table.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      343 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/cel-text.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      981 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/doc-access-collections.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      395 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/doc-access-sections.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      840 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/doc-add-heading.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      358 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/doc-add-page-break.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      883 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/doc-add-paragraph.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      997 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/doc-add-picture.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1110 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/doc-add-section.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      729 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/doc-add-table.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      892 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/doc-coreprops.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1398 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/doc-settings.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      598 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/doc-styles.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      310 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/environment.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3116 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/hdr-header-footer.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1499 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/img-characterize-image.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      402 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/num-access-numbering-part.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      312 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/par-access-parfmt.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      527 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/par-add-run.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      632 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/par-alignment-prop.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      405 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/par-clear-paragraph.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      577 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/par-insert-paragraph.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      390 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/par-set-text.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      871 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/par-style-prop.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      312 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/run-access-content.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      269 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/run-access-font.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      467 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/run-add-content.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      804 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/run-add-picture.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1173 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/run-char-style.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      373 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/run-clear-run.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1757 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/run-enum-props.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     5082 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/sct-section.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1070 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/shp-inline-shape-access.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      575 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/shp-inline-shape-size.feature
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.064939 docx-hitalent-0.8.50/features/steps/
--rw-r--r--   0 ghoul      (501) staff       (20)     1680 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/api.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1266 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/block.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1468 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/cell.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4455 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/coreprops.py
--rw-r--r--   0 ghoul      (501) staff       (20)     8937 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/document.py
--rw-r--r--   0 ghoul      (501) staff       (20)     7114 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/font.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5163 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/hdrftr.py
--rw-r--r--   0 ghoul      (501) staff       (20)      853 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/helpers.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2273 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/image.py
--rw-r--r--   0 ghoul      (501) staff       (20)      970 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/numbering.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5460 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/paragraph.py
--rw-r--r--   0 ghoul      (501) staff       (20)     8249 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/parfmt.py
--rw-r--r--   0 ghoul      (501) staff       (20)     8963 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/section.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1942 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/settings.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5304 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/shape.py
--rw-r--r--   0 ghoul      (501) staff       (20)      563 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/shared.py
--rw-r--r--   0 ghoul      (501) staff       (20)    18220 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/styles.py
--rw-r--r--   0 ghoul      (501) staff       (20)    15719 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/table.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4670 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/tabstops.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.158547 docx-hitalent-0.8.50/features/steps/test_files/
--rw-r--r--   0 ghoul      (501) staff       (20)    25142 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/blk-containing-table.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    80603 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/court-exif.jpg
--rw-r--r--   0 ghoul      (501) staff       (20)    25591 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/doc-access-sections.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    17956 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/doc-add-section.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    11992 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/doc-coreprops.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    21366 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/doc-default.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    11394 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/doc-no-coreprops.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    17711 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/doc-odd-even-hdrs.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    21309 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/doc-word-default-blank.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    15846 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/fnt-color.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    18079 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/hdr-header-footer.docx
--rw-r--r--   0 ghoul      (501) staff       (20)   355196 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/jfif-300-dpi.jpg
--rw-r--r--   0 ghoul      (501) staff       (20)   768608 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/jpeg420exif.jpg
--rw-r--r--   0 ghoul      (501) staff       (20)   263222 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/lena.bmp
--rw-r--r--   0 ghoul      (501) staff       (20)    72985 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/lena.gif
--rw-r--r--   0 ghoul      (501) staff       (20)   786572 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/lena.tif
--rw-r--r--   0 ghoul      (501) staff       (20)   104428 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/lena_std.jpg
--rw-r--r--   0 ghoul      (501) staff       (20)    64276 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/monty-truth.png
--rw-r--r--   0 ghoul      (501) staff       (20)   308280 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/mountain.bmp
--rw-r--r--   0 ghoul      (501) staff       (20)    24334 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/num-having-numbering-part.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    15126 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/par-alignment.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    27969 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/par-known-paragraphs.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    20901 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/par-known-styles.docx
--rw-r--r--   0 ghoul      (501) staff       (20)     3277 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/python-icon.jpeg
--rw-r--r--   0 ghoul      (501) staff       (20)    26645 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/run-char-style.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    14645 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/run-enumerated-props.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    10409 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/sample.tif
--rw-r--r--   0 ghoul      (501) staff       (20)    14849 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/sct-first-page-hdrftr.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    28168 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/sct-section-props.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    10760 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/set-no-settings-part.docx
--rw-r--r--   0 ghoul      (501) staff       (20)   122610 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/shp-inline-shape-access.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    12195 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/sty-behav-props.docx
--rw-r--r--   0 ghoul      (501) staff       (20)     8358 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/sty-having-no-styles-part.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    21573 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/sty-having-styles-part.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    13560 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/sty-known-styles.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    13170 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/tab-stops.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    25129 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/tbl-2x2-table.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    36051 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/tbl-cell-access.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    13654 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/tbl-col-props.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    50294 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/tbl-having-applied-style.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    32010 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/tbl-having-tables.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    16017 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/tbl-on-off-props.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    20178 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/tbl-props.docx
--rw-r--r--   0 ghoul      (501) staff       (20)   146892 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/test.png
--rw-r--r--   0 ghoul      (501) staff       (20)    12859 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/txt-font-highlight-color.docx
--rw-r--r--   0 ghoul      (501) staff       (20)    37924 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/test_files/txt-font-props.docx
--rw-r--r--   0 ghoul      (501) staff       (20)     8848 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/steps/text.py
--rw-r--r--   0 ghoul      (501) staff       (20)      463 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/sty-access-font.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      568 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/sty-access-latent-styles.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      488 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/sty-access-parfmt.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      767 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/sty-add-style.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      352 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/sty-delete-style.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      654 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/sty-latent-add-del.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     4102 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/sty-latent-props.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     5464 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/sty-style-props.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1264 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/tab-access-tabs.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1877 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/tab-tabstop-props.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      594 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/tbl-add-row-or-col.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1523 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/tbl-cell-access.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1861 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/tbl-cell-props.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1062 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/tbl-col-props.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      944 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/tbl-item-access.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     2294 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/tbl-merge-cells.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     2907 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/tbl-props.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1665 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/tbl-row-props.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     1169 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/tbl-style.feature
--rw-r--r--   0 ghoul      (501) staff       (20)      645 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/txt-add-break.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     2279 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/txt-font-color.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     8120 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/txt-font-props.feature
--rw-r--r--   0 ghoul      (501) staff       (20)     7648 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/features/txt-parfmt-props.feature
--rw-r--r--   0 ghoul      (501) staff       (20)       38 2022-11-22 07:19:39.285449 docx-hitalent-0.8.50/setup.cfg
--rw-r--r--   0 ghoul      (501) staff       (20)     2389 2021-12-27 03:04:55.000000 docx-hitalent-0.8.50/setup.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.174839 docx-hitalent-0.8.50/tests/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/__init__.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.176157 docx-hitalent-0.8.50/tests/dml/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/dml/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5411 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/dml/test_color.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.183546 docx-hitalent-0.8.50/tests/image/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/image/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1211 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/image/test_bmp.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1061 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/image/test_gif.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1659 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/image/test_helpers.py
--rw-r--r--   0 ghoul      (501) staff       (20)    12157 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/image/test_image.py
--rw-r--r--   0 ghoul      (501) staff       (20)    21667 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/image/test_jpeg.py
--rw-r--r--   0 ghoul      (501) staff       (20)    15009 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/image/test_png.py
--rw-r--r--   0 ghoul      (501) staff       (20)    14805 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/image/test_tiff.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.195086 docx-hitalent-0.8.50/tests/opc/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/__init__.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.196654 docx-hitalent-0.8.50/tests/opc/parts/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/parts/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1991 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/parts/test_coreprops.py
--rw-r--r--   0 ghoul      (501) staff       (20)     7910 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/test_coreprops.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4913 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/test_oxml.py
--rw-r--r--   0 ghoul      (501) staff       (20)    16878 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/test_package.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3203 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/test_packuri.py
--rw-r--r--   0 ghoul      (501) staff       (20)    16641 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/test_part.py
--rw-r--r--   0 ghoul      (501) staff       (20)     6560 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/test_phys_pkg.py
--rw-r--r--   0 ghoul      (501) staff       (20)    18670 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/test_pkgreader.py
--rw-r--r--   0 ghoul      (501) staff       (20)     7099 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/test_pkgwriter.py
--rw-r--r--   0 ghoul      (501) staff       (20)     9759 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/test_rel.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.199213 docx-hitalent-0.8.50/tests/opc/unitdata/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/unitdata/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     8804 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/unitdata/rels.py
--rw-r--r--   0 ghoul      (501) staff       (20)      859 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/opc/unitdata/types.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.204501 docx-hitalent-0.8.50/tests/oxml/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/__init__.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.205531 docx-hitalent-0.8.50/tests/oxml/parts/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/parts/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1543 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/parts/test_document.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.206448 docx-hitalent-0.8.50/tests/oxml/parts/unitdata/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/parts/unitdata/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)      409 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/parts/unitdata/document.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4237 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/test__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1750 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/test_ns.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1284 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/test_styles.py
--rw-r--r--   0 ghoul      (501) staff       (20)    12720 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/test_table.py
--rw-r--r--   0 ghoul      (501) staff       (20)    28182 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/test_xmlchemy.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.207626 docx-hitalent-0.8.50/tests/oxml/text/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/text/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)      998 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/text/test_run.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.215719 docx-hitalent-0.8.50/tests/oxml/unitdata/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/unitdata/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4060 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/unitdata/dml.py
--rw-r--r--   0 ghoul      (501) staff       (20)      434 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/unitdata/numbering.py
--rw-r--r--   0 ghoul      (501) staff       (20)      872 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/unitdata/section.py
--rw-r--r--   0 ghoul      (501) staff       (20)      699 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/unitdata/shared.py
--rw-r--r--   0 ghoul      (501) staff       (20)      469 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/unitdata/styles.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1444 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/unitdata/table.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3187 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/oxml/unitdata/text.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.222828 docx-hitalent-0.8.50/tests/parts/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/parts/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)    12469 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/parts/test_document.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5152 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/parts/test_hdrftr.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4056 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/parts/test_image.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2641 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/parts/test_numbering.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2688 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/parts/test_settings.py
--rw-r--r--   0 ghoul      (501) staff       (20)     5429 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/parts/test_story.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1820 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/parts/test_styles.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.227287 docx-hitalent-0.8.50/tests/styles/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/styles/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)    13842 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/styles/test_latent.py
--rw-r--r--   0 ghoul      (501) staff       (20)    20568 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/styles/test_style.py
--rw-r--r--   0 ghoul      (501) staff       (20)    14432 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/styles/test_styles.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2401 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_api.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4824 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_blkcntnr.py
--rw-r--r--   0 ghoul      (501) staff       (20)    13332 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_document.py
--rw-r--r--   0 ghoul      (501) staff       (20)     3055 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_enum.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.254412 docx-hitalent-0.8.50/tests/test_files/
--rw-r--r--   0 ghoul      (501) staff       (20)   146892 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/150-dpi.png
--rw-r--r--   0 ghoul      (501) staff       (20)   125824 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/300-dpi.TIF
--rw-r--r--   0 ghoul      (501) staff       (20)   355196 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/300-dpi.jpg
--rw-r--r--   0 ghoul      (501) staff       (20)    39921 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/300-dpi.png
--rw-r--r--   0 ghoul      (501) staff       (20)     9454 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/72-dpi.tiff
--rw-r--r--   0 ghoul      (501) staff       (20)     1526 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/CVS_LOGO.WMF
--rw-r--r--   0 ghoul      (501) staff       (20)   768608 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/exif-420-dpi.jpg
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.254905 docx-hitalent-0.8.50/tests/test_files/expanded_docx/
--rw-r--r--   0 ghoul      (501) staff       (20)     1738 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/[Content_Types].xml
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.255458 docx-hitalent-0.8.50/tests/test_files/expanded_docx/_rels/
--rw-r--r--   0 ghoul      (501) staff       (20)      734 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/_rels/.rels
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.256787 docx-hitalent-0.8.50/tests/test_files/expanded_docx/customXml/
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.257382 docx-hitalent-0.8.50/tests/test_files/expanded_docx/customXml/_rels/
--rw-r--r--   0 ghoul      (501) staff       (20)      295 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/customXml/_rels/item1.xml.rels
--rw-r--r--   0 ghoul      (501) staff       (20)      217 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/customXml/item1.xml
--rw-r--r--   0 ghoul      (501) staff       (20)      340 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/customXml/itemProps1.xml
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.259456 docx-hitalent-0.8.50/tests/test_files/expanded_docx/docProps/
--rw-r--r--   0 ghoul      (501) staff       (20)     1036 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/docProps/app.xml
--rw-r--r--   0 ghoul      (501) staff       (20)      802 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/docProps/core.xml
--rw-r--r--   0 ghoul      (501) staff       (20)    13032 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/docProps/thumbnail.jpeg
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.269917 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.270887 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/_rels/
--rw-r--r--   0 ghoul      (501) staff       (20)     1227 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/_rels/document.xml.rels
--rw-r--r--   0 ghoul      (501) staff       (20)     1819 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/document.xml
--rw-r--r--   0 ghoul      (501) staff       (20)     2566 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/fontTable.xml
--rw-r--r--   0 ghoul      (501) staff       (20)     5513 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/numbering.xml
--rw-r--r--   0 ghoul      (501) staff       (20)     2520 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/settings.xml
--rw-r--r--   0 ghoul      (501) staff       (20)    26715 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/styles.xml
--rw-r--r--   0 ghoul      (501) staff       (20)    27581 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/stylesWithEffects.xml
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.271858 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/theme/
--rw-r--r--   0 ghoul      (501) staff       (20)     7642 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/theme/theme1.xml
--rw-r--r--   0 ghoul      (501) staff       (20)      430 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/webSettings.xml
--rw-r--r--   0 ghoul      (501) staff       (20)   132875 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/having-images.docx
--rw-r--r--   0 ghoul      (501) staff       (20)     7958 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/jfif-iguana.jpg
--rw-r--r--   0 ghoul      (501) staff       (20)    10409 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/little-endian.tif
--rw-r--r--   0 ghoul      (501) staff       (20)    64276 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/monty-truth.png
--rw-r--r--   0 ghoul      (501) staff       (20)     3277 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/python-icon.jpeg
--rw-r--r--   0 ghoul      (501) staff       (20)     2036 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/python-icon.png
--rw-r--r--   0 ghoul      (501) staff       (20)     6111 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/python-powered.png
--rw-r--r--   0 ghoul      (501) staff       (20)    45210 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/python.bmp
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.275503 docx-hitalent-0.8.50/tests/test_files/snippets/
--rw-r--r--   0 ghoul      (501) staff       (20)     2949 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/snippets/add-row-col.txt
--rw-r--r--   0 ghoul      (501) staff       (20)     1110 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/snippets/inline.txt
--rw-r--r--   0 ghoul      (501) staff       (20)     1756 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/snippets/new-tbl.txt
--rw-r--r--   0 ghoul      (501) staff       (20)     4595 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/snippets/tbl-cells.txt
--rw-r--r--   0 ghoul      (501) staff       (20)    33273 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/sonic.gif
--rw-r--r--   0 ghoul      (501) staff       (20)    31773 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_files/test.docx
--rw-r--r--   0 ghoul      (501) staff       (20)     5418 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_package.py
--rw-r--r--   0 ghoul      (501) staff       (20)    29075 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_section.py
--rw-r--r--   0 ghoul      (501) staff       (20)     2279 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_settings.py
--rw-r--r--   0 ghoul      (501) staff       (20)     6591 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_shape.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4398 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_shared.py
--rw-r--r--   0 ghoul      (501) staff       (20)    34086 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/test_table.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.281503 docx-hitalent-0.8.50/tests/text/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/text/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)    17045 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/text/test_font.py
--rw-r--r--   0 ghoul      (501) staff       (20)    11267 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/text/test_paragraph.py
--rw-r--r--   0 ghoul      (501) staff       (20)    19399 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/text/test_parfmt.py
--rw-r--r--   0 ghoul      (501) staff       (20)    13565 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/text/test_run.py
--rw-r--r--   0 ghoul      (501) staff       (20)    11016 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/text/test_tabstops.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4329 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/unitdata.py
-drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2022-11-22 07:19:39.283758 docx-hitalent-0.8.50/tests/unitutil/
--rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/unitutil/__init__.py
--rw-r--r--   0 ghoul      (501) staff       (20)     8334 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/unitutil/cxml.py
--rw-r--r--   0 ghoul      (501) staff       (20)     1600 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/unitutil/file.py
--rw-r--r--   0 ghoul      (501) staff       (20)     4281 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tests/unitutil/mock.py
--rw-r--r--   0 ghoul      (501) staff       (20)      667 2021-12-27 02:12:49.000000 docx-hitalent-0.8.50/tox.ini
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:46.003644 docx-hitalent-0.8.51/
+-rw-r--r--   0 ghoul      (501) staff       (20)     8933 2023-07-17 03:15:53.000000 docx-hitalent-0.8.51/HISTORY.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     1104 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/LICENSE
+-rw-r--r--   0 ghoul      (501) staff       (20)      200 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/MANIFEST.in
+-rw-r--r--   0 ghoul      (501) staff       (20)    11557 2023-07-17 05:08:46.003150 docx-hitalent-0.8.51/PKG-INFO
+-rw-r--r--   0 ghoul      (501) staff       (20)      382 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/README.rst
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.518345 docx-hitalent-0.8.51/docs/
+-rw-r--r--   0 ghoul      (501) staff       (20)     5580 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/Makefile
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.519457 docx-hitalent-0.8.51/docs/_static/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/_static/.gitignore
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.523934 docx-hitalent-0.8.51/docs/_static/img/
+-rw-r--r--   0 ghoul      (501) staff       (20)    77526 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/_static/img/example-docx-01.png
+-rw-r--r--   0 ghoul      (501) staff       (20)    56762 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/_static/img/hdrftr-01.png
+-rw-r--r--   0 ghoul      (501) staff       (20)    16218 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/_static/img/hdrftr-02.png
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.524901 docx-hitalent-0.8.51/docs/_templates/
+-rw-r--r--   0 ghoul      (501) staff       (20)      299 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/_templates/sidebarlinks.html
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.491846 docx-hitalent-0.8.51/docs/_themes/
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.531315 docx-hitalent-0.8.51/docs/_themes/armstrong/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1164 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/_themes/armstrong/LICENSE
+-rw-r--r--   0 ghoul      (501) staff       (20)     1661 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/_themes/armstrong/layout.html
+-rw-r--r--   0 ghoul      (501) staff       (20)     1147 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/_themes/armstrong/rtd-themes.conf
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.532677 docx-hitalent-0.8.51/docs/_themes/armstrong/static/
+-rw-r--r--   0 ghoul      (501) staff       (20)    16885 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/_themes/armstrong/static/rtd.css_t
+-rw-r--r--   0 ghoul      (501) staff       (20)     1147 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/_themes/armstrong/theme.conf
+-rw-r--r--   0 ghoul      (501) staff       (20)     1400 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/_themes/armstrong/theme.conf.orig
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.543255 docx-hitalent-0.8.51/docs/api/
+-rw-r--r--   0 ghoul      (501) staff       (20)      255 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/dml.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     3363 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/document.rst
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.564568 docx-hitalent-0.8.51/docs/api/enum/
+-rw-r--r--   0 ghoul      (501) staff       (20)      382 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/MsoColorType.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     1270 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/MsoThemeColorIndex.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      791 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdAlignParagraph.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     4567 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdBuiltinStyle.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      804 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdCellVerticalAlignment.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      692 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdColorIndex.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      771 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdLineSpacing.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      339 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdOrientation.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      336 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdRowAlignment.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      519 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdRowHeightRule.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      486 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdSectionStart.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      421 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdStyleType.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      434 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdTabAlignment.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      285 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdTabLeader.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      495 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdTableDirection.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     1334 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/WdUnderline.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      446 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/enum/index.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      565 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/section.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      206 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/settings.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      613 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/shape.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     1174 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/shared.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     1808 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/style.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      621 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/table.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      778 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/api/text.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    10904 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/conf.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.492739 docx-hitalent-0.8.51/docs/dev/
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.565323 docx-hitalent-0.8.51/docs/dev/analysis/
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.574195 docx-hitalent-0.8.51/docs/dev/analysis/features/
+-rw-r--r--   0 ghoul      (501) staff       (20)     7557 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/coreprops.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    11261 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/header.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     2015 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/numbering.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    10642 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/sections.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    13252 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/settings.rst
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.580929 docx-hitalent-0.8.51/docs/dev/analysis/features/shapes/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1935 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/shapes/index.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     9428 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/shapes/picture.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     3459 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/shapes/shapes-inline-size.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     6584 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/shapes/shapes-inline.rst
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.589449 docx-hitalent-0.8.51/docs/dev/analysis/features/styles/
+-rw-r--r--   0 ghoul      (501) staff       (20)     5471 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/styles/character-style.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    12771 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/styles/index.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     8560 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/styles/latent-styles.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     5508 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/styles/paragraph-style.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    13979 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/styles/style.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     8145 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/styles/styles.rst
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.597030 docx-hitalent-0.8.51/docs/dev/analysis/features/table/
+-rw-r--r--   0 ghoul      (501) staff       (20)    20675 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/table/cell-merge.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     9218 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/table/index.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     8041 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/table/table-cell.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     7949 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/table/table-props.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     4150 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/table/table-row.rst
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.607060 docx-hitalent-0.8.51/docs/dev/analysis/features/text/
+-rw-r--r--   0 ghoul      (501) staff       (20)     7581 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/text/breaks.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     9879 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/text/font-color.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     5902 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/text/font-highlight-color.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    18391 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/text/font.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      159 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/text/index.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    16282 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/text/paragraph-format.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     3094 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/text/run-content.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     9567 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/text/tab-stops.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     4247 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/features/text/underline.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)      576 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/index.rst
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.610827 docx-hitalent-0.8.51/docs/dev/analysis/schema/
+-rw-r--r--   0 ghoul      (501) staff       (20)     7226 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/schema/ct_body.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     4659 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/schema/ct_document.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     6406 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/dev/analysis/schema/ct_p.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     3824 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/index.rst
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.625578 docx-hitalent-0.8.51/docs/user/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1287 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/user/api-concepts.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     3635 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/user/documents.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     6897 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/user/hdrftr.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     1031 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/user/install.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    11875 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/user/quickstart.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     3859 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/user/sections.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)     1477 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/user/shapes.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    12392 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/user/styles-understanding.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    13587 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/user/styles-using.rst
+-rw-r--r--   0 ghoul      (501) staff       (20)    14125 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docs/user/text.rst
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.647128 docx-hitalent-0.8.51/docx/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1480 2023-07-17 03:15:18.000000 docx-hitalent-0.8.51/docx/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1242 2021-12-29 08:23:13.000000 docx-hitalent-0.8.51/docx/api.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2872 2022-01-22 07:43:55.000000 docx-hitalent-0.8.51/docx/blkcntnr.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1043 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/compat.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.651256 docx-hitalent-0.8.51/docx/dml/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/dml/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3978 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/dml/color.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     7497 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/document.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.662545 docx-hitalent-0.8.51/docx/enum/
+-rw-r--r--   0 ghoul      (501) staff       (20)      343 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/enum/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    11042 2022-10-08 03:28:45.000000 docx-hitalent-0.8.51/docx/enum/base.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3533 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/enum/dml.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2666 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/enum/section.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      475 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/enum/shape.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    12189 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/enum/style.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3929 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/enum/table.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    10810 2021-12-27 05:07:08.000000 docx-hitalent-0.8.51/docx/enum/text.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      503 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/exceptions.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.679228 docx-hitalent-0.8.51/docx/image/
+-rw-r--r--   0 ghoul      (501) staff       (20)      754 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/image/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1512 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/image/bmp.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3471 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/image/constants.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      432 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/image/exceptions.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1260 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/image/gif.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3286 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/image/helpers.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     8029 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/image/image.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    16099 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/image/jpeg.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     8789 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/image/png.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    11140 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/image/tiff.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.700703 docx-hitalent-0.8.51/docx/opc/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1327 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/compat.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    20515 2021-12-29 08:23:13.000000 docx-hitalent-0.8.51/docx/opc/constants.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3246 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/coreprops.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      302 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/exceptions.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     8540 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/oxml.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     8510 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/package.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3880 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/packuri.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     8157 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/part.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.703323 docx-hitalent-0.8.51/docx/opc/parts/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/parts/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1664 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/parts/coreprops.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4370 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/phys_pkg.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    10311 2022-10-20 09:06:50.000000 docx-hitalent-0.8.51/docx/opc/pkgreader.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4524 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/pkgwriter.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5385 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/rel.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1453 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/shared.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      716 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/opc/spec.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.721155 docx-hitalent-0.8.51/docx/oxml/
+-rw-r--r--   0 ghoul      (501) staff       (20)    11906 2022-10-09 09:15:37.000000 docx-hitalent-0.8.51/docx/oxml/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    10278 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/oxml/coreprops.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2513 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/oxml/document.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      290 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/oxml/exceptions.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3969 2022-01-13 09:30:22.000000 docx-hitalent-0.8.51/docx/oxml/ns.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5265 2022-10-08 02:41:55.000000 docx-hitalent-0.8.51/docx/oxml/numbering.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    11463 2022-10-21 09:12:28.000000 docx-hitalent-0.8.51/docx/oxml/section.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3491 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/oxml/settings.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    12070 2022-10-08 02:37:34.000000 docx-hitalent-0.8.51/docx/oxml/shape.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1623 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/oxml/shared.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    12305 2023-07-17 05:08:40.000000 docx-hitalent-0.8.51/docx/oxml/simpletypes.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    11125 2022-01-21 07:38:50.000000 docx-hitalent-0.8.51/docx/oxml/styles.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    30495 2022-10-09 09:19:04.000000 docx-hitalent-0.8.51/docx/oxml/table.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.731450 docx-hitalent-0.8.51/docx/oxml/text/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/oxml/text/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    10114 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/oxml/text/font.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2247 2022-01-22 07:41:15.000000 docx-hitalent-0.8.51/docx/oxml/text/paragraph.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    10767 2022-01-21 09:09:02.000000 docx-hitalent-0.8.51/docx/oxml/text/parfmt.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5088 2022-01-22 07:07:07.000000 docx-hitalent-0.8.51/docx/oxml/text/run.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    10050 2022-10-11 08:10:53.000000 docx-hitalent-0.8.51/docx/oxml/textbox.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    24645 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/oxml/xmlchemy.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3868 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/package.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.741702 docx-hitalent-0.8.51/docx/parts/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/parts/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5355 2022-08-05 07:07:54.000000 docx-hitalent-0.8.51/docx/parts/document.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1717 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/parts/hdrftr.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2668 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/parts/image.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2788 2022-10-08 01:57:26.000000 docx-hitalent-0.8.51/docx/parts/numbering.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1465 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/parts/settings.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3238 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/parts/story.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1428 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/parts/styles.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2315 2022-09-30 06:39:26.000000 docx-hitalent-0.8.51/docx/picture.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1215 2022-10-11 09:47:10.000000 docx-hitalent-0.8.51/docx/rect.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    16201 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/section.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      780 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/settings.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2811 2022-01-13 09:33:30.000000 docx-hitalent-0.8.51/docx/shape.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     6836 2022-09-22 06:55:10.000000 docx-hitalent-0.8.51/docx/shared.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.749902 docx-hitalent-0.8.51/docx/styles/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1500 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/styles/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     7549 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/styles/latent.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     7987 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/styles/style.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5637 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/styles/styles.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    18479 2022-11-22 02:10:56.000000 docx-hitalent-0.8.51/docx/table.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.756736 docx-hitalent-0.8.51/docx/templates/
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.758030 docx-hitalent-0.8.51/docx/templates/default-docx-template/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1782 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/[Content_Types].xml
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.759141 docx-hitalent-0.8.51/docx/templates/default-docx-template/_rels/
+-rw-r--r--   0 ghoul      (501) staff       (20)      748 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/_rels/.rels
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.762456 docx-hitalent-0.8.51/docx/templates/default-docx-template/customXml/
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.764020 docx-hitalent-0.8.51/docx/templates/default-docx-template/customXml/_rels/
+-rw-r--r--   0 ghoul      (501) staff       (20)      300 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/customXml/_rels/item1.xml.rels
+-rw-r--r--   0 ghoul      (501) staff       (20)      262 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/customXml/item1.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)      354 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/customXml/itemProps1.xml
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.767311 docx-hitalent-0.8.51/docx/templates/default-docx-template/docProps/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1132 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/docProps/app.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)      753 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/docProps/core.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)     8324 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/docProps/thumbnail.jpeg
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.787795 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.788454 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/_rels/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1253 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/_rels/document.xml.rels
+-rw-r--r--   0 ghoul      (501) staff       (20)     1594 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/document.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)     2811 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/fontTable.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)     6747 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/numbering.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)     2749 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/settings.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)   438677 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/styles.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)   438131 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/stylesWithEffects.xml
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.790030 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/theme/
+-rw-r--r--   0 ghoul      (501) staff       (20)    10939 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/theme/theme1.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)      438 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-docx-template/word/webSettings.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)     1395 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-footer.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)     1395 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-header.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)     1640 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-settings.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)    15823 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default-styles.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)    38116 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/templates/default.docx
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.795825 docx-hitalent-0.8.51/docx/text/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/text/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    12072 2022-01-21 09:41:56.000000 docx-hitalent-0.8.51/docx/text/font.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5737 2022-10-08 01:51:39.000000 docx-hitalent-0.8.51/docx/text/paragraph.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    10833 2022-09-22 07:58:07.000000 docx-hitalent-0.8.51/docx/text/parfmt.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     8035 2022-11-22 03:01:09.000000 docx-hitalent-0.8.51/docx/text/run.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4183 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/docx/text/tabstops.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2070 2022-11-22 07:19:35.000000 docx-hitalent-0.8.51/docx/textbox.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.799188 docx-hitalent-0.8.51/docx_hitalent.egg-info/
+-rw-r--r--   0 ghoul      (501) staff       (20)    11557 2023-07-17 05:08:45.000000 docx-hitalent-0.8.51/docx_hitalent.egg-info/PKG-INFO
+-rw-r--r--   0 ghoul      (501) staff       (20)    14393 2023-07-17 05:08:45.000000 docx-hitalent-0.8.51/docx_hitalent.egg-info/SOURCES.txt
+-rw-r--r--   0 ghoul      (501) staff       (20)        1 2023-07-17 05:08:45.000000 docx-hitalent-0.8.51/docx_hitalent.egg-info/dependency_links.txt
+-rw-r--r--   0 ghoul      (501) staff       (20)        1 2021-12-27 02:59:56.000000 docx-hitalent-0.8.51/docx_hitalent.egg-info/not-zip-safe
+-rw-r--r--   0 ghoul      (501) staff       (20)       12 2023-07-17 05:08:45.000000 docx-hitalent-0.8.51/docx_hitalent.egg-info/requires.txt
+-rw-r--r--   0 ghoul      (501) staff       (20)        5 2023-07-17 05:08:45.000000 docx-hitalent-0.8.51/docx_hitalent.egg-info/top_level.txt
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.843046 docx-hitalent-0.8.51/features/
+-rw-r--r--   0 ghoul      (501) staff       (20)      476 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/api-open-document.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      407 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/blk-add-paragraph.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      378 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/blk-add-table.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      428 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/cel-add-table.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      343 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/cel-text.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      981 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/doc-access-collections.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      395 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/doc-access-sections.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      840 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/doc-add-heading.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      358 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/doc-add-page-break.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      883 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/doc-add-paragraph.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      997 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/doc-add-picture.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1110 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/doc-add-section.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      729 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/doc-add-table.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      892 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/doc-coreprops.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1398 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/doc-settings.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      598 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/doc-styles.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      310 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/environment.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3116 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/hdr-header-footer.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1499 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/img-characterize-image.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      402 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/num-access-numbering-part.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      312 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/par-access-parfmt.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      527 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/par-add-run.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      632 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/par-alignment-prop.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      405 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/par-clear-paragraph.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      577 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/par-insert-paragraph.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      390 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/par-set-text.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      871 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/par-style-prop.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      312 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/run-access-content.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      269 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/run-access-font.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      467 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/run-add-content.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      804 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/run-add-picture.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1173 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/run-char-style.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      373 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/run-clear-run.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1757 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/run-enum-props.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     5082 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/sct-section.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1070 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/shp-inline-shape-access.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      575 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/shp-inline-shape-size.feature
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.856353 docx-hitalent-0.8.51/features/steps/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1680 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/api.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1266 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/block.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1468 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/cell.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4455 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/coreprops.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     8937 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/document.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     7114 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/font.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5163 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/hdrftr.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      853 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/helpers.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2273 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/image.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      970 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/numbering.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5460 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/paragraph.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     8249 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/parfmt.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     8963 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/section.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1942 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/settings.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5304 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/shape.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      563 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/shared.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    18220 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/styles.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    15719 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/table.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4670 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/tabstops.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.912115 docx-hitalent-0.8.51/features/steps/test_files/
+-rw-r--r--   0 ghoul      (501) staff       (20)    25142 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/blk-containing-table.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    80603 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/court-exif.jpg
+-rw-r--r--   0 ghoul      (501) staff       (20)    25591 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/doc-access-sections.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    17956 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/doc-add-section.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    11992 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/doc-coreprops.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    21366 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/doc-default.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    11394 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/doc-no-coreprops.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    17711 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/doc-odd-even-hdrs.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    21309 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/doc-word-default-blank.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    15846 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/fnt-color.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    18079 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/hdr-header-footer.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)   355196 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/jfif-300-dpi.jpg
+-rw-r--r--   0 ghoul      (501) staff       (20)   768608 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/jpeg420exif.jpg
+-rw-r--r--   0 ghoul      (501) staff       (20)   263222 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/lena.bmp
+-rw-r--r--   0 ghoul      (501) staff       (20)    72985 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/lena.gif
+-rw-r--r--   0 ghoul      (501) staff       (20)   786572 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/lena.tif
+-rw-r--r--   0 ghoul      (501) staff       (20)   104428 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/lena_std.jpg
+-rw-r--r--   0 ghoul      (501) staff       (20)    64276 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/monty-truth.png
+-rw-r--r--   0 ghoul      (501) staff       (20)   308280 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/mountain.bmp
+-rw-r--r--   0 ghoul      (501) staff       (20)    24334 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/num-having-numbering-part.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    15126 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/par-alignment.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    27969 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/par-known-paragraphs.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    20901 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/par-known-styles.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)     3277 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/python-icon.jpeg
+-rw-r--r--   0 ghoul      (501) staff       (20)    26645 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/run-char-style.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    14645 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/run-enumerated-props.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    10409 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/sample.tif
+-rw-r--r--   0 ghoul      (501) staff       (20)    14849 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/sct-first-page-hdrftr.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    28168 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/sct-section-props.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    10760 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/set-no-settings-part.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)   122610 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/shp-inline-shape-access.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    12195 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/sty-behav-props.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)     8358 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/sty-having-no-styles-part.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    21573 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/sty-having-styles-part.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    13560 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/sty-known-styles.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    13170 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/tab-stops.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    25129 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/tbl-2x2-table.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    36051 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/tbl-cell-access.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    13654 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/tbl-col-props.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    50294 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/tbl-having-applied-style.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    32010 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/tbl-having-tables.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    16017 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/tbl-on-off-props.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    20178 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/tbl-props.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)   146892 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/test.png
+-rw-r--r--   0 ghoul      (501) staff       (20)    12859 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/txt-font-highlight-color.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)    37924 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/test_files/txt-font-props.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)     8848 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/steps/text.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      463 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/sty-access-font.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      568 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/sty-access-latent-styles.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      488 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/sty-access-parfmt.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      767 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/sty-add-style.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      352 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/sty-delete-style.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      654 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/sty-latent-add-del.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     4102 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/sty-latent-props.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     5464 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/sty-style-props.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1264 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/tab-access-tabs.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1877 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/tab-tabstop-props.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      594 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/tbl-add-row-or-col.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1523 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/tbl-cell-access.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1861 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/tbl-cell-props.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1062 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/tbl-col-props.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      944 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/tbl-item-access.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     2294 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/tbl-merge-cells.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     2907 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/tbl-props.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1665 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/tbl-row-props.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     1169 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/tbl-style.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)      645 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/txt-add-break.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     2279 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/txt-font-color.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     8120 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/txt-font-props.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)     7648 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/features/txt-parfmt-props.feature
+-rw-r--r--   0 ghoul      (501) staff       (20)       38 2023-07-17 05:08:46.003749 docx-hitalent-0.8.51/setup.cfg
+-rw-r--r--   0 ghoul      (501) staff       (20)     2389 2021-12-27 03:04:55.000000 docx-hitalent-0.8.51/setup.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.920906 docx-hitalent-0.8.51/tests/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/__init__.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.922613 docx-hitalent-0.8.51/tests/dml/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/dml/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5411 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/dml/test_color.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.928162 docx-hitalent-0.8.51/tests/image/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/image/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1211 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/image/test_bmp.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1061 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/image/test_gif.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1659 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/image/test_helpers.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    12157 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/image/test_image.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    21667 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/image/test_jpeg.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    15009 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/image/test_png.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    14805 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/image/test_tiff.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.934455 docx-hitalent-0.8.51/tests/opc/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/__init__.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.935288 docx-hitalent-0.8.51/tests/opc/parts/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/parts/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1991 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/parts/test_coreprops.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     7910 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/test_coreprops.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4913 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/test_oxml.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    16878 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/test_package.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3203 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/test_packuri.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    16641 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/test_part.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     6560 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/test_phys_pkg.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    18670 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/test_pkgreader.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     7099 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/test_pkgwriter.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     9759 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/test_rel.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.936727 docx-hitalent-0.8.51/tests/opc/unitdata/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/unitdata/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     8804 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/unitdata/rels.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      859 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/opc/unitdata/types.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.940995 docx-hitalent-0.8.51/tests/oxml/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/__init__.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.942503 docx-hitalent-0.8.51/tests/oxml/parts/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/parts/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1543 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/parts/test_document.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.943439 docx-hitalent-0.8.51/tests/oxml/parts/unitdata/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/parts/unitdata/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      409 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/parts/unitdata/document.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4237 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/test__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1750 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/test_ns.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1284 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/test_styles.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    12720 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/test_table.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    28182 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/test_xmlchemy.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.944557 docx-hitalent-0.8.51/tests/oxml/text/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/text/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      998 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/text/test_run.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.949577 docx-hitalent-0.8.51/tests/oxml/unitdata/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/unitdata/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4060 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/unitdata/dml.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      434 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/unitdata/numbering.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      872 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/unitdata/section.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      699 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/unitdata/shared.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      469 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/unitdata/styles.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1444 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/unitdata/table.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3187 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/oxml/unitdata/text.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.955386 docx-hitalent-0.8.51/tests/parts/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/parts/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    12469 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/parts/test_document.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5152 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/parts/test_hdrftr.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4056 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/parts/test_image.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2641 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/parts/test_numbering.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2688 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/parts/test_settings.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     5429 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/parts/test_story.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1820 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/parts/test_styles.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.958942 docx-hitalent-0.8.51/tests/styles/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/styles/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    13842 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/styles/test_latent.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    20568 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/styles/test_style.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    14432 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/styles/test_styles.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2401 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_api.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4824 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_blkcntnr.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    13332 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_document.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     3055 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_enum.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.982006 docx-hitalent-0.8.51/tests/test_files/
+-rw-r--r--   0 ghoul      (501) staff       (20)   146892 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/150-dpi.png
+-rw-r--r--   0 ghoul      (501) staff       (20)   125824 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/300-dpi.TIF
+-rw-r--r--   0 ghoul      (501) staff       (20)   355196 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/300-dpi.jpg
+-rw-r--r--   0 ghoul      (501) staff       (20)    39921 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/300-dpi.png
+-rw-r--r--   0 ghoul      (501) staff       (20)     9454 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/72-dpi.tiff
+-rw-r--r--   0 ghoul      (501) staff       (20)     1526 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/CVS_LOGO.WMF
+-rw-r--r--   0 ghoul      (501) staff       (20)   768608 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/exif-420-dpi.jpg
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.982833 docx-hitalent-0.8.51/tests/test_files/expanded_docx/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1738 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/[Content_Types].xml
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.983573 docx-hitalent-0.8.51/tests/test_files/expanded_docx/_rels/
+-rw-r--r--   0 ghoul      (501) staff       (20)      734 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/_rels/.rels
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.984959 docx-hitalent-0.8.51/tests/test_files/expanded_docx/customXml/
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.985685 docx-hitalent-0.8.51/tests/test_files/expanded_docx/customXml/_rels/
+-rw-r--r--   0 ghoul      (501) staff       (20)      295 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/customXml/_rels/item1.xml.rels
+-rw-r--r--   0 ghoul      (501) staff       (20)      217 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/customXml/item1.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)      340 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/customXml/itemProps1.xml
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.987566 docx-hitalent-0.8.51/tests/test_files/expanded_docx/docProps/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1036 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/docProps/app.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)      802 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/docProps/core.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)    13032 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/docProps/thumbnail.jpeg
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.992146 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.992771 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/_rels/
+-rw-r--r--   0 ghoul      (501) staff       (20)     1227 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/_rels/document.xml.rels
+-rw-r--r--   0 ghoul      (501) staff       (20)     1819 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/document.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)     2566 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/fontTable.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)     5513 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/numbering.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)     2520 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/settings.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)    26715 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/styles.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)    27581 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/stylesWithEffects.xml
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.993369 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/theme/
+-rw-r--r--   0 ghoul      (501) staff       (20)     7642 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/theme/theme1.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)      430 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/webSettings.xml
+-rw-r--r--   0 ghoul      (501) staff       (20)   132875 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/having-images.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)     7958 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/jfif-iguana.jpg
+-rw-r--r--   0 ghoul      (501) staff       (20)    10409 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/little-endian.tif
+-rw-r--r--   0 ghoul      (501) staff       (20)    64276 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/monty-truth.png
+-rw-r--r--   0 ghoul      (501) staff       (20)     3277 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/python-icon.jpeg
+-rw-r--r--   0 ghoul      (501) staff       (20)     2036 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/python-icon.png
+-rw-r--r--   0 ghoul      (501) staff       (20)     6111 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/python-powered.png
+-rw-r--r--   0 ghoul      (501) staff       (20)    45210 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/python.bmp
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.996090 docx-hitalent-0.8.51/tests/test_files/snippets/
+-rw-r--r--   0 ghoul      (501) staff       (20)     2949 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/snippets/add-row-col.txt
+-rw-r--r--   0 ghoul      (501) staff       (20)     1110 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/snippets/inline.txt
+-rw-r--r--   0 ghoul      (501) staff       (20)     1756 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/snippets/new-tbl.txt
+-rw-r--r--   0 ghoul      (501) staff       (20)     4595 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/snippets/tbl-cells.txt
+-rw-r--r--   0 ghoul      (501) staff       (20)    33273 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/sonic.gif
+-rw-r--r--   0 ghoul      (501) staff       (20)    31773 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_files/test.docx
+-rw-r--r--   0 ghoul      (501) staff       (20)     5418 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_package.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    29075 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_section.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     2279 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_settings.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     6591 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_shape.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4398 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_shared.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    34086 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/test_table.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:45.999862 docx-hitalent-0.8.51/tests/text/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/text/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    17045 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/text/test_font.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    11267 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/text/test_paragraph.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    19399 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/text/test_parfmt.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    13565 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/text/test_run.py
+-rw-r--r--   0 ghoul      (501) staff       (20)    11016 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/text/test_tabstops.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4329 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/unitdata.py
+drwxr-xr-x   0 ghoul      (501) staff       (20)        0 2023-07-17 05:08:46.002384 docx-hitalent-0.8.51/tests/unitutil/
+-rw-r--r--   0 ghoul      (501) staff       (20)        0 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/unitutil/__init__.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     8334 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/unitutil/cxml.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     1600 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/unitutil/file.py
+-rw-r--r--   0 ghoul      (501) staff       (20)     4281 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tests/unitutil/mock.py
+-rw-r--r--   0 ghoul      (501) staff       (20)      667 2021-12-27 02:12:49.000000 docx-hitalent-0.8.51/tox.ini
```

### Comparing `docx-hitalent-0.8.50/HISTORY.rst` & `docx-hitalent-0.8.51/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 .. :changelog:
 
 Release History
 ---------------
+0.8.51 (2023-07-17)
++++++++++++++++++++
+
+- Fixed HEX color value "ff"
+
+
 0.8.50 (2022-11-22)
 +++++++++++++++++++
 
 - Run add ``compare_other_properties`` function
 
 0.8.49 (2022-10-21)
 +++++++++++++++++++
```

### Comparing `docx-hitalent-0.8.50/LICENSE` & `docx-hitalent-0.8.51/LICENSE`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/PKG-INFO` & `docx-hitalent-0.8.51/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx-hitalent
-Version: 0.8.50
+Version: 0.8.51
 Summary: Create and update Microsoft Word .docx files.
 Home-page: https://github.com/HiTalentAlgorithms/python-docx
 Author: Steve Canny + Guo hao Li
 Author-email: ghoullh@gmail.com
 License: The MIT License (MIT)
         Copyright (c) 2013 Steve Canny, https://github.com/scanny
         
@@ -23,15 +23,14 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Keywords: docx office openxml word
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -56,14 +55,20 @@
    https://python-docx.readthedocs.org/en/latest/
 
 
 .. :changelog:
 
 Release History
 ---------------
+0.8.51 (2023-07-17)
++++++++++++++++++++
+
+- Fixed HEX color value "ff"
+
+
 0.8.50 (2022-11-22)
 +++++++++++++++++++
 
 - Run add ``compare_other_properties`` function
 
 0.8.49 (2022-10-21)
 +++++++++++++++++++
@@ -502,9 +507,7 @@
 0.3.0dev1 (2013-12-14)
 ++++++++++++++++++++++
 
 - Round-trip .docx file, preserving all parts and relationships
 - Load default "template" .docx on open with no filename
 - Open from stream and save to stream (file-like object)
 - Add paragraph at and of document
-
-
```

### Comparing `docx-hitalent-0.8.50/docs/Makefile` & `docx-hitalent-0.8.51/docs/Makefile`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/_static/img/example-docx-01.png` & `docx-hitalent-0.8.51/docs/_static/img/example-docx-01.png`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/_static/img/hdrftr-01.png` & `docx-hitalent-0.8.51/docs/_static/img/hdrftr-01.png`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/_static/img/hdrftr-02.png` & `docx-hitalent-0.8.51/docs/_static/img/hdrftr-02.png`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/_themes/armstrong/LICENSE` & `docx-hitalent-0.8.51/docs/_themes/armstrong/LICENSE`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/_themes/armstrong/layout.html` & `docx-hitalent-0.8.51/docs/_themes/armstrong/layout.html`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/_themes/armstrong/rtd-themes.conf` & `docx-hitalent-0.8.51/docs/_themes/armstrong/rtd-themes.conf`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/_themes/armstrong/static/rtd.css_t` & `docx-hitalent-0.8.51/docs/_themes/armstrong/static/rtd.css_t`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/_themes/armstrong/theme.conf` & `docx-hitalent-0.8.51/docs/_themes/armstrong/theme.conf`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/_themes/armstrong/theme.conf.orig` & `docx-hitalent-0.8.51/docs/_themes/armstrong/theme.conf.orig`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/document.rst` & `docx-hitalent-0.8.51/docs/api/document.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/enum/MsoThemeColorIndex.rst` & `docx-hitalent-0.8.51/docs/api/enum/MsoThemeColorIndex.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/enum/WdAlignParagraph.rst` & `docx-hitalent-0.8.51/docs/api/enum/WdAlignParagraph.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/enum/WdBuiltinStyle.rst` & `docx-hitalent-0.8.51/docs/api/enum/WdBuiltinStyle.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/enum/WdCellVerticalAlignment.rst` & `docx-hitalent-0.8.51/docs/api/enum/WdCellVerticalAlignment.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/enum/WdColorIndex.rst` & `docx-hitalent-0.8.51/docs/api/enum/WdColorIndex.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/enum/WdLineSpacing.rst` & `docx-hitalent-0.8.51/docs/api/enum/WdLineSpacing.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/enum/WdRowHeightRule.rst` & `docx-hitalent-0.8.51/docs/api/enum/WdRowHeightRule.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/enum/WdUnderline.rst` & `docx-hitalent-0.8.51/docs/api/enum/WdUnderline.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/section.rst` & `docx-hitalent-0.8.51/docs/api/section.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/shape.rst` & `docx-hitalent-0.8.51/docs/api/shape.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/shared.rst` & `docx-hitalent-0.8.51/docs/api/shared.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/style.rst` & `docx-hitalent-0.8.51/docs/api/style.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/table.rst` & `docx-hitalent-0.8.51/docs/api/table.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/api/text.rst` & `docx-hitalent-0.8.51/docs/api/text.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/conf.py` & `docx-hitalent-0.8.51/docs/conf.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/coreprops.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/coreprops.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/header.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/header.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/numbering.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/numbering.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/sections.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/sections.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/settings.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/settings.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/shapes/index.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/shapes/index.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/shapes/picture.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/shapes/picture.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/shapes/shapes-inline-size.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/shapes/shapes-inline-size.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/shapes/shapes-inline.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/shapes/shapes-inline.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/styles/character-style.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/styles/character-style.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/styles/index.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/styles/index.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/styles/latent-styles.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/styles/latent-styles.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/styles/paragraph-style.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/styles/paragraph-style.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/styles/style.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/styles/style.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/styles/styles.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/styles/styles.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/table/cell-merge.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/table/cell-merge.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/table/index.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/table/index.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/table/table-cell.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/table/table-cell.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/table/table-props.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/table/table-props.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/table/table-row.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/table/table-row.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/text/breaks.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/text/breaks.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/text/font-color.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/text/font-color.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/text/font-highlight-color.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/text/font-highlight-color.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/text/font.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/text/font.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/text/paragraph-format.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/text/paragraph-format.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/text/run-content.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/text/run-content.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/text/tab-stops.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/text/tab-stops.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/features/text/underline.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/features/text/underline.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/index.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/index.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/schema/ct_body.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/schema/ct_body.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/schema/ct_document.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/schema/ct_document.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/dev/analysis/schema/ct_p.rst` & `docx-hitalent-0.8.51/docs/dev/analysis/schema/ct_p.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/index.rst` & `docx-hitalent-0.8.51/docs/index.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/user/api-concepts.rst` & `docx-hitalent-0.8.51/docs/user/api-concepts.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/user/documents.rst` & `docx-hitalent-0.8.51/docs/user/documents.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/user/hdrftr.rst` & `docx-hitalent-0.8.51/docs/user/hdrftr.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/user/install.rst` & `docx-hitalent-0.8.51/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/user/quickstart.rst` & `docx-hitalent-0.8.51/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/user/sections.rst` & `docx-hitalent-0.8.51/docs/user/sections.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/user/shapes.rst` & `docx-hitalent-0.8.51/docs/user/shapes.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/user/styles-understanding.rst` & `docx-hitalent-0.8.51/docs/user/styles-understanding.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/user/styles-using.rst` & `docx-hitalent-0.8.51/docs/user/styles-using.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docs/user/text.rst` & `docx-hitalent-0.8.51/docs/user/text.rst`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/__init__.py` & `docx-hitalent-0.8.51/docx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 
 from docx.api import Document  # noqa
 
-__version__ = "0.8.50"
+__version__ = "0.8.51"
 
 
 # register custom Part classes with opc package reader
 
 from docx.opc.constants import CONTENT_TYPE as CT, RELATIONSHIP_TYPE as RT
 from docx.opc.part import PartFactory
 from docx.opc.parts.coreprops import CorePropertiesPart
```

### Comparing `docx-hitalent-0.8.50/docx/api.py` & `docx-hitalent-0.8.51/docx/api.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/blkcntnr.py` & `docx-hitalent-0.8.51/docx/blkcntnr.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/compat.py` & `docx-hitalent-0.8.51/docx/compat.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/dml/color.py` & `docx-hitalent-0.8.51/docx/dml/color.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/document.py` & `docx-hitalent-0.8.51/docx/document.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/enum/base.py` & `docx-hitalent-0.8.51/docx/enum/base.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/enum/dml.py` & `docx-hitalent-0.8.51/docx/enum/dml.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/enum/section.py` & `docx-hitalent-0.8.51/docx/enum/section.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/enum/style.py` & `docx-hitalent-0.8.51/docx/enum/style.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/enum/table.py` & `docx-hitalent-0.8.51/docx/enum/table.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/enum/text.py` & `docx-hitalent-0.8.51/docx/enum/text.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/image/__init__.py` & `docx-hitalent-0.8.51/docx/image/__init__.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/image/bmp.py` & `docx-hitalent-0.8.51/docx/image/bmp.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/image/constants.py` & `docx-hitalent-0.8.51/docx/image/constants.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/image/gif.py` & `docx-hitalent-0.8.51/docx/image/gif.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/image/helpers.py` & `docx-hitalent-0.8.51/docx/image/helpers.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/image/image.py` & `docx-hitalent-0.8.51/docx/image/image.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/image/jpeg.py` & `docx-hitalent-0.8.51/docx/image/jpeg.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/image/png.py` & `docx-hitalent-0.8.51/docx/image/png.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/image/tiff.py` & `docx-hitalent-0.8.51/docx/image/tiff.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/compat.py` & `docx-hitalent-0.8.51/docx/opc/compat.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/constants.py` & `docx-hitalent-0.8.51/docx/opc/constants.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/coreprops.py` & `docx-hitalent-0.8.51/docx/opc/coreprops.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/oxml.py` & `docx-hitalent-0.8.51/docx/opc/oxml.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/package.py` & `docx-hitalent-0.8.51/docx/opc/package.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/packuri.py` & `docx-hitalent-0.8.51/docx/opc/packuri.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/part.py` & `docx-hitalent-0.8.51/docx/opc/part.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/parts/coreprops.py` & `docx-hitalent-0.8.51/docx/opc/parts/coreprops.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/phys_pkg.py` & `docx-hitalent-0.8.51/docx/opc/phys_pkg.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/pkgreader.py` & `docx-hitalent-0.8.51/docx/opc/pkgreader.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/pkgwriter.py` & `docx-hitalent-0.8.51/docx/opc/pkgwriter.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/rel.py` & `docx-hitalent-0.8.51/docx/opc/rel.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/shared.py` & `docx-hitalent-0.8.51/docx/opc/shared.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/opc/spec.py` & `docx-hitalent-0.8.51/docx/opc/spec.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/__init__.py` & `docx-hitalent-0.8.51/docx/oxml/__init__.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/coreprops.py` & `docx-hitalent-0.8.51/docx/oxml/coreprops.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/document.py` & `docx-hitalent-0.8.51/docx/oxml/document.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/ns.py` & `docx-hitalent-0.8.51/docx/oxml/ns.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/numbering.py` & `docx-hitalent-0.8.51/docx/oxml/numbering.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/section.py` & `docx-hitalent-0.8.51/docx/oxml/section.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/settings.py` & `docx-hitalent-0.8.51/docx/oxml/settings.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/shape.py` & `docx-hitalent-0.8.51/docx/oxml/shape.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/shared.py` & `docx-hitalent-0.8.51/docx/oxml/shared.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/simpletypes.py` & `docx-hitalent-0.8.51/docx/oxml/simpletypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -239,14 +239,18 @@
 
 class ST_HexColor(BaseStringType):
 
     @classmethod
     def convert_from_xml(cls, str_value):
         if str_value == 'auto':
             return ST_HexColorAuto.AUTO
+        if str_value == '0':
+            return RGBColor.from_string('000000')
+        if len(str_value) == 2:  # e.g. "ff"
+            return RGBColor.from_string(str_value * 3)
         return RGBColor.from_string(str_value)
 
     @classmethod
     def convert_to_xml(cls, value):
         """
         Keep alpha hex numerals all uppercase just for consistency.
         """
```

### Comparing `docx-hitalent-0.8.50/docx/oxml/styles.py` & `docx-hitalent-0.8.51/docx/oxml/styles.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/table.py` & `docx-hitalent-0.8.51/docx/oxml/table.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/text/font.py` & `docx-hitalent-0.8.51/docx/oxml/text/font.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/text/paragraph.py` & `docx-hitalent-0.8.51/docx/oxml/text/paragraph.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/text/parfmt.py` & `docx-hitalent-0.8.51/docx/oxml/text/parfmt.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/text/run.py` & `docx-hitalent-0.8.51/docx/oxml/text/run.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/textbox.py` & `docx-hitalent-0.8.51/docx/oxml/textbox.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/oxml/xmlchemy.py` & `docx-hitalent-0.8.51/docx/oxml/xmlchemy.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/package.py` & `docx-hitalent-0.8.51/docx/package.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/parts/document.py` & `docx-hitalent-0.8.51/docx/parts/document.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/parts/hdrftr.py` & `docx-hitalent-0.8.51/docx/parts/hdrftr.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/parts/image.py` & `docx-hitalent-0.8.51/docx/parts/image.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/parts/numbering.py` & `docx-hitalent-0.8.51/docx/parts/numbering.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/parts/settings.py` & `docx-hitalent-0.8.51/docx/parts/settings.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/parts/story.py` & `docx-hitalent-0.8.51/docx/parts/story.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/parts/styles.py` & `docx-hitalent-0.8.51/docx/parts/styles.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/picture.py` & `docx-hitalent-0.8.51/docx/picture.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/rect.py` & `docx-hitalent-0.8.51/docx/rect.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/section.py` & `docx-hitalent-0.8.51/docx/section.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/settings.py` & `docx-hitalent-0.8.51/docx/settings.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/shape.py` & `docx-hitalent-0.8.51/docx/shape.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/shared.py` & `docx-hitalent-0.8.51/docx/shared.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/styles/__init__.py` & `docx-hitalent-0.8.51/docx/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/styles/latent.py` & `docx-hitalent-0.8.51/docx/styles/latent.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/styles/style.py` & `docx-hitalent-0.8.51/docx/styles/style.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/styles/styles.py` & `docx-hitalent-0.8.51/docx/styles/styles.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/table.py` & `docx-hitalent-0.8.51/docx/table.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/[Content_Types].xml` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/_rels/.rels` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/_rels/.rels`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/docProps/app.xml` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/docProps/core.xml` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/docProps/thumbnail.jpeg` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/word/_rels/document.xml.rels` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/word/_rels/document.xml.rels`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/word/document.xml` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/word/document.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/word/fontTable.xml` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/word/fontTable.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/word/numbering.xml` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/word/numbering.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/word/settings.xml` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/word/settings.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/word/styles.xml` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/word/styles.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/word/stylesWithEffects.xml` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/word/stylesWithEffects.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-docx-template/word/theme/theme1.xml` & `docx-hitalent-0.8.51/docx/templates/default-docx-template/word/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-footer.xml` & `docx-hitalent-0.8.51/docx/templates/default-footer.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-header.xml` & `docx-hitalent-0.8.51/docx/templates/default-header.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-settings.xml` & `docx-hitalent-0.8.51/docx/templates/default-settings.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default-styles.xml` & `docx-hitalent-0.8.51/docx/templates/default-styles.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/templates/default.docx` & `docx-hitalent-0.8.51/docx/templates/default.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/text/font.py` & `docx-hitalent-0.8.51/docx/text/font.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/text/paragraph.py` & `docx-hitalent-0.8.51/docx/text/paragraph.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/text/parfmt.py` & `docx-hitalent-0.8.51/docx/text/parfmt.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/text/run.py` & `docx-hitalent-0.8.51/docx/text/run.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/text/tabstops.py` & `docx-hitalent-0.8.51/docx/text/tabstops.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx/textbox.py` & `docx-hitalent-0.8.51/docx/textbox.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/docx_hitalent.egg-info/PKG-INFO` & `docx-hitalent-0.8.51/docx_hitalent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx-hitalent
-Version: 0.8.50
+Version: 0.8.51
 Summary: Create and update Microsoft Word .docx files.
 Home-page: https://github.com/HiTalentAlgorithms/python-docx
 Author: Steve Canny + Guo hao Li
 Author-email: ghoullh@gmail.com
 License: The MIT License (MIT)
         Copyright (c) 2013 Steve Canny, https://github.com/scanny
         
@@ -23,15 +23,14 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Keywords: docx office openxml word
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -56,14 +55,20 @@
    https://python-docx.readthedocs.org/en/latest/
 
 
 .. :changelog:
 
 Release History
 ---------------
+0.8.51 (2023-07-17)
++++++++++++++++++++
+
+- Fixed HEX color value "ff"
+
+
 0.8.50 (2022-11-22)
 +++++++++++++++++++
 
 - Run add ``compare_other_properties`` function
 
 0.8.49 (2022-10-21)
 +++++++++++++++++++
@@ -502,9 +507,7 @@
 0.3.0dev1 (2013-12-14)
 ++++++++++++++++++++++
 
 - Round-trip .docx file, preserving all parts and relationships
 - Load default "template" .docx on open with no filename
 - Open from stream and save to stream (file-like object)
 - Add paragraph at and of document
-
-
```

### Comparing `docx-hitalent-0.8.50/docx_hitalent.egg-info/SOURCES.txt` & `docx-hitalent-0.8.51/docx_hitalent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/doc-access-collections.feature` & `docx-hitalent-0.8.51/features/doc-access-collections.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/doc-add-heading.feature` & `docx-hitalent-0.8.51/features/doc-add-heading.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/doc-add-paragraph.feature` & `docx-hitalent-0.8.51/features/doc-add-paragraph.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/doc-add-picture.feature` & `docx-hitalent-0.8.51/features/doc-add-picture.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/doc-add-section.feature` & `docx-hitalent-0.8.51/features/doc-add-section.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/doc-add-table.feature` & `docx-hitalent-0.8.51/features/doc-add-table.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/doc-coreprops.feature` & `docx-hitalent-0.8.51/features/doc-coreprops.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/doc-settings.feature` & `docx-hitalent-0.8.51/features/doc-settings.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/doc-styles.feature` & `docx-hitalent-0.8.51/features/doc-styles.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/hdr-header-footer.feature` & `docx-hitalent-0.8.51/features/hdr-header-footer.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/img-characterize-image.feature` & `docx-hitalent-0.8.51/features/img-characterize-image.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/par-add-run.feature` & `docx-hitalent-0.8.51/features/par-add-run.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/par-alignment-prop.feature` & `docx-hitalent-0.8.51/features/par-alignment-prop.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/par-insert-paragraph.feature` & `docx-hitalent-0.8.51/features/par-insert-paragraph.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/par-style-prop.feature` & `docx-hitalent-0.8.51/features/par-style-prop.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/run-add-picture.feature` & `docx-hitalent-0.8.51/features/run-add-picture.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/run-char-style.feature` & `docx-hitalent-0.8.51/features/run-char-style.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/run-enum-props.feature` & `docx-hitalent-0.8.51/features/run-enum-props.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/sct-section.feature` & `docx-hitalent-0.8.51/features/sct-section.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/shp-inline-shape-access.feature` & `docx-hitalent-0.8.51/features/shp-inline-shape-access.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/shp-inline-shape-size.feature` & `docx-hitalent-0.8.51/features/shp-inline-shape-size.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/api.py` & `docx-hitalent-0.8.51/features/steps/api.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/block.py` & `docx-hitalent-0.8.51/features/steps/block.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/cell.py` & `docx-hitalent-0.8.51/features/steps/cell.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/coreprops.py` & `docx-hitalent-0.8.51/features/steps/coreprops.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/document.py` & `docx-hitalent-0.8.51/features/steps/document.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/font.py` & `docx-hitalent-0.8.51/features/steps/font.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/hdrftr.py` & `docx-hitalent-0.8.51/features/steps/hdrftr.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/helpers.py` & `docx-hitalent-0.8.51/features/steps/helpers.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/image.py` & `docx-hitalent-0.8.51/features/steps/image.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/numbering.py` & `docx-hitalent-0.8.51/features/steps/numbering.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/paragraph.py` & `docx-hitalent-0.8.51/features/steps/paragraph.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/parfmt.py` & `docx-hitalent-0.8.51/features/steps/parfmt.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/section.py` & `docx-hitalent-0.8.51/features/steps/section.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/settings.py` & `docx-hitalent-0.8.51/features/steps/settings.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/shape.py` & `docx-hitalent-0.8.51/features/steps/shape.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/shared.py` & `docx-hitalent-0.8.51/features/steps/shared.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/styles.py` & `docx-hitalent-0.8.51/features/steps/styles.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/table.py` & `docx-hitalent-0.8.51/features/steps/table.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/tabstops.py` & `docx-hitalent-0.8.51/features/steps/tabstops.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/blk-containing-table.docx` & `docx-hitalent-0.8.51/features/steps/test_files/blk-containing-table.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/court-exif.jpg` & `docx-hitalent-0.8.51/features/steps/test_files/court-exif.jpg`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/doc-access-sections.docx` & `docx-hitalent-0.8.51/features/steps/test_files/doc-access-sections.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/doc-add-section.docx` & `docx-hitalent-0.8.51/features/steps/test_files/doc-add-section.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/doc-coreprops.docx` & `docx-hitalent-0.8.51/features/steps/test_files/doc-coreprops.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/doc-default.docx` & `docx-hitalent-0.8.51/features/steps/test_files/doc-default.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/doc-no-coreprops.docx` & `docx-hitalent-0.8.51/features/steps/test_files/doc-no-coreprops.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/doc-odd-even-hdrs.docx` & `docx-hitalent-0.8.51/features/steps/test_files/doc-odd-even-hdrs.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/doc-word-default-blank.docx` & `docx-hitalent-0.8.51/features/steps/test_files/doc-word-default-blank.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/fnt-color.docx` & `docx-hitalent-0.8.51/features/steps/test_files/fnt-color.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/hdr-header-footer.docx` & `docx-hitalent-0.8.51/features/steps/test_files/hdr-header-footer.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/jfif-300-dpi.jpg` & `docx-hitalent-0.8.51/features/steps/test_files/jfif-300-dpi.jpg`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/jpeg420exif.jpg` & `docx-hitalent-0.8.51/features/steps/test_files/jpeg420exif.jpg`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/lena.bmp` & `docx-hitalent-0.8.51/features/steps/test_files/lena.bmp`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/lena.gif` & `docx-hitalent-0.8.51/features/steps/test_files/lena.gif`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/lena.tif` & `docx-hitalent-0.8.51/features/steps/test_files/lena.tif`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/lena_std.jpg` & `docx-hitalent-0.8.51/features/steps/test_files/lena_std.jpg`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/monty-truth.png` & `docx-hitalent-0.8.51/features/steps/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/mountain.bmp` & `docx-hitalent-0.8.51/features/steps/test_files/mountain.bmp`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/num-having-numbering-part.docx` & `docx-hitalent-0.8.51/features/steps/test_files/num-having-numbering-part.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/par-alignment.docx` & `docx-hitalent-0.8.51/features/steps/test_files/par-alignment.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/par-known-paragraphs.docx` & `docx-hitalent-0.8.51/features/steps/test_files/par-known-paragraphs.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/par-known-styles.docx` & `docx-hitalent-0.8.51/features/steps/test_files/par-known-styles.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/python-icon.jpeg` & `docx-hitalent-0.8.51/features/steps/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/run-char-style.docx` & `docx-hitalent-0.8.51/features/steps/test_files/run-char-style.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/run-enumerated-props.docx` & `docx-hitalent-0.8.51/features/steps/test_files/run-enumerated-props.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/sample.tif` & `docx-hitalent-0.8.51/features/steps/test_files/sample.tif`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/sct-first-page-hdrftr.docx` & `docx-hitalent-0.8.51/features/steps/test_files/sct-first-page-hdrftr.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/sct-section-props.docx` & `docx-hitalent-0.8.51/features/steps/test_files/sct-section-props.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/set-no-settings-part.docx` & `docx-hitalent-0.8.51/features/steps/test_files/set-no-settings-part.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/shp-inline-shape-access.docx` & `docx-hitalent-0.8.51/features/steps/test_files/shp-inline-shape-access.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/sty-behav-props.docx` & `docx-hitalent-0.8.51/features/steps/test_files/sty-behav-props.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/sty-having-no-styles-part.docx` & `docx-hitalent-0.8.51/features/steps/test_files/sty-having-no-styles-part.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/sty-having-styles-part.docx` & `docx-hitalent-0.8.51/features/steps/test_files/sty-having-styles-part.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/sty-known-styles.docx` & `docx-hitalent-0.8.51/features/steps/test_files/sty-known-styles.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/tab-stops.docx` & `docx-hitalent-0.8.51/features/steps/test_files/tab-stops.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/tbl-2x2-table.docx` & `docx-hitalent-0.8.51/features/steps/test_files/tbl-2x2-table.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/tbl-cell-access.docx` & `docx-hitalent-0.8.51/features/steps/test_files/tbl-cell-access.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/tbl-col-props.docx` & `docx-hitalent-0.8.51/features/steps/test_files/tbl-col-props.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/tbl-having-applied-style.docx` & `docx-hitalent-0.8.51/features/steps/test_files/tbl-having-applied-style.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/tbl-having-tables.docx` & `docx-hitalent-0.8.51/features/steps/test_files/tbl-having-tables.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/tbl-on-off-props.docx` & `docx-hitalent-0.8.51/features/steps/test_files/tbl-on-off-props.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/tbl-props.docx` & `docx-hitalent-0.8.51/features/steps/test_files/tbl-props.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/test.png` & `docx-hitalent-0.8.51/features/steps/test_files/test.png`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/txt-font-highlight-color.docx` & `docx-hitalent-0.8.51/features/steps/test_files/txt-font-highlight-color.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/test_files/txt-font-props.docx` & `docx-hitalent-0.8.51/features/steps/test_files/txt-font-props.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/steps/text.py` & `docx-hitalent-0.8.51/features/steps/text.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/sty-access-latent-styles.feature` & `docx-hitalent-0.8.51/features/sty-access-latent-styles.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/sty-add-style.feature` & `docx-hitalent-0.8.51/features/sty-add-style.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/sty-latent-add-del.feature` & `docx-hitalent-0.8.51/features/sty-latent-add-del.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/sty-latent-props.feature` & `docx-hitalent-0.8.51/features/sty-latent-props.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/sty-style-props.feature` & `docx-hitalent-0.8.51/features/sty-style-props.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/tab-access-tabs.feature` & `docx-hitalent-0.8.51/features/tab-access-tabs.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/tab-tabstop-props.feature` & `docx-hitalent-0.8.51/features/tab-tabstop-props.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/tbl-add-row-or-col.feature` & `docx-hitalent-0.8.51/features/tbl-add-row-or-col.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/tbl-cell-access.feature` & `docx-hitalent-0.8.51/features/tbl-cell-access.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/tbl-cell-props.feature` & `docx-hitalent-0.8.51/features/tbl-cell-props.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/tbl-col-props.feature` & `docx-hitalent-0.8.51/features/tbl-col-props.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/tbl-item-access.feature` & `docx-hitalent-0.8.51/features/tbl-item-access.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/tbl-merge-cells.feature` & `docx-hitalent-0.8.51/features/tbl-merge-cells.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/tbl-props.feature` & `docx-hitalent-0.8.51/features/tbl-props.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/tbl-row-props.feature` & `docx-hitalent-0.8.51/features/tbl-row-props.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/tbl-style.feature` & `docx-hitalent-0.8.51/features/tbl-style.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/txt-add-break.feature` & `docx-hitalent-0.8.51/features/txt-add-break.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/txt-font-color.feature` & `docx-hitalent-0.8.51/features/txt-font-color.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/txt-font-props.feature` & `docx-hitalent-0.8.51/features/txt-font-props.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/features/txt-parfmt-props.feature` & `docx-hitalent-0.8.51/features/txt-parfmt-props.feature`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/setup.py` & `docx-hitalent-0.8.51/setup.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/dml/test_color.py` & `docx-hitalent-0.8.51/tests/dml/test_color.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/image/test_bmp.py` & `docx-hitalent-0.8.51/tests/image/test_bmp.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/image/test_gif.py` & `docx-hitalent-0.8.51/tests/image/test_gif.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/image/test_helpers.py` & `docx-hitalent-0.8.51/tests/image/test_helpers.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/image/test_image.py` & `docx-hitalent-0.8.51/tests/image/test_image.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/image/test_jpeg.py` & `docx-hitalent-0.8.51/tests/image/test_jpeg.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/image/test_png.py` & `docx-hitalent-0.8.51/tests/image/test_png.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/image/test_tiff.py` & `docx-hitalent-0.8.51/tests/image/test_tiff.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/parts/test_coreprops.py` & `docx-hitalent-0.8.51/tests/opc/parts/test_coreprops.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/test_coreprops.py` & `docx-hitalent-0.8.51/tests/opc/test_coreprops.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/test_oxml.py` & `docx-hitalent-0.8.51/tests/opc/test_oxml.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/test_package.py` & `docx-hitalent-0.8.51/tests/opc/test_package.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/test_packuri.py` & `docx-hitalent-0.8.51/tests/opc/test_packuri.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/test_part.py` & `docx-hitalent-0.8.51/tests/opc/test_part.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/test_phys_pkg.py` & `docx-hitalent-0.8.51/tests/opc/test_phys_pkg.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/test_pkgreader.py` & `docx-hitalent-0.8.51/tests/opc/test_pkgreader.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/test_pkgwriter.py` & `docx-hitalent-0.8.51/tests/opc/test_pkgwriter.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/test_rel.py` & `docx-hitalent-0.8.51/tests/opc/test_rel.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/unitdata/rels.py` & `docx-hitalent-0.8.51/tests/opc/unitdata/rels.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/opc/unitdata/types.py` & `docx-hitalent-0.8.51/tests/opc/unitdata/types.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/parts/test_document.py` & `docx-hitalent-0.8.51/tests/oxml/parts/test_document.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/test__init__.py` & `docx-hitalent-0.8.51/tests/oxml/test__init__.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/test_ns.py` & `docx-hitalent-0.8.51/tests/oxml/test_ns.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/test_styles.py` & `docx-hitalent-0.8.51/tests/oxml/test_styles.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/test_table.py` & `docx-hitalent-0.8.51/tests/oxml/test_table.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/test_xmlchemy.py` & `docx-hitalent-0.8.51/tests/oxml/test_xmlchemy.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/text/test_run.py` & `docx-hitalent-0.8.51/tests/oxml/text/test_run.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/unitdata/dml.py` & `docx-hitalent-0.8.51/tests/oxml/unitdata/dml.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/unitdata/section.py` & `docx-hitalent-0.8.51/tests/oxml/unitdata/section.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/unitdata/shared.py` & `docx-hitalent-0.8.51/tests/oxml/unitdata/shared.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/unitdata/table.py` & `docx-hitalent-0.8.51/tests/oxml/unitdata/table.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/oxml/unitdata/text.py` & `docx-hitalent-0.8.51/tests/oxml/unitdata/text.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/parts/test_document.py` & `docx-hitalent-0.8.51/tests/parts/test_document.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/parts/test_hdrftr.py` & `docx-hitalent-0.8.51/tests/parts/test_hdrftr.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/parts/test_image.py` & `docx-hitalent-0.8.51/tests/parts/test_image.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/parts/test_numbering.py` & `docx-hitalent-0.8.51/tests/parts/test_numbering.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/parts/test_settings.py` & `docx-hitalent-0.8.51/tests/parts/test_settings.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/parts/test_story.py` & `docx-hitalent-0.8.51/tests/parts/test_story.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/parts/test_styles.py` & `docx-hitalent-0.8.51/tests/parts/test_styles.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/styles/test_latent.py` & `docx-hitalent-0.8.51/tests/styles/test_latent.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/styles/test_style.py` & `docx-hitalent-0.8.51/tests/styles/test_style.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/styles/test_styles.py` & `docx-hitalent-0.8.51/tests/styles/test_styles.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_api.py` & `docx-hitalent-0.8.51/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_blkcntnr.py` & `docx-hitalent-0.8.51/tests/test_blkcntnr.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_document.py` & `docx-hitalent-0.8.51/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_enum.py` & `docx-hitalent-0.8.51/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/150-dpi.png` & `docx-hitalent-0.8.51/tests/test_files/150-dpi.png`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/300-dpi.TIF` & `docx-hitalent-0.8.51/tests/test_files/300-dpi.TIF`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/300-dpi.jpg` & `docx-hitalent-0.8.51/tests/test_files/300-dpi.jpg`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/300-dpi.png` & `docx-hitalent-0.8.51/tests/test_files/300-dpi.png`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/72-dpi.tiff` & `docx-hitalent-0.8.51/tests/test_files/72-dpi.tiff`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/CVS_LOGO.WMF` & `docx-hitalent-0.8.51/tests/test_files/CVS_LOGO.WMF`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/exif-420-dpi.jpg` & `docx-hitalent-0.8.51/tests/test_files/exif-420-dpi.jpg`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/[Content_Types].xml` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/[Content_Types].xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/_rels/.rels` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/_rels/.rels`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/docProps/app.xml` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/docProps/app.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/docProps/core.xml` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/docProps/core.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/docProps/thumbnail.jpeg` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/docProps/thumbnail.jpeg`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/_rels/document.xml.rels` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/_rels/document.xml.rels`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/document.xml` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/document.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/fontTable.xml` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/fontTable.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/numbering.xml` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/numbering.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/settings.xml` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/settings.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/styles.xml` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/styles.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/stylesWithEffects.xml` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/stylesWithEffects.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/expanded_docx/word/theme/theme1.xml` & `docx-hitalent-0.8.51/tests/test_files/expanded_docx/word/theme/theme1.xml`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/having-images.docx` & `docx-hitalent-0.8.51/tests/test_files/having-images.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/jfif-iguana.jpg` & `docx-hitalent-0.8.51/tests/test_files/jfif-iguana.jpg`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/little-endian.tif` & `docx-hitalent-0.8.51/tests/test_files/little-endian.tif`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/monty-truth.png` & `docx-hitalent-0.8.51/tests/test_files/monty-truth.png`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/python-icon.jpeg` & `docx-hitalent-0.8.51/tests/test_files/python-icon.jpeg`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/python-icon.png` & `docx-hitalent-0.8.51/tests/test_files/python-icon.png`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/python-powered.png` & `docx-hitalent-0.8.51/tests/test_files/python-powered.png`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/python.bmp` & `docx-hitalent-0.8.51/tests/test_files/python.bmp`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/snippets/add-row-col.txt` & `docx-hitalent-0.8.51/tests/test_files/snippets/add-row-col.txt`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/snippets/inline.txt` & `docx-hitalent-0.8.51/tests/test_files/snippets/inline.txt`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/snippets/new-tbl.txt` & `docx-hitalent-0.8.51/tests/test_files/snippets/new-tbl.txt`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/snippets/tbl-cells.txt` & `docx-hitalent-0.8.51/tests/test_files/snippets/tbl-cells.txt`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/sonic.gif` & `docx-hitalent-0.8.51/tests/test_files/sonic.gif`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_files/test.docx` & `docx-hitalent-0.8.51/tests/test_files/test.docx`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_package.py` & `docx-hitalent-0.8.51/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_section.py` & `docx-hitalent-0.8.51/tests/test_section.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_settings.py` & `docx-hitalent-0.8.51/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_shape.py` & `docx-hitalent-0.8.51/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_shared.py` & `docx-hitalent-0.8.51/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/test_table.py` & `docx-hitalent-0.8.51/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/text/test_font.py` & `docx-hitalent-0.8.51/tests/text/test_font.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/text/test_paragraph.py` & `docx-hitalent-0.8.51/tests/text/test_paragraph.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/text/test_parfmt.py` & `docx-hitalent-0.8.51/tests/text/test_parfmt.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/text/test_run.py` & `docx-hitalent-0.8.51/tests/text/test_run.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/text/test_tabstops.py` & `docx-hitalent-0.8.51/tests/text/test_tabstops.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/unitdata.py` & `docx-hitalent-0.8.51/tests/unitdata.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/unitutil/cxml.py` & `docx-hitalent-0.8.51/tests/unitutil/cxml.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/unitutil/file.py` & `docx-hitalent-0.8.51/tests/unitutil/file.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tests/unitutil/mock.py` & `docx-hitalent-0.8.51/tests/unitutil/mock.py`

 * *Files identical despite different names*

### Comparing `docx-hitalent-0.8.50/tox.ini` & `docx-hitalent-0.8.51/tox.ini`

 * *Files identical despite different names*

