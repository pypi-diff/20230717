# Comparing `tmp/collective.behavior.relatedmedia-3.2.0.tar.gz` & `tmp/collective.behavior.relatedmedia-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.behavior.relatedmedia-3.2.0.tar", last modified: Wed Jul 20 08:43:54 2022, max compression
+gzip compressed data, was "collective.behavior.relatedmedia-3.3.0.tar", last modified: Mon Jul 17 15:03:02 2023, max compression
```

## Comparing `collective.behavior.relatedmedia-3.2.0.tar` & `collective.behavior.relatedmedia-3.3.0.tar`

### file list

```diff
@@ -1,87 +1,85 @@
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.089759 collective.behavior.relatedmedia-3.2.0/
--rw-r--r--   0 peterm     (501) staff       (20)      749 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/.gitignore
--rw-r--r--   0 peterm     (501) staff       (20)     3003 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/CHANGES.md
--rw-r--r--   0 peterm     (501) staff       (20)      107 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/MANIFEST.in
--rw-r--r--   0 peterm     (501) staff       (20)    11526 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/Makefile
--rw-r--r--   0 peterm     (501) staff       (20)     5665 2022-07-20 08:43:54.089833 collective.behavior.relatedmedia-3.2.0/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     1626 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/README.md
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.082000 collective.behavior.relatedmedia-3.2.0/collective/
--rw-r--r--   0 peterm     (501) staff       (20)      245 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.083001 collective.behavior.relatedmedia-3.2.0/collective/behavior/
--rw-r--r--   0 peterm     (501) staff       (20)      245 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.084748 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/
--rw-r--r--   0 peterm     (501) staff       (20)      124 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)     7745 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/behavior.py
--rw-r--r--   0 peterm     (501) staff       (20)     8398 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/browser.py
--rw-r--r--   0 peterm     (501) staff       (20)     5738 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     3665 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/events.py
--rw-r--r--   0 peterm     (501) staff       (20)     2637 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/interfaces.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.084880 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.079682 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/de/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.085147 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/
--rw-r--r--   0 peterm     (501) staff       (20)     3818 2022-07-20 08:43:53.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.mo
--rw-r--r--   0 peterm     (501) staff       (20)     7885 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.po
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.079789 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/en/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.085396 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/
--rw-r--r--   0 peterm     (501) staff       (20)      458 2022-07-20 08:43:53.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.mo
--rw-r--r--   0 peterm     (501) staff       (20)     6392 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.po
--rwxr-xr-x   0 peterm     (501) staff       (20)      503 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/update.sh
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.080164 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.086204 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/default/
--rw-r--r--   0 peterm     (501) staff       (20)      205 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/default/browserlayer.xml
--rw-r--r--   0 peterm     (501) staff       (20)      610 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/default/controlpanel.xml
--rw-r--r--   0 peterm     (501) staff       (20)       71 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/default/metadata.xml
--rw-r--r--   0 peterm     (501) staff       (20)     1196 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/default/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.086343 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/default/types/
--rw-r--r--   0 peterm     (501) staff       (20)      288 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/default/types/Document.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.086709 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/uninstall/
--rw-r--r--   0 peterm     (501) staff       (20)      230 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 peterm     (501) staff       (20)      357 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 peterm     (501) staff       (20)      407 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/uninstall/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.086835 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/uninstall/types/
--rw-r--r--   0 peterm     (501) staff       (20)      304 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/uninstall/types/Document.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.080405 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/upgrades/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.086964 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/upgrades/local_config/
--rw-r--r--   0 peterm     (501) staff       (20)      541 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/upgrades/local_config/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.087090 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/
--rw-r--r--   0 peterm     (501) staff       (20)      539 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.087225 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/types/
--rw-r--r--   0 peterm     (501) staff       (20)      305 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/types/Document.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.087349 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/upgrades/registry_cleanup/
--rw-r--r--   0 peterm     (501) staff       (20)      223 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/upgrades/registry_cleanup/registry.xml
--rw-r--r--   0 peterm     (501) staff       (20)      832 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/related_attachments.pt
--rw-r--r--   0 peterm     (501) staff       (20)      846 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/related_images.pt
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.087600 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/resources/
--rw-r--r--   0 peterm     (501) staff       (20)      671 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/resources/relateditems_selection.xml
--rw-r--r--   0 peterm     (501) staff       (20)      797 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/resources/relatedmedia.js
--rw-r--r--   0 peterm     (501) staff       (20)     1597 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/testing.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.087860 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/tests/
--rw-r--r--   0 peterm     (501) staff       (20)        2 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/tests/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)     2195 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/tests/test_setup.py
--rw-r--r--   0 peterm     (501) staff       (20)      748 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/upgrades.py
--rw-r--r--   0 peterm     (501) staff       (20)     3144 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/upgrades.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     2974 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/utils.py
--rw-r--r--   0 peterm     (501) staff       (20)      480 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/viewlet_uploader.pt
--rw-r--r--   0 peterm     (501) staff       (20)     1158 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/widget.py
--rw-r--r--   0 peterm     (501) staff       (20)       60 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/widget_attachments_display.pt
--rw-r--r--   0 peterm     (501) staff       (20)       55 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/widget_images_display.pt
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.082895 collective.behavior.relatedmedia-3.2.0/collective.behavior.relatedmedia.egg-info/
--rw-r--r--   0 peterm     (501) staff       (20)     5665 2022-07-20 08:43:53.000000 collective.behavior.relatedmedia-3.2.0/collective.behavior.relatedmedia.egg-info/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     3158 2022-07-20 08:43:53.000000 collective.behavior.relatedmedia-3.2.0/collective.behavior.relatedmedia.egg-info/SOURCES.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2022-07-20 08:43:53.000000 collective.behavior.relatedmedia-3.2.0/collective.behavior.relatedmedia.egg-info/dependency_links.txt
--rw-r--r--   0 peterm     (501) staff       (20)       40 2022-07-20 08:43:53.000000 collective.behavior.relatedmedia-3.2.0/collective.behavior.relatedmedia.egg-info/entry_points.txt
--rw-r--r--   0 peterm     (501) staff       (20)       31 2022-07-20 08:43:53.000000 collective.behavior.relatedmedia-3.2.0/collective.behavior.relatedmedia.egg-info/namespace_packages.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2022-07-20 08:43:53.000000 collective.behavior.relatedmedia-3.2.0/collective.behavior.relatedmedia.egg-info/not-zip-safe
--rw-r--r--   0 peterm     (501) staff       (20)      205 2022-07-20 08:43:53.000000 collective.behavior.relatedmedia-3.2.0/collective.behavior.relatedmedia.egg-info/requires.txt
--rw-r--r--   0 peterm     (501) staff       (20)       11 2022-07-20 08:43:53.000000 collective.behavior.relatedmedia-3.2.0/collective.behavior.relatedmedia.egg-info/top_level.txt
--rw-r--r--   0 peterm     (501) staff       (20)       58 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/constraints.txt
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-07-20 08:43:54.088794 collective.behavior.relatedmedia-3.2.0/docs/
--rw-r--r--   0 peterm     (501) staff       (20)    17987 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/docs/LICENSE.GPL
--rw-r--r--   0 peterm     (501) staff       (20)      747 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/docs/LICENSE.txt
--rw-r--r--   0 peterm     (501) staff       (20)   299492 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/docs/collective.behavior.relatedmedia_basepath.png
--rw-r--r--   0 peterm     (501) staff       (20)   189513 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/docs/collective.behavior.relatedmedia_settings.png
--rw-r--r--   0 peterm     (501) staff       (20)  1497793 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/docs/collective.behavior.relatedmedia_view.png
--rw-r--r--   0 peterm     (501) staff       (20)      647 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/mx.ini
--rw-r--r--   0 peterm     (501) staff       (20)      207 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/requirements.txt
--rw-r--r--   0 peterm     (501) staff       (20)      418 2022-07-20 08:43:54.090119 collective.behavior.relatedmedia-3.2.0/setup.cfg
--rw-r--r--   0 peterm     (501) staff       (20)     2218 2022-07-20 08:43:52.000000 collective.behavior.relatedmedia-3.2.0/setup.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.675646 collective.behavior.relatedmedia-3.3.0/
+-rw-r--r--   0 peterm     (501) staff       (20)      749 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/.gitignore
+-rw-r--r--   0 peterm     (501) staff       (20)     3330 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/CHANGES.md
+-rw-r--r--   0 peterm     (501) staff       (20)      107 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/MANIFEST.in
+-rw-r--r--   0 peterm     (501) staff       (20)    11526 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/Makefile
+-rw-r--r--   0 peterm     (501) staff       (20)     5972 2023-07-17 15:03:02.675713 collective.behavior.relatedmedia-3.3.0/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     1626 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/README.md
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.667471 collective.behavior.relatedmedia-3.3.0/collective/
+-rw-r--r--   0 peterm     (501) staff       (20)      245 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.668717 collective.behavior.relatedmedia-3.3.0/collective/behavior/
+-rw-r--r--   0 peterm     (501) staff       (20)      245 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.670846 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/
+-rw-r--r--   0 peterm     (501) staff       (20)      124 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     8209 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/behavior.py
+-rw-r--r--   0 peterm     (501) staff       (20)     8652 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/browser.py
+-rw-r--r--   0 peterm     (501) staff       (20)     5973 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     3977 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/events.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2790 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/interfaces.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.670987 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.665001 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/de/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.671137 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/
+-rw-r--r--   0 peterm     (501) staff       (20)     7885 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.po
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.665135 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/en/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.671288 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/
+-rw-r--r--   0 peterm     (501) staff       (20)     6392 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.po
+-rwxr-xr-x   0 peterm     (501) staff       (20)      503 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/update.sh
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.665568 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.671840 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/
+-rw-r--r--   0 peterm     (501) staff       (20)      205 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      610 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/controlpanel.xml
+-rw-r--r--   0 peterm     (501) staff       (20)       71 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/metadata.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     1258 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.671964 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/types/
+-rw-r--r--   0 peterm     (501) staff       (20)      288 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/types/Document.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.672356 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/
+-rw-r--r--   0 peterm     (501) staff       (20)      230 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      357 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      407 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.672493 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/types/
+-rw-r--r--   0 peterm     (501) staff       (20)      304 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/types/Document.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.665856 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.672641 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/local_config/
+-rw-r--r--   0 peterm     (501) staff       (20)      541 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/local_config/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.672783 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/
+-rw-r--r--   0 peterm     (501) staff       (20)      539 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.672925 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/types/
+-rw-r--r--   0 peterm     (501) staff       (20)      305 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/types/Document.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.673084 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/registry_cleanup/
+-rw-r--r--   0 peterm     (501) staff       (20)      223 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/registry_cleanup/registry.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      841 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/related_attachments.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      931 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/related_images.pt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.673359 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/resources/
+-rw-r--r--   0 peterm     (501) staff       (20)      824 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/resources/relateditems_selection.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      797 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/resources/relatedmedia.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1597 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/testing.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.673648 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/tests/
+-rw-r--r--   0 peterm     (501) staff       (20)        2 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/tests/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2195 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/tests/test_setup.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2621 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/upgrades.py
+-rw-r--r--   0 peterm     (501) staff       (20)     3699 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/upgrades.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     2974 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/utils.py
+-rw-r--r--   0 peterm     (501) staff       (20)      480 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/viewlet_uploader.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     1165 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/widget.py
+-rw-r--r--   0 peterm     (501) staff       (20)       60 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/widget_attachments_display.pt
+-rw-r--r--   0 peterm     (501) staff       (20)       55 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/widget_images_display.pt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.668576 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/
+-rw-r--r--   0 peterm     (501) staff       (20)     5972 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     2974 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/SOURCES.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/dependency_links.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       40 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/entry_points.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       31 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/namespace_packages.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/not-zip-safe
+-rw-r--r--   0 peterm     (501) staff       (20)      231 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/requires.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       11 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/top_level.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       58 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/constraints.txt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.674695 collective.behavior.relatedmedia-3.3.0/docs/
+-rw-r--r--   0 peterm     (501) staff       (20)    17987 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/docs/LICENSE.GPL
+-rw-r--r--   0 peterm     (501) staff       (20)      747 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/docs/LICENSE.txt
+-rw-r--r--   0 peterm     (501) staff       (20)   299492 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_basepath.png
+-rw-r--r--   0 peterm     (501) staff       (20)   189513 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_settings.png
+-rw-r--r--   0 peterm     (501) staff       (20)  1497793 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_view.png
+-rw-r--r--   0 peterm     (501) staff       (20)      647 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/mx.ini
+-rw-r--r--   0 peterm     (501) staff       (20)      182 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/requirements.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      418 2023-07-17 15:03:02.675985 collective.behavior.relatedmedia-3.3.0/setup.cfg
+-rw-r--r--   0 peterm     (501) staff       (20)     2266 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/setup.py
```

### Comparing `collective.behavior.relatedmedia-3.2.0/.gitignore` & `collective.behavior.relatedmedia-3.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/CHANGES.md` & `collective.behavior.relatedmedia-3.3.0/CHANGES.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 Changelog
 =========
 
 
+## 3.3.0 (2023-07-17)
+------------------
+
+Feature:
+
+- Mark `base_path` concept as deprecated and add a migration script for it.
+  [petschki]
+
+- Convenience short name for behavior.
+  [petschki]
+
+- Use `plone.base.utils.human_readable_size` for attachment size and implement
+  mimetype icons for attachment list.
+  [petschki]
+
+
 3.2.0 (2022-07-20)
 ------------------
 
 - Fixed customized `selection.xml` template for `pat-relateditems`.
   [petschki]
 
 - CI Test setup with `mxdev`.
```

### Comparing `collective.behavior.relatedmedia-3.2.0/Makefile` & `collective.behavior.relatedmedia-3.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/PKG-INFO` & `collective.behavior.relatedmedia-3.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: collective.behavior.relatedmedia
-Version: 3.2.0
+Version: 3.3.0
 Summary: Adds Various configuration fields and viewlets to manage and show content related images and attachments
 Home-page: https://github.com/kombinat/collective.behavior.relatedmedia
 Author: petschki
 Author-email: peter.mathis@kombinat.at
 License: gpl
 Keywords: plone richmedia relatedmedia
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 
 # Upload and Manage Related Images and Attachments
 
 
@@ -85,14 +84,30 @@
 - Peter Holzer [agitator]
 
 
 Changelog
 =========
 
 
+## 3.3.0 (2023-07-17)
+------------------
+
+Feature:
+
+- Mark `base_path` concept as deprecated and add a migration script for it.
+  [petschki]
+
+- Convenience short name for behavior.
+  [petschki]
+
+- Use `plone.base.utils.human_readable_size` for attachment size and implement
+  mimetype icons for attachment list.
+  [petschki]
+
+
 3.2.0 (2022-07-20)
 ------------------
 
 - Fixed customized `selection.xml` template for `pat-relateditems`.
   [petschki]
 
 - CI Test setup with `mxdev`.
@@ -266,9 +281,7 @@
   [petschki]
 
 
 1.0a1 (2015-07-14)
 ------------------
 
 - Initial release
-
-
```

### Comparing `collective.behavior.relatedmedia-3.2.0/README.md` & `collective.behavior.relatedmedia-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/behavior.py` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/behavior.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
+from zope.deferredimport import deprecated
 from collective.behavior.relatedmedia import messageFactory as _
 from collective.behavior.relatedmedia.utils import media_root_path
 from collective.behavior.relatedmedia.widget import RelatedAttachmentsFieldWidget
 from collective.behavior.relatedmedia.widget import RelatedImagesFieldWidget
 from plone import api
 from plone.autoform import directives as form
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.supermodel import model
-from z3c.form.interfaces import IEditForm
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
 from zope import schema
 from zope.interface import alsoProvides
 from zope.interface import implementer
 from zope.interface import provider
 from zope.schema.interfaces import IVocabularyFactory
@@ -65,22 +65,28 @@
 
 def default_preview_scale_direction():
     return api.portal.get_registry_record(
         "collective.behavior.relatedmedia.image_gallery_default_preview_scale_direction"
     )
 
 
+def default_titles_as_caption():
+    return api.portal.get_registry_record(
+        "collective.behavior.relatedmedia.show_titles_as_caption_default", default=False
+    )
+
+
 def default_include_leadimage():
     return api.portal.get_registry_record(
         "collective.behavior.relatedmedia.include_leadimage_default", default=True
     )
 
 
 @provider(IFormFieldProvider)
-class IRelatedMedia(model.Schema):
+class IRelatedMediaBehavior(model.Schema):
 
     related_images = RelationList(
         title=_("label_images", default="Related Images"),
         value_type=RelationChoice(
             title=_("Pictures"),
             vocabulary="plone.app.vocabularies.Catalog",
         ),
@@ -94,14 +100,26 @@
         pattern_options={
             "recentlyUsed": True,  # Just turn on. Config in plone.app.widgets.
             "selectableTypes": ["Image"],
             "basePath": media_root_path,
             "selectionTemplate": read_js_template(
                 "resources/relateditems_selection.xml"
             ),
+            # add Description to the returned attributes
+            "attributes": [
+                "UID",
+                "Title",
+                "Description",
+                "portal_type",
+                "path",
+                "getURL",
+                "getIcon",
+                "is_folderish",
+                "review_state",
+            ],
             "upload": True,
         },
     )
 
     related_attachments = RelationList(
         title=_("label_attachments", default="Related Attachments"),
         value_type=RelationChoice(
@@ -119,21 +137,32 @@
         pattern_options={
             "recentlyUsed": True,  # Just turn on. Config in plone.app.widgets.
             "selectableTypes": ["File"],
             "basePath": media_root_path,
             "selectionTemplate": read_js_template(
                 "resources/relateditems_selection.xml"
             ),
+            "attributes": [
+                "UID",
+                "Title",
+                "Description",
+                "portal_type",
+                "path",
+                "getURL",
+                "getIcon",
+                "is_folderish",
+                "review_state",
+            ],
             "upload": True,
         },
     )
 
     show_titles_as_caption = schema.Bool(
         title=_("Show image titles as caption"),
-        default=False,
+        defaultFactory=default_titles_as_caption,
         required=False,
     )
 
     include_leadimage = schema.Bool(
         title=_("Include leadimage in image gallery?"),
         defaultFactory=default_include_leadimage,
         required=False,
@@ -181,40 +210,14 @@
             "the base path is automatically generated as "
             "[configured media root path]/[this id].",
         ),
         vocabulary="plone.app.vocabularies.Catalog",
         required=False,
     )
 
-    form.omitted(
-        "first_image_scale",
-        "first_image_scale_direction",
-        "gallery_css_class",
-        "include_leadimage",
-        "preview_scale",
-        "preview_scale_direction",
-        "related_attachments",
-        "related_images",
-        "related_media_base_path",
-        "show_titles_as_caption",
-    )
-
-    form.no_omit(
-        IEditForm,
-        "first_image_scale",
-        "first_image_scale_direction",
-        "gallery_css_class",
-        "include_leadimage",
-        "preview_scale",
-        "preview_scale_direction",
-        "related_attachments",
-        "related_images",
-        "show_titles_as_caption",
-    )
-
     model.fieldset(
         "relatedmedia",
         label=_("Related Media"),
         fields=[
             "related_images",
             "related_attachments",
             "show_titles_as_caption",
@@ -227,17 +230,24 @@
             "related_media_base_path",
         ],
     )
 
 
 # define languageindependent fields if p.a.multilingual is installed
 if HAS_PAM:
-    alsoProvides(IRelatedMedia["related_media_base_path"], ILanguageIndependentField)
-    alsoProvides(IRelatedMedia["show_titles_as_caption"], ILanguageIndependentField)
-    alsoProvides(IRelatedMedia["include_leadimage"], ILanguageIndependentField)
-    alsoProvides(IRelatedMedia["first_image_scale"], ILanguageIndependentField)
+    alsoProvides(IRelatedMediaBehavior["related_media_base_path"], ILanguageIndependentField)
+    alsoProvides(IRelatedMediaBehavior["show_titles_as_caption"], ILanguageIndependentField)
+    alsoProvides(IRelatedMediaBehavior["include_leadimage"], ILanguageIndependentField)
+    alsoProvides(IRelatedMediaBehavior["first_image_scale"], ILanguageIndependentField)
     alsoProvides(
-        IRelatedMedia["first_image_scale_direction"], ILanguageIndependentField
+        IRelatedMediaBehavior["first_image_scale_direction"], ILanguageIndependentField
     )
-    alsoProvides(IRelatedMedia["preview_scale"], ILanguageIndependentField)
-    alsoProvides(IRelatedMedia["preview_scale_direction"], ILanguageIndependentField)
-    alsoProvides(IRelatedMedia["gallery_css_class"], ILanguageIndependentField)
+    alsoProvides(IRelatedMediaBehavior["preview_scale"], ILanguageIndependentField)
+    alsoProvides(IRelatedMediaBehavior["preview_scale_direction"], ILanguageIndependentField)
+    alsoProvides(IRelatedMediaBehavior["gallery_css_class"], ILanguageIndependentField)
+
+
+# mark old name as depreacted
+deprecated(
+    "Renamed to 'IRelatedMediaBehavior'. Will be removed in Version 4.",
+    IRelatedMedia="collective.behavior.relatedmedia.behavior:IRelatedMediaBehavior",
+)
```

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/browser.py` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/browser.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from collective.behavior.relatedmedia.utils import get_media_root
 from collective.behavior.relatedmedia.utils import get_related_media
 from plone import api
 from plone.app.contenttypes.behaviors.leadimage import ILeadImage
 from plone.app.layout.globals.interfaces import IViewView
 from plone.app.layout.viewlets.common import ViewletBase
 from plone.app.registry.browser import controlpanel
+from plone.base.utils import human_readable_size
 from plone.dexterity.utils import createContentInContainer
 from plone.event.interfaces import IOccurrence
 from plone.memoize.instance import memoize
 from plone.namedfile.file import NamedBlobFile
 from plone.namedfile.file import NamedBlobImage
 from Products.CMFPlone.utils import safe_unicode
 from Products.Five import BrowserView
@@ -66,30 +67,32 @@
 
         if not rm_behavior:
             return
 
         context = aq_inner(self.context)
         imgs = get_related_media(context, portal_type="Image")
         show_caption = rm_behavior.show_titles_as_caption
+        first_img_title = ""
         first_img_scales = None
-        first_img_caption = ""
+        first_img_description = ""
         further_images = []
         gallery = []
 
         if rm_behavior.include_leadimage and ILeadImage.providedBy(context):
             # include leadimage if no related images are defined
             first_img_scales = context.restrictedTraverse("@@images")
-            first_img_caption = ILeadImage(context).image_caption
+            first_img_title = ILeadImage(context).image_caption
             further_images = imgs
 
         if not first_img_scales and len(imgs):
             first_img = imgs[0]
             if first_img:
                 first_img_scales = first_img.restrictedTraverse("@@images")
-                first_img_caption = first_img.Title()
+                first_img_title = first_img.Title()
+                first_img_description = first_img.Description()
                 further_images = imgs[1:]
 
         if first_img_scales:
             scale = first_img_scales.scale(
                 "image",
                 scale=rm_behavior.first_image_scale,
                 direction=rm_behavior.first_image_scale_direction
@@ -98,21 +101,22 @@
             )
             if scale:
                 large_scale_url = first_img_scales.scale("image", scale="large").url
                 gallery.append(
                     dict(
                         url=large_scale_url,
                         tag=scale.tag(
-                            title=first_img_caption,
-                            alt=first_img_caption,
+                            title=first_img_title,
+                            alt=first_img_title,
                             css_class="img-fluid",
                         ),
-                        caption=first_img_caption,
+                        caption=first_img_title,
                         show_caption=show_caption,
-                        title=first_img_caption,
+                        title=first_img_title,
+                        description=first_img_description,
                     )
                 )
 
         for img in further_images:
             if img:
                 scales = img.restrictedTraverse("@@images")
                 scale = scales.scale(
@@ -127,14 +131,15 @@
                     gallery.append(
                         dict(
                             url=large_scale_url,
                             tag=scale.tag(css_class="img-fluid"),
                             caption=img.Title(),
                             show_caption=show_caption,
                             title=img.Title(),
+                            description=img.Description(),
                         )
                     )
 
         return gallery
 
 
 class RelatedAttachmentsView(RelatedBaseView):
@@ -146,30 +151,32 @@
     @memoize
     def get_attachments(self):
         _target_blank = api.portal.get_registry_record(
             "collective.behavior.relatedmedia.open_attachment_in_new_window"
         )
         link_target = _target_blank and "blank" or "top"
         atts = []
+
         for att in self.attachments:
             if att:
-                download_url = "{}/@@download/file/{}".format(
-                    att.absolute_url(), att.file.filename
+                download_url = (
+                    "{}/@@download/file/{}".format(
+                        att.absolute_url(), att.file.filename
+                    )
+                    if att.file
+                    else "#"
                 )
-                file_size = (att.file.getSize() or 0.0) / 1024.0
-                unit = "kB"
-                if file_size > 1000:
-                    file_size = file_size / 1024.0
-                    unit = "MB"
                 atts.append(
                     dict(
                         url=download_url,
                         title=att.Title(),
-                        size="{:.1f} {}".format(file_size, unit),
-                        icon=att.getIcon(),
+                        size=human_readable_size(att.file.getSize())
+                        if att.file
+                        else "missing",
+                        mimetype=att.content_type() or "application",
                         target=link_target,
                     )
                 )
         return atts
 
 
 class RelatedMediaControlPanelForm(controlpanel.RegistryEditForm):
```

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/configure.zcml` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/configure.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -23,26 +23,29 @@
         name="uninstall"
         title="Related media behavior"
         directory="profiles/uninstall"
         description="Uninstallation profile"
         provides="Products.GenericSetup.interfaces.EXTENSION"
         />
 
+    <include package="Products.CMFCore"/>
     <include package="plone.behavior" file="meta.zcml"/>
 
     <utility
         provides="zope.schema.interfaces.IVocabularyFactory"
         factory=".behavior.GalleryCSSClassesVocabulary"
         name="collective.relatedmedia.gallerycssclasses"
         />
 
     <plone:behavior
+        name="collective.relatedmedia"
         title="Related Media"
         description="Manage content-related images and attachments"
-        provides=".behavior.IRelatedMedia"
+        provides=".behavior.IRelatedMediaBehavior"
+        former_dotted_names="collective.behavior.relatedmedia.behavior.IRelatedMedia"
         />
 
     <plone:static
         directory="resources"
         name="collective.behavior.relatedmedia.resources"
         type="plone"
         />
@@ -61,14 +64,16 @@
         for="*"
         manager="plone.app.layout.viewlets.interfaces.IBelowContentTitle"
         template="widget_images_display.pt"
         permission="zope2.View"
         layer=".interfaces.ICollectiveBehaviorRelatedmediaLayer"
         />
 
+    <include package="z3c.form" file="meta.zcml"/>
+
     <z3c:widgetTemplate
         mode="display"
         field="z3c.relationfield.interfaces.IRelationList"
         widget=".widget.IRelatedImagesWidget"
         template="widget_images_display.pt"
         />
 
@@ -143,15 +148,15 @@
 
     <!-- convenience: upload viewlet for view mode -->
     <browser:viewlet
         name="collective.behavior.relatedmedia.uploader"
         manager="plone.app.layout.viewlets.interfaces.IBelowContent"
         class=".browser.UploadViewlet"
         template="viewlet_uploader.pt"
-        for=".behavior.IRelatedMedia"
+        for=".behavior.IRelatedMediaBehavior"
         permission="cmf.ModifyPortalContent"
         layer=".interfaces.ICollectiveBehaviorRelatedmediaLayer"
         />
 
     <!-- uploader -->
     <browser:page
         name="upload_related_media"
```

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/events.py` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,29 +102,33 @@
     if not ILeadImageBehavior(obj).image:
         # set first related image as lead image (incl. caption)
         ILeadImageBehavior(obj).image = imgs[0].image
         ILeadImageBehavior(obj).image_caption = safe_unicode(imgs[0].Title())
         obj.reindexObject()
 
 
+def get_obj_from_relateditem_path(value, prefix=19):
+    item_path = value[prefix:].replace("--", "/")
+    rel_obj = None
+
+    try:
+        rel_obj = api.content.get(path=item_path)
+    except Exception:
+        logger.warn("Could not find related item {}".format(item_path))
+
+    return rel_obj
+
+
 def update_titles(obj, event):
     req_form = obj.REQUEST.form
 
     for k in req_form:
-        if not k.startswith("relatedmedia-title-"):
-            continue
-
-        item_path = k[19:].replace("--", "/")
-        rel_obj = None
-
-        try:
-            rel_obj = api.content.get(path=item_path)
-        except Exception:
-            logger.warn("Could not find related item {}".format(item_path))
-            pass
-
-        if rel_obj is None:
-            return
-
-        if rel_obj.title != req_form[k]:
-            rel_obj.title = req_form[k]
-            rel_obj.reindexObject()
+        if k.startswith("relatedmedia-title-"):
+            rel_obj = get_obj_from_relateditem_path(k)
+            if rel_obj and rel_obj.title != req_form[k]:
+                rel_obj.title = req_form[k]
+                rel_obj.reindexObject()
+        if k.startswith("relatedmedia-description-"):
+            rel_obj = get_obj_from_relateditem_path(k, 25)
+            if rel_obj and rel_obj.description != req_form[k]:
+                rel_obj.description = req_form[k]
+                rel_obj.reindexObject()
```

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/interfaces.py` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,20 @@
 
     image_gallery_default_preview_scale_direction = schema.Bool(
         title=_("Default setting for cropping gallery images"),
         default=False,
         required=False,
     )
 
+    show_titles_as_caption_default = schema.Bool(
+        title=_("Show image titles as caption"),
+        default=False,
+        required=False,
+    )
+
     include_leadimage_default = schema.Bool(
         title=_("Include leadimage in image gallery?"),
         default=True,
         required=False,
     )
 
     update_leadimage = schema.Bool(
```

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.po` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.po`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.po` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.po`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/default/controlpanel.xml` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/default/registry.xml` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/registry.xml`

 * *Files 6% similar despite different names*

#### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/default/registry.xml` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/registry.xml`

```diff
@@ -5,14 +5,15 @@
     <value key="create_media_container_base_paths">False</value>
     <value key="image_gallery_cssclass" purge="false">
       <element>floatLeft</element>
       <element>floatRight</element>
       <element>fullWidth</element>
     </value>
     <value key="image_gallery_default_class">fullWidth</value>
+    <value key="show_titles_as_caption_default">False</value>
     <value key="include_leadimage_default">True</value>
   </records>
   <records prefix="plone.bundles/relatedmedia" interface="Products.CMFPlone.interfaces.IBundleRegistry">
     <value key="enabled">True</value>
     <value key="expression">python: member is not None</value>
     <value key="jscompilation">++plone++collective.behavior.relatedmedia.resources/relatedmedia.js</value>
     <value key="csscompilation"/>
```

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/upgrades/local_config/registry.xml` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/local_config/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/registry.xml` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/related_attachments.pt` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/related_attachments.pt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-<div tal:define="attachments view/get_attachments"
+<div tal:define="attachments view/get_attachments; icons nocall:context/@@iconresolver"
      tal:condition="python:attachments or view.can_upload"
      i18n:domain="collective.behavior.relatedmedia">
     <h2 i18n:translate="title_attachments">Attachments</h2>
-    <ul id="related-attachments">
+    <ul id="related-attachments" class="list-unstyled">
 
         <li tal:repeat="att attachments" class="attachment-item">
             <a tal:attributes="href att/url;
                                target att/target">
-                <img tal:condition="att/icon|nothing" border="0"
-                     tal:attributes="src string:${view/site_url}/${att/icon}"
+                <img tal:replace="structure python:icons.tag('mimetype-' + att['mimetype'])"
                 /> <span tal:content="att/title" /> (<span tal:content="att/size" />)
             </a>
         </li>
 
         <li tal:condition="not:attachments" i18n:translate="" class="discreet">
             No attachments uploaded yet
         </li>
```

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/resources/relateditems_selection.xml` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/resources/relateditems_selection.xml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <div class="pat-relateditems-item">
   <div class="pat-relateditems-result-info">
     <span
       class="pat-relateditems-item-title <%- portal_type ? 'contenttype-' + portal_type.toLowerCase() : '' %> <%- review_state ? 'state-' + review_state : '' %>"
       title="<%- portal_type %>">
-      <input type="text" value="<%- Title %>" name="relatedmedia-title-<%- path.replace(/\//g, '--') %>" />
+      <input type="text" value="<%- Title %>" name="relatedmedia-title-<%- path.replace(/\//g, '--') %>" class="form-control" />
+      <textarea name="relatedmedia-description-<%- path.replace(/\//g, '--') %>" class="form-control"><%- Description %></textarea>
     </span>
     <span class="pat-relateditems-item-path"><%- path %></span>
   </div>
   <% if (getURL && (getIcon || portal_type === "Image")) { %>
     <div class="pat-relateditems-item-image">
       <img src="<%- getURL %>/@@images/image/thumb" />
     </div>
```

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/resources/relatedmedia.js` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/resources/relatedmedia.js`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/testing.py` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/testing.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/tests/test_setup.py` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/upgrades.zcml` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/upgrades.zcml`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 
     <registerProfile
         name="package_rename"
         title="Profile for upgrade step 'Package rename'"
         directory="profiles/upgrades/package_rename"
         description=""
-        provides="Products.GenericSetup.interfaces.EXTENSION"
-        />
+        provides="Products.GenericSetup.interfaces.EXTENSION" />
 
     <upgradeStep
         source="*"
         destination="1002"
         profile="collective.behavior.relatedmedia:default"
         title="Package rename"
         description="'collective.behavior.relatedimages' -> 'collective.behavior.relatedmedia'"
@@ -19,16 +18,15 @@
         handler=".upgrades.package_rename" />
 
     <registerProfile
         name="local_config"
         title="Profile for upgrade step 'Local configuration'"
         directory="profiles/upgrades/local_config"
         description=""
-        provides="Products.GenericSetup.interfaces.EXTENSION"
-        />
+        provides="Products.GenericSetup.interfaces.EXTENSION" />
 
     <upgradeStep
         source="1002"
         destination="1003"
         profile="collective.behavior.relatedmedia:default"
         title="Local gallery configuration"
         description="expose gallery image settings to local tab"
@@ -76,25 +74,40 @@
         run_deps="True" />
 
     <registerProfile
         name="registry_cleanup"
         title="Remove resources from registry"
         directory="profiles/upgrades/registry_cleanup"
         description=""
-        provides="Products.GenericSetup.interfaces.EXTENSION"
-        />
+        provides="Products.GenericSetup.interfaces.EXTENSION" />
 
     <upgradeSteps
         source="2011"
         destination="2100"
         profile="collective.behavior.relatedmedia:default">
         <upgradeStep
             title="Resourceregistry cleanup"
             handler=".upgrades.registry_cleanup" />
         <upgradeDepends
             title="Upgrade registry -> new resource bundle"
             import_steps="plone.app.registry"
             run_deps="True" />
     </upgradeSteps>
 
+    <upgradeDepends
+        source="2100"
+        destination="2101"
+        profile="collective.behavior.relatedmedia:default"
+        title="Upgrade registry -> new default settings"
+        import_steps="plone.app.registry"
+        run_deps="True" />
+
+    <upgradeSteps
+        source="2101"
+        destination="3000"
+        profile="collective.behavior.relatedmedia:default">
+        <upgradeStep
+            title="Remove deprecated 'related_media_base_path' folder and migrate relations"
+            handler=".upgrades.migrate_base_path_relations" />
+    </upgradeSteps>
 
 </configure>
```

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/utils.py` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/utils.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/collective/behavior/relatedmedia/widget.py` & `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/widget.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
-from plone.app.z3cform.widget import RelatedItemsWidget
-from Products.CMFPlone import PloneMessageFactory as _
+from plone.app.z3cform.widgets.relateditems import RelatedItemsWidget
+from plone.base import PloneMessageFactory as _
 from z3c.form.interfaces import IFieldWidget
 from z3c.form.interfaces import ITextWidget
 from z3c.form.widget import FieldWidget
 from zope.interface import implementer
 from zope.interface import implementer_only
```

### Comparing `collective.behavior.relatedmedia-3.2.0/collective.behavior.relatedmedia.egg-info/PKG-INFO` & `collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: collective.behavior.relatedmedia
-Version: 3.2.0
+Version: 3.3.0
 Summary: Adds Various configuration fields and viewlets to manage and show content related images and attachments
 Home-page: https://github.com/kombinat/collective.behavior.relatedmedia
 Author: petschki
 Author-email: peter.mathis@kombinat.at
 License: gpl
 Keywords: plone richmedia relatedmedia
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 
 # Upload and Manage Related Images and Attachments
 
 
@@ -85,14 +84,30 @@
 - Peter Holzer [agitator]
 
 
 Changelog
 =========
 
 
+## 3.3.0 (2023-07-17)
+------------------
+
+Feature:
+
+- Mark `base_path` concept as deprecated and add a migration script for it.
+  [petschki]
+
+- Convenience short name for behavior.
+  [petschki]
+
+- Use `plone.base.utils.human_readable_size` for attachment size and implement
+  mimetype icons for attachment list.
+  [petschki]
+
+
 3.2.0 (2022-07-20)
 ------------------
 
 - Fixed customized `selection.xml` template for `pat-relateditems`.
   [petschki]
 
 - CI Test setup with `mxdev`.
@@ -266,9 +281,7 @@
   [petschki]
 
 
 1.0a1 (2015-07-14)
 ------------------
 
 - Initial release
-
-
```

### Comparing `collective.behavior.relatedmedia-3.2.0/collective.behavior.relatedmedia.egg-info/SOURCES.txt` & `collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,17 +31,15 @@
 collective/behavior/relatedmedia/upgrades.zcml
 collective/behavior/relatedmedia/utils.py
 collective/behavior/relatedmedia/viewlet_uploader.pt
 collective/behavior/relatedmedia/widget.py
 collective/behavior/relatedmedia/widget_attachments_display.pt
 collective/behavior/relatedmedia/widget_images_display.pt
 collective/behavior/relatedmedia/locales/update.sh
-collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.mo
 collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.po
-collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.mo
 collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.po
 collective/behavior/relatedmedia/profiles/default/browserlayer.xml
 collective/behavior/relatedmedia/profiles/default/controlpanel.xml
 collective/behavior/relatedmedia/profiles/default/metadata.xml
 collective/behavior/relatedmedia/profiles/default/registry.xml
 collective/behavior/relatedmedia/profiles/default/types/Document.xml
 collective/behavior/relatedmedia/profiles/uninstall/browserlayer.xml
```

### Comparing `collective.behavior.relatedmedia-3.2.0/docs/LICENSE.GPL` & `collective.behavior.relatedmedia-3.3.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/docs/LICENSE.txt` & `collective.behavior.relatedmedia-3.3.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/docs/collective.behavior.relatedmedia_basepath.png` & `collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_basepath.png`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/docs/collective.behavior.relatedmedia_settings.png` & `collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_settings.png`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/docs/collective.behavior.relatedmedia_view.png` & `collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_view.png`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/mx.ini` & `collective.behavior.relatedmedia-3.3.0/mx.ini`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.2.0/setup.py` & `collective.behavior.relatedmedia-3.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.2.0"
+version = "3.3.0"
 
 this_directory = Path(__file__).parent
 long_description = (
     (this_directory / "README.md").read_text()
     + "\n\n"
     + (this_directory / "CHANGES.md").read_text()
 )
@@ -41,21 +41,23 @@
     author_email="peter.mathis@kombinat.at",
     url="https://github.com/kombinat/collective.behavior.relatedmedia",
     license="gpl",
     packages=find_packages(exclude=["ez_setup"]),
     namespace_packages=["collective", "collective.behavior"],
     include_package_data=True,
     zip_safe=False,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
         "setuptools",
         # -*- Extra requirements: -*-
         "plone.api",
         "plone.behavior",
         "plone.app.dexterity",
+        "Products.CMFCore",
+        "z3c.form",
     ],
     extras_require={
         "test": [
             "plone.app.testing[robot]",
             "plone.app.robotframework",
             "plone.app.contenttypes",
             "robotframework-selenium2library",
```

