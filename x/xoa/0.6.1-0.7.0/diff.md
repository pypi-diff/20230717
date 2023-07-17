# Comparing `tmp/xoa-0.6.1.tar.gz` & `tmp/xoa-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoa-0.6.1.tar", last modified: Thu Feb 24 15:02:54 2022, max compression
+gzip compressed data, was "xoa-0.7.0.tar", last modified: Mon Jul 17 11:31:22 2023, max compression
```

## Comparing `xoa-0.6.1.tar` & `xoa-0.7.0.tar`

### file list

```diff
@@ -1,119 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.335735 xoa-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.323735 xoa-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.327735 xoa-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-02-24 15:02:37.000000 xoa-0.6.1/.github/workflows/python-package-conda.yml
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-02-24 15:02:37.000000 xoa-0.6.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-02-24 15:02:37.000000 xoa-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-02-24 15:02:37.000000 xoa-0.6.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6854 2022-02-24 15:02:37.000000 xoa-0.6.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-24 15:02:37.000000 xoa-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-02-24 15:02:37.000000 xoa-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-02-24 15:02:54.335735 xoa-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1696 2022-02-24 15:02:37.000000 xoa-0.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3795 2022-02-24 15:02:37.000000 xoa-0.6.1/ROADMAP.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.327735 xoa-0.6.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)      115 2022-02-24 15:02:37.000000 xoa-0.6.1/bin/xoa
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.327735 xoa-0.6.1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/.nojekill
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.327735 xoa-0.6.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/_static/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (121)     2678 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.323735 xoa-0.6.1/doc/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.327735 xoa-0.6.1/doc/_templates/autosummary/
--rwxr-xr-x   0 runner    (1001) docker     (121)      618 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/_templates/autosummary/class.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      687 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/accessors.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.327735 xoa-0.6.1/doc/api/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/api/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/appendix.cf.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/appendix.options.rst
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/appendix.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.327735 xoa-0.6.1/doc/binder/
--rwxr-xr-x   0 runner    (1001) docker     (121)        4 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/binder/apt.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      259 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/binder/environment.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)      178 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/binder/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5051 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1857 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/configure.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.327735 xoa-0.6.1/doc/ext/
--rwxr-xr-x   0 runner    (1001) docker     (121)     5238 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/ext/gencfspecs.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4758 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/ext/genfortran.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2296 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/ext/genoptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/howtostart.rst
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (121)    23125 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/uses.cf.rst
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/uses.cfgm.cfg2rst.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6453 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/uses.cfgm.rst
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-24 15:02:37.000000 xoa-0.6.1/doc/uses.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.327735 xoa-0.6.1/env/
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-02-24 15:02:37.000000 xoa-0.6.1/env/environment.rtd.yml
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-02-24 15:02:37.000000 xoa-0.6.1/env/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-02-24 15:02:37.000000 xoa-0.6.1/env/requirements-doc.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.331735 xoa-0.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-02-24 15:02:37.000000 xoa-0.6.1/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2781 2022-02-24 15:02:37.000000 xoa-0.6.1/examples/plot_croco_section.py
--rw-r--r--   0 runner    (1001) docker     (121)     6420 2022-02-24 15:02:37.000000 xoa-0.6.1/examples/plot_hycom_gdp.py
--rw-r--r--   0 runner    (1001) docker     (121)     8752 2022-02-24 15:02:37.000000 xoa-0.6.1/examples/plot_mercator_argo.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-02-24 15:02:37.000000 xoa-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-02-24 15:02:37.000000 xoa-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-02-24 15:02:54.335735 xoa-0.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1868 2022-02-24 15:02:37.000000 xoa-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.331735 xoa-0.6.1/xoa/
--rw-r--r--   0 runner    (1001) docker     (121)    13649 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.335735 xoa-0.6.1/xoa/_samples/
--rw-r--r--   0 runner    (1001) docker     (121)    94162 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/argo-7900573.nc
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/argo.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/croco.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    62376 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/croco.south-africa.meridional.nc
--rw-r--r--   0 runner    (1001) docker     (121)   194356 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/croco.south-africa.surf.nc
--rw-r--r--   0 runner    (1001) docker     (121)    62376 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/croco.south-africa.zonal.nc
--rw-r--r--   0 runner    (1001) docker     (121)    43153 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/gdp-6203641.csv
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/gdp.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/hycom.cfg
--rw-r--r--   0 runner    (1001) docker     (121)   177500 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/hycom.gdp.h.nc
--rw-r--r--   0 runner    (1001) docker     (121)   176804 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/hycom.gdp.u.nc
--rw-r--r--   0 runner    (1001) docker     (121)   176804 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/hycom.gdp.v.nc
--rw-r--r--   0 runner    (1001) docker     (121)    71836 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/ibi-argo-7900573.nc
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/_samples/mercator.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    19909 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/accessors.py
--rw-r--r--   0 runner    (1001) docker     (121)    29627 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/cf.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/cf.ini
--rw-r--r--   0 runner    (1001) docker     (121)   121607 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/cf.py
--rw-r--r--   0 runner    (1001) docker     (121)    67879 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/cfgm.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2098 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3691 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/color.py
--rw-r--r--   0 runner    (1001) docker     (121)    23136 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/coords.py
--rw-r--r--   0 runner    (1001) docker     (121)     5056 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/dyn.py
--rw-r--r--   0 runner    (1001) docker     (121)    30405 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    15011 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/geo.py
--rw-r--r--   0 runner    (1001) docker     (121)    17718 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    27111 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/interp.py
--rw-r--r--   0 runner    (1001) docker     (121)    26161 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/krig.py
--rw-r--r--   0 runner    (1001) docker     (121)    21585 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    19745 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    13727 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/regrid.py
--rw-r--r--   0 runner    (1001) docker     (121)    21328 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/sigma.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.335735 xoa-0.6.1/xoa/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    34797 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/tests/test_cf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/tests/test_coords.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/tests/test_dyn.py
--rw-r--r--   0 runner    (1001) docker     (121)     4886 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/tests/test_geo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4788 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    11574 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/tests/test_interp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3579 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4883 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/tests/test_regrid.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-02-24 15:02:37.000000 xoa-0.6.1/xoa/tests/test_sigma.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 15:02:54.331735 xoa-0.6.1/xoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-02-24 15:02:54.000000 xoa-0.6.1/xoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-02-24 15:02:54.000000 xoa-0.6.1/xoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 15:02:54.000000 xoa-0.6.1/xoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-24 15:02:54.000000 xoa-0.6.1/xoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 15:02:54.000000 xoa-0.6.1/xoa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-02-24 15:02:54.000000 xoa-0.6.1/xoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-02-24 15:02:54.000000 xoa-0.6.1/xoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.473256 xoa-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-17 11:31:04.000000 xoa-0.7.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-17 11:31:04.000000 xoa-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-17 11:31:04.000000 xoa-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-17 11:31:04.000000 xoa-0.7.0/.github/workflows/python-package-conda.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-17 11:31:04.000000 xoa-0.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-17 11:31:04.000000 xoa-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 11:31:04.000000 xoa-0.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-17 11:31:04.000000 xoa-0.7.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 11:31:04.000000 xoa-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 11:31:04.000000 xoa-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-17 11:31:22.473256 xoa-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-17 11:31:04.000000 xoa-0.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-17 11:31:04.000000 xoa-0.7.0/ROADMAP.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      115 2023-07-17 11:31:04.000000 xoa-0.7.0/bin/xoa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/.nojekill
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/_static/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2678 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.457254 xoa-0.7.0/doc/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.461254 xoa-0.7.0/doc/_templates/autosummary/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/_templates/autosummary/class.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/accessors.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.465255 xoa-0.7.0/doc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/api/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/appendix.cf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/appendix.options.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/appendix.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.465255 xoa-0.7.0/doc/binder/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        4 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/binder/apt.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/binder/environment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/binder/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/configure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.465255 xoa-0.7.0/doc/ext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5238 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/ext/gencfspecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4758 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/ext/genfortran.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2296 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/ext/genoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/howtostart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23125 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/uses.cf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/uses.cfgm.cfg2rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/uses.cfgm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 11:31:04.000000 xoa-0.7.0/doc/uses.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.465255 xoa-0.7.0/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-17 11:31:04.000000 xoa-0.7.0/env/environment.rtd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-17 11:31:04.000000 xoa-0.7.0/env/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 11:31:04.000000 xoa-0.7.0/env/requirements-doc.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.465255 xoa-0.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 11:31:04.000000 xoa-0.7.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-17 11:31:04.000000 xoa-0.7.0/examples/plot_croco_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-17 11:31:04.000000 xoa-0.7.0/examples/plot_hycom_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-17 11:31:04.000000 xoa-0.7.0/examples/plot_mercator_argo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 11:31:04.000000 xoa-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 11:31:04.000000 xoa-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 11:31:22.473256 xoa-0.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-07-17 11:31:04.000000 xoa-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.469255 xoa-0.7.0/xoa/
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.469255 xoa-0.7.0/xoa/_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    94162 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/argo-7900573.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/argo.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/croco.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    62376 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/croco.south-africa.meridional.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   194356 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/croco.south-africa.surf.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    62376 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/croco.south-africa.zonal.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    43153 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/gdp-6203641.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/gdp.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/hycom.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)   177500 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/hycom.gdp.h.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   176804 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/hycom.gdp.u.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   176804 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/hycom.gdp.v.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    71836 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/ibi-argo-7900573.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/_samples/mercator.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/cf.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/cf.ini
+-rw-r--r--   0 runner    (1001) docker     (123)   121868 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68086 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/cfgm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2098 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/dyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29740 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26161 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/krig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22623 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/num.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/sigma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.473256 xoa-0.7.0/xoa/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35220 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_dyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_sigma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/tests/test_thermdyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-17 11:31:04.000000 xoa-0.7.0/xoa/thermdyn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:31:22.469255 xoa-0.7.0/xoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 11:31:22.000000 xoa-0.7.0/xoa.egg-info/top_level.txt
```

### Comparing `xoa-0.6.1/.github/workflows/python-package-conda.yml` & `xoa-0.7.0/.github/workflows/python-package-conda.yml`

 * *Files 21% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 jobs:
   build-linux:
     runs-on: ubuntu-latest
     strategy:
       max-parallel: 5
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
     - name: Add conda to system path
       run: |
         # $CONDA is an environment variable pointing to the root of the miniconda directory
         echo $CONDA/bin >> $GITHUB_PATH
     - name: Install dependencies
```

### Comparing `xoa-0.6.1/.github/workflows/python-publish.yml` & `xoa-0.7.0/.github/workflows/python-publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
     - name: Build and publish
```

### Comparing `xoa-0.6.1/.gitignore` & `xoa-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/CHANGES.rst` & `xoa-0.7.0/CHANGES.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,64 @@
 What's new
 ##########
 
-0.6.0 (2022-02-24)
+
+0.7.0 (2023-07-17)
+==================
+
+New features
+------------
+- Add issue and pull request templates.
+- Add the :func:`xoa.filter.smooth` function [:pull:`76`].
+- Improved the default `sig` and `std` parameter values for filter windows
+  that accept them [:pull:`76`].
+- Add the :func:`xoa.plot.plot_minimap` and :func:`xoa.plot.plot_double_minimap`
+  functions to display the
+  geographic situation of a set of coordinates [:pull:`73`].
+- Add support for the `min_extent` keyword to :func:`xoa.geo.get_extent` [:pull:`73`]
+- Add dask support to :mod:`xoa.sigma` sigma to depth converters [:pull:`72`].
+- Add the :mod:`xoa.num` module that contains low level numeric utilities.
+- Add the :func:`xoa.thermdyn.mixed_layer_depth` function to compute
+  the mixed layer depth with three different methods [:pull:`67`, :pull:`75`].
+- Add the :func:`xoa.thermdyn.is_temp`, :func:`xoa.thermdyn.is_sal`
+  and :func:`xoa.thermdyn.is_dens` functions
+  to infer if an array of temperature, salinity or density type,
+  and added the related :func:`xoa.thermdyn.get_temp`,
+  :func:`xoa.thermdyn.get_sal` and :func:`xoa.thermdyn.get_dens`
+  function to search in datasets[:pull:`67`, :pull:`79`].
+- Add `kernel_kwargs` keyword to :func:`xoa.filter.convolve` to better control
+  the kernel generation by :func:`xoa.filter.generate_kernel` [:pull:`64`].
+- Add inference of parameters for some window functions, like the gaussian
+  shape, in :func:`xoa.filter.get_window_func` [:pull:`64`].
+- Add :func:`xoa.regrid.isoslice` based on :func:`xoa.interp.isoslice` core function
+  [:pull:`63`].
+
+Breaking changes
+----------------
+- func:`~xoa.filter.get_window_func` accepts now only one positional argument
+  and all other arguments must be named.
+
+Bug fixes
+---------
+- Fix :func:`xoa.cfgm.is_boolstr` which now supports the new :mod:`configobj`.
+- Fix broadcasting :mod:`xoa.interp` 1d interpolation routines [:issue:`69`].
+- Fix :func:`xoa.sigma.get_sigma_terms` so that it works in case of multiple
+  levels coordinates [:pull:`60`].
+- Fix :func:`xoa.grid.to_rect` that now infers coordinates and can emit a warning or raise an error.
+
+Documentation
+-------------
+- Add an example of `xoa.plot.plot_double_minimap` to
+  :ref:`sphx_glr_examples_plot_mercator_argo.py`
+  and :ref:`sphx_glr_examples_plot_hycom_gdp.py` examples [:pull:`73`].
+- Add an example of `xoa.thermdyn.mixed_layer_depth` to
+  :ref:`sphx_glr_examples_plot_croco_section.py` example [:pull:`67`].
+
+
+0.6.1 (2022-02-24)
 ==================
 
 New features
 ------------
 - Add a warning to :func:`xoa.open_data_sample` that is emitted when the request edfile
   is not an internal data sample [:pull:`47`].
 - Add the :func:`xoa.plot.add_shadow`, :func:`xoa.plot.add_glow` and
@@ -31,29 +84,32 @@
 
 Breaking changes
 ----------------
 - A single Nan now contaminates the data over the kernel emprise in :func:`xoa.filter.convolve`
   since `na_thres` is set to zero by default  [:pull:`40`].
 - xoa now requires the :mod:`gsw` package.
 
-Deprecations
-------------
-
 Bug fixes
 ---------
 - Fix :func:`xoa.regrid.regrid1d` so that it works now with time coordinates [:pull:`48`].
 - Fix :func:`xoa.regrid.grid2loc` so that it works with scalar output coordinates.
 - Fix :func:`xoa.regrid.regrid1d` to prevent conflict in the presence of MultiIndexes.
 - Fix search for coordinates that are hidden due to :meth:`xarray.DataArray.stack`.
 
 Documentation
 -------------
 - Add the :ref:`Compare Mercator to ARGO <sphx_glr_examples_plot_mercator_argo.py>` example.
 
 
+0.6.0 (2022-02-24)
+==================
+
+Empty with non existing tag.
+
+
 0.5.1 (2021-10-13)
 ==================
 
 New features
 ------------
 - Switch the CI workflow to github  [:pull:`36`].
```

### Comparing `xoa-0.6.1/LICENSE` & `xoa-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/PKG-INFO` & `xoa-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: xoa
-Version: 0.6.1
+Version: 0.7.0
 Summary: xarray-based ocean analysis library
 Home-page: https://github.com/vacumm/xoa
 Author: Shom
 Author-email: stephane.raynaud@shom.fr
 License: Apache
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -21,53 +20,68 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 xoa - xarray-based ocean analysis library
 =========================================
 
-.. image:: https://anaconda.org/conda-forge/xoa/badges/installer/conda.svg
-    :alt: Install with conda
-    :target: https://conda.anaconda.org/conda-forge
-.. image:: https://github.com/VACUMM/xoa/actions/workflows/python-package-conda.yml/badge.svg
+.. image:: https://github.com/shom-fr/xoa/actions/workflows/python-package-conda.yml/badge.svg
     :alt: Install, linting and tests
+.. image:: https://anaconda.org/conda-forge/xoa/badges/version.svg
+    :alt: Available on conda-forge
+    :target: https://conda.anaconda.org/conda-forge/xoa
 .. image:: https://readthedocs.org/projects/docs/badge/?version=latest
     :alt: Documentation Status
     :target: https://xoa.readthedocs.io/en/latest/
 .. image:: https://anaconda.org/conda-forge/xoa/badges/downloads.svg
     :alt: Number of downloads on anaconda.org/conda-forge
     :target: https://anaconda.org/conda-forge/xoa/
 .. image:: https://pepy.tech/badge/xoa
     :alt: Number of downloads on pypi
     :target: https://pypi.org/project/xoa
+.. image:: https://anaconda.org/conda-forge/xoa/badges/platforms.svg
+    :alt: noarch
+    :target: https://anaconda.org/conda-forge/xoa
+.. image:: https://anaconda.org/conda-forge/xoa/badges/license.svg
+    :alt: Apache 2.0
+    :target: https://anaconda.org/conda-forge/xoa
 
 xoa is intended to help reading and manipulating observed
 and simulated ocean data.
 It is heavily based on `xarray <http://xarray.pydata.org/en/stable/>`_.
 For those who know it, it is the successor of
 `vacumm <https://github.com/VACUMM/vacumm>`_.
 
+Installation
+------------
+
+From conda::
+
+   conda install -c conda-forge xoa
+
+From pypi::
+
+   pip install xoa
+
 Documentation
 -------------
 
 The xoa documentation is currently generated and hosted by readthedocs:
 https://xoa.readthedocs.io
 
 Sources and help
 -----------------
 
 Sources are available on the xoa github page:
-https://github.com/VACUMM/xoa.
+https://github.com/shom-fr/xoa.
 Here you can also
-participate to `discussions <https://github.com/VACUMM/xoa/discussions>`_
+participate to `discussions <https://github.com/shom-fr/xoa/discussions>`_
 and post tickets for
-`requests <https://github.com/VACUMM/xoa/pulls>`_ and
-`issues <https://github.com/VACUMM/xoa/issues>`_.
+`requests <https://github.com/shom-fr/xoa/pulls>`_ and
+`issues <https://github.com/shom-fr/xoa/issues>`_.
 
 License
 -------
 
 xoa is a property of `Shom <https://www.shom.fr>`_
 and is published under the
 `Apache 2.0 license <https://www.apache.org/licenses/LICENSE-2.0>`_.
-
-
```

### Comparing `xoa-0.6.1/README.rst` & `xoa-0.7.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,64 @@
 xoa - xarray-based ocean analysis library
 =========================================
 
-.. image:: https://anaconda.org/conda-forge/xoa/badges/installer/conda.svg
-    :alt: Install with conda
-    :target: https://conda.anaconda.org/conda-forge
-.. image:: https://github.com/VACUMM/xoa/actions/workflows/python-package-conda.yml/badge.svg
+.. image:: https://github.com/shom-fr/xoa/actions/workflows/python-package-conda.yml/badge.svg
     :alt: Install, linting and tests
+.. image:: https://anaconda.org/conda-forge/xoa/badges/version.svg
+    :alt: Available on conda-forge
+    :target: https://conda.anaconda.org/conda-forge/xoa
 .. image:: https://readthedocs.org/projects/docs/badge/?version=latest
     :alt: Documentation Status
     :target: https://xoa.readthedocs.io/en/latest/
 .. image:: https://anaconda.org/conda-forge/xoa/badges/downloads.svg
     :alt: Number of downloads on anaconda.org/conda-forge
     :target: https://anaconda.org/conda-forge/xoa/
 .. image:: https://pepy.tech/badge/xoa
     :alt: Number of downloads on pypi
     :target: https://pypi.org/project/xoa
+.. image:: https://anaconda.org/conda-forge/xoa/badges/platforms.svg
+    :alt: noarch
+    :target: https://anaconda.org/conda-forge/xoa
+.. image:: https://anaconda.org/conda-forge/xoa/badges/license.svg
+    :alt: Apache 2.0
+    :target: https://anaconda.org/conda-forge/xoa
 
 xoa is intended to help reading and manipulating observed
 and simulated ocean data.
 It is heavily based on `xarray <http://xarray.pydata.org/en/stable/>`_.
 For those who know it, it is the successor of
 `vacumm <https://github.com/VACUMM/vacumm>`_.
 
+Installation
+------------
+
+From conda::
+
+   conda install -c conda-forge xoa
+
+From pypi::
+
+   pip install xoa
+
 Documentation
 -------------
 
 The xoa documentation is currently generated and hosted by readthedocs:
 https://xoa.readthedocs.io
 
 Sources and help
 -----------------
 
 Sources are available on the xoa github page:
-https://github.com/VACUMM/xoa.
+https://github.com/shom-fr/xoa.
 Here you can also
-participate to `discussions <https://github.com/VACUMM/xoa/discussions>`_
+participate to `discussions <https://github.com/shom-fr/xoa/discussions>`_
 and post tickets for
-`requests <https://github.com/VACUMM/xoa/pulls>`_ and
-`issues <https://github.com/VACUMM/xoa/issues>`_.
+`requests <https://github.com/shom-fr/xoa/pulls>`_ and
+`issues <https://github.com/shom-fr/xoa/issues>`_.
 
 License
 -------
 
 xoa is a property of `Shom <https://www.shom.fr>`_
 and is published under the
 `Apache 2.0 license <https://www.apache.org/licenses/LICENSE-2.0>`_.
```

### Comparing `xoa-0.6.1/ROADMAP.rst` & `xoa-0.7.0/ROADMAP.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/Makefile` & `xoa-0.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/_static/custom.css` & `xoa-0.7.0/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/_templates/autosummary/class.rst` & `xoa-0.7.0/doc/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/_templates/autosummary/module.rst` & `xoa-0.7.0/doc/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/accessors.rst` & `xoa-0.7.0/doc/accessors.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/appendix.cf.rst` & `xoa-0.7.0/doc/appendix.cf.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/cli.rst` & `xoa-0.7.0/doc/cli.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/conf.py` & `xoa-0.7.0/doc/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,28 +114,28 @@
 import xoa.cf
 
 cfgm_get_cfgm_func = xoa.cf._get_cfgm_
 cfgm_rst_file = "cf.txt"
 
 # %% Extlinks
 extlinks = {
-    "issue": ("https://github.com/pydata/xarray/issues/%s", "GH"),
-    "pull": ("https://github.com/pydata/xarray/pull/%s", "PR"),
+    "issue": ("https://github.com/shom-fr/xoa/issues/%s", "GH"),
+    "pull": ("https://github.com/shom-fr/xoa/pulls/%s", "PR"),
 }
 
 # %% Nbsphinx
 # nbsphinx_timeout = 120  # in seconds
 
 # %% Sphinx gallery
 warnings.simplefilter("ignore", MatplotlibDeprecationWarning)
 sphinx_gallery_conf = {
     "examples_dirs": "../examples",
     "gallery_dirs": "examples",
     "binder": {
-        'org': 'VACUMM',
+        'org': 'shom-fr',
         'repo': 'xoa',
         'branch': 'master',
         'binderhub_url': 'https://mybinder.org',
         'dependencies': ['./binder/environment.yml', './binder/apt.txt', './binder/setup.py'],
         'notebooks_dir': 'notebooks',
         'use_jupyter_lab': True,
     },
```

### Comparing `xoa-0.6.1/doc/configure.rst` & `xoa-0.7.0/doc/configure.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/ext/gencfspecs.py` & `xoa-0.7.0/doc/ext/gencfspecs.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/ext/genfortran.py` & `xoa-0.7.0/doc/ext/genfortran.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/ext/genoptions.py` & `xoa-0.7.0/doc/ext/genoptions.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/howtostart.rst` & `xoa-0.7.0/doc/howtostart.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/install.rst` & `xoa-0.7.0/doc/install.rst`

 * *Files 2% similar despite different names*

```diff
@@ -55,13 +55,13 @@
 
 
 From sources
 ------------
 
 Clone the repository::
 
-    $ git clone https://github.com/VACUMM/xoa.git
+    $ git clone https://github.com/shom-fr/xoa.git
 
 Run the installation command::
 
     $ cd xoa
     $ python setup.py install
```

### Comparing `xoa-0.6.1/doc/uses.cf.rst` & `xoa-0.7.0/doc/uses.cf.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/uses.cfgm.cfg2rst.txt` & `xoa-0.7.0/doc/uses.cfgm.cfg2rst.txt`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/doc/uses.cfgm.rst` & `xoa-0.7.0/doc/uses.cfgm.rst`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/examples/plot_hycom_gdp.py` & `xoa-0.7.0/examples/plot_hycom_gdp.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import matplotlib.pyplot as plt
 import cartopy.crs as ccrs
 import xoa
 from xoa.grid import dz2depth, shift
 from xoa.regrid import grid2loc, regrid1d
 import xoa.cf as xcf
 import xoa.geo as xgeo
-from xoa.plot import plot_flow
+from xoa.plot import plot_flow, plot_double_minimap
 
 xr.set_options(display_style="text")
 
 # %%
 # Register the :ref:`xoa <accessors>` accessors:
 
 xoa.register_accessors()
@@ -171,15 +171,16 @@
 # ----
 #
 # The geographic extent is easily computed with the :func:`xoa.geo.get_extent` function.
 # The background currents are plotted with the :func:`xoa.plot.plot_flow` function.
 
 pmerc = ccrs.Mercator()
 pcarr = ccrs.PlateCarree()
-fig, ax = plt.subplots(figsize=(7, 7), subplot_kw={"facecolor": "teal", "projection": pmerc})
+fig, ax = plt.subplots(figsize=(8, 7), subplot_kw={"facecolor": "teal", "projection": pmerc})
+plt.subplots_adjust(right=0.85)
 ax.gridlines(draw_labels=True, dms=True)
 ax.set_extent(xgeo.get_extent(uh15))
 kwqv = dict(scale_units="dots", scale=0.1 / 20, units="dots", transform=pcarr)
 plot_flow(uh15, vh15, axes=ax, transform=pcarr, color="w", alpha=(0.3, 1), linewidth=0.6)
 qv = ax.quiver(
     uloc.lon.values,
     uloc.lat.values,
@@ -199,13 +200,14 @@
     color="C1",
     label="Drifter",
     width=2,
     **kwqv,
 )
 plt.quiverkey(qv, 0.1, 1.06, 0.1, r"0.1 $m\,s^{-1}$", color="k", alpha=1, labelpos="E")
 plt.legend()
+plot_double_minimap(drifter);
 
 # %%
 # The discrepancies between the lagrangian and mean eulerian currents highlight
 # the variability due to the mesocale activity.
 # The differences between the observed and modeled currents are partly due to
 # the lack of data assimilation in the model.
```

### Comparing `xoa-0.6.1/examples/plot_mercator_argo.py` & `xoa-0.7.0/examples/plot_mercator_argo.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,15 +185,17 @@
     ds_merc_prof.sal + 1.96 * ds_merc_ens_std.sal,
     fc="C1",
     alpha=0.2,
 )
 ds_merc_prof.sal.plot(y="depth", color="C1", label="Mercator")
 plt.plot(ds_merc_prof.sal.values, ds_merc_prof.depth, "o-", color="C1")
 ds_argo_prof.sal.plot(y="depth", label="ARGO", color="C0")
-plt.legend();
+plt.title("Uncertain profile")
+plt.legend()
+xplot.plot_double_minimap(ds_argo_prof, regional_ax="left", global_ax=(0.88, 0.88, 0.11),);
 
 # %%
 # Therefore, if we accept an uncertainty in the positioning of the ocean
 # structure in the model, it differences with (assimilated) observations
 # become acceptables.
 
 # %%
```

### Comparing `xoa-0.6.1/setup.cfg` & `xoa-0.7.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -48,19 +48,19 @@
 [options.entry_points]
 console_scripts = 
 	xoa = xoa.cli:main
 
 [flake8]
 max-line-length = 100
 ignore = 
-	E203 # whitespace before ':' - doesn't work well with black
-	E402 # module level import not at top of file
-	E501 # line too long - let black worry about that
-	E731 # do not assign a lambda expression, use a def
-	W503 # line break before binary operator
+	E203,
+	E402,
+	E501,
+	E731,
+	W503
 exclude = 
 	.eggs
 	doc
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `xoa-0.6.1/setup.py` & `xoa-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/__init__.py` & `xoa-0.7.0/xoa/__init__.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/_samples/argo-7900573.nc` & `xoa-0.7.0/xoa/_samples/argo-7900573.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/_samples/croco.cfg` & `xoa-0.7.0/xoa/_samples/croco.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [register]
 name=croco
 
     [[attrs]]
     ini_file=*CROCO*
+    type=*ROMS*
 
 [sglocator]
 valid_locations=rho,w,u,v,r
 
 [accessors]
 
     [[properties]]
```

### Comparing `xoa-0.6.1/xoa/_samples/croco.south-africa.meridional.nc` & `xoa-0.7.0/xoa/_samples/croco.south-africa.meridional.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/_samples/croco.south-africa.surf.nc` & `xoa-0.7.0/xoa/_samples/croco.south-africa.surf.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/_samples/croco.south-africa.zonal.nc` & `xoa-0.7.0/xoa/_samples/croco.south-africa.zonal.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/_samples/gdp-6203641.csv` & `xoa-0.7.0/xoa/_samples/gdp-6203641.csv`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/_samples/hycom.gdp.h.nc` & `xoa-0.7.0/xoa/_samples/hycom.gdp.h.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/_samples/hycom.gdp.u.nc` & `xoa-0.7.0/xoa/_samples/hycom.gdp.u.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/_samples/hycom.gdp.v.nc` & `xoa-0.7.0/xoa/_samples/hycom.gdp.v.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/_samples/ibi-argo-7900573.nc` & `xoa-0.7.0/xoa/_samples/ibi-argo-7900573.nc`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/accessors.py` & `xoa-0.7.0/xoa/accessors.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/cf.cfg` & `xoa-0.7.0/xoa/cf.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,57 @@
     [[ptemp]]
     cmap = cmo.thermal
         [[[attrs]]]
         standard_name = sea_water_potential_temperature
         long_name = Potential temperature
         units = degrees_celsius
 
+    [[ctemp]]
+    cmap = cmo.thermal
+        [[[attrs]]]
+        standard_name = sea_water_conservative_temperature
+        long_name = Conservative temperature
+        units = degrees_celsius
 
     [[temp]]
-    inherit = ptemp
     alt_names = temperature
+    cmap = cmo.thermal
         [[[attrs]]]
         standard_name = sea_water_temperature
-        long_name = Temperature
+        long_name = Sea water in situ temperature
+        units = degrees_celsius,kelvin
+
+    [[asal]]
+    cmap = cmo.haline
+        [[[attrs]]]
+        standard_name = sea_water_absolute_salinity
+        long_name = Absolute salinity
+        units = g kg-1
+
+    [[pfsal]]
+    cmap = cmo.haline
+        [[[attrs]]]
+        standard_name = sea_water_preformed_salinity
+        long_name = Preformed salinity
+        units = g kg-1
+
+    [[psal]]
+    cmap = cmo.haline
+        [[[attrs]]]
+        standard_name = sea_water_practical_salinity
+        long_name = Practical salinity
+        units = 1,PSU
 
     [[sal]]
-    alt_names = psal,salinity
+    alt_names = salinity,salt,saln
     cmap = cmo.haline
         [[[attrs]]]
         standard_name = sea_water_salinity
         long_name = Salinity
-        units = 1e-3,PSU
+        units = 1e-3
 
     [[sst]]
     cmap = cmo.thermal
         [[[attrs]]]
         standard_name = sea_surface_temperature,surface_sea_water_temperature
         long_name = Sea surface temperature
         units = degrees_celsius
@@ -36,21 +64,14 @@
     [[sss]]
     cmap = cmo.haline
         [[[attrs]]]
         standard_name = sea_surface_salinity
         long_name = Sea surface salinity
         units = PSU
 
-    [[dens]]
-    cmap = cmo.dense
-        [[[attrs]]]
-        standard_name = sea_water_density
-        long_name = Sea water density
-        units = kg m-3
-
     [[sigmat]]
     cmap = cmo.dense
         [[[attrs]]]
         standard_name = sea_water_sigma_t
         long_name = Sea water density minus 1000
         units = kg m-3
 
@@ -79,39 +100,42 @@
     [[sigma0]]
     inherit = pdens
     cmap = cmo.dense
 
     [[sigma1]]
     cmap = cmo.dense
         [[[attrs]]]
-        standard_name = sea_water_potential_density
         long_name = Sea water potential density with ref at 1000 dbar
         units = kg m-3
 
     [[sigma2]]
     cmap = cmo.dense
         [[[attrs]]]
-        standard_name = sea_water_potential_density
         long_name = Sea water potential density with ref at 2000 dbar
         units = kg m-3
 
     [[sigma3]]
     cmap = cmo.dense
         [[[attrs]]]
-        standard_name = sea_water_potential_density
         long_name = Sea water potential density with ref at 3000 dbar
         units = kg m-3
 
     [[sigma4]]
     cmap = cmo.dense
         [[[attrs]]]
-        standard_name = sea_water_potential_density
         long_name = Sea water potential density with ref at 4000 dbar
         units = kg m-3
 
+    [[dens]]
+    cmap = cmo.dense
+        [[[attrs]]]
+        standard_name = sea_water_density
+        long_name = Sea water density
+        units = kg m-3
+
     [[pres]]
         [[[attrs]]]
         standard_name = sea_water_pressure
         long_name = Sea water pressure
         units = dbar
 
     [[ssd]]
@@ -996,14 +1020,28 @@
     alt_names = altitudet,altitudeu,altitudev
     cmap = cmo.deep
         [[[attrs]]]
         standard_name = atmosphere_layer_altitude
         long_name = Altitude
         units = hPa,m
 
+    # Misc
+    [[station]]
+    alt_names = stations
+        [[[attrs]]]
+        long_name = Station number
+
+    [[calday]]
+        [[[attrs]]]
+        long_name = Calendar day
+
+    [[echoint]]
+        [[[attrs]]]
+        long_name = Echo intensity
+        units = db
 
 [coords]
 
     # Non physical
 
     [[x]]
     alt_names = xi,nx,ni,x,imt,ipi
@@ -1079,15 +1117,15 @@
     [[freq]]
     alt_names = frequency
         [[[attrs]]]
         long_name = Frequency
         units = s-1
 
     [[station]]
-    alt_names = stations
+    inherit = data_vars:station
         [[[attrs]]]
-        long_name = Station number
+        axis = Z
 
     [[member]]
     alt_names = members
         [[[attrs]]]
         long_name = Ensemble member
```

### Comparing `xoa-0.6.1/xoa/cf.ini` & `xoa-0.7.0/xoa/cf.ini`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/cf.py` & `xoa-0.7.0/xoa/cf.py`

 * *Files 0% similar despite different names*

```diff
@@ -2578,15 +2578,15 @@
 0000a110: 6f63 3d4e 6f6e 652c 0a20 2020 2020 2020  oc=None,.       
 0000a120: 2023 2061 6464 5f6c 6f63 5f74 6f5f 6e61   # add_loc_to_na
 0000a130: 6d65 3d4e 6f6e 652c 2061 6464 5f6c 6f63  me=None, add_loc
 0000a140: 5f74 6f5f 636f 6f72 645f 6e61 6d65 733d  _to_coord_names=
 0000a150: 4e6f 6e65 2c0a 2020 2020 2020 2020 7370  None,.        sp
 0000a160: 6563 6961 6c69 7a65 3d46 616c 7365 2c0a  ecialize=False,.
 0000a170: 2020 2020 2020 2020 7265 6e61 6d65 5f64          rename_d
-0000a180: 696d 733d 5472 7565 2c0a 2020 2020 2020  ims=True,.      
+0000a180: 696d 733d 4e6f 6e65 2c0a 2020 2020 2020  ims=None,.      
 0000a190: 2020 6361 7465 676f 7269 6573 3d5b 2263    categories=["c
 0000a1a0: 6f6f 7264 7322 2c20 2264 6174 615f 7661  oords", "data_va
 0000a1b0: 7273 225d 2c0a 2020 2020 293a 0a20 2020  rs"],.    ):.   
 0000a1c0: 2020 2020 2022 2222 4175 746f 2d66 6f72       """Auto-for
 0000a1d0: 6d61 7420 6120 7768 6f6c 6520 7861 7272  mat a whole xarr
 0000a1e0: 6179 2e44 6174 6173 6574 0a0a 2020 2020  ay.Dataset..    
 0000a1f0: 2020 2020 5365 6520 616c 736f 0a20 2020      See also.   
@@ -2597,5005 +2597,5021 @@
 0000a240: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
 0000a250: 2043 6f70 790a 2020 2020 2020 2020 6966   Copy.        if
 0000a260: 2063 6f70 793a 0a20 2020 2020 2020 2020   copy:.         
 0000a270: 2020 206f 626a 203d 206f 626a 2e63 6f70     obj = obj.cop
 0000a280: 7928 290a 0a20 2020 2020 2020 2023 2049  y()..        # I
 0000a290: 6e69 7420 7265 6e61 6d65 2064 6963 740a  nit rename dict.
 0000a2a0: 2020 2020 2020 2020 7265 6e61 6d65 5f61          rename_a
-0000a2b0: 7267 7320 3d20 7b7d 0a0a 2020 2020 2020  rgs = {}..      
-0000a2c0: 2020 2320 436f 6d6d 6f6e 2066 6f72 6d61    # Common forma
-0000a2d0: 7474 696e 6720 6b77 6172 6773 0a20 2020  tting kwargs.   
-0000a2e0: 2020 2020 206b 7761 7267 7320 3d20 6469       kwargs = di
-0000a2f0: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
-0000a300: 636f 7079 3d46 616c 7365 2c0a 2020 2020  copy=False,.    
-0000a310: 2020 2020 2020 2020 7265 6e61 6d65 3d46          rename=F
-0000a320: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-0000a330: 2020 7265 706c 6163 655f 6174 7472 733d    replace_attrs=
-0000a340: 7265 706c 6163 655f 6174 7472 732c 0a20  replace_attrs,. 
-0000a350: 2020 2020 2020 2020 2020 2073 7461 6e64             stand
-0000a360: 6172 6469 7a65 3d54 7275 652c 0a20 2020  ardize=True,.   
-0000a370: 2020 2020 2020 2020 2073 7065 6369 616c           special
-0000a380: 697a 653d 7370 6563 6961 6c69 7a65 2c0a  ize=specialize,.
-0000a390: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000a3a0: 2020 2023 2053 7461 6767 6172 6564 2067     # Staggared g
-0000a3b0: 7269 6420 6c6f 6361 7469 6f6e 730a 2020  rid locations.  
-0000a3c0: 2020 2020 2020 6c6f 6361 7469 6f6e 7320        locations 
-0000a3d0: 3d20 7365 6c66 2e67 6574 5f6c 6f63 5f6d  = self.get_loc_m
-0000a3e0: 6170 7069 6e67 286f 626a 2c20 6366 5f6e  apping(obj, cf_n
-0000a3f0: 616d 6573 3d63 665f 6e61 6d65 732c 206c  ames=cf_names, l
-0000a400: 6f63 3d6c 6f63 2c20 6361 7465 676f 7269  oc=loc, categori
-0000a410: 6573 3d63 6174 6567 6f72 6965 7329 0a0a  es=categories)..
-0000a420: 2020 2020 2020 2020 2320 4461 7461 2061          # Data a
-0000a430: 7272 6179 730a 2020 2020 2020 2020 6973  rrays.        is
-0000a440: 5f64 6174 6173 6574 203d 2068 6173 6174  _dataset = hasat
-0000a450: 7472 286f 626a 2c20 2264 6174 615f 7661  tr(obj, "data_va
-0000a460: 7273 2229 0a20 2020 2020 2020 2069 6620  rs").        if 
-0000a470: 6973 5f64 6174 6173 6574 3a20 2023 2064  is_dataset:  # d
-0000a480: 6174 6173 6574 0a20 2020 2020 2020 2020  ataset.         
-0000a490: 2020 2064 6174 615f 7661 7273 203d 206f     data_vars = o
-0000a4a0: 626a 2e76 616c 7565 7328 290a 2020 2020  bj.values().    
-0000a4b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000a4c0: 2020 2020 2020 6461 7461 5f76 6172 7320        data_vars 
-0000a4d0: 3d20 5b6f 626a 5d0a 2020 2020 2020 2020  = [obj].        
-0000a4e0: 666f 7220 6461 2069 6e20 6461 7461 5f76  for da in data_v
-0000a4f0: 6172 733a 0a20 2020 2020 2020 2020 2020  ars:.           
-0000a500: 2066 6f72 2063 6174 2069 6e20 6361 7465   for cat in cate
-0000a510: 676f 7269 6573 3a0a 2020 2020 2020 2020  gories:.        
-0000a520: 2020 2020 2020 2020 6366 5f6e 616d 6520          cf_name 
-0000a530: 3d20 6366 5f6e 616d 6573 2e67 6574 2864  = cf_names.get(d
-0000a540: 612e 6e61 6d65 2920 6966 2063 665f 6e61  a.name) if cf_na
-0000a550: 6d65 7320 656c 7365 204e 6f6e 650a 2020  mes else None.  
-0000a560: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000a570: 2063 665f 6e61 6d65 2061 6e64 2063 665f   cf_name and cf_
-0000a580: 6e61 6d65 206e 6f74 2069 6e20 7365 6c66  name not in self
-0000a590: 5b63 6174 5d3a 0a20 2020 2020 2020 2020  [cat]:.         
-0000a5a0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-0000a5b0: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
-0000a5c0: 2020 2020 6e65 775f 6e61 6d65 203d 2073      new_name = s
-0000a5d0: 656c 665b 6361 745d 2e66 6f72 6d61 745f  elf[cat].format_
-0000a5e0: 6461 7461 6172 7261 7928 0a20 2020 2020  dataarray(.     
-0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000a600: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-0000a610: 2020 2020 2020 2063 665f 6e61 6d65 3d63         cf_name=c
-0000a620: 665f 6e61 6d65 2c0a 2020 2020 2020 2020  f_name,.        
-0000a630: 2020 2020 2020 2020 2020 2020 6174 7472              attr
-0000a640: 733d 6174 7472 7320 6966 2069 7369 6e73  s=attrs if isins
-0000a650: 7461 6e63 6528 6174 7472 732c 2062 6f6f  tance(attrs, boo
-0000a660: 6c29 2065 6c73 6520 6174 7472 732e 6765  l) else attrs.ge
-0000a670: 7428 6461 2e6e 616d 6529 2c0a 2020 2020  t(da.name),.    
-0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a690: 2320 666f 726d 6174 5f63 6f6f 7264 733d  # format_coords=
-0000a6a0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-0000a6b0: 2020 2020 2020 2020 2020 206c 6f63 3d6c             loc=l
-0000a6c0: 6f63 6174 696f 6e73 2e67 6574 2864 612e  ocations.get(da.
-0000a6d0: 6e61 6d65 292c 0a20 2020 2020 2020 2020  name),.         
-0000a6e0: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-0000a6f0: 7267 732c 0a20 2020 2020 2020 2020 2020  rgs,.           
-0000a700: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000a710: 2020 2020 2020 2069 6620 6e65 775f 6e61         if new_na
-0000a720: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
-0000a730: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
-0000a740: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a760: 6e65 775f 6e61 6d65 203d 204e 6f6e 650a  new_name = None.
-0000a770: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-0000a780: 656e 616d 6520 616e 6420 6e65 775f 6e61  ename and new_na
-0000a790: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
-0000a7a0: 2020 2020 6966 2069 735f 6461 7461 7365      if is_datase
-0000a7b0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0000a7c0: 2020 2020 2020 2072 656e 616d 655f 6172         rename_ar
-0000a7d0: 6773 5b64 612e 6e61 6d65 5d20 3d20 6e65  gs[da.name] = ne
-0000a7e0: 775f 6e61 6d65 0a20 2020 2020 2020 2020  w_name.         
-0000a7f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a810: 2064 612e 6e61 6d65 203d 206e 6577 5f6e   da.name = new_n
-0000a820: 616d 650a 0a20 2020 2020 2020 2023 2043  ame..        # C
-0000a830: 6f6f 7264 696e 6174 6573 0a20 2020 2020  oordinates.     
-0000a840: 2020 2069 6620 666f 726d 6174 5f63 6f6f     if format_coo
-0000a850: 7264 733a 0a20 2020 2020 2020 2020 2020  rds:.           
-0000a860: 2023 2066 6f72 2063 6e61 6d65 2c20 6364   # for cname, cd
-0000a870: 6120 696e 206c 6973 7428 6f62 6a2e 636f  a in list(obj.co
-0000a880: 6f72 6473 2e69 7465 6d73 2829 293a 0a20  ords.items()):. 
-0000a890: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-0000a8a0: 6e61 6d65 2069 6e20 5f6c 6973 745f 7872  name in _list_xr
-0000a8b0: 5f6e 616d 6573 5f28 6f62 6a2c 2064 6174  _names_(obj, dat
-0000a8c0: 615f 7661 7273 3d46 616c 7365 2c20 6469  a_vars=False, di
-0000a8d0: 6d73 3d46 616c 7365 293a 0a20 2020 2020  ms=False):.     
-0000a8e0: 2020 2020 2020 2020 2020 2063 6461 203d             cda =
-0000a8f0: 206f 626a 2e63 6f6f 7264 735b 636e 616d   obj.coords[cnam
-0000a900: 655d 0a20 2020 2020 2020 2020 2020 2020  e].             
-0000a910: 2020 206e 6577 5f63 6f6f 7264 5f6e 616d     new_coord_nam
-0000a920: 6520 3d20 7365 6c66 2e63 6f6f 7264 732e  e = self.coords.
-0000a930: 666f 726d 6174 5f64 6174 6161 7272 6179  format_dataarray
-0000a940: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000a950: 2020 2020 2020 6364 612c 0a20 2020 2020        cda,.     
-0000a960: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000a970: 665f 6e61 6d65 3d63 665f 6e61 6d65 732e  f_name=cf_names.
-0000a980: 6765 7428 636e 616d 6529 2069 6620 6973  get(cname) if is
-0000a990: 696e 7374 616e 6365 2863 665f 6e61 6d65  instance(cf_name
-0000a9a0: 732c 2064 6963 7429 2065 6c73 6520 4e6f  s, dict) else No
-0000a9b0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0000a9c0: 2020 2020 2020 2020 6174 7472 733d 6174          attrs=at
-0000a9d0: 7472 7320 6966 2069 7369 6e73 7461 6e63  trs if isinstanc
-0000a9e0: 6528 6174 7472 732c 2062 6f6f 6c29 2065  e(attrs, bool) e
-0000a9f0: 6c73 6520 6174 7472 732e 6765 7428 636e  lse attrs.get(cn
-0000aa00: 616d 652c 2054 7275 6529 2c0a 2020 2020  ame, True),.    
-0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa20: 2320 7265 6c61 7465 643d 6f62 6a2c 0a20  # related=obj,. 
-0000aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa40: 2020 2023 2066 6f72 6d61 745f 636f 6f72     # format_coor
-0000aa50: 6473 3d46 616c 7365 2c0a 2020 2020 2020  ds=False,.      
-0000aa60: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000aa70: 6c6f 633d 6c6f 632c 2061 6464 5f6c 6f63  loc=loc, add_loc
-0000aa80: 5f74 6f5f 6e61 6d65 3d61 6464 5f6c 6f63  _to_name=add_loc
-0000aa90: 5f74 6f5f 636f 6f72 645f 6e61 6d65 732c  _to_coord_names,
-0000aaa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000aab0: 2020 2020 206c 6f63 3d6c 6f63 6174 696f       loc=locatio
-0000aac0: 6e73 2e67 6574 2863 6461 2e6e 616d 6529  ns.get(cda.name)
-0000aad0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000aae0: 2020 2020 2020 2320 7265 6e61 6d65 5f64        # rename_d
-0000aaf0: 696d 3d46 616c 7365 2c0a 2020 2020 2020  im=False,.      
-0000ab00: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
-0000ab10: 6b77 6172 6773 2c0a 2020 2020 2020 2020  kwargs,.        
-0000ab20: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000ab30: 2020 2020 2020 2020 2020 6966 2072 656e            if ren
-0000ab40: 616d 6520 616e 6420 6e65 775f 636f 6f72  ame and new_coor
-0000ab50: 645f 6e61 6d65 3a0a 2020 2020 2020 2020  d_name:.        
-0000ab60: 2020 2020 2020 2020 2020 2020 7265 6e61              rena
-0000ab70: 6d65 5f61 7267 735b 6364 612e 6e61 6d65  me_args[cda.name
-0000ab80: 5d20 3d20 6e65 775f 636f 6f72 645f 6e61  ] = new_coord_na
-0000ab90: 6d65 0a0a 2020 2020 2020 2020 2320 4469  me..        # Di
-0000aba0: 6d65 6e73 696f 6e73 0a20 2020 2020 2020  mensions.       
-0000abb0: 2069 6620 7265 6e61 6d65 5f64 696d 733a   if rename_dims:
-0000abc0: 0a20 2020 2020 2020 2020 2020 2072 656e  .            ren
-0000abd0: 616d 655f 6469 6d73 5f61 7267 7320 3d20  ame_dims_args = 
-0000abe0: 7365 6c66 2e63 6f6f 7264 732e 6765 745f  self.coords.get_
-0000abf0: 7265 6e61 6d65 5f64 696d 735f 6172 6773  rename_dims_args
-0000ac00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000ac10: 2020 6f62 6a2c 206c 6f63 6174 696f 6e73    obj, locations
-0000ac20: 3d6c 6f63 6174 696f 6e73 2c20 7370 6563  =locations, spec
-0000ac30: 6961 6c69 7a65 3d73 7065 6369 616c 697a  ialize=specializ
-0000ac40: 650a 2020 2020 2020 2020 2020 2020 2920  e.            ) 
-0000ac50: 2023 202c 2065 7863 6c75 6465 3d6c 6973   # , exclude=lis
-0000ac60: 7428 7265 6e61 6d65 5f61 7267 732e 6b65  t(rename_args.ke
-0000ac70: 7973 2829 2929 0a20 2020 2020 2020 2020  ys())).         
-0000ac80: 2020 2072 656e 616d 655f 6172 6773 2e75     rename_args.u
-0000ac90: 7064 6174 6528 7265 6e61 6d65 5f64 696d  pdate(rename_dim
-0000aca0: 735f 6172 6773 290a 0a20 2020 2020 2020  s_args)..       
-0000acb0: 2023 2046 696e 616c 2072 656e 616d 696e   # Final renamin
-0000acc0: 670a 2020 2020 2020 2020 6966 2072 656e  g.        if ren
-0000acd0: 616d 6520 616e 6420 7265 6e61 6d65 5f61  ame and rename_a
-0000ace0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000acf0: 205f 736f 6c76 655f 7265 6e61 6d65 5f63   _solve_rename_c
-0000ad00: 6f6e 666c 6963 7473 5f28 7265 6e61 6d65  onflicts_(rename
-0000ad10: 5f61 7267 7329 0a20 2020 2020 2020 2020  _args).         
-0000ad20: 2020 206f 626a 203d 206f 626a 2e72 656e     obj = obj.ren
-0000ad30: 616d 6528 7265 6e61 6d65 5f61 7267 7329  ame(rename_args)
-0000ad40: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000ad50: 206f 626a 0a0a 2020 2020 6465 6620 666f   obj..    def fo
-0000ad60: 726d 6174 5f63 6f6f 7264 280a 2020 2020  rmat_coord(.    
-0000ad70: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000ad80: 2020 6461 2c0a 2020 2020 2020 2020 6366    da,.        cf
-0000ad90: 5f6e 616d 653d 4e6f 6e65 2c0a 2020 2020  _name=None,.    
-0000ada0: 2020 2020 6c6f 633d 4e6f 6e65 2c0a 2020      loc=None,.  
-0000adb0: 2020 2020 2020 636f 7079 3d54 7275 652c        copy=True,
-0000adc0: 0a20 2020 2020 2020 2066 6f72 6d61 745f  .        format_
-0000add0: 636f 6f72 6473 3d54 7275 652c 0a20 2020  coords=True,.   
-0000ade0: 2020 2020 2073 7461 6e64 6172 6469 7a65       standardize
-0000adf0: 3d54 7275 652c 0a20 2020 2020 2020 2072  =True,.        r
-0000ae00: 656e 616d 653d 5472 7565 2c0a 2020 2020  ename=True,.    
-0000ae10: 2020 2020 7370 6563 6961 6c69 7a65 3d46      specialize=F
-0000ae20: 616c 7365 2c0a 2020 2020 2020 2020 6174  alse,.        at
-0000ae30: 7472 733d 5472 7565 2c0a 2020 2020 2020  trs=True,.      
-0000ae40: 2020 7265 706c 6163 655f 6174 7472 733d    replace_attrs=
-0000ae50: 4661 6c73 652c 0a20 2020 2020 2020 2023  False,.        #
-0000ae60: 2061 6464 5f6c 6f63 5f74 6f5f 6e61 6d65   add_loc_to_name
-0000ae70: 3d4e 6f6e 652c 0a20 2020 2020 2020 2072  =None,.        r
-0000ae80: 656e 616d 655f 6469 6d73 3d54 7275 652c  ename_dims=True,
-0000ae90: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-0000aea0: 2222 2246 6f72 6d61 7420 6120 636f 6f72  """Format a coor
-0000aeb0: 6469 6e61 7465 2061 7272 6179 0a0a 2020  dinate array..  
-0000aec0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0000aed0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000aee0: 2d2d 2d0a 2020 2020 2020 2020 6461 3a20  ---.        da: 
-0000aef0: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-0000af00: 0a20 2020 2020 2020 2063 665f 6e61 6d65  .        cf_name
-0000af10: 3a20 7374 722c 204e 6f6e 650a 2020 2020  : str, None.    
-0000af20: 2020 2020 2020 2020 4120 6765 6e65 7269          A generi
-0000af30: 6320 4346 206e 616d 652e 2049 6620 6e6f  c CF name. If no
-0000af40: 7420 7072 6f76 6964 6564 2c20 6974 2067  t provided, it g
-0000af50: 7565 7373 6564 2077 6974 6820 3a6d 6574  uessed with :met
-0000af60: 683a 606d 6174 6368 602e 0a20 2020 2020  h:`match`..     
-0000af70: 2020 206c 6f63 3a20 7374 722c 207b 2261     loc: str, {"a
-0000af80: 6e79 222c 204e 6f6e 657d 2c20 7b22 222c  ny", None}, {"",
-0000af90: 2046 616c 7365 7d0a 2020 2020 2020 2020   False}.        
-0000afa0: 2020 2020 2d20 7374 723a 206f 6e65 206f      - str: one o
-0000afb0: 6620 7468 6573 6520 6c6f 6361 7469 6f6e  f these location
-0000afc0: 730a 2020 2020 2020 2020 2020 2020 2d20  s.            - 
-0000afd0: 4e6f 6e65 206f 7220 2261 6e79 223a 2061  None or "any": a
-0000afe0: 6e79 0a20 2020 2020 2020 2020 2020 202d  ny.            -
-0000aff0: 2046 616c 7365 206f 7220 2722 223a 206e   False or '"": n
-0000b000: 6f20 6c6f 6361 7469 6f6e 0a20 2020 2020  o location.     
-0000b010: 2020 2072 656e 616d 653a 2062 6f6f 6c0a     rename: bool.
-0000b020: 2020 2020 2020 2020 2020 2020 5265 6e61              Rena
-0000b030: 6d65 2061 7272 6179 730a 2020 2020 2020  me arrays.      
-0000b040: 2020 6164 645f 6c6f 635f 746f 5f6e 616d    add_loc_to_nam
-0000b050: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
-0000b060: 2020 2020 4164 6420 6c6f 6320 746f 2074      Add loc to t
-0000b070: 6865 206e 616d 650a 2020 2020 2020 2020  he name.        
-0000b080: 7370 6563 6961 6c69 7a65 3a20 626f 6f6c  specialize: bool
-0000b090: 0a20 2020 2020 2020 2020 2020 2044 6f65  .            Doe
-0000b0a0: 7320 6e6f 7420 7573 6520 7468 6520 4346  s not use the CF
-0000b0b0: 206e 616d 6520 666f 7220 7265 6e61 6d69   name for renami
-0000b0c0: 6e67 2c20 6275 7420 7468 6520 6669 7273  ng, but the firs
-0000b0d0: 7420 6e61 6d65 0a20 2020 2020 2020 2020  t name.         
-0000b0e0: 2020 2061 7320 6c69 7374 6564 2069 6e20     as listed in 
-0000b0f0: 7370 6563 732c 2077 6869 6368 2069 7320  specs, which is 
-0000b100: 6765 6e65 7261 6c6c 7920 6120 7370 6563  generally a spec
-0000b110: 6961 6c69 7a65 6420 6f6e 652c 0a20 2020  ialized one,.   
-0000b120: 2020 2020 2020 2020 206c 696b 6520 6120           like a 
-0000b130: 6e61 6d65 2061 646f 7074 6564 2062 7920  name adopted by 
-0000b140: 7370 6563 6961 6c69 7a65 6420 6461 7461  specialized data
-0000b150: 7365 742e 0a20 2020 2020 2020 2073 7461  set..        sta
-0000b160: 6e64 6172 6469 7a65 3a20 626f 6f6c 0a20  ndardize: bool. 
-0000b170: 2020 2020 2020 2072 656e 616d 655f 6469         rename_di
-0000b180: 6d3a 2062 6f6f 6c0a 2020 2020 2020 2020  m: bool.        
-0000b190: 2020 2020 466f 7220 6120 3144 2061 7272      For a 1D arr
-0000b1a0: 6179 2c20 7265 6e61 6d65 2074 6865 2064  ay, rename the d
-0000b1b0: 696d 656e 7369 6f6e 2069 6620 6974 2068  imension if it h
-0000b1c0: 6173 2074 6865 2073 616d 6520 6e61 6d65  as the same name
-0000b1d0: 0a20 2020 2020 2020 2020 2020 2061 7320  .            as 
-0000b1e0: 7468 6520 6172 7261 792e 0a20 2020 2020  the array..     
-0000b1f0: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
-0000b200: 2069 7420 6973 2073 6574 2074 6f20 4661   it is set to Fa
-0000b210: 6c73 652c 2069 6620 6060 7265 6e61 6d65  lse, if ``rename
-0000b220: 6060 2069 7320 4661 6c73 652e 0a20 2020  `` is False..   
-0000b230: 2020 2020 2061 7474 7273 3a20 626f 6f6c       attrs: bool
-0000b240: 2c20 6469 6374 0a20 2020 2020 2020 2020  , dict.         
-0000b250: 2020 2049 6620 4661 6c73 652c 2064 6f65     If False, doe
-0000b260: 7320 6e6f 7420 6368 616e 6765 2061 7474  s not change att
-0000b270: 7269 6275 7465 7320 6174 2061 6c6c 2e0a  ributes at all..
-0000b280: 2020 2020 2020 2020 2020 2020 4966 2054              If T
-0000b290: 7275 652c 2075 7365 2043 6620 6174 7472  rue, use Cf attr
-0000b2a0: 6962 7574 6573 2e0a 2020 2020 2020 2020  ibutes..        
-0000b2b0: 2020 2020 4966 2061 2064 6963 742c 2075      If a dict, u
-0000b2c0: 7365 2074 6869 7320 6469 6374 2e0a 2020  se this dict..  
-0000b2d0: 2020 2020 2020 7265 706c 6163 655f 6174        replace_at
-0000b2e0: 7472 733a 2062 6f6f 6c0a 2020 2020 2020  trs: bool.      
-0000b2f0: 2020 2020 2020 5265 706c 6163 6520 6578        Replace ex
-0000b300: 6973 7469 6e67 2061 7474 7269 6275 7465  isting attribute
-0000b310: 733f 0a0a 2020 2020 2020 2020 5265 7475  s?..        Retu
-0000b320: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0000b330: 2d2d 2d0a 2020 2020 2020 2020 7861 7272  ---.        xarr
-0000b340: 6179 2e44 6174 6141 7272 6179 2c20 7374  ay.DataArray, st
-0000b350: 722c 204e 6f6e 650a 2020 2020 2020 2020  r, None.        
-0000b360: 2020 2020 5468 6520 666f 726d 6174 7465      The formatte
-0000b370: 6420 6172 7261 7920 6f72 2063 6f70 7920  d array or copy 
-0000b380: 6f66 2069 742e 0a20 2020 2020 2020 2020  of it..         
-0000b390: 2020 2054 6865 2043 4620 6e61 6d65 2c20     The CF name, 
-0000b3a0: 6769 7665 6e20 6f72 206d 6174 6368 696e  given or matchin
-0000b3b0: 672c 2069 6620 7265 6e61 6d65 2069 6620  g, if rename if 
-0000b3c0: 4661 6c73 653b 2061 6e64 204e 6f6e 650a  False; and None.
-0000b3d0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000b3e0: 6f74 206d 6174 6368 696e 672e 0a0a 2020  ot matching...  
-0000b3f0: 2020 2020 2020 5365 6520 616c 736f 0a20        See also. 
-0000b400: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0a         --------.
-0000b410: 2020 2020 2020 2020 4346 436f 6f72 6453          CFCoordS
-0000b420: 7065 6373 2e66 6f72 6d61 745f 6461 7461  pecs.format_data
-0000b430: 6172 7261 790a 2020 2020 2020 2020 2222  array.        ""
-0000b440: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-0000b450: 2073 656c 662e 5f66 6f72 6d61 745f 6f62   self._format_ob
-0000b460: 6a5f 280a 2020 2020 2020 2020 2020 2020  j_(.            
-0000b470: 6461 2c0a 2020 2020 2020 2020 2020 2020  da,.            
-0000b480: 6366 5f6e 616d 6573 3d7b 6461 2e6e 616d  cf_names={da.nam
-0000b490: 653a 2063 665f 6e61 6d65 7d2c 0a20 2020  e: cf_name},.   
-0000b4a0: 2020 2020 2020 2020 2063 6f70 793d 636f           copy=co
-0000b4b0: 7079 2c0a 2020 2020 2020 2020 2020 2020  py,.            
-0000b4c0: 7374 616e 6461 7264 697a 653d 7374 616e  standardize=stan
-0000b4d0: 6461 7264 697a 652c 0a20 2020 2020 2020  dardize,.       
-0000b4e0: 2020 2020 2072 656e 616d 653d 7265 6e61       rename=rena
-0000b4f0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-0000b500: 7265 6e61 6d65 5f64 696d 733d 7265 6e61  rename_dims=rena
-0000b510: 6d65 5f64 696d 732c 0a20 2020 2020 2020  me_dims,.       
-0000b520: 2020 2020 2066 6f72 6d61 745f 636f 6f72       format_coor
-0000b530: 6473 3d66 6f72 6d61 745f 636f 6f72 6473  ds=format_coords
-0000b540: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
-0000b550: 706c 6163 655f 6174 7472 733d 7265 706c  place_attrs=repl
-0000b560: 6163 655f 6174 7472 732c 0a20 2020 2020  ace_attrs,.     
-0000b570: 2020 2020 2020 2061 7474 7273 3d61 7474         attrs=att
-0000b580: 7273 2069 6620 6973 696e 7374 616e 6365  rs if isinstance
-0000b590: 2861 7474 7273 2c20 626f 6f6c 2920 656c  (attrs, bool) el
-0000b5a0: 7365 207b 6461 2e6e 616d 653a 2061 7474  se {da.name: att
-0000b5b0: 7273 7d2c 0a20 2020 2020 2020 2020 2020  rs},.           
-0000b5c0: 2073 7065 6369 616c 697a 653d 7370 6563   specialize=spec
-0000b5d0: 6961 6c69 7a65 2c0a 2020 2020 2020 2020  ialize,.        
-0000b5e0: 2020 2020 6361 7465 676f 7269 6573 3d5b      categories=[
-0000b5f0: 2263 6f6f 7264 7322 5d2c 0a20 2020 2020  "coords"],.     
-0000b600: 2020 2020 2020 206c 6f63 3d6c 6f63 2c0a         loc=loc,.
-0000b610: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-0000b620: 6566 2066 6f72 6d61 745f 6461 7461 5f76  ef format_data_v
-0000b630: 6172 280a 2020 2020 2020 2020 7365 6c66  ar(.        self
-0000b640: 2c0a 2020 2020 2020 2020 6461 2c0a 2020  ,.        da,.  
-0000b650: 2020 2020 2020 6366 5f6e 616d 653d 4e6f        cf_name=No
-0000b660: 6e65 2c0a 2020 2020 2020 2020 6c6f 633d  ne,.        loc=
-0000b670: 4e6f 6e65 2c0a 2020 2020 2020 2020 636f  None,.        co
-0000b680: 7079 3d54 7275 652c 0a20 2020 2020 2020  py=True,.       
-0000b690: 2072 656e 616d 653d 5472 7565 2c0a 2020   rename=True,.  
-0000b6a0: 2020 2020 2020 7265 6e61 6d65 5f64 696d        rename_dim
-0000b6b0: 733d 5472 7565 2c0a 2020 2020 2020 2020  s=True,.        
-0000b6c0: 7370 6563 6961 6c69 7a65 3d46 616c 7365  specialize=False
-0000b6d0: 2c0a 2020 2020 2020 2020 666f 726d 6174  ,.        format
-0000b6e0: 5f63 6f6f 7264 733d 5472 7565 2c0a 2020  _coords=True,.  
-0000b6f0: 2020 2020 2020 6174 7472 733d 5472 7565        attrs=True
-0000b700: 2c0a 2020 2020 2020 2020 7265 706c 6163  ,.        replac
-0000b710: 655f 6174 7472 733d 4661 6c73 652c 0a20  e_attrs=False,. 
-0000b720: 2020 2020 2020 2073 7461 6e64 6172 6469         standardi
-0000b730: 7a65 3d54 7275 652c 0a20 2020 2020 2020  ze=True,.       
-0000b740: 2023 2061 6464 5f6c 6f63 5f74 6f5f 6e61   # add_loc_to_na
-0000b750: 6d65 3d4e 6f6e 652c 0a20 2020 2029 3a0a  me=None,.    ):.
-0000b760: 2020 2020 2020 2020 2222 2246 6f72 6d61          """Forma
-0000b770: 7420 6120 6461 7461 5f76 6172 2061 7272  t a data_var arr
-0000b780: 6179 0a0a 2020 2020 2020 2020 5061 7261  ay..        Para
-0000b790: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0000b7a0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0000b7b0: 2020 6461 3a20 7861 7272 6179 2e44 6174    da: xarray.Dat
-0000b7c0: 6141 7272 6179 0a20 2020 2020 2020 2063  aArray.        c
-0000b7d0: 665f 6e61 6d65 3a20 7374 722c 204e 6f6e  f_name: str, Non
-0000b7e0: 650a 2020 2020 2020 2020 2020 2020 4120  e.            A 
-0000b7f0: 6765 6e65 7269 6320 4346 206e 616d 652e  generic CF name.
-0000b800: 2049 6620 6e6f 7420 7072 6f76 6964 6564   If not provided
-0000b810: 2c20 6974 2067 7565 7373 6564 2077 6974  , it guessed wit
-0000b820: 6820 3a6d 6574 683a 606d 6174 6368 602e  h :meth:`match`.
-0000b830: 0a20 2020 2020 2020 206c 6f63 3a20 7374  .        loc: st
-0000b840: 722c 207b 2261 6e79 222c 204e 6f6e 657d  r, {"any", None}
-0000b850: 2c20 7b22 222c 2046 616c 7365 7d0a 2020  , {"", False}.  
-0000b860: 2020 2020 2020 2020 2020 2d20 7374 723a            - str:
-0000b870: 206f 6e65 206f 6620 7468 6573 6520 6c6f   one of these lo
-0000b880: 6361 7469 6f6e 730a 2020 2020 2020 2020  cations.        
-0000b890: 2020 2020 2d20 4e6f 6e65 206f 7220 2261      - None or "a
-0000b8a0: 6e79 223a 2061 6e79 0a20 2020 2020 2020  ny": any.       
-0000b8b0: 2020 2020 202d 2046 616c 7365 206f 7220       - False or 
-0000b8c0: 2722 223a 206e 6f20 6c6f 6361 7469 6f6e  '"": no location
-0000b8d0: 0a20 2020 2020 2020 2072 656e 616d 653a  .        rename:
-0000b8e0: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
-0000b8f0: 2020 5265 6e61 6d65 2061 7272 6179 730a    Rename arrays.
-0000b900: 2020 2020 2020 2020 6164 645f 6c6f 635f          add_loc_
-0000b910: 746f 5f6e 616d 653a 2062 6f6f 6c0a 2020  to_name: bool.  
-0000b920: 2020 2020 2020 2020 2020 4164 6420 6c6f            Add lo
-0000b930: 6320 746f 2074 6865 206e 616d 650a 2020  c to the name.  
-0000b940: 2020 2020 2020 7370 6563 6961 6c69 7a65        specialize
-0000b950: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
-0000b960: 2020 2044 6f65 7320 6e6f 7420 7573 6520     Does not use 
-0000b970: 7468 6520 4346 206e 616d 6520 666f 7220  the CF name for 
-0000b980: 7265 6e61 6d69 6e67 2c20 6275 7420 7468  renaming, but th
-0000b990: 6520 6669 7273 7420 6e61 6d65 0a20 2020  e first name.   
-0000b9a0: 2020 2020 2020 2020 2061 7320 6c69 7374           as list
-0000b9b0: 6564 2069 6e20 7370 6563 732c 2077 6869  ed in specs, whi
-0000b9c0: 6368 2069 7320 6765 6e65 7261 6c6c 7920  ch is generally 
-0000b9d0: 6120 7370 6563 6961 6c69 7a65 6420 6f6e  a specialized on
-0000b9e0: 652c 0a20 2020 2020 2020 2020 2020 206c  e,.            l
-0000b9f0: 696b 6520 6120 6e61 6d65 2061 646f 7074  ike a name adopt
-0000ba00: 6564 2062 7920 7370 6563 6961 6c69 7a65  ed by specialize
-0000ba10: 6420 6461 7461 7365 742e 0a20 2020 2020  d dataset..     
-0000ba20: 2020 2073 7461 6e64 6172 6469 7a65 3a20     standardize: 
-0000ba30: 626f 6f6c 0a20 2020 2020 2020 2072 656e  bool.        ren
-0000ba40: 616d 655f 6469 6d73 3a20 626f 6f6c 0a20  ame_dims: bool. 
-0000ba50: 2020 2020 2020 2020 2020 2046 6f72 2061             For a
-0000ba60: 2031 4420 6172 7261 792c 2072 656e 616d   1D array, renam
-0000ba70: 6520 7468 6520 6469 6d65 6e73 696f 6e20  e the dimension 
-0000ba80: 6966 2069 7420 6861 7320 7468 6520 7361  if it has the sa
-0000ba90: 6d65 206e 616d 650a 2020 2020 2020 2020  me name.        
-0000baa0: 2020 2020 6173 2074 6865 2061 7272 6179      as the array
-0000bab0: 2e0a 2020 2020 2020 2020 2020 2020 4e6f  ..            No
-0000bac0: 7465 2074 6861 7420 6974 2069 7320 7365  te that it is se
-0000bad0: 7420 746f 2046 616c 7365 2c20 6966 2060  t to False, if `
-0000bae0: 6072 656e 616d 6560 6020 6973 2046 616c  `rename`` is Fal
-0000baf0: 7365 2e0a 2020 2020 2020 2020 6174 7472  se..        attr
-0000bb00: 733a 2062 6f6f 6c2c 2064 6963 740a 2020  s: bool, dict.  
-0000bb10: 2020 2020 2020 2020 2020 4966 2046 616c            If Fal
-0000bb20: 7365 2c20 646f 6573 206e 6f74 2063 6861  se, does not cha
-0000bb30: 6e67 6520 6174 7472 6962 7574 6573 2061  nge attributes a
-0000bb40: 7420 616c 6c2e 0a20 2020 2020 2020 2020  t all..         
-0000bb50: 2020 2049 6620 5472 7565 2c20 7573 6520     If True, use 
-0000bb60: 4366 2061 7474 7269 6275 7465 732e 0a20  Cf attributes.. 
-0000bb70: 2020 2020 2020 2020 2020 2049 6620 6120             If a 
-0000bb80: 6469 6374 2c20 7573 6520 7468 6973 2064  dict, use this d
-0000bb90: 6963 742e 0a20 2020 2020 2020 2072 6570  ict..        rep
-0000bba0: 6c61 6365 5f61 7474 7273 3a20 626f 6f6c  lace_attrs: bool
-0000bbb0: 0a20 2020 2020 2020 2020 2020 2052 6570  .            Rep
-0000bbc0: 6c61 6365 2065 7869 7374 696e 6720 6174  lace existing at
-0000bbd0: 7472 6962 7574 6573 3f0a 0a20 2020 2020  tributes?..     
-0000bbe0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0000bbf0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0000bc00: 2020 2078 6172 7261 792e 4461 7461 4172     xarray.DataAr
-0000bc10: 7261 792c 2073 7472 2c20 4e6f 6e65 0a20  ray, str, None. 
-0000bc20: 2020 2020 2020 2020 2020 2054 6865 2066             The f
-0000bc30: 6f72 6d61 7474 6564 2061 7272 6179 206f  ormatted array o
-0000bc40: 7220 636f 7079 206f 6620 6974 2e0a 2020  r copy of it..  
-0000bc50: 2020 2020 2020 2020 2020 5468 6520 4346            The CF
-0000bc60: 206e 616d 652c 2067 6976 656e 206f 7220   name, given or 
-0000bc70: 6d61 7463 6869 6e67 2c20 6966 2072 656e  matching, if ren
-0000bc80: 616d 6520 6966 2046 616c 7365 3b20 616e  ame if False; an
-0000bc90: 6420 4e6f 6e65 0a20 2020 2020 2020 2020  d None.         
-0000bca0: 2020 2069 6620 6e6f 7420 6d61 7463 6869     if not matchi
-0000bcb0: 6e67 2e0a 0a20 2020 2020 2020 2053 6565  ng...        See
-0000bcc0: 2061 6c73 6f0a 2020 2020 2020 2020 2d2d   also.        --
-0000bcd0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2043  ------.        C
-0000bce0: 4643 6f6f 7264 5370 6563 732e 666f 726d  FCoordSpecs.form
-0000bcf0: 6174 5f64 6174 6161 7272 6179 0a20 2020  at_dataarray.   
-0000bd00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000bd10: 2072 6574 7572 6e20 7365 6c66 2e5f 666f   return self._fo
-0000bd20: 726d 6174 5f6f 626a 5f28 0a20 2020 2020  rmat_obj_(.     
-0000bd30: 2020 2020 2020 2064 612c 0a20 2020 2020         da,.     
-0000bd40: 2020 2020 2020 2063 665f 6e61 6d65 733d         cf_names=
-0000bd50: 7b64 612e 6e61 6d65 3a20 6366 5f6e 616d  {da.name: cf_nam
-0000bd60: 657d 2c0a 2020 2020 2020 2020 2020 2020  e},.            
-0000bd70: 636f 7079 3d63 6f70 792c 0a20 2020 2020  copy=copy,.     
-0000bd80: 2020 2020 2020 2072 656e 616d 653d 7265         rename=re
-0000bd90: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-0000bda0: 2020 7265 6e61 6d65 5f64 696d 733d 7265    rename_dims=re
-0000bdb0: 6e61 6d65 5f64 696d 732c 0a20 2020 2020  name_dims,.     
-0000bdc0: 2020 2020 2020 2073 7065 6369 616c 697a         specializ
-0000bdd0: 653d 7370 6563 6961 6c69 7a65 2c0a 2020  e=specialize,.  
-0000bde0: 2020 2020 2020 2020 2020 666f 726d 6174            format
-0000bdf0: 5f63 6f6f 7264 733d 666f 726d 6174 5f63  _coords=format_c
-0000be00: 6f6f 7264 732c 0a20 2020 2020 2020 2020  oords,.         
-0000be10: 2020 2072 6570 6c61 6365 5f61 7474 7273     replace_attrs
-0000be20: 3d72 6570 6c61 6365 5f61 7474 7273 2c0a  =replace_attrs,.
-0000be30: 2020 2020 2020 2020 2020 2020 6174 7472              attr
-0000be40: 733d 6174 7472 7320 6966 2069 7369 6e73  s=attrs if isins
-0000be50: 7461 6e63 6528 6174 7472 732c 2062 6f6f  tance(attrs, boo
-0000be60: 6c29 2065 6c73 6520 7b64 612e 6e61 6d65  l) else {da.name
-0000be70: 3a20 6174 7472 737d 2c0a 2020 2020 2020  : attrs},.      
-0000be80: 2020 2020 2020 7374 616e 6461 7264 697a        standardiz
-0000be90: 653d 7374 616e 6461 7264 697a 652c 0a20  e=standardize,. 
-0000bea0: 2020 2020 2020 2020 2020 2063 6174 6567             categ
-0000beb0: 6f72 6965 733d 5b22 636f 6f72 6473 222c  ories=["coords",
-0000bec0: 2022 6461 7461 5f76 6172 7322 5d2c 0a20   "data_vars"],. 
-0000bed0: 2020 2020 2020 2020 2020 206c 6f63 3d6c             loc=l
-0000bee0: 6f63 2c0a 2020 2020 2020 2020 290a 0a20  oc,.        ).. 
-0000bef0: 2020 2064 6566 2066 6f72 6d61 745f 6461     def format_da
-0000bf00: 7461 7365 7428 0a20 2020 2020 2020 2073  taset(.        s
-0000bf10: 656c 662c 0a20 2020 2020 2020 2064 732c  elf,.        ds,
-0000bf20: 0a20 2020 2020 2020 2063 665f 6e61 6d65  .        cf_name
-0000bf30: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-0000bf40: 2320 6c6f 633d 4e6f 6e65 2c0a 2020 2020  # loc=None,.    
-0000bf50: 2020 2020 636f 7079 3d54 7275 652c 0a20      copy=True,. 
-0000bf60: 2020 2020 2020 2066 6f72 6d61 745f 636f         format_co
-0000bf70: 6f72 6473 3d54 7275 652c 0a20 2020 2020  ords=True,.     
-0000bf80: 2020 2073 7461 6e64 6172 6469 7a65 3d54     standardize=T
-0000bf90: 7275 652c 0a20 2020 2020 2020 2072 656e  rue,.        ren
-0000bfa0: 616d 653d 5472 7565 2c0a 2020 2020 2020  ame=True,.      
-0000bfb0: 2020 7265 6e61 6d65 5f64 696d 733d 5472    rename_dims=Tr
-0000bfc0: 7565 2c0a 2020 2020 2020 2020 7370 6563  ue,.        spec
-0000bfd0: 6961 6c69 7a65 3d46 616c 7365 2c0a 2020  ialize=False,.  
-0000bfe0: 2020 2020 2020 6174 7472 733d 5472 7565        attrs=True
-0000bff0: 2c0a 2020 2020 2020 2020 7265 706c 6163  ,.        replac
-0000c000: 655f 6174 7472 733d 4661 6c73 652c 0a20  e_attrs=False,. 
-0000c010: 2020 2020 2020 2023 2061 6464 5f6c 6f63         # add_loc
-0000c020: 5f74 6f5f 6e61 6d65 3d4e 6f6e 650a 2020  _to_name=None.  
-0000c030: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-0000c040: 466f 726d 6174 2061 2077 686f 6c65 2064  Format a whole d
-0000c050: 6174 6173 6574 0a0a 2020 2020 2020 2020  ataset..        
-0000c060: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0000c070: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000c080: 2020 2020 2020 6473 3a20 7861 7272 6179        ds: xarray
-0000c090: 2e44 6174 6173 6574 0a20 2020 2020 2020  .Dataset.       
-0000c0a0: 2063 665f 6e61 6d65 733a 2064 6963 742c   cf_names: dict,
-0000c0b0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0000c0c0: 2020 4469 6374 206f 6620 6e61 6d65 7320    Dict of names 
-0000c0d0: 6173 206b 6579 7320 616e 6420 6765 6e65  as keys and gene
-0000c0e0: 7269 6320 4346 206e 616d 6573 2061 7320  ric CF names as 
-0000c0f0: 7661 6c75 6573 2e0a 2020 2020 2020 2020  values..        
-0000c100: 2020 2020 4966 206e 6f74 2070 726f 7669      If not provi
-0000c110: 6465 642c 2043 4620 6e61 6d65 7320 6172  ded, CF names ar
-0000c120: 6520 6775 6573 7365 6420 7769 7468 203a  e guessed with :
-0000c130: 6d65 7468 3a60 6d61 7463 6860 2e0a 2020  meth:`match`..  
-0000c140: 2020 2020 2020 6c6f 633a 2073 7472 2c20        loc: str, 
-0000c150: 7b22 616e 7922 2c20 4e6f 6e65 7d2c 207b  {"any", None}, {
-0000c160: 2222 2c20 4661 6c73 657d 0a20 2020 2020  "", False}.     
-0000c170: 2020 2020 2020 202d 2073 7472 3a20 6f6e         - str: on
-0000c180: 6520 6f66 2074 6865 7365 206c 6f63 6174  e of these locat
-0000c190: 696f 6e73 0a20 2020 2020 2020 2020 2020  ions.           
-0000c1a0: 202d 204e 6f6e 6520 6f72 2022 616e 7922   - None or "any"
-0000c1b0: 3a20 616e 790a 2020 2020 2020 2020 2020  : any.          
-0000c1c0: 2020 2d20 4661 6c73 6520 6f72 2027 2222    - False or '""
-0000c1d0: 3a20 6e6f 206c 6f63 6174 696f 6e0a 2020  : no location.  
-0000c1e0: 2020 2020 2020 7265 6e61 6d65 3a20 626f        rename: bo
-0000c1f0: 6f6c 0a20 2020 2020 2020 2020 2020 2052  ol.            R
-0000c200: 656e 616d 6520 6172 7261 7973 0a20 2020  ename arrays.   
-0000c210: 2020 2020 2061 6464 5f6c 6f63 5f74 6f5f       add_loc_to_
-0000c220: 6e61 6d65 3a20 626f 6f6c 0a20 2020 2020  name: bool.     
-0000c230: 2020 2020 2020 2041 6464 206c 6f63 2074         Add loc t
-0000c240: 6f20 7468 6520 6e61 6d65 0a20 2020 2020  o the name.     
-0000c250: 2020 2073 7065 6369 616c 697a 653a 2062     specialize: b
-0000c260: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-0000c270: 446f 6573 206e 6f74 2075 7365 2074 6865  Does not use the
-0000c280: 2043 4620 6e61 6d65 2066 6f72 2072 656e   CF name for ren
-0000c290: 616d 696e 672c 2062 7574 2074 6865 2066  aming, but the f
-0000c2a0: 6972 7374 206e 616d 650a 2020 2020 2020  irst name.      
-0000c2b0: 2020 2020 2020 6173 206c 6973 7465 6420        as listed 
-0000c2c0: 696e 2073 7065 6373 2c20 7768 6963 6820  in specs, which 
-0000c2d0: 6973 2067 656e 6572 616c 6c79 2061 2073  is generally a s
-0000c2e0: 7065 6369 616c 697a 6564 206f 6e65 2c0a  pecialized one,.
-0000c2f0: 2020 2020 2020 2020 2020 2020 6c69 6b65              like
-0000c300: 2061 206e 616d 6520 6164 6f70 7465 6420   a name adopted 
-0000c310: 6279 2073 7065 6369 616c 697a 6564 2064  by specialized d
-0000c320: 6174 6173 6574 2e0a 2020 2020 2020 2020  ataset..        
-0000c330: 7374 616e 6461 7264 697a 653a 2062 6f6f  standardize: boo
-0000c340: 6c0a 2020 2020 2020 2020 7265 6e61 6d65  l.        rename
-0000c350: 5f64 696d 3a20 626f 6f6c 0a20 2020 2020  _dim: bool.     
-0000c360: 2020 2020 2020 2046 6f72 2061 2031 4420         For a 1D 
-0000c370: 6172 7261 792c 2072 656e 616d 6520 7468  array, rename th
-0000c380: 6520 6469 6d65 6e73 696f 6e20 6966 2069  e dimension if i
-0000c390: 7420 6861 7320 7468 6520 7361 6d65 206e  t has the same n
-0000c3a0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-0000c3b0: 6173 2074 6865 2061 7272 6179 2e0a 2020  as the array..  
-0000c3c0: 2020 2020 2020 2020 2020 4e6f 7465 2074            Note t
-0000c3d0: 6861 7420 6974 2069 7320 7365 7420 746f  hat it is set to
-0000c3e0: 2046 616c 7365 2c20 6966 2060 6072 656e   False, if ``ren
-0000c3f0: 616d 6560 6020 6973 2046 616c 7365 2e0a  ame`` is False..
-0000c400: 2020 2020 2020 2020 6174 7472 733a 2062          attrs: b
-0000c410: 6f6f 6c2c 2064 6963 7420 6f66 2064 6963  ool, dict of dic
-0000c420: 740a 2020 2020 2020 2020 2020 2020 4966  t.            If
-0000c430: 2046 616c 7365 2c20 646f 6573 206e 6f74   False, does not
-0000c440: 2063 6861 6e67 6520 6174 7472 6962 7574   change attribut
-0000c450: 6573 2061 7420 616c 6c2e 0a20 2020 2020  es at all..     
-0000c460: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
-0000c470: 7573 6520 4366 2061 7474 7269 6275 7465  use Cf attribute
-0000c480: 732e 0a20 2020 2020 2020 2020 2020 2049  s..            I
-0000c490: 6620 6120 6469 6374 2c20 7573 6520 7468  f a dict, use th
-0000c4a0: 6973 2064 6963 742e 0a20 2020 2020 2020  is dict..       
-0000c4b0: 2072 6570 6c61 6365 5f61 7474 7273 3a20   replace_attrs: 
-0000c4c0: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
-0000c4d0: 2052 6570 6c61 6365 2065 7869 7374 696e   Replace existin
-0000c4e0: 6720 6174 7472 6962 7574 6573 3f0a 0a20  g attributes?.. 
-0000c4f0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-0000c500: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-0000c510: 2020 2020 2020 2078 6172 7261 792e 4461         xarray.Da
-0000c520: 7461 4172 7261 792c 2073 7472 2c20 4e6f  taArray, str, No
-0000c530: 6e65 0a20 2020 2020 2020 2020 2020 2054  ne.            T
-0000c540: 6865 2066 6f72 6d61 7474 6564 2061 7272  he formatted arr
-0000c550: 6179 206f 7220 636f 7079 206f 6620 6974  ay or copy of it
-0000c560: 2e0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-0000c570: 6520 4346 206e 616d 652c 2067 6976 656e  e CF name, given
-0000c580: 206f 7220 6d61 7463 6869 6e67 2c20 6966   or matching, if
-0000c590: 2072 656e 616d 6520 6966 2046 616c 7365   rename if False
-0000c5a0: 3b20 616e 6420 4e6f 6e65 0a20 2020 2020  ; and None.     
-0000c5b0: 2020 2020 2020 2069 6620 6e6f 7420 6d61         if not ma
-0000c5c0: 7463 6869 6e67 2e0a 0a20 2020 2020 2020  tching...       
-0000c5d0: 2053 6565 2061 6c73 6f0a 2020 2020 2020   See also.      
-0000c5e0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020    --------.     
-0000c5f0: 2020 2043 4643 6f6f 7264 5370 6563 732e     CFCoordSpecs.
-0000c600: 666f 726d 6174 5f64 6174 6161 7272 6179  format_dataarray
-0000c610: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c620: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000c630: 2e5f 666f 726d 6174 5f6f 626a 5f28 0a20  ._format_obj_(. 
-0000c640: 2020 2020 2020 2020 2020 2064 732c 0a20             ds,. 
-0000c650: 2020 2020 2020 2020 2020 2063 665f 6e61             cf_na
-0000c660: 6d65 733d 6366 5f6e 616d 6573 2c0a 2020  mes=cf_names,.  
-0000c670: 2020 2020 2020 2020 2020 636f 7079 3d63            copy=c
-0000c680: 6f70 792c 0a20 2020 2020 2020 2020 2020  opy,.           
-0000c690: 2073 7461 6e64 6172 6469 7a65 3d73 7461   standardize=sta
-0000c6a0: 6e64 6172 6469 7a65 2c0a 2020 2020 2020  ndardize,.      
-0000c6b0: 2020 2020 2020 7265 6e61 6d65 3d72 656e        rename=ren
-0000c6c0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-0000c6d0: 2072 656e 616d 655f 6469 6d73 3d72 656e   rename_dims=ren
-0000c6e0: 616d 655f 6469 6d73 2c0a 2020 2020 2020  ame_dims,.      
-0000c6f0: 2020 2020 2020 666f 726d 6174 5f63 6f6f        format_coo
-0000c700: 7264 733d 666f 726d 6174 5f63 6f6f 7264  rds=format_coord
-0000c710: 732c 0a20 2020 2020 2020 2020 2020 2072  s,.            r
-0000c720: 6570 6c61 6365 5f61 7474 7273 3d72 6570  eplace_attrs=rep
-0000c730: 6c61 6365 5f61 7474 7273 2c0a 2020 2020  lace_attrs,.    
-0000c740: 2020 2020 2020 2020 6174 7472 733d 6174          attrs=at
-0000c750: 7472 732c 0a20 2020 2020 2020 2020 2020  trs,.           
-0000c760: 2073 7065 6369 616c 697a 653d 7370 6563   specialize=spec
-0000c770: 6961 6c69 7a65 2c0a 2020 2020 2020 2020  ialize,.        
-0000c780: 2020 2020 6361 7465 676f 7269 6573 3d5b      categories=[
-0000c790: 2263 6f6f 7264 7322 2c20 2264 6174 615f  "coords", "data_
-0000c7a0: 7661 7273 225d 2c0a 2020 2020 2020 2020  vars"],.        
-0000c7b0: 290a 0a20 2020 2064 6566 2061 7574 6f5f  )..    def auto_
-0000c7c0: 666f 726d 6174 2873 656c 662c 206f 626a  format(self, obj
-0000c7d0: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-0000c7e0: 2020 2020 2022 2222 5265 6e61 6d65 2076       """Rename v
-0000c7f0: 6172 6961 626c 6573 2061 6e64 2063 6f6f  ariables and coo
-0000c800: 7264 696e 6174 6573 2061 6e64 2066 696c  rdinates and fil
-0000c810: 6c20 7468 6569 7220 6174 7472 6962 7574  l their attribut
-0000c820: 6573 0a0a 2020 2020 2020 2020 5365 6520  es..        See 
-0000c830: 616c 736f 0a20 2020 2020 2020 202d 2d2d  also.        ---
-0000c840: 2d2d 2d2d 2d0a 2020 2020 2020 2020 656e  -----.        en
-0000c850: 636f 6465 0a20 2020 2020 2020 2066 6f72  code.        for
-0000c860: 6d61 745f 6461 7461 5f76 6172 0a20 2020  mat_data_var.   
-0000c870: 2020 2020 2066 6f72 6d61 745f 6461 7461       format_data
-0000c880: 7365 740a 2020 2020 2020 2020 6669 6c6c  set.        fill
-0000c890: 5f61 7474 7273 0a20 2020 2020 2020 2022  _attrs.        "
-0000c8a0: 2222 0a20 2020 2020 2020 2069 6620 6861  "".        if ha
-0000c8b0: 7361 7474 7228 6f62 6a2c 2022 6461 7461  sattr(obj, "data
-0000c8c0: 5f76 6172 7322 293a 0a20 2020 2020 2020  _vars"):.       
-0000c8d0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000c8e0: 2e66 6f72 6d61 745f 6461 7461 7365 7428  .format_dataset(
-0000c8f0: 6f62 6a2c 202a 2a6b 7761 7267 7329 0a20  obj, **kwargs). 
-0000c900: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000c910: 6c66 2e66 6f72 6d61 745f 6461 7461 5f76  lf.format_data_v
-0000c920: 6172 286f 626a 2c20 2a2a 6b77 6172 6773  ar(obj, **kwargs
-0000c930: 290a 0a20 2020 2064 6566 2064 6563 6f64  )..    def decod
-0000c940: 6528 7365 6c66 2c20 6f62 6a2c 202a 2a6b  e(self, obj, **k
-0000c950: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-0000c960: 2222 2241 7574 6f20 666f 726d 6174 2c20  """Auto format, 
-0000c970: 696e 6665 7220 636f 6f72 6469 6e61 7465  infer coordinate
-0000c980: 7320 616e 6420 7265 6e61 6d65 2074 6f20  s and rename to 
-0000c990: 6765 6e65 7269 6320 6e61 6d65 730a 0a20  generic names.. 
-0000c9a0: 2020 2020 2020 2053 6565 2061 6c73 6f0a         See also.
-0000c9b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-0000c9c0: 0a20 2020 2020 2020 2061 7574 6f5f 666f  .        auto_fo
-0000c9d0: 726d 6174 0a20 2020 2020 2020 2065 6e63  rmat.        enc
-0000c9e0: 6f64 650a 2020 2020 2020 2020 666f 726d  ode.        form
-0000c9f0: 6174 5f64 6174 6161 7272 6179 0a20 2020  at_dataarray.   
-0000ca00: 2020 2020 2066 6f72 6d61 745f 6461 7461       format_data
-0000ca10: 7365 740a 2020 2020 2020 2020 6669 6c6c  set.        fill
-0000ca20: 5f61 7474 7273 0a20 2020 2020 2020 2022  _attrs.        "
-0000ca30: 2222 0a20 2020 2020 2020 2023 2043 6f6f  "".        # Coo
-0000ca40: 7264 696e 6174 6573 0a20 2020 2020 2020  rdinates.       
-0000ca50: 206f 626a 203d 2073 656c 662e 696e 6665   obj = self.infe
-0000ca60: 725f 636f 6f72 6473 286f 626a 290a 0a20  r_coords(obj).. 
-0000ca70: 2020 2020 2020 2023 204e 616d 6573 2061         # Names a
-0000ca80: 6e64 2061 7474 7269 6275 7465 730a 2020  nd attributes.  
-0000ca90: 2020 2020 2020 6f62 6a20 3d20 7365 6c66        obj = self
-0000caa0: 2e61 7574 6f5f 666f 726d 6174 286f 626a  .auto_format(obj
-0000cab0: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
-0000cac0: 2020 2020 2023 2041 7373 6967 6e20 6366       # Assign cf
-0000cad0: 2073 7065 6373 0a20 2020 2020 2020 2069   specs.        i
-0000cae0: 6620 7365 6c66 2e6e 616d 6520 616e 6420  f self.name and 
-0000caf0: 7365 6c66 2069 6e20 6765 745f 7265 6769  self in get_regi
-0000cb00: 7374 6572 6564 5f63 665f 7370 6563 7328  stered_cf_specs(
-0000cb10: 293a 0a20 2020 2020 2020 2020 2020 206f  ):.            o
-0000cb20: 626a 203d 2061 7373 6967 6e5f 6366 5f73  bj = assign_cf_s
-0000cb30: 7065 6373 286f 626a 2c20 7365 6c66 2e6e  pecs(obj, self.n
-0000cb40: 616d 6529 0a0a 2020 2020 2020 2020 7265  ame)..        re
-0000cb50: 7475 726e 206f 626a 0a0a 2020 2020 6465  turn obj..    de
-0000cb60: 6620 656e 636f 6465 2873 656c 662c 206f  f encode(self, o
-0000cb70: 626a 2c20 2a2a 6b77 6172 6773 293a 0a20  bj, **kwargs):. 
-0000cb80: 2020 2020 2020 2022 2222 5361 6d65 2061         """Same a
-0000cb90: 7320 3a6d 6574 683a 6064 6563 6f64 6560  s :meth:`decode`
-0000cba0: 2062 7574 2072 656e 616d 6520 7769 7468   but rename with
-0000cbb0: 2074 6865 2073 7065 6369 616c 697a 6564   the specialized
-0000cbc0: 206e 616d 650a 0a20 2020 2020 2020 2053   name..        S
-0000cbd0: 6565 2061 6c73 6f0a 2020 2020 2020 2020  ee also.        
-0000cbe0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0000cbf0: 2064 6563 6f64 650a 2020 2020 2020 2020   decode.        
-0000cc00: 6175 746f 5f66 6f72 6d61 740a 2020 2020  auto_format.    
-0000cc10: 2020 2020 666f 726d 6174 5f64 6174 6161      format_dataa
-0000cc20: 7272 6179 0a20 2020 2020 2020 2066 6f72  rray.        for
-0000cc30: 6d61 745f 6461 7461 7365 740a 2020 2020  mat_dataset.    
-0000cc40: 2020 2020 6669 6c6c 5f61 7474 7273 0a20      fill_attrs. 
-0000cc50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000cc60: 2020 206b 7761 7267 732e 7365 7464 6566     kwargs.setdef
-0000cc70: 6175 6c74 2822 7370 6563 6961 6c69 7a65  ault("specialize
-0000cc80: 222c 2054 7275 6529 0a20 2020 2020 2020  ", True).       
-0000cc90: 2072 6574 7572 6e20 7365 6c66 2e64 6563   return self.dec
-0000cca0: 6f64 6528 6f62 6a2c 202a 2a6b 7761 7267  ode(obj, **kwarg
-0000ccb0: 7329 0a0a 2020 2020 6465 6620 746f 5f6c  s)..    def to_l
-0000ccc0: 6f63 2873 656c 662c 206f 626a 2c20 2a2a  oc(self, obj, **
-0000ccd0: 6c6f 6373 293a 0a20 2020 2020 2020 2022  locs):.        "
-0000cce0: 2222 5365 7420 7468 6520 7374 6167 6765  ""Set the stagge
-0000ccf0: 7265 6420 6772 6964 206c 6f63 6174 696f  red grid locatio
-0000cd00: 6e20 666f 7220 7370 6563 6966 6965 6420  n for specified 
-0000cd10: 6e61 6d65 730a 0a20 2020 2020 2020 202e  names..        .
-0000cd20: 2e20 6e6f 7465 3a3a 2049 7420 6f6e 6c79  . note:: It only
-0000cd30: 2063 6861 6e67 6573 2074 6865 206e 616d   changes the nam
-0000cd40: 6573 2c20 6e6f 7420 7468 6520 6174 7472  es, not the attr
-0000cd50: 6962 7574 6573 2e0a 0a20 2020 2020 2020  ibutes...       
-0000cd60: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000cd70: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000cd80: 2020 2020 2020 206f 626a 3a20 7861 7272         obj: xarr
-0000cd90: 6179 2e44 6174 6173 6574 2c20 7861 7272  ay.Dataset, xarr
-0000cda0: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
-0000cdb0: 2020 2020 206c 6f63 733a 2064 6963 740a       locs: dict.
-0000cdc0: 2020 2020 2020 2020 2020 2020 2a2a 4b65              **Ke
-0000cdd0: 7973 2061 7265 2072 6f6f 7420 6e61 6d65  ys are root name
-0000cde0: 732a 2a2c 2076 616c 7565 7320 6172 6520  s**, values are 
-0000cdf0: 6e65 7720 6c6f 6361 7469 6f6e 732e 0a20  new locations.. 
-0000ce00: 2020 2020 2020 2020 2020 2041 2076 616c             A val
-0000ce10: 7565 206f 6620 6046 616c 7365 602c 2072  ue of `False`, r
-0000ce20: 656d 6f76 6520 7468 6520 6c6f 6361 7469  emove the locati
-0000ce30: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-0000ce40: 4120 7661 6c75 6520 6f66 2060 4e6f 6e65  A value of `None
-0000ce50: 6020 6c65 6674 2069 7420 6173 2069 732e  ` left it as is.
-0000ce60: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000ce70: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d0a  .        ------.
-0000ce80: 2020 2020 2020 2020 7861 7272 6179 2e44          xarray.D
-0000ce90: 6174 6173 6574 2c20 7861 7272 6179 2e44  ataset, xarray.D
-0000cea0: 6174 6141 7272 6179 0a0a 2020 2020 2020  ataArray..      
-0000ceb0: 2020 5365 6520 616c 736f 0a20 2020 2020    See also.     
-0000cec0: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
-0000ced0: 2020 2020 7265 6c6f 630a 2020 2020 2020      reloc.      
-0000cee0: 2020 7367 6c6f 6361 746f 720a 2020 2020    sglocator.    
-0000cef0: 2020 2020 5347 4c6f 6361 746f 722e 666f      SGLocator.fo
-0000cf00: 726d 6174 5f61 7474 720a 2020 2020 2020  rmat_attr.      
-0000cf10: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-0000cf20: 6e61 6d65 5f61 7267 7320 3d20 7b7d 0a20  name_args = {}. 
-0000cf30: 2020 2020 2020 206e 616d 6573 203d 205f         names = _
-0000cf40: 6c69 7374 5f78 725f 6e61 6d65 735f 286f  list_xr_names_(o
-0000cf50: 626a 290a 2020 2020 2020 2020 6966 2068  bj).        if h
-0000cf60: 6173 6174 7472 286f 626a 2c20 226e 616d  asattr(obj, "nam
-0000cf70: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
-0000cf80: 206e 616d 6573 203d 206e 616d 6573 2e75   names = names.u
-0000cf90: 6e69 6f6e 287b 6f62 6a2e 6e61 6d65 7d29  nion({obj.name})
-0000cfa0: 0a20 2020 2020 2020 2066 6f72 206e 616d  .        for nam
-0000cfb0: 6520 696e 206e 616d 6573 3a0a 2020 2020  e in names:.    
-0000cfc0: 2020 2020 2020 2020 6966 206e 616d 6520          if name 
-0000cfd0: 6e6f 7420 696e 2072 656e 616d 655f 6172  not in rename_ar
-0000cfe0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000cff0: 2020 2020 726f 6f74 5f6e 616d 652c 206f      root_name, o
-0000d000: 6c64 5f6c 6f63 203d 2073 656c 662e 7367  ld_loc = self.sg
-0000d010: 6c6f 6361 746f 722e 7061 7273 655f 6174  locator.parse_at
-0000d020: 7472 2822 6e61 6d65 222c 206e 616d 6529  tr("name", name)
-0000d030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d040: 2069 6620 726f 6f74 5f6e 616d 6520 696e   if root_name in
-0000d050: 206c 6f63 7320 616e 6420 6c6f 6373 5b72   locs and locs[r
-0000d060: 6f6f 745f 6e61 6d65 5d20 6973 206e 6f74  oot_name] is not
-0000d070: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000d080: 2020 2020 2020 2020 2020 2072 656e 616d             renam
-0000d090: 655f 6172 6773 5b6e 616d 655d 203d 2073  e_args[name] = s
-0000d0a0: 656c 662e 7367 6c6f 6361 746f 722e 666f  elf.sglocator.fo
-0000d0b0: 726d 6174 5f61 7474 7228 0a20 2020 2020  rmat_attr(.     
+0000a2b0: 7267 7320 3d20 7b7d 0a20 2020 2020 2020  rgs = {}.       
+0000a2c0: 2069 6620 7265 6e61 6d65 5f64 696d 7320   if rename_dims 
+0000a2d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000a2e0: 2020 2020 2072 656e 616d 655f 6469 6d73       rename_dims
+0000a2f0: 203d 2066 6f72 6d61 745f 636f 6f72 6473   = format_coords
+0000a300: 0a0a 2020 2020 2020 2020 2320 436f 6d6d  ..        # Comm
+0000a310: 6f6e 2066 6f72 6d61 7474 696e 6720 6b77  on formatting kw
+0000a320: 6172 6773 0a20 2020 2020 2020 206b 7761  args.        kwa
+0000a330: 7267 7320 3d20 6469 6374 280a 2020 2020  rgs = dict(.    
+0000a340: 2020 2020 2020 2020 636f 7079 3d46 616c          copy=Fal
+0000a350: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+0000a360: 7265 6e61 6d65 3d46 616c 7365 2c0a 2020  rename=False,.  
+0000a370: 2020 2020 2020 2020 2020 7265 706c 6163            replac
+0000a380: 655f 6174 7472 733d 7265 706c 6163 655f  e_attrs=replace_
+0000a390: 6174 7472 732c 0a20 2020 2020 2020 2020  attrs,.         
+0000a3a0: 2020 2073 7461 6e64 6172 6469 7a65 3d54     standardize=T
+0000a3b0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+0000a3c0: 2073 7065 6369 616c 697a 653d 7370 6563   specialize=spec
+0000a3d0: 6961 6c69 7a65 2c0a 2020 2020 2020 2020  ialize,.        
+0000a3e0: 290a 0a20 2020 2020 2020 2023 2053 7461  )..        # Sta
+0000a3f0: 6767 6172 6564 2067 7269 6420 6c6f 6361  ggared grid loca
+0000a400: 7469 6f6e 730a 2020 2020 2020 2020 6c6f  tions.        lo
+0000a410: 6361 7469 6f6e 7320 3d20 7365 6c66 2e67  cations = self.g
+0000a420: 6574 5f6c 6f63 5f6d 6170 7069 6e67 286f  et_loc_mapping(o
+0000a430: 626a 2c20 6366 5f6e 616d 6573 3d63 665f  bj, cf_names=cf_
+0000a440: 6e61 6d65 732c 206c 6f63 3d6c 6f63 2c20  names, loc=loc, 
+0000a450: 6361 7465 676f 7269 6573 3d63 6174 6567  categories=categ
+0000a460: 6f72 6965 7329 0a0a 2020 2020 2020 2020  ories)..        
+0000a470: 2320 4461 7461 2061 7272 6179 730a 2020  # Data arrays.  
+0000a480: 2020 2020 2020 6973 5f64 6174 6173 6574        is_dataset
+0000a490: 203d 2068 6173 6174 7472 286f 626a 2c20   = hasattr(obj, 
+0000a4a0: 2264 6174 615f 7661 7273 2229 0a20 2020  "data_vars").   
+0000a4b0: 2020 2020 2069 6620 6973 5f64 6174 6173       if is_datas
+0000a4c0: 6574 3a20 2023 2064 6174 6173 6574 0a20  et:  # dataset. 
+0000a4d0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+0000a4e0: 7661 7273 203d 206f 626a 2e76 616c 7565  vars = obj.value
+0000a4f0: 7328 290a 2020 2020 2020 2020 656c 7365  s().        else
+0000a500: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
+0000a510: 7461 5f76 6172 7320 3d20 5b6f 626a 5d0a  ta_vars = [obj].
+0000a520: 2020 2020 2020 2020 666f 7220 6461 2069          for da i
+0000a530: 6e20 6461 7461 5f76 6172 733a 0a20 2020  n data_vars:.   
+0000a540: 2020 2020 2020 2020 2066 6f72 2063 6174           for cat
+0000a550: 2069 6e20 6361 7465 676f 7269 6573 3a0a   in categories:.
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a570: 6366 5f6e 616d 6520 3d20 6366 5f6e 616d  cf_name = cf_nam
+0000a580: 6573 2e67 6574 2864 612e 6e61 6d65 2920  es.get(da.name) 
+0000a590: 6966 2063 665f 6e61 6d65 7320 656c 7365  if cf_names else
+0000a5a0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+0000a5b0: 2020 2020 2020 6966 2063 665f 6e61 6d65        if cf_name
+0000a5c0: 2061 6e64 2063 665f 6e61 6d65 206e 6f74   and cf_name not
+0000a5d0: 2069 6e20 7365 6c66 5b63 6174 5d3a 0a20   in self[cat]:. 
+0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5f0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+0000a600: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000a610: 6e61 6d65 203d 2073 656c 665b 6361 745d  name = self[cat]
+0000a620: 2e66 6f72 6d61 745f 6461 7461 6172 7261  .format_dataarra
+0000a630: 7928 0a20 2020 2020 2020 2020 2020 2020  y(.             
+0000a640: 2020 2020 2020 2064 612c 0a20 2020 2020         da,.     
+0000a650: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000a660: 665f 6e61 6d65 3d63 665f 6e61 6d65 2c0a  f_name=cf_name,.
+0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a680: 2020 2020 6174 7472 733d 6174 7472 7320      attrs=attrs 
+0000a690: 6966 2069 7369 6e73 7461 6e63 6528 6174  if isinstance(at
+0000a6a0: 7472 732c 2062 6f6f 6c29 2065 6c73 6520  trs, bool) else 
+0000a6b0: 6174 7472 732e 6765 7428 6461 2e6e 616d  attrs.get(da.nam
+0000a6c0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+0000a6d0: 2020 2020 2020 2020 2320 666f 726d 6174          # format
+0000a6e0: 5f63 6f6f 7264 733d 4661 6c73 652c 0a20  _coords=False,. 
+0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a700: 2020 206c 6f63 3d6c 6f63 6174 696f 6e73     loc=locations
+0000a710: 2e67 6574 2864 612e 6e61 6d65 292c 0a20  .get(da.name),. 
+0000a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a730: 2020 202a 2a6b 7761 7267 732c 0a20 2020     **kwargs,.   
+0000a740: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000a750: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000a760: 6620 6e65 775f 6e61 6d65 3a0a 2020 2020  f new_name:.    
+0000a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a780: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+0000a790: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000a7a0: 2020 2020 2020 2020 6e65 775f 6e61 6d65          new_name
+0000a7b0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000a7c0: 2020 2020 6966 2072 656e 616d 6520 616e      if rename an
+0000a7d0: 6420 6e65 775f 6e61 6d65 3a0a 2020 2020  d new_name:.    
+0000a7e0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0000a7f0: 735f 6461 7461 7365 743a 0a20 2020 2020  s_dataset:.     
+0000a800: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000a810: 656e 616d 655f 6172 6773 5b64 612e 6e61  ename_args[da.na
+0000a820: 6d65 5d20 3d20 6e65 775f 6e61 6d65 0a20  me] = new_name. 
+0000a830: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000a840: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000a850: 2020 2020 2020 2020 2064 612e 6e61 6d65           da.name
+0000a860: 203d 206e 6577 5f6e 616d 650a 0a20 2020   = new_name..   
+0000a870: 2020 2020 2023 2043 6f6f 7264 696e 6174       # Coordinat
+0000a880: 6573 0a20 2020 2020 2020 2069 6620 666f  es.        if fo
+0000a890: 726d 6174 5f63 6f6f 7264 733a 0a20 2020  rmat_coords:.   
+0000a8a0: 2020 2020 2020 2020 2023 2066 6f72 2063           # for c
+0000a8b0: 6e61 6d65 2c20 6364 6120 696e 206c 6973  name, cda in lis
+0000a8c0: 7428 6f62 6a2e 636f 6f72 6473 2e69 7465  t(obj.coords.ite
+0000a8d0: 6d73 2829 293a 0a20 2020 2020 2020 2020  ms()):.         
+0000a8e0: 2020 2066 6f72 2063 6e61 6d65 2069 6e20     for cname in 
+0000a8f0: 5f6c 6973 745f 7872 5f6e 616d 6573 5f28  _list_xr_names_(
+0000a900: 6f62 6a2c 2064 6174 615f 7661 7273 3d46  obj, data_vars=F
+0000a910: 616c 7365 2c20 6469 6d73 3d46 616c 7365  alse, dims=False
+0000a920: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000a930: 2020 2063 6461 203d 206f 626a 2e63 6f6f     cda = obj.coo
+0000a940: 7264 735b 636e 616d 655d 0a20 2020 2020  rds[cname].     
+0000a950: 2020 2020 2020 2020 2020 206e 6577 5f63             new_c
+0000a960: 6f6f 7264 5f6e 616d 6520 3d20 7365 6c66  oord_name = self
+0000a970: 2e63 6f6f 7264 732e 666f 726d 6174 5f64  .coords.format_d
+0000a980: 6174 6161 7272 6179 280a 2020 2020 2020  ataarray(.      
+0000a990: 2020 2020 2020 2020 2020 2020 2020 6364                cd
+0000a9a0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+0000a9b0: 2020 2020 2020 2063 665f 6e61 6d65 3d63         cf_name=c
+0000a9c0: 665f 6e61 6d65 732e 6765 7428 636e 616d  f_names.get(cnam
+0000a9d0: 6529 2069 6620 6973 696e 7374 616e 6365  e) if isinstance
+0000a9e0: 2863 665f 6e61 6d65 732c 2064 6963 7429  (cf_names, dict)
+0000a9f0: 2065 6c73 6520 4e6f 6e65 2c0a 2020 2020   else None,.    
+0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa10: 6174 7472 733d 6174 7472 7320 6966 2069  attrs=attrs if i
+0000aa20: 7369 6e73 7461 6e63 6528 6174 7472 732c  sinstance(attrs,
+0000aa30: 2062 6f6f 6c29 2065 6c73 6520 6174 7472   bool) else attr
+0000aa40: 732e 6765 7428 636e 616d 652c 2054 7275  s.get(cname, Tru
+0000aa50: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+0000aa60: 2020 2020 2020 2020 2320 7265 6c61 7465          # relate
+0000aa70: 643d 6f62 6a2c 0a20 2020 2020 2020 2020  d=obj,.         
+0000aa80: 2020 2020 2020 2020 2020 2023 2066 6f72             # for
+0000aa90: 6d61 745f 636f 6f72 6473 3d46 616c 7365  mat_coords=False
+0000aaa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000aab0: 2020 2020 2020 2320 6c6f 633d 6c6f 632c        # loc=loc,
+0000aac0: 2061 6464 5f6c 6f63 5f74 6f5f 6e61 6d65   add_loc_to_name
+0000aad0: 3d61 6464 5f6c 6f63 5f74 6f5f 636f 6f72  =add_loc_to_coor
+0000aae0: 645f 6e61 6d65 732c 0a20 2020 2020 2020  d_names,.       
+0000aaf0: 2020 2020 2020 2020 2020 2020 206c 6f63               loc
+0000ab00: 3d6c 6f63 6174 696f 6e73 2e67 6574 2863  =locations.get(c
+0000ab10: 6461 2e6e 616d 6529 2c0a 2020 2020 2020  da.name),.      
+0000ab20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000ab30: 7265 6e61 6d65 5f64 696d 3d46 616c 7365  rename_dim=False
+0000ab40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ab50: 2020 2020 2020 2a2a 6b77 6172 6773 2c0a        **kwargs,.
+0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ab80: 2020 6966 2072 656e 616d 6520 616e 6420    if rename and 
+0000ab90: 6e65 775f 636f 6f72 645f 6e61 6d65 3a0a  new_coord_name:.
+0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abb0: 2020 2020 7265 6e61 6d65 5f61 7267 735b      rename_args[
+0000abc0: 6364 612e 6e61 6d65 5d20 3d20 6e65 775f  cda.name] = new_
+0000abd0: 636f 6f72 645f 6e61 6d65 0a0a 2020 2020  coord_name..    
+0000abe0: 2020 2020 2320 4469 6d65 6e73 696f 6e73      # Dimensions
+0000abf0: 0a20 2020 2020 2020 2069 6620 7265 6e61  .        if rena
+0000ac00: 6d65 5f64 696d 733a 0a20 2020 2020 2020  me_dims:.       
+0000ac10: 2020 2020 2072 656e 616d 655f 6469 6d73       rename_dims
+0000ac20: 5f61 7267 7320 3d20 7365 6c66 2e63 6f6f  _args = self.coo
+0000ac30: 7264 732e 6765 745f 7265 6e61 6d65 5f64  rds.get_rename_d
+0000ac40: 696d 735f 6172 6773 280a 2020 2020 2020  ims_args(.      
+0000ac50: 2020 2020 2020 2020 2020 6f62 6a2c 206c            obj, l
+0000ac60: 6f63 6174 696f 6e73 3d6c 6f63 6174 696f  ocations=locatio
+0000ac70: 6e73 2c20 7370 6563 6961 6c69 7a65 3d73  ns, specialize=s
+0000ac80: 7065 6369 616c 697a 650a 2020 2020 2020  pecialize.      
+0000ac90: 2020 2020 2020 2920 2023 202c 2065 7863        )  # , exc
+0000aca0: 6c75 6465 3d6c 6973 7428 7265 6e61 6d65  lude=list(rename
+0000acb0: 5f61 7267 732e 6b65 7973 2829 2929 0a20  _args.keys())). 
+0000acc0: 2020 2020 2020 2020 2020 2072 656e 616d             renam
+0000acd0: 655f 6172 6773 2e75 7064 6174 6528 7265  e_args.update(re
+0000ace0: 6e61 6d65 5f64 696d 735f 6172 6773 290a  name_dims_args).
+0000acf0: 0a20 2020 2020 2020 2023 2046 696e 616c  .        # Final
+0000ad00: 2072 656e 616d 696e 670a 2020 2020 2020   renaming.      
+0000ad10: 2020 6966 2072 656e 616d 6520 616e 6420    if rename and 
+0000ad20: 7265 6e61 6d65 5f61 7267 733a 0a20 2020  rename_args:.   
+0000ad30: 2020 2020 2020 2020 205f 736f 6c76 655f           _solve_
+0000ad40: 7265 6e61 6d65 5f63 6f6e 666c 6963 7473  rename_conflicts
+0000ad50: 5f28 7265 6e61 6d65 5f61 7267 7329 0a20  _(rename_args). 
+0000ad60: 2020 2020 2020 2020 2020 206f 626a 203d             obj =
+0000ad70: 206f 626a 2e72 656e 616d 6528 7265 6e61   obj.rename(rena
+0000ad80: 6d65 5f61 7267 7329 0a0a 2020 2020 2020  me_args)..      
+0000ad90: 2020 7265 7475 726e 206f 626a 0a0a 2020    return obj..  
+0000ada0: 2020 6465 6620 666f 726d 6174 5f63 6f6f    def format_coo
+0000adb0: 7264 280a 2020 2020 2020 2020 7365 6c66  rd(.        self
+0000adc0: 2c0a 2020 2020 2020 2020 6461 2c0a 2020  ,.        da,.  
+0000add0: 2020 2020 2020 6366 5f6e 616d 653d 4e6f        cf_name=No
+0000ade0: 6e65 2c0a 2020 2020 2020 2020 6c6f 633d  ne,.        loc=
+0000adf0: 4e6f 6e65 2c0a 2020 2020 2020 2020 636f  None,.        co
+0000ae00: 7079 3d54 7275 652c 0a20 2020 2020 2020  py=True,.       
+0000ae10: 2066 6f72 6d61 745f 636f 6f72 6473 3d54   format_coords=T
+0000ae20: 7275 652c 0a20 2020 2020 2020 2073 7461  rue,.        sta
+0000ae30: 6e64 6172 6469 7a65 3d54 7275 652c 0a20  ndardize=True,. 
+0000ae40: 2020 2020 2020 2072 656e 616d 653d 5472         rename=Tr
+0000ae50: 7565 2c0a 2020 2020 2020 2020 7370 6563  ue,.        spec
+0000ae60: 6961 6c69 7a65 3d46 616c 7365 2c0a 2020  ialize=False,.  
+0000ae70: 2020 2020 2020 6174 7472 733d 5472 7565        attrs=True
+0000ae80: 2c0a 2020 2020 2020 2020 7265 706c 6163  ,.        replac
+0000ae90: 655f 6174 7472 733d 4661 6c73 652c 0a20  e_attrs=False,. 
+0000aea0: 2020 2020 2020 2023 2061 6464 5f6c 6f63         # add_loc
+0000aeb0: 5f74 6f5f 6e61 6d65 3d4e 6f6e 652c 0a20  _to_name=None,. 
+0000aec0: 2020 2020 2020 2072 656e 616d 655f 6469         rename_di
+0000aed0: 6d73 3d54 7275 652c 0a20 2020 2029 3a0a  ms=True,.    ):.
+0000aee0: 2020 2020 2020 2020 2222 2246 6f72 6d61          """Forma
+0000aef0: 7420 6120 636f 6f72 6469 6e61 7465 2061  t a coordinate a
+0000af00: 7272 6179 0a0a 2020 2020 2020 2020 5061  rray..        Pa
+0000af10: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0000af20: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000af30: 2020 2020 6461 3a20 7861 7272 6179 2e44      da: xarray.D
+0000af40: 6174 6141 7272 6179 0a20 2020 2020 2020  ataArray.       
+0000af50: 2063 665f 6e61 6d65 3a20 7374 722c 204e   cf_name: str, N
+0000af60: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000af70: 4120 6765 6e65 7269 6320 4346 206e 616d  A generic CF nam
+0000af80: 652e 2049 6620 6e6f 7420 7072 6f76 6964  e. If not provid
+0000af90: 6564 2c20 6974 2067 7565 7373 6564 2077  ed, it guessed w
+0000afa0: 6974 6820 3a6d 6574 683a 606d 6174 6368  ith :meth:`match
+0000afb0: 602e 0a20 2020 2020 2020 206c 6f63 3a20  `..        loc: 
+0000afc0: 7374 722c 207b 2261 6e79 222c 204e 6f6e  str, {"any", Non
+0000afd0: 657d 2c20 7b22 222c 2046 616c 7365 7d0a  e}, {"", False}.
+0000afe0: 2020 2020 2020 2020 2020 2020 2d20 7374              - st
+0000aff0: 723a 206f 6e65 206f 6620 7468 6573 6520  r: one of these 
+0000b000: 6c6f 6361 7469 6f6e 730a 2020 2020 2020  locations.      
+0000b010: 2020 2020 2020 2d20 4e6f 6e65 206f 7220        - None or 
+0000b020: 2261 6e79 223a 2061 6e79 0a20 2020 2020  "any": any.     
+0000b030: 2020 2020 2020 202d 2046 616c 7365 206f         - False o
+0000b040: 7220 2722 223a 206e 6f20 6c6f 6361 7469  r '"": no locati
+0000b050: 6f6e 0a20 2020 2020 2020 2072 656e 616d  on.        renam
+0000b060: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+0000b070: 2020 2020 5265 6e61 6d65 2061 7272 6179      Rename array
+0000b080: 730a 2020 2020 2020 2020 6164 645f 6c6f  s.        add_lo
+0000b090: 635f 746f 5f6e 616d 653a 2062 6f6f 6c0a  c_to_name: bool.
+0000b0a0: 2020 2020 2020 2020 2020 2020 4164 6420              Add 
+0000b0b0: 6c6f 6320 746f 2074 6865 206e 616d 650a  loc to the name.
+0000b0c0: 2020 2020 2020 2020 7370 6563 6961 6c69          speciali
+0000b0d0: 7a65 3a20 626f 6f6c 0a20 2020 2020 2020  ze: bool.       
+0000b0e0: 2020 2020 2044 6f65 7320 6e6f 7420 7573       Does not us
+0000b0f0: 6520 7468 6520 4346 206e 616d 6520 666f  e the CF name fo
+0000b100: 7220 7265 6e61 6d69 6e67 2c20 6275 7420  r renaming, but 
+0000b110: 7468 6520 6669 7273 7420 6e61 6d65 0a20  the first name. 
+0000b120: 2020 2020 2020 2020 2020 2061 7320 6c69             as li
+0000b130: 7374 6564 2069 6e20 7370 6563 732c 2077  sted in specs, w
+0000b140: 6869 6368 2069 7320 6765 6e65 7261 6c6c  hich is generall
+0000b150: 7920 6120 7370 6563 6961 6c69 7a65 6420  y a specialized 
+0000b160: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0000b170: 206c 696b 6520 6120 6e61 6d65 2061 646f   like a name ado
+0000b180: 7074 6564 2062 7920 7370 6563 6961 6c69  pted by speciali
+0000b190: 7a65 6420 6461 7461 7365 742e 0a20 2020  zed dataset..   
+0000b1a0: 2020 2020 2073 7461 6e64 6172 6469 7a65       standardize
+0000b1b0: 3a20 626f 6f6c 0a20 2020 2020 2020 2072  : bool.        r
+0000b1c0: 656e 616d 655f 6469 6d3a 2062 6f6f 6c0a  ename_dim: bool.
+0000b1d0: 2020 2020 2020 2020 2020 2020 466f 7220              For 
+0000b1e0: 6120 3144 2061 7272 6179 2c20 7265 6e61  a 1D array, rena
+0000b1f0: 6d65 2074 6865 2064 696d 656e 7369 6f6e  me the dimension
+0000b200: 2069 6620 6974 2068 6173 2074 6865 2073   if it has the s
+0000b210: 616d 6520 6e61 6d65 0a20 2020 2020 2020  ame name.       
+0000b220: 2020 2020 2061 7320 7468 6520 6172 7261       as the arra
+0000b230: 792e 0a20 2020 2020 2020 2020 2020 204e  y..            N
+0000b240: 6f74 6520 7468 6174 2069 7420 6973 2073  ote that it is s
+0000b250: 6574 2074 6f20 4661 6c73 652c 2069 6620  et to False, if 
+0000b260: 6060 7265 6e61 6d65 6060 2069 7320 4661  ``rename`` is Fa
+0000b270: 6c73 652e 0a20 2020 2020 2020 2061 7474  lse..        att
+0000b280: 7273 3a20 626f 6f6c 2c20 6469 6374 0a20  rs: bool, dict. 
+0000b290: 2020 2020 2020 2020 2020 2049 6620 4661             If Fa
+0000b2a0: 6c73 652c 2064 6f65 7320 6e6f 7420 6368  lse, does not ch
+0000b2b0: 616e 6765 2061 7474 7269 6275 7465 7320  ange attributes 
+0000b2c0: 6174 2061 6c6c 2e0a 2020 2020 2020 2020  at all..        
+0000b2d0: 2020 2020 4966 2054 7275 652c 2075 7365      If True, use
+0000b2e0: 2043 6620 6174 7472 6962 7574 6573 2e0a   Cf attributes..
+0000b2f0: 2020 2020 2020 2020 2020 2020 4966 2061              If a
+0000b300: 2064 6963 742c 2075 7365 2074 6869 7320   dict, use this 
+0000b310: 6469 6374 2e0a 2020 2020 2020 2020 7265  dict..        re
+0000b320: 706c 6163 655f 6174 7472 733a 2062 6f6f  place_attrs: boo
+0000b330: 6c0a 2020 2020 2020 2020 2020 2020 5265  l.            Re
+0000b340: 706c 6163 6520 6578 6973 7469 6e67 2061  place existing a
+0000b350: 7474 7269 6275 7465 733f 0a0a 2020 2020  ttributes?..    
+0000b360: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+0000b370: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0000b380: 2020 2020 7861 7272 6179 2e44 6174 6141      xarray.DataA
+0000b390: 7272 6179 2c20 7374 722c 204e 6f6e 650a  rray, str, None.
+0000b3a0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000b3b0: 666f 726d 6174 7465 6420 6172 7261 7920  formatted array 
+0000b3c0: 6f72 2063 6f70 7920 6f66 2069 742e 0a20  or copy of it.. 
+0000b3d0: 2020 2020 2020 2020 2020 2054 6865 2043             The C
+0000b3e0: 4620 6e61 6d65 2c20 6769 7665 6e20 6f72  F name, given or
+0000b3f0: 206d 6174 6368 696e 672c 2069 6620 7265   matching, if re
+0000b400: 6e61 6d65 2069 6620 4661 6c73 653b 2061  name if False; a
+0000b410: 6e64 204e 6f6e 650a 2020 2020 2020 2020  nd None.        
+0000b420: 2020 2020 6966 206e 6f74 206d 6174 6368      if not match
+0000b430: 696e 672e 0a0a 2020 2020 2020 2020 5365  ing...        Se
+0000b440: 6520 616c 736f 0a20 2020 2020 2020 202d  e also.        -
+0000b450: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000b460: 4346 436f 6f72 6453 7065 6373 2e66 6f72  CFCoordSpecs.for
+0000b470: 6d61 745f 6461 7461 6172 7261 790a 2020  mat_dataarray.  
+0000b480: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000b490: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
+0000b4a0: 6f72 6d61 745f 6f62 6a5f 280a 2020 2020  ormat_obj_(.    
+0000b4b0: 2020 2020 2020 2020 6461 2c0a 2020 2020          da,.    
+0000b4c0: 2020 2020 2020 2020 6366 5f6e 616d 6573          cf_names
+0000b4d0: 3d7b 6461 2e6e 616d 653a 2063 665f 6e61  ={da.name: cf_na
+0000b4e0: 6d65 7d2c 0a20 2020 2020 2020 2020 2020  me},.           
+0000b4f0: 2063 6f70 793d 636f 7079 2c0a 2020 2020   copy=copy,.    
+0000b500: 2020 2020 2020 2020 7374 616e 6461 7264          standard
+0000b510: 697a 653d 7374 616e 6461 7264 697a 652c  ize=standardize,
+0000b520: 0a20 2020 2020 2020 2020 2020 2072 656e  .            ren
+0000b530: 616d 653d 7265 6e61 6d65 2c0a 2020 2020  ame=rename,.    
+0000b540: 2020 2020 2020 2020 7265 6e61 6d65 5f64          rename_d
+0000b550: 696d 733d 7265 6e61 6d65 5f64 696d 732c  ims=rename_dims,
+0000b560: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000b570: 6d61 745f 636f 6f72 6473 3d66 6f72 6d61  mat_coords=forma
+0000b580: 745f 636f 6f72 6473 2c0a 2020 2020 2020  t_coords,.      
+0000b590: 2020 2020 2020 7265 706c 6163 655f 6174        replace_at
+0000b5a0: 7472 733d 7265 706c 6163 655f 6174 7472  trs=replace_attr
+0000b5b0: 732c 0a20 2020 2020 2020 2020 2020 2061  s,.            a
+0000b5c0: 7474 7273 3d61 7474 7273 2069 6620 6973  ttrs=attrs if is
+0000b5d0: 696e 7374 616e 6365 2861 7474 7273 2c20  instance(attrs, 
+0000b5e0: 626f 6f6c 2920 656c 7365 207b 6461 2e6e  bool) else {da.n
+0000b5f0: 616d 653a 2061 7474 7273 7d2c 0a20 2020  ame: attrs},.   
+0000b600: 2020 2020 2020 2020 2073 7065 6369 616c           special
+0000b610: 697a 653d 7370 6563 6961 6c69 7a65 2c0a  ize=specialize,.
+0000b620: 2020 2020 2020 2020 2020 2020 6361 7465              cate
+0000b630: 676f 7269 6573 3d5b 2263 6f6f 7264 7322  gories=["coords"
+0000b640: 5d2c 0a20 2020 2020 2020 2020 2020 206c  ],.            l
+0000b650: 6f63 3d6c 6f63 2c0a 2020 2020 2020 2020  oc=loc,.        
+0000b660: 290a 0a20 2020 2064 6566 2066 6f72 6d61  )..    def forma
+0000b670: 745f 6461 7461 5f76 6172 280a 2020 2020  t_data_var(.    
+0000b680: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000b690: 2020 6461 2c0a 2020 2020 2020 2020 6366    da,.        cf
+0000b6a0: 5f6e 616d 653d 4e6f 6e65 2c0a 2020 2020  _name=None,.    
+0000b6b0: 2020 2020 6c6f 633d 4e6f 6e65 2c0a 2020      loc=None,.  
+0000b6c0: 2020 2020 2020 636f 7079 3d54 7275 652c        copy=True,
+0000b6d0: 0a20 2020 2020 2020 2072 656e 616d 653d  .        rename=
+0000b6e0: 5472 7565 2c0a 2020 2020 2020 2020 7265  True,.        re
+0000b6f0: 6e61 6d65 5f64 696d 733d 5472 7565 2c0a  name_dims=True,.
+0000b700: 2020 2020 2020 2020 7370 6563 6961 6c69          speciali
+0000b710: 7a65 3d46 616c 7365 2c0a 2020 2020 2020  ze=False,.      
+0000b720: 2020 666f 726d 6174 5f63 6f6f 7264 733d    format_coords=
+0000b730: 5472 7565 2c0a 2020 2020 2020 2020 6174  True,.        at
+0000b740: 7472 733d 5472 7565 2c0a 2020 2020 2020  trs=True,.      
+0000b750: 2020 7265 706c 6163 655f 6174 7472 733d    replace_attrs=
+0000b760: 4661 6c73 652c 0a20 2020 2020 2020 2073  False,.        s
+0000b770: 7461 6e64 6172 6469 7a65 3d54 7275 652c  tandardize=True,
+0000b780: 0a20 2020 2020 2020 2023 2061 6464 5f6c  .        # add_l
+0000b790: 6f63 5f74 6f5f 6e61 6d65 3d4e 6f6e 652c  oc_to_name=None,
+0000b7a0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0000b7b0: 2222 2246 6f72 6d61 7420 6120 6461 7461  """Format a data
+0000b7c0: 5f76 6172 2061 7272 6179 0a0a 2020 2020  _var array..    
+0000b7d0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000b7e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000b7f0: 2d0a 2020 2020 2020 2020 6461 3a20 7861  -.        da: xa
+0000b800: 7272 6179 2e44 6174 6141 7272 6179 0a20  rray.DataArray. 
+0000b810: 2020 2020 2020 2063 665f 6e61 6d65 3a20         cf_name: 
+0000b820: 7374 722c 204e 6f6e 650a 2020 2020 2020  str, None.      
+0000b830: 2020 2020 2020 4120 6765 6e65 7269 6320        A generic 
+0000b840: 4346 206e 616d 652e 2049 6620 6e6f 7420  CF name. If not 
+0000b850: 7072 6f76 6964 6564 2c20 6974 2067 7565  provided, it gue
+0000b860: 7373 6564 2077 6974 6820 3a6d 6574 683a  ssed with :meth:
+0000b870: 606d 6174 6368 602e 0a20 2020 2020 2020  `match`..       
+0000b880: 206c 6f63 3a20 7374 722c 207b 2261 6e79   loc: str, {"any
+0000b890: 222c 204e 6f6e 657d 2c20 7b22 222c 2046  ", None}, {"", F
+0000b8a0: 616c 7365 7d0a 2020 2020 2020 2020 2020  alse}.          
+0000b8b0: 2020 2d20 7374 723a 206f 6e65 206f 6620    - str: one of 
+0000b8c0: 7468 6573 6520 6c6f 6361 7469 6f6e 730a  these locations.
+0000b8d0: 2020 2020 2020 2020 2020 2020 2d20 4e6f              - No
+0000b8e0: 6e65 206f 7220 2261 6e79 223a 2061 6e79  ne or "any": any
+0000b8f0: 0a20 2020 2020 2020 2020 2020 202d 2046  .            - F
+0000b900: 616c 7365 206f 7220 2722 223a 206e 6f20  alse or '"": no 
+0000b910: 6c6f 6361 7469 6f6e 0a20 2020 2020 2020  location.       
+0000b920: 2072 656e 616d 653a 2062 6f6f 6c0a 2020   rename: bool.  
+0000b930: 2020 2020 2020 2020 2020 5265 6e61 6d65            Rename
+0000b940: 2061 7272 6179 730a 2020 2020 2020 2020   arrays.        
+0000b950: 6164 645f 6c6f 635f 746f 5f6e 616d 653a  add_loc_to_name:
+0000b960: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
+0000b970: 2020 4164 6420 6c6f 6320 746f 2074 6865    Add loc to the
+0000b980: 206e 616d 650a 2020 2020 2020 2020 7370   name.        sp
+0000b990: 6563 6961 6c69 7a65 3a20 626f 6f6c 0a20  ecialize: bool. 
+0000b9a0: 2020 2020 2020 2020 2020 2044 6f65 7320             Does 
+0000b9b0: 6e6f 7420 7573 6520 7468 6520 4346 206e  not use the CF n
+0000b9c0: 616d 6520 666f 7220 7265 6e61 6d69 6e67  ame for renaming
+0000b9d0: 2c20 6275 7420 7468 6520 6669 7273 7420  , but the first 
+0000b9e0: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+0000b9f0: 2061 7320 6c69 7374 6564 2069 6e20 7370   as listed in sp
+0000ba00: 6563 732c 2077 6869 6368 2069 7320 6765  ecs, which is ge
+0000ba10: 6e65 7261 6c6c 7920 6120 7370 6563 6961  nerally a specia
+0000ba20: 6c69 7a65 6420 6f6e 652c 0a20 2020 2020  lized one,.     
+0000ba30: 2020 2020 2020 206c 696b 6520 6120 6e61         like a na
+0000ba40: 6d65 2061 646f 7074 6564 2062 7920 7370  me adopted by sp
+0000ba50: 6563 6961 6c69 7a65 6420 6461 7461 7365  ecialized datase
+0000ba60: 742e 0a20 2020 2020 2020 2073 7461 6e64  t..        stand
+0000ba70: 6172 6469 7a65 3a20 626f 6f6c 0a20 2020  ardize: bool.   
+0000ba80: 2020 2020 2072 656e 616d 655f 6469 6d73       rename_dims
+0000ba90: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
+0000baa0: 2020 2046 6f72 2061 2031 4420 6172 7261     For a 1D arra
+0000bab0: 792c 2072 656e 616d 6520 7468 6520 6469  y, rename the di
+0000bac0: 6d65 6e73 696f 6e20 6966 2069 7420 6861  mension if it ha
+0000bad0: 7320 7468 6520 7361 6d65 206e 616d 650a  s the same name.
+0000bae0: 2020 2020 2020 2020 2020 2020 6173 2074              as t
+0000baf0: 6865 2061 7272 6179 2e0a 2020 2020 2020  he array..      
+0000bb00: 2020 2020 2020 4e6f 7465 2074 6861 7420        Note that 
+0000bb10: 6974 2069 7320 7365 7420 746f 2046 616c  it is set to Fal
+0000bb20: 7365 2c20 6966 2060 6072 656e 616d 6560  se, if ``rename`
+0000bb30: 6020 6973 2046 616c 7365 2e0a 2020 2020  ` is False..    
+0000bb40: 2020 2020 6174 7472 733a 2062 6f6f 6c2c      attrs: bool,
+0000bb50: 2064 6963 740a 2020 2020 2020 2020 2020   dict.          
+0000bb60: 2020 4966 2046 616c 7365 2c20 646f 6573    If False, does
+0000bb70: 206e 6f74 2063 6861 6e67 6520 6174 7472   not change attr
+0000bb80: 6962 7574 6573 2061 7420 616c 6c2e 0a20  ibutes at all.. 
+0000bb90: 2020 2020 2020 2020 2020 2049 6620 5472             If Tr
+0000bba0: 7565 2c20 7573 6520 4366 2061 7474 7269  ue, use Cf attri
+0000bbb0: 6275 7465 732e 0a20 2020 2020 2020 2020  butes..         
+0000bbc0: 2020 2049 6620 6120 6469 6374 2c20 7573     If a dict, us
+0000bbd0: 6520 7468 6973 2064 6963 742e 0a20 2020  e this dict..   
+0000bbe0: 2020 2020 2072 6570 6c61 6365 5f61 7474       replace_att
+0000bbf0: 7273 3a20 626f 6f6c 0a20 2020 2020 2020  rs: bool.       
+0000bc00: 2020 2020 2052 6570 6c61 6365 2065 7869       Replace exi
+0000bc10: 7374 696e 6720 6174 7472 6962 7574 6573  sting attributes
+0000bc20: 3f0a 0a20 2020 2020 2020 2052 6574 7572  ?..        Retur
+0000bc30: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+0000bc40: 2d2d 0a20 2020 2020 2020 2078 6172 7261  --.        xarra
+0000bc50: 792e 4461 7461 4172 7261 792c 2073 7472  y.DataArray, str
+0000bc60: 2c20 4e6f 6e65 0a20 2020 2020 2020 2020  , None.         
+0000bc70: 2020 2054 6865 2066 6f72 6d61 7474 6564     The formatted
+0000bc80: 2061 7272 6179 206f 7220 636f 7079 206f   array or copy o
+0000bc90: 6620 6974 2e0a 2020 2020 2020 2020 2020  f it..          
+0000bca0: 2020 5468 6520 4346 206e 616d 652c 2067    The CF name, g
+0000bcb0: 6976 656e 206f 7220 6d61 7463 6869 6e67  iven or matching
+0000bcc0: 2c20 6966 2072 656e 616d 6520 6966 2046  , if rename if F
+0000bcd0: 616c 7365 3b20 616e 6420 4e6f 6e65 0a20  alse; and None. 
+0000bce0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000bcf0: 7420 6d61 7463 6869 6e67 2e0a 0a20 2020  t matching...   
+0000bd00: 2020 2020 2053 6565 2061 6c73 6f0a 2020       See also.  
+0000bd10: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20        --------. 
+0000bd20: 2020 2020 2020 2043 4643 6f6f 7264 5370         CFCoordSp
+0000bd30: 6563 732e 666f 726d 6174 5f64 6174 6161  ecs.format_dataa
+0000bd40: 7272 6179 0a20 2020 2020 2020 2022 2222  rray.        """
+0000bd50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000bd60: 7365 6c66 2e5f 666f 726d 6174 5f6f 626a  self._format_obj
+0000bd70: 5f28 0a20 2020 2020 2020 2020 2020 2064  _(.            d
+0000bd80: 612c 0a20 2020 2020 2020 2020 2020 2063  a,.            c
+0000bd90: 665f 6e61 6d65 733d 7b64 612e 6e61 6d65  f_names={da.name
+0000bda0: 3a20 6366 5f6e 616d 657d 2c0a 2020 2020  : cf_name},.    
+0000bdb0: 2020 2020 2020 2020 636f 7079 3d63 6f70          copy=cop
+0000bdc0: 792c 0a20 2020 2020 2020 2020 2020 2072  y,.            r
+0000bdd0: 656e 616d 653d 7265 6e61 6d65 2c0a 2020  ename=rename,.  
+0000bde0: 2020 2020 2020 2020 2020 7265 6e61 6d65            rename
+0000bdf0: 5f64 696d 733d 7265 6e61 6d65 5f64 696d  _dims=rename_dim
+0000be00: 732c 0a20 2020 2020 2020 2020 2020 2073  s,.            s
+0000be10: 7065 6369 616c 697a 653d 7370 6563 6961  pecialize=specia
+0000be20: 6c69 7a65 2c0a 2020 2020 2020 2020 2020  lize,.          
+0000be30: 2020 666f 726d 6174 5f63 6f6f 7264 733d    format_coords=
+0000be40: 666f 726d 6174 5f63 6f6f 7264 732c 0a20  format_coords,. 
+0000be50: 2020 2020 2020 2020 2020 2072 6570 6c61             repla
+0000be60: 6365 5f61 7474 7273 3d72 6570 6c61 6365  ce_attrs=replace
+0000be70: 5f61 7474 7273 2c0a 2020 2020 2020 2020  _attrs,.        
+0000be80: 2020 2020 6174 7472 733d 6174 7472 7320      attrs=attrs 
+0000be90: 6966 2069 7369 6e73 7461 6e63 6528 6174  if isinstance(at
+0000bea0: 7472 732c 2062 6f6f 6c29 2065 6c73 6520  trs, bool) else 
+0000beb0: 7b64 612e 6e61 6d65 3a20 6174 7472 737d  {da.name: attrs}
+0000bec0: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
+0000bed0: 616e 6461 7264 697a 653d 7374 616e 6461  andardize=standa
+0000bee0: 7264 697a 652c 0a20 2020 2020 2020 2020  rdize,.         
+0000bef0: 2020 2063 6174 6567 6f72 6965 733d 5b22     categories=["
+0000bf00: 636f 6f72 6473 222c 2022 6461 7461 5f76  coords", "data_v
+0000bf10: 6172 7322 5d2c 0a20 2020 2020 2020 2020  ars"],.         
+0000bf20: 2020 206c 6f63 3d6c 6f63 2c0a 2020 2020     loc=loc,.    
+0000bf30: 2020 2020 290a 0a20 2020 2064 6566 2066      )..    def f
+0000bf40: 6f72 6d61 745f 6461 7461 7365 7428 0a20  ormat_dataset(. 
+0000bf50: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000bf60: 2020 2020 2064 732c 0a20 2020 2020 2020       ds,.       
+0000bf70: 2063 665f 6e61 6d65 733d 4e6f 6e65 2c0a   cf_names=None,.
+0000bf80: 2020 2020 2020 2020 2320 6c6f 633d 4e6f          # loc=No
+0000bf90: 6e65 2c0a 2020 2020 2020 2020 636f 7079  ne,.        copy
+0000bfa0: 3d54 7275 652c 0a20 2020 2020 2020 2066  =True,.        f
+0000bfb0: 6f72 6d61 745f 636f 6f72 6473 3d54 7275  ormat_coords=Tru
+0000bfc0: 652c 0a20 2020 2020 2020 2073 7461 6e64  e,.        stand
+0000bfd0: 6172 6469 7a65 3d54 7275 652c 0a20 2020  ardize=True,.   
+0000bfe0: 2020 2020 2072 656e 616d 653d 5472 7565       rename=True
+0000bff0: 2c0a 2020 2020 2020 2020 7265 6e61 6d65  ,.        rename
+0000c000: 5f64 696d 733d 5472 7565 2c0a 2020 2020  _dims=True,.    
+0000c010: 2020 2020 7370 6563 6961 6c69 7a65 3d46      specialize=F
+0000c020: 616c 7365 2c0a 2020 2020 2020 2020 6174  alse,.        at
+0000c030: 7472 733d 5472 7565 2c0a 2020 2020 2020  trs=True,.      
+0000c040: 2020 7265 706c 6163 655f 6174 7472 733d    replace_attrs=
+0000c050: 4661 6c73 652c 0a20 2020 2020 2020 2023  False,.        #
+0000c060: 2061 6464 5f6c 6f63 5f74 6f5f 6e61 6d65   add_loc_to_name
+0000c070: 3d4e 6f6e 650a 2020 2020 293a 0a20 2020  =None.    ):.   
+0000c080: 2020 2020 2022 2222 466f 726d 6174 2061       """Format a
+0000c090: 2077 686f 6c65 2064 6174 6173 6574 0a0a   whole dataset..
+0000c0a0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0000c0b0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+0000c0c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6473  -----.        ds
+0000c0d0: 3a20 7861 7272 6179 2e44 6174 6173 6574  : xarray.Dataset
+0000c0e0: 0a20 2020 2020 2020 2063 665f 6e61 6d65  .        cf_name
+0000c0f0: 733a 2064 6963 742c 204e 6f6e 650a 2020  s: dict, None.  
+0000c100: 2020 2020 2020 2020 2020 4469 6374 206f            Dict o
+0000c110: 6620 6e61 6d65 7320 6173 206b 6579 7320  f names as keys 
+0000c120: 616e 6420 6765 6e65 7269 6320 4346 206e  and generic CF n
+0000c130: 616d 6573 2061 7320 7661 6c75 6573 2e0a  ames as values..
+0000c140: 2020 2020 2020 2020 2020 2020 4966 206e              If n
+0000c150: 6f74 2070 726f 7669 6465 642c 2043 4620  ot provided, CF 
+0000c160: 6e61 6d65 7320 6172 6520 6775 6573 7365  names are guesse
+0000c170: 6420 7769 7468 203a 6d65 7468 3a60 6d61  d with :meth:`ma
+0000c180: 7463 6860 2e0a 2020 2020 2020 2020 6c6f  tch`..        lo
+0000c190: 633a 2073 7472 2c20 7b22 616e 7922 2c20  c: str, {"any", 
+0000c1a0: 4e6f 6e65 7d2c 207b 2222 2c20 4661 6c73  None}, {"", Fals
+0000c1b0: 657d 0a20 2020 2020 2020 2020 2020 202d  e}.            -
+0000c1c0: 2073 7472 3a20 6f6e 6520 6f66 2074 6865   str: one of the
+0000c1d0: 7365 206c 6f63 6174 696f 6e73 0a20 2020  se locations.   
+0000c1e0: 2020 2020 2020 2020 202d 204e 6f6e 6520           - None 
+0000c1f0: 6f72 2022 616e 7922 3a20 616e 790a 2020  or "any": any.  
+0000c200: 2020 2020 2020 2020 2020 2d20 4661 6c73            - Fals
+0000c210: 6520 6f72 2027 2222 3a20 6e6f 206c 6f63  e or '"": no loc
+0000c220: 6174 696f 6e0a 2020 2020 2020 2020 7265  ation.        re
+0000c230: 6e61 6d65 3a20 626f 6f6c 0a20 2020 2020  name: bool.     
+0000c240: 2020 2020 2020 2052 656e 616d 6520 6172         Rename ar
+0000c250: 7261 7973 0a20 2020 2020 2020 2061 6464  rays.        add
+0000c260: 5f6c 6f63 5f74 6f5f 6e61 6d65 3a20 626f  _loc_to_name: bo
+0000c270: 6f6c 0a20 2020 2020 2020 2020 2020 2041  ol.            A
+0000c280: 6464 206c 6f63 2074 6f20 7468 6520 6e61  dd loc to the na
+0000c290: 6d65 0a20 2020 2020 2020 2073 7065 6369  me.        speci
+0000c2a0: 616c 697a 653a 2062 6f6f 6c0a 2020 2020  alize: bool.    
+0000c2b0: 2020 2020 2020 2020 446f 6573 206e 6f74          Does not
+0000c2c0: 2075 7365 2074 6865 2043 4620 6e61 6d65   use the CF name
+0000c2d0: 2066 6f72 2072 656e 616d 696e 672c 2062   for renaming, b
+0000c2e0: 7574 2074 6865 2066 6972 7374 206e 616d  ut the first nam
+0000c2f0: 650a 2020 2020 2020 2020 2020 2020 6173  e.            as
+0000c300: 206c 6973 7465 6420 696e 2073 7065 6373   listed in specs
+0000c310: 2c20 7768 6963 6820 6973 2067 656e 6572  , which is gener
+0000c320: 616c 6c79 2061 2073 7065 6369 616c 697a  ally a specializ
+0000c330: 6564 206f 6e65 2c0a 2020 2020 2020 2020  ed one,.        
+0000c340: 2020 2020 6c69 6b65 2061 206e 616d 6520      like a name 
+0000c350: 6164 6f70 7465 6420 6279 2073 7065 6369  adopted by speci
+0000c360: 616c 697a 6564 2064 6174 6173 6574 2e0a  alized dataset..
+0000c370: 2020 2020 2020 2020 7374 616e 6461 7264          standard
+0000c380: 697a 653a 2062 6f6f 6c0a 2020 2020 2020  ize: bool.      
+0000c390: 2020 7265 6e61 6d65 5f64 696d 3a20 626f    rename_dim: bo
+0000c3a0: 6f6c 0a20 2020 2020 2020 2020 2020 2046  ol.            F
+0000c3b0: 6f72 2061 2031 4420 6172 7261 792c 2072  or a 1D array, r
+0000c3c0: 656e 616d 6520 7468 6520 6469 6d65 6e73  ename the dimens
+0000c3d0: 696f 6e20 6966 2069 7420 6861 7320 7468  ion if it has th
+0000c3e0: 6520 7361 6d65 206e 616d 650a 2020 2020  e same name.    
+0000c3f0: 2020 2020 2020 2020 6173 2074 6865 2061          as the a
+0000c400: 7272 6179 2e0a 2020 2020 2020 2020 2020  rray..          
+0000c410: 2020 4e6f 7465 2074 6861 7420 6974 2069    Note that it i
+0000c420: 7320 7365 7420 746f 2046 616c 7365 2c20  s set to False, 
+0000c430: 6966 2060 6072 656e 616d 6560 6020 6973  if ``rename`` is
+0000c440: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
+0000c450: 6174 7472 733a 2062 6f6f 6c2c 2064 6963  attrs: bool, dic
+0000c460: 7420 6f66 2064 6963 740a 2020 2020 2020  t of dict.      
+0000c470: 2020 2020 2020 4966 2046 616c 7365 2c20        If False, 
+0000c480: 646f 6573 206e 6f74 2063 6861 6e67 6520  does not change 
+0000c490: 6174 7472 6962 7574 6573 2061 7420 616c  attributes at al
+0000c4a0: 6c2e 0a20 2020 2020 2020 2020 2020 2049  l..            I
+0000c4b0: 6620 5472 7565 2c20 7573 6520 4366 2061  f True, use Cf a
+0000c4c0: 7474 7269 6275 7465 732e 0a20 2020 2020  ttributes..     
+0000c4d0: 2020 2020 2020 2049 6620 6120 6469 6374         If a dict
+0000c4e0: 2c20 7573 6520 7468 6973 2064 6963 742e  , use this dict.
+0000c4f0: 0a20 2020 2020 2020 2072 6570 6c61 6365  .        replace
+0000c500: 5f61 7474 7273 3a20 626f 6f6c 0a20 2020  _attrs: bool.   
+0000c510: 2020 2020 2020 2020 2052 6570 6c61 6365           Replace
+0000c520: 2065 7869 7374 696e 6720 6174 7472 6962   existing attrib
+0000c530: 7574 6573 3f0a 0a20 2020 2020 2020 2052  utes?..        R
+0000c540: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+0000c550: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2078  ------.        x
+0000c560: 6172 7261 792e 4461 7461 4172 7261 792c  array.DataArray,
+0000c570: 2073 7472 2c20 4e6f 6e65 0a20 2020 2020   str, None.     
+0000c580: 2020 2020 2020 2054 6865 2066 6f72 6d61         The forma
+0000c590: 7474 6564 2061 7272 6179 206f 7220 636f  tted array or co
+0000c5a0: 7079 206f 6620 6974 2e0a 2020 2020 2020  py of it..      
+0000c5b0: 2020 2020 2020 5468 6520 4346 206e 616d        The CF nam
+0000c5c0: 652c 2067 6976 656e 206f 7220 6d61 7463  e, given or matc
+0000c5d0: 6869 6e67 2c20 6966 2072 656e 616d 6520  hing, if rename 
+0000c5e0: 6966 2046 616c 7365 3b20 616e 6420 4e6f  if False; and No
+0000c5f0: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
+0000c600: 6620 6e6f 7420 6d61 7463 6869 6e67 2e0a  f not matching..
+0000c610: 0a20 2020 2020 2020 2053 6565 2061 6c73  .        See als
+0000c620: 6f0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  o.        ------
+0000c630: 2d2d 0a20 2020 2020 2020 2043 4643 6f6f  --.        CFCoo
+0000c640: 7264 5370 6563 732e 666f 726d 6174 5f64  rdSpecs.format_d
+0000c650: 6174 6161 7272 6179 0a20 2020 2020 2020  ataarray.       
+0000c660: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+0000c670: 7572 6e20 7365 6c66 2e5f 666f 726d 6174  urn self._format
+0000c680: 5f6f 626a 5f28 0a20 2020 2020 2020 2020  _obj_(.         
+0000c690: 2020 2064 732c 0a20 2020 2020 2020 2020     ds,.         
+0000c6a0: 2020 2063 665f 6e61 6d65 733d 6366 5f6e     cf_names=cf_n
+0000c6b0: 616d 6573 2c0a 2020 2020 2020 2020 2020  ames,.          
+0000c6c0: 2020 636f 7079 3d63 6f70 792c 0a20 2020    copy=copy,.   
+0000c6d0: 2020 2020 2020 2020 2073 7461 6e64 6172           standar
+0000c6e0: 6469 7a65 3d73 7461 6e64 6172 6469 7a65  dize=standardize
+0000c6f0: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
+0000c700: 6e61 6d65 3d72 656e 616d 652c 0a20 2020  name=rename,.   
+0000c710: 2020 2020 2020 2020 2072 656e 616d 655f           rename_
+0000c720: 6469 6d73 3d72 656e 616d 655f 6469 6d73  dims=rename_dims
+0000c730: 2c0a 2020 2020 2020 2020 2020 2020 666f  ,.            fo
+0000c740: 726d 6174 5f63 6f6f 7264 733d 666f 726d  rmat_coords=form
+0000c750: 6174 5f63 6f6f 7264 732c 0a20 2020 2020  at_coords,.     
+0000c760: 2020 2020 2020 2072 6570 6c61 6365 5f61         replace_a
+0000c770: 7474 7273 3d72 6570 6c61 6365 5f61 7474  ttrs=replace_att
+0000c780: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
+0000c790: 6174 7472 733d 6174 7472 732c 0a20 2020  attrs=attrs,.   
+0000c7a0: 2020 2020 2020 2020 2073 7065 6369 616c           special
+0000c7b0: 697a 653d 7370 6563 6961 6c69 7a65 2c0a  ize=specialize,.
+0000c7c0: 2020 2020 2020 2020 2020 2020 6361 7465              cate
+0000c7d0: 676f 7269 6573 3d5b 2263 6f6f 7264 7322  gories=["coords"
+0000c7e0: 2c20 2264 6174 615f 7661 7273 225d 2c0a  , "data_vars"],.
+0000c7f0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+0000c800: 6566 2061 7574 6f5f 666f 726d 6174 2873  ef auto_format(s
+0000c810: 656c 662c 206f 626a 2c20 2a2a 6b77 6172  elf, obj, **kwar
+0000c820: 6773 293a 0a20 2020 2020 2020 2022 2222  gs):.        """
+0000c830: 5265 6e61 6d65 2076 6172 6961 626c 6573  Rename variables
+0000c840: 2061 6e64 2063 6f6f 7264 696e 6174 6573   and coordinates
+0000c850: 2061 6e64 2066 696c 6c20 7468 6569 7220   and fill their 
+0000c860: 6174 7472 6962 7574 6573 0a0a 2020 2020  attributes..    
+0000c870: 2020 2020 5365 6520 616c 736f 0a20 2020      See also.   
+0000c880: 2020 2020 202d 2d2d 2d2d 2d2d 2d0a 2020       --------.  
+0000c890: 2020 2020 2020 656e 636f 6465 0a20 2020        encode.   
+0000c8a0: 2020 2020 2066 6f72 6d61 745f 6461 7461       format_data
+0000c8b0: 5f76 6172 0a20 2020 2020 2020 2066 6f72  _var.        for
+0000c8c0: 6d61 745f 6461 7461 7365 740a 2020 2020  mat_dataset.    
+0000c8d0: 2020 2020 6669 6c6c 5f61 7474 7273 0a20      fill_attrs. 
+0000c8e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000c8f0: 2020 2069 6620 6861 7361 7474 7228 6f62     if hasattr(ob
+0000c900: 6a2c 2022 6461 7461 5f76 6172 7322 293a  j, "data_vars"):
+0000c910: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000c920: 7572 6e20 7365 6c66 2e66 6f72 6d61 745f  urn self.format_
+0000c930: 6461 7461 7365 7428 6f62 6a2c 202a 2a6b  dataset(obj, **k
+0000c940: 7761 7267 7329 0a20 2020 2020 2020 2072  wargs).        r
+0000c950: 6574 7572 6e20 7365 6c66 2e66 6f72 6d61  eturn self.forma
+0000c960: 745f 6461 7461 5f76 6172 286f 626a 2c20  t_data_var(obj, 
+0000c970: 2a2a 6b77 6172 6773 290a 0a20 2020 2064  **kwargs)..    d
+0000c980: 6566 2064 6563 6f64 6528 7365 6c66 2c20  ef decode(self, 
+0000c990: 6f62 6a2c 202a 2a6b 7761 7267 7329 3a0a  obj, **kwargs):.
+0000c9a0: 2020 2020 2020 2020 2222 2241 7574 6f20          """Auto 
+0000c9b0: 666f 726d 6174 2c20 696e 6665 7220 636f  format, infer co
+0000c9c0: 6f72 6469 6e61 7465 7320 616e 6420 7265  ordinates and re
+0000c9d0: 6e61 6d65 2074 6f20 6765 6e65 7269 6320  name to generic 
+0000c9e0: 6e61 6d65 730a 0a20 2020 2020 2020 2053  names..        S
+0000c9f0: 6565 2061 6c73 6f0a 2020 2020 2020 2020  ee also.        
+0000ca00: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000ca10: 2061 7574 6f5f 666f 726d 6174 0a20 2020   auto_format.   
+0000ca20: 2020 2020 2065 6e63 6f64 650a 2020 2020       encode.    
+0000ca30: 2020 2020 666f 726d 6174 5f64 6174 6161      format_dataa
+0000ca40: 7272 6179 0a20 2020 2020 2020 2066 6f72  rray.        for
+0000ca50: 6d61 745f 6461 7461 7365 740a 2020 2020  mat_dataset.    
+0000ca60: 2020 2020 6669 6c6c 5f61 7474 7273 0a20      fill_attrs. 
+0000ca70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000ca80: 2020 2023 2043 6f6f 7264 696e 6174 6573     # Coordinates
+0000ca90: 0a20 2020 2020 2020 206f 626a 203d 2073  .        obj = s
+0000caa0: 656c 662e 696e 6665 725f 636f 6f72 6473  elf.infer_coords
+0000cab0: 286f 626a 290a 0a20 2020 2020 2020 2023  (obj)..        #
+0000cac0: 204e 616d 6573 2061 6e64 2061 7474 7269   Names and attri
+0000cad0: 6275 7465 730a 2020 2020 2020 2020 6f62  butes.        ob
+0000cae0: 6a20 3d20 7365 6c66 2e61 7574 6f5f 666f  j = self.auto_fo
+0000caf0: 726d 6174 286f 626a 2c20 2a2a 6b77 6172  rmat(obj, **kwar
+0000cb00: 6773 290a 0a20 2020 2020 2020 2023 2041  gs)..        # A
+0000cb10: 7373 6967 6e20 6366 2073 7065 6373 0a20  ssign cf specs. 
+0000cb20: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+0000cb30: 616d 6520 616e 6420 7365 6c66 2069 6e20  ame and self in 
+0000cb40: 6765 745f 7265 6769 7374 6572 6564 5f63  get_registered_c
+0000cb50: 665f 7370 6563 7328 293a 0a20 2020 2020  f_specs():.     
+0000cb60: 2020 2020 2020 206f 626a 203d 2061 7373         obj = ass
+0000cb70: 6967 6e5f 6366 5f73 7065 6373 286f 626a  ign_cf_specs(obj
+0000cb80: 2c20 7365 6c66 2e6e 616d 6529 0a0a 2020  , self.name)..  
+0000cb90: 2020 2020 2020 7265 7475 726e 206f 626a        return obj
+0000cba0: 0a0a 2020 2020 6465 6620 656e 636f 6465  ..    def encode
+0000cbb0: 2873 656c 662c 206f 626a 2c20 2a2a 6b77  (self, obj, **kw
+0000cbc0: 6172 6773 293a 0a20 2020 2020 2020 2022  args):.        "
+0000cbd0: 2222 5361 6d65 2061 7320 3a6d 6574 683a  ""Same as :meth:
+0000cbe0: 6064 6563 6f64 6560 2062 7574 2072 656e  `decode` but ren
+0000cbf0: 616d 6520 7769 7468 2074 6865 2073 7065  ame with the spe
+0000cc00: 6369 616c 697a 6564 206e 616d 650a 0a20  cialized name.. 
+0000cc10: 2020 2020 2020 2053 6565 2061 6c73 6f0a         See also.
+0000cc20: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0000cc30: 0a20 2020 2020 2020 2064 6563 6f64 650a  .        decode.
+0000cc40: 2020 2020 2020 2020 6175 746f 5f66 6f72          auto_for
+0000cc50: 6d61 740a 2020 2020 2020 2020 666f 726d  mat.        form
+0000cc60: 6174 5f64 6174 6161 7272 6179 0a20 2020  at_dataarray.   
+0000cc70: 2020 2020 2066 6f72 6d61 745f 6461 7461       format_data
+0000cc80: 7365 740a 2020 2020 2020 2020 6669 6c6c  set.        fill
+0000cc90: 5f61 7474 7273 0a20 2020 2020 2020 2022  _attrs.        "
+0000cca0: 2222 0a20 2020 2020 2020 206b 7761 7267  "".        kwarg
+0000ccb0: 732e 7365 7464 6566 6175 6c74 2822 7370  s.setdefault("sp
+0000ccc0: 6563 6961 6c69 7a65 222c 2054 7275 6529  ecialize", True)
+0000ccd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000cce0: 7365 6c66 2e64 6563 6f64 6528 6f62 6a2c  self.decode(obj,
+0000ccf0: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
+0000cd00: 6465 6620 746f 5f6c 6f63 2873 656c 662c  def to_loc(self,
+0000cd10: 206f 626a 2c20 2a2a 6c6f 6373 293a 0a20   obj, **locs):. 
+0000cd20: 2020 2020 2020 2022 2222 5365 7420 7468         """Set th
+0000cd30: 6520 7374 6167 6765 7265 6420 6772 6964  e staggered grid
+0000cd40: 206c 6f63 6174 696f 6e20 666f 7220 7370   location for sp
+0000cd50: 6563 6966 6965 6420 6e61 6d65 730a 0a20  ecified names.. 
+0000cd60: 2020 2020 2020 202e 2e20 6e6f 7465 3a3a         .. note::
+0000cd70: 2049 7420 6f6e 6c79 2063 6861 6e67 6573   It only changes
+0000cd80: 2074 6865 206e 616d 6573 2c20 6e6f 7420   the names, not 
+0000cd90: 7468 6520 6174 7472 6962 7574 6573 2e0a  the attributes..
+0000cda0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0000cdb0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+0000cdc0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 206f  ------.        o
+0000cdd0: 626a 3a20 7861 7272 6179 2e44 6174 6173  bj: xarray.Datas
+0000cde0: 6574 2c20 7861 7272 6179 2e44 6174 6141  et, xarray.DataA
+0000cdf0: 7272 6179 0a20 2020 2020 2020 206c 6f63  rray.        loc
+0000ce00: 733a 2064 6963 740a 2020 2020 2020 2020  s: dict.        
+0000ce10: 2020 2020 2a2a 4b65 7973 2061 7265 2072      **Keys are r
+0000ce20: 6f6f 7420 6e61 6d65 732a 2a2c 2076 616c  oot names**, val
+0000ce30: 7565 7320 6172 6520 6e65 7720 6c6f 6361  ues are new loca
+0000ce40: 7469 6f6e 732e 0a20 2020 2020 2020 2020  tions..         
+0000ce50: 2020 2041 2076 616c 7565 206f 6620 6046     A value of `F
+0000ce60: 616c 7365 602c 2072 656d 6f76 6520 7468  alse`, remove th
+0000ce70: 6520 6c6f 6361 7469 6f6e 2e0a 2020 2020  e location..    
+0000ce80: 2020 2020 2020 2020 4120 7661 6c75 6520          A value 
+0000ce90: 6f66 2060 4e6f 6e65 6020 6c65 6674 2069  of `None` left i
+0000cea0: 7420 6173 2069 732e 0a0a 2020 2020 2020  t as is...      
+0000ceb0: 2020 5265 7475 726e 0a20 2020 2020 2020    Return.       
+0000cec0: 202d 2d2d 2d2d 2d0a 2020 2020 2020 2020   ------.        
+0000ced0: 7861 7272 6179 2e44 6174 6173 6574 2c20  xarray.Dataset, 
+0000cee0: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
+0000cef0: 0a0a 2020 2020 2020 2020 5365 6520 616c  ..        See al
+0000cf00: 736f 0a20 2020 2020 2020 202d 2d2d 2d2d  so.        -----
+0000cf10: 2d2d 2d0a 2020 2020 2020 2020 7265 6c6f  ---.        relo
+0000cf20: 630a 2020 2020 2020 2020 7367 6c6f 6361  c.        sgloca
+0000cf30: 746f 720a 2020 2020 2020 2020 5347 4c6f  tor.        SGLo
+0000cf40: 6361 746f 722e 666f 726d 6174 5f61 7474  cator.format_att
+0000cf50: 720a 2020 2020 2020 2020 2222 220a 2020  r.        """.  
+0000cf60: 2020 2020 2020 7265 6e61 6d65 5f61 7267        rename_arg
+0000cf70: 7320 3d20 7b7d 0a20 2020 2020 2020 206e  s = {}.        n
+0000cf80: 616d 6573 203d 205f 6c69 7374 5f78 725f  ames = _list_xr_
+0000cf90: 6e61 6d65 735f 286f 626a 290a 2020 2020  names_(obj).    
+0000cfa0: 2020 2020 6966 2068 6173 6174 7472 286f      if hasattr(o
+0000cfb0: 626a 2c20 226e 616d 6522 293a 0a20 2020  bj, "name"):.   
+0000cfc0: 2020 2020 2020 2020 206e 616d 6573 203d           names =
+0000cfd0: 206e 616d 6573 2e75 6e69 6f6e 287b 6f62   names.union({ob
+0000cfe0: 6a2e 6e61 6d65 7d29 0a20 2020 2020 2020  j.name}).       
+0000cff0: 2066 6f72 206e 616d 6520 696e 206e 616d   for name in nam
+0000d000: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0000d010: 6966 206e 616d 6520 6e6f 7420 696e 2072  if name not in r
+0000d020: 656e 616d 655f 6172 6773 3a0a 2020 2020  ename_args:.    
+0000d030: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+0000d040: 5f6e 616d 652c 206f 6c64 5f6c 6f63 203d  _name, old_loc =
+0000d050: 2073 656c 662e 7367 6c6f 6361 746f 722e   self.sglocator.
+0000d060: 7061 7273 655f 6174 7472 2822 6e61 6d65  parse_attr("name
+0000d070: 222c 206e 616d 6529 0a20 2020 2020 2020  ", name).       
+0000d080: 2020 2020 2020 2020 2069 6620 726f 6f74           if root
+0000d090: 5f6e 616d 6520 696e 206c 6f63 7320 616e  _name in locs an
+0000d0a0: 6420 6c6f 6373 5b72 6f6f 745f 6e61 6d65  d locs[root_name
+0000d0b0: 5d20 6973 206e 6f74 204e 6f6e 653a 0a20  ] is not None:. 
 0000d0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0d0: 2020 2022 6e61 6d65 222c 2072 6f6f 745f     "name", root_
-0000d0e0: 6e61 6d65 2c20 6c6f 6373 5b72 6f6f 745f  name, locs[root_
-0000d0f0: 6e61 6d65 5d0a 2020 2020 2020 2020 2020  name].          
-0000d100: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000d110: 2020 2020 7265 7475 726e 206f 626a 2e72      return obj.r
-0000d120: 656e 616d 6528 7265 6e61 6d65 5f61 7267  ename(rename_arg
-0000d130: 7329 0a0a 2020 2020 6465 6620 7265 6c6f  s)..    def relo
-0000d140: 6328 7365 6c66 2c20 6f62 6a2c 202a 2a6c  c(self, obj, **l
-0000d150: 6f63 7329 3a0a 2020 2020 2020 2020 2222  ocs):.        ""
-0000d160: 2243 6f6e 7665 7274 2067 6976 656e 2073  "Convert given s
-0000d170: 7461 6767 6572 6564 2067 7269 6420 6c6f  taggered grid lo
-0000d180: 6361 7469 6f6e 7320 746f 206f 7468 6572  cations to other
-0000d190: 206c 6f63 6174 696f 6e73 0a0a 2020 2020   locations..    
-0000d1a0: 2020 2020 2e2e 206e 6f74 653a 3a20 4974      .. note:: It
-0000d1b0: 206f 6e6c 7920 6368 616e 6765 7320 7468   only changes th
-0000d1c0: 6520 6e61 6d65 732c 206e 6f74 2074 6865  e names, not the
-0000d1d0: 2061 7474 7269 6275 7465 732e 0a0a 2020   attributes...  
-0000d1e0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0000d1f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000d200: 2d2d 2d0a 2020 2020 2020 2020 6f62 6a3a  ---.        obj:
-0000d210: 2078 6172 7261 792e 4461 7461 7365 742c   xarray.Dataset,
-0000d220: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
-0000d230: 790a 2020 2020 2020 2020 6c6f 6373 3a20  y.        locs: 
-0000d240: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
-0000d250: 202a 2a4b 6579 7320 6172 6520 6c6f 6361   **Keys are loca
-0000d260: 7469 6f6e 732a 2a2c 2076 616c 7565 7320  tions**, values 
-0000d270: 6172 6520 6e65 7720 6c6f 6361 7469 6f6e  are new location
-0000d280: 732e 0a20 2020 2020 2020 2020 2020 2041  s..            A
-0000d290: 2076 616c 7565 206f 6620 6046 616c 7365   value of `False
-0000d2a0: 6020 6f72 2060 4e6f 6e65 602c 2072 656d  ` or `None`, rem
-0000d2b0: 6f76 6520 7468 6520 6c6f 6361 7469 6f6e  ove the location
-0000d2c0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0000d2d0: 6e0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  n.        ------
-0000d2e0: 0a20 2020 2020 2020 2078 6172 7261 792e  .        xarray.
-0000d2f0: 4461 7461 7365 742c 2078 6172 7261 792e  Dataset, xarray.
-0000d300: 4461 7461 4172 7261 790a 0a20 2020 2020  DataArray..     
-0000d310: 2020 2053 6565 2061 6c73 6f0a 2020 2020     See also.    
-0000d320: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-0000d330: 2020 2020 2074 6f5f 6c6f 630a 2020 2020       to_loc.    
-0000d340: 2020 2020 7367 6c6f 6361 746f 720a 2020      sglocator.  
-0000d350: 2020 2020 2020 5347 4c6f 6361 746f 722e        SGLocator.
-0000d360: 666f 726d 6174 5f61 7474 720a 2020 2020  format_attr.    
-0000d370: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000d380: 7265 6e61 6d65 5f61 7267 7320 3d20 7b7d  rename_args = {}
-0000d390: 0a20 2020 2020 2020 206e 616d 6573 203d  .        names =
-0000d3a0: 205f 6c69 7374 5f78 725f 6e61 6d65 735f   _list_xr_names_
-0000d3b0: 286f 626a 290a 2020 2020 2020 2020 2320  (obj).        # 
-0000d3c0: 6e61 6d65 7320 3d20 7365 7428 6f62 6a2e  names = set(obj.
-0000d3d0: 6469 6d73 292e 756e 696f 6e28 6f62 6a2e  dims).union(obj.
-0000d3e0: 636f 6f72 6473 290a 2020 2020 2020 2020  coords).        
-0000d3f0: 2320 6966 2068 6173 6174 7472 286f 626a  # if hasattr(obj
-0000d400: 2c20 2264 6174 615f 7661 7273 2229 3a0a  , "data_vars"):.
-0000d410: 2020 2020 2020 2020 2320 2020 2020 6e61          #     na
-0000d420: 6d65 7320 3d20 6e61 6d65 732e 756e 696f  mes = names.unio
-0000d430: 6e28 6f62 6a2e 6461 7461 5f76 6172 7329  n(obj.data_vars)
-0000d440: 0a20 2020 2020 2020 2066 6f72 206e 616d  .        for nam
-0000d450: 6520 696e 206e 616d 6573 3a0a 2020 2020  e in names:.    
-0000d460: 2020 2020 2020 2020 6966 206e 616d 6520          if name 
-0000d470: 6e6f 7420 696e 2072 656e 616d 655f 6172  not in rename_ar
-0000d480: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000d490: 2020 2020 726f 6f74 5f6e 616d 652c 206f      root_name, o
-0000d4a0: 6c64 5f6c 6f63 203d 2073 656c 662e 7367  ld_loc = self.sg
-0000d4b0: 6c6f 6361 746f 722e 7061 7273 655f 6174  locator.parse_at
-0000d4c0: 7472 2822 6e61 6d65 222c 206e 616d 6529  tr("name", name)
-0000d4d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d4e0: 2069 6620 6f6c 645f 6c6f 6320 616e 6420   if old_loc and 
-0000d4f0: 6f6c 645f 6c6f 6320 696e 206c 6f63 733a  old_loc in locs:
-0000d500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d510: 2020 2020 2072 656e 616d 655f 6172 6773       rename_args
-0000d520: 5b6e 616d 655d 203d 2073 656c 662e 7367  [name] = self.sg
-0000d530: 6c6f 6361 746f 722e 666f 726d 6174 5f61  locator.format_a
-0000d540: 7474 7228 226e 616d 6522 2c20 726f 6f74  ttr("name", root
-0000d550: 5f6e 616d 652c 206c 6f63 735b 6f6c 645f  _name, locs[old_
-0000d560: 6c6f 635d 290a 0a20 2020 2020 2020 2072  loc])..        r
-0000d570: 6574 7572 6e20 6f62 6a2e 7265 6e61 6d65  eturn obj.rename
-0000d580: 2872 656e 616d 655f 6172 6773 290a 0a20  (rename_args).. 
-0000d590: 2020 2064 6566 2066 696c 6c5f 6174 7472     def fill_attr
-0000d5a0: 7328 7365 6c66 2c20 6f62 6a2c 202a 2a6b  s(self, obj, **k
-0000d5b0: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-0000d5c0: 2222 2246 696c 6c20 6d69 7373 696e 6720  """Fill missing 
-0000d5d0: 6174 7472 6962 7574 6573 206f 6620 6120  attributes of a 
-0000d5e0: 7861 7272 6179 2e44 6174 6173 6574 206f  xarray.Dataset o
-0000d5f0: 7220 7861 7272 6179 2e44 6174 6141 7272  r xarray.DataArr
-0000d600: 6179 0a0a 2020 2020 2020 2020 2e2e 206e  ay..        .. n
-0000d610: 6f74 653a 3a20 4974 2064 6f65 7320 6e6f  ote:: It does no
-0000d620: 7420 7265 6e61 6d65 2061 6e79 7468 696e  t rename anythin
-0000d630: 670a 0a20 2020 2020 2020 2053 6565 2061  g..        See a
-0000d640: 6c73 6f0a 2020 2020 2020 2020 2d2d 2d2d  lso.        ----
-0000d650: 2d2d 2d2d 0a20 2020 2020 2020 2066 6f72  ----.        for
-0000d660: 6d61 745f 6461 7461 6172 7261 790a 2020  mat_dataarray.  
-0000d670: 2020 2020 2020 666f 726d 6174 5f64 6174        format_dat
-0000d680: 6173 6574 0a20 2020 2020 2020 2061 7574  aset.        aut
-0000d690: 6f5f 666f 726d 6174 0a20 2020 2020 2020  o_format.       
-0000d6a0: 2022 2222 0a20 2020 2020 2020 206b 7761   """.        kwa
-0000d6b0: 7267 732e 7570 6461 7465 2872 656e 616d  rgs.update(renam
-0000d6c0: 653d 4661 6c73 652c 2072 6570 6c61 6365  e=False, replace
-0000d6d0: 5f61 7474 7273 3d46 616c 7365 290a 2020  _attrs=False).  
-0000d6e0: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
-0000d6f0: 286f 626a 2c20 2264 6174 615f 7661 7273  (obj, "data_vars
-0000d700: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-0000d710: 7265 7475 726e 2073 656c 662e 666f 726d  return self.form
-0000d720: 6174 5f64 6174 6173 6574 286f 626a 2c20  at_dataset(obj, 
-0000d730: 666f 726d 6174 5f63 6f6f 7264 733d 5472  format_coords=Tr
-0000d740: 7565 2c20 2a2a 6b77 6172 6773 290a 2020  ue, **kwargs).  
-0000d750: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000d760: 662e 666f 726d 6174 5f64 6174 615f 7661  f.format_data_va
-0000d770: 7228 6f62 6a2c 202a 2a6b 7761 7267 7329  r(obj, **kwargs)
-0000d780: 0a0a 2020 2020 6465 6620 6d61 7463 685f  ..    def match_
-0000d790: 636f 6f72 6428 7365 6c66 2c20 6461 2c20  coord(self, da, 
-0000d7a0: 6366 5f6e 616d 653d 4e6f 6e65 2c20 6c6f  cf_name=None, lo
-0000d7b0: 633d 2261 6e79 2229 3a0a 2020 2020 2020  c="any"):.      
-0000d7c0: 2020 2222 2243 6865 636b 2069 6620 616e    """Check if an
-0000d7d0: 2061 7272 6179 206d 6174 6368 6573 2061   array matches a
-0000d7e0: 2067 6976 656e 206f 7220 616e 7920 636f   given or any co
-0000d7f0: 6f72 6420 7370 6563 730a 0a20 2020 2020  ord specs..     
-0000d800: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000d810: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0000d820: 0a20 2020 2020 2020 2064 613a 2078 6172  .        da: xar
-0000d830: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
-0000d840: 2020 2020 2020 6366 5f6e 616d 653a 2073        cf_name: s
-0000d850: 7472 2c20 6469 6374 2c20 4e6f 6e65 0a20  tr, dict, None. 
-0000d860: 2020 2020 2020 2020 2020 2043 6620 6e61             Cf na
-0000d870: 6d65 2e0a 2020 2020 2020 2020 2020 2020  me..            
-0000d880: 4966 204e 6f6e 652c 2061 6c6c 206e 616d  If None, all nam
-0000d890: 6573 2061 7265 2075 7365 642e 0a20 2020  es are used..   
-0000d8a0: 2020 2020 2020 2020 2049 6620 6120 6469           If a di
-0000d8b0: 6374 2c20 6e61 6d65 2069 7320 696e 7465  ct, name is inte
-0000d8c0: 7270 7265 7465 6420 6173 2061 6e20 6578  rpreted as an ex
-0000d8d0: 706c 6963 6974 2073 6574 206f 660a 2020  plicit set of.  
-0000d8e0: 2020 2020 2020 2020 2020 7370 6563 6966            specif
-0000d8f0: 6963 6174 696f 6e73 2e0a 2020 2020 2020  ications..      
-0000d900: 2020 6c6f 633a 2073 7472 2c20 7b22 616e    loc: str, {"an
-0000d910: 7922 2c20 4e6f 6e65 7d2c 207b 2222 2c20  y", None}, {"", 
-0000d920: 4661 6c73 657d 0a20 2020 2020 2020 2020  False}.         
-0000d930: 2020 202d 2073 7472 3a20 6f6e 6520 6f66     - str: one of
-0000d940: 2074 6865 7365 206c 6f63 6174 696f 6e73   these locations
-0000d950: 0a20 2020 2020 2020 2020 2020 202d 204e  .            - N
-0000d960: 6f6e 6520 6f72 2022 616e 7922 3a20 616e  one or "any": an
-0000d970: 790a 2020 2020 2020 2020 2020 2020 2d20  y.            - 
-0000d980: 4661 6c73 6520 6f72 2027 2222 3a20 6e6f  False or '"": no
-0000d990: 206c 6f63 6174 696f 6e0a 0a20 2020 2020   location..     
-0000d9a0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0000d9b0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0000d9c0: 2020 2062 6f6f 6c2c 2073 7472 0a20 2020     bool, str.   
-0000d9d0: 2020 2020 2020 2020 2054 7275 6520 6f72           True or
-0000d9e0: 2046 616c 7365 2069 6620 6e61 6d65 2069   False if name i
-0000d9f0: 7320 7072 6f76 6964 6564 2c20 656c 7365  s provided, else
-0000da00: 2066 6f75 6e64 206e 616d 6520 6f72 204e   found name or N
-0000da10: 6f6e 650a 0a20 2020 2020 2020 2053 6565  one..        See
-0000da20: 2061 6c73 6f0a 2020 2020 2020 2020 2d2d   also.        --
-0000da30: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2043  ------.        C
-0000da40: 4643 6f6f 7264 5370 6563 732e 6d61 7463  FCoordSpecs.matc
-0000da50: 680a 2020 2020 2020 2020 2222 220a 2020  h.        """.  
-0000da60: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000da70: 662e 636f 6f72 6473 2e6d 6174 6368 2864  f.coords.match(d
-0000da80: 612c 2063 665f 6e61 6d65 3d63 665f 6e61  a, cf_name=cf_na
-0000da90: 6d65 2c20 6c6f 633d 6c6f 6329 0a0a 2020  me, loc=loc)..  
-0000daa0: 2020 6465 6620 6d61 7463 685f 6461 7461    def match_data
-0000dab0: 5f76 6172 2873 656c 662c 2064 612c 2063  _var(self, da, c
-0000dac0: 665f 6e61 6d65 3d4e 6f6e 652c 206c 6f63  f_name=None, loc
-0000dad0: 3d22 616e 7922 293a 0a20 2020 2020 2020  ="any"):.       
-0000dae0: 2022 2222 4368 6563 6b20 6966 2061 6e20   """Check if an 
-0000daf0: 6172 7261 7920 6d61 7463 6865 7320 6769  array matches gi
-0000db00: 7665 6e20 6f72 2061 6e79 2064 6174 615f  ven or any data_
-0000db10: 7661 7220 7370 6563 730a 0a20 2020 2020  var specs..     
-0000db20: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000db30: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0000db40: 0a20 2020 2020 2020 2064 613a 2078 6172  .        da: xar
-0000db50: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
-0000db60: 2020 2020 2020 6e61 6d65 3a20 7374 722c        name: str,
-0000db70: 2064 6963 742c 204e 6f6e 650a 2020 2020   dict, None.    
-0000db80: 2020 2020 2020 2020 4366 206e 616d 652e          Cf name.
-0000db90: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-0000dba0: 4e6f 6e65 2c20 616c 6c20 6e61 6d65 7320  None, all names 
-0000dbb0: 6172 6520 7573 6564 2e0a 2020 2020 2020  are used..      
-0000dbc0: 2020 2020 2020 4966 2061 2064 6963 742c        If a dict,
-0000dbd0: 206e 616d 6520 6973 2069 6e74 6572 7072   name is interpr
-0000dbe0: 6574 6564 2061 7320 616e 2065 7870 6c69  eted as an expli
-0000dbf0: 6369 7420 7365 7420 6f66 0a20 2020 2020  cit set of.     
-0000dc00: 2020 2020 2020 2073 7065 6369 6669 6361         specifica
-0000dc10: 7469 6f6e 732e 0a20 2020 2020 2020 206c  tions..        l
-0000dc20: 6f63 3a20 7374 722c 207b 2261 6e79 222c  oc: str, {"any",
-0000dc30: 204e 6f6e 657d 2c20 7b22 222c 2046 616c   None}, {"", Fal
-0000dc40: 7365 7d0a 2020 2020 2020 2020 2020 2020  se}.            
-0000dc50: 2d20 7374 723a 206f 6e65 206f 6620 7468  - str: one of th
-0000dc60: 6573 6520 6c6f 6361 7469 6f6e 730a 2020  ese locations.  
-0000dc70: 2020 2020 2020 2020 2020 2d20 4e6f 6e65            - None
-0000dc80: 206f 7220 2261 6e79 223a 2061 6e79 0a20   or "any": any. 
-0000dc90: 2020 2020 2020 2020 2020 202d 2046 616c             - Fal
-0000dca0: 7365 206f 7220 2722 223a 206e 6f20 6c6f  se or '"": no lo
-0000dcb0: 6361 7469 6f6e 0a0a 2020 2020 2020 2020  cation..        
-0000dcc0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-0000dcd0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000dce0: 626f 6f6c 2c20 7374 720a 2020 2020 2020  bool, str.      
-0000dcf0: 2020 2020 2020 5472 7565 206f 7220 4661        True or Fa
-0000dd00: 6c73 6520 6966 206e 616d 6520 6973 2070  lse if name is p
-0000dd10: 726f 7669 6465 642c 2065 6c73 6520 666f  rovided, else fo
-0000dd20: 756e 6420 6e61 6d65 206f 7220 4e6f 6e65  und name or None
-0000dd30: 0a0a 2020 2020 2020 2020 5365 6520 616c  ..        See al
-0000dd40: 736f 0a20 2020 2020 2020 202d 2d2d 2d2d  so.        -----
-0000dd50: 2d2d 2d0a 2020 2020 2020 2020 4346 5661  ---.        CFVa
-0000dd60: 7253 7065 6373 2e6d 6174 6368 0a20 2020  rSpecs.match.   
-0000dd70: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000dd80: 2072 6574 7572 6e20 7365 6c66 2e64 6174   return self.dat
-0000dd90: 615f 7661 7273 2e6d 6174 6368 2864 612c  a_vars.match(da,
-0000dda0: 2063 665f 6e61 6d65 3d63 665f 6e61 6d65   cf_name=cf_name
-0000ddb0: 2c20 6c6f 633d 6c6f 6329 0a0a 2020 2020  , loc=loc)..    
-0000ddc0: 6465 6620 6d61 7463 685f 6469 6d28 7365  def match_dim(se
-0000ddd0: 6c66 2c20 6469 6d2c 2063 665f 6e61 6d65  lf, dim, cf_name
-0000dde0: 3d4e 6f6e 652c 206c 6f63 3d4e 6f6e 6529  =None, loc=None)
-0000ddf0: 3a0a 2020 2020 2020 2020 2222 2243 6865  :.        """Che
-0000de00: 636b 2069 6620 6120 6469 6d65 6e73 696f  ck if a dimensio
-0000de10: 6e20 6e61 6d65 206d 6174 6368 6573 2067  n name matches g
-0000de20: 6976 656e 206f 7220 616e 7920 636f 6f72  iven or any coor
-0000de30: 6420 7370 6563 730a 0a20 2020 2020 2020  d specs..       
-0000de40: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000de50: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000de60: 2020 2020 2020 2064 696d 3a20 7374 720a         dim: str.
-0000de70: 2020 2020 2020 2020 2020 2020 4469 6d65              Dime
-0000de80: 6e73 696f 6e20 6e61 6d65 0a20 2020 2020  nsion name.     
-0000de90: 2020 2063 665f 6e61 6d65 3a20 7374 722c     cf_name: str,
-0000dea0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0000deb0: 2020 4366 206e 616d 652e 0a20 2020 2020    Cf name..     
-0000dec0: 2020 206c 6f63 3a20 7374 722c 207b 2261     loc: str, {"a
-0000ded0: 6e79 222c 204e 6f6e 657d 2c20 7b22 222c  ny", None}, {"",
-0000dee0: 2046 616c 7365 7d0a 2020 2020 2020 2020   False}.        
-0000def0: 2020 2020 2d20 7374 723a 206f 6e65 206f      - str: one o
-0000df00: 6620 7468 6573 6520 6c6f 6361 7469 6f6e  f these location
-0000df10: 730a 2020 2020 2020 2020 2020 2020 2d20  s.            - 
-0000df20: 4e6f 6e65 206f 7220 2261 6e79 223a 2061  None or "any": a
-0000df30: 6e79 0a20 2020 2020 2020 2020 2020 202d  ny.            -
-0000df40: 2046 616c 7365 206f 7220 2722 223a 206e   False or '"": n
-0000df50: 6f20 6c6f 6361 7469 6f6e 0a0a 2020 2020  o location..    
-0000df60: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0000df70: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0000df80: 2020 2020 626f 6f6c 2c20 7374 720a 2020      bool, str.  
-0000df90: 2020 2020 2020 2020 2020 5472 7565 206f            True o
-0000dfa0: 7220 4661 6c73 6520 6966 206e 616d 6520  r False if name 
-0000dfb0: 6973 2070 726f 7669 6465 642c 2065 6c73  is provided, els
-0000dfc0: 6520 666f 756e 6420 6e61 6d65 206f 7220  e found name or 
-0000dfd0: 4e6f 6e65 0a0a 2020 2020 2020 2020 5365  None..        Se
-0000dfe0: 6520 616c 736f 0a20 2020 2020 2020 202d  e also.        -
-0000dff0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000e000: 4346 5661 7253 7065 6373 2e6d 6174 6368  CFVarSpecs.match
-0000e010: 5f66 726f 6d5f 6e61 6d65 0a20 2020 2020  _from_name.     
-0000e020: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0000e030: 6574 7572 6e20 7365 6c66 2e63 6f6f 7264  eturn self.coord
-0000e040: 732e 6d61 7463 685f 6672 6f6d 5f6e 616d  s.match_from_nam
-0000e050: 6528 6469 6d2c 2063 665f 6e61 6d65 3d63  e(dim, cf_name=c
-0000e060: 665f 6e61 6d65 2c20 6c6f 633d 6c6f 6329  f_name, loc=loc)
-0000e070: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-0000e080: 686f 640a 2020 2020 6465 6620 6765 745f  hod.    def get_
-0000e090: 6361 7465 676f 7279 2864 6129 3a0a 2020  category(da):.  
-0000e0a0: 2020 2020 2020 2222 2247 7565 7373 2069        """Guess i
-0000e0b0: 6620 6120 6461 7461 6172 7261 7920 6265  f a dataarray be
-0000e0c0: 6c6f 6e67 7320 746f 2064 6174 615f 7661  longs to data_va
-0000e0d0: 7273 206f 7220 636f 6f72 6473 0a0a 2020  rs or coords..  
-0000e0e0: 2020 2020 2020 4974 2062 656c 6f6e 6773        It belongs
-0000e0f0: 2074 6f20 636f 6f72 6473 2069 6620 6f6e   to coords if on
-0000e100: 6520 6f66 2069 7473 2064 696d 656e 7369  e of its dimensi
-0000e110: 6f6e 7320 6f72 0a20 2020 2020 2020 2063  ons or.        c
-0000e120: 6f6f 7264 696e 6174 6573 2068 6173 2069  oordinates has i
-0000e130: 7473 206e 616d 652e 0a0a 2020 2020 2020  ts name...      
-0000e140: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0000e150: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-0000e160: 2020 2020 2020 2020 6461 3a20 7861 7272          da: xarr
-0000e170: 6179 2e44 6174 6141 7272 6179 0a0a 2020  ay.DataArray..  
-0000e180: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-0000e190: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-0000e1a0: 2020 2020 2020 7374 720a 2020 2020 2020        str.      
-0000e1b0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
-0000e1c0: 6966 2064 612e 6e61 6d65 2069 7320 6e6f  if da.name is no
-0000e1d0: 7420 4e6f 6e65 2061 6e64 2028 6461 2e6e  t None and (da.n
-0000e1e0: 616d 6520 696e 2064 612e 6469 6d73 206f  ame in da.dims o
-0000e1f0: 7220 6461 2e6e 616d 6520 696e 2064 612e  r da.name in da.
-0000e200: 636f 6f72 6473 293a 0a20 2020 2020 2020  coords):.       
-0000e210: 2069 6620 6461 2e6e 616d 6520 6973 206e   if da.name is n
-0000e220: 6f74 204e 6f6e 6520 616e 6420 5f6c 6973  ot None and _lis
-0000e230: 745f 7872 5f6e 616d 6573 5f28 6461 2c20  t_xr_names_(da, 
-0000e240: 6461 7461 5f76 6172 733d 4661 6c73 6529  data_vars=False)
-0000e250: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000e260: 7475 726e 2022 636f 6f72 6473 220a 2020  turn "coords".  
-0000e270: 2020 2020 2020 7265 7475 726e 2022 6461        return "da
-0000e280: 7461 5f76 6172 7322 0a0a 2020 2020 6465  ta_vars"..    de
-0000e290: 6620 6d61 7463 6828 7365 6c66 2c20 6461  f match(self, da
-0000e2a0: 2c20 6c6f 633d 2261 6e79 2229 3a0a 2020  , loc="any"):.  
-0000e2b0: 2020 2020 2020 2222 2243 6865 636b 2069        """Check i
-0000e2c0: 6620 616e 2061 7272 6179 206d 6174 6368  f an array match
-0000e2d0: 6573 2061 6e79 2064 6174 615f 7661 7220  es any data_var 
-0000e2e0: 6f72 2063 6f6f 7264 2073 7065 6373 0a0a  or coord specs..
-0000e2f0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000e300: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000e310: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6461  -----.        da
-0000e320: 3a20 7861 7272 6179 2e44 6174 6141 7272  : xarray.DataArr
-0000e330: 6179 0a20 2020 2020 2020 206c 6f63 3a20  ay.        loc: 
-0000e340: 7374 722c 207b 2261 6e79 222c 204e 6f6e  str, {"any", Non
-0000e350: 657d 2c20 7b22 222c 2046 616c 7365 7d0a  e}, {"", False}.
-0000e360: 2020 2020 2020 2020 2020 2020 2d20 7374              - st
-0000e370: 723a 206f 6e65 206f 6620 7468 6573 6520  r: one of these 
-0000e380: 6c6f 6361 7469 6f6e 730a 2020 2020 2020  locations.      
-0000e390: 2020 2020 2020 2d20 4e6f 6e65 206f 7220        - None or 
-0000e3a0: 2261 6e79 223a 2061 6e79 0a20 2020 2020  "any": any.     
-0000e3b0: 2020 2020 2020 202d 2046 616c 7365 206f         - False o
-0000e3c0: 7220 2722 223a 206e 6f20 6c6f 6361 7469  r '"": no locati
-0000e3d0: 6f6e 0a0a 2020 2020 2020 2020 5265 7475  on..        Retu
-0000e3e0: 726e 0a20 2020 2020 2020 202d 2d2d 2d2d  rn.        -----
-0000e3f0: 2d0a 2020 2020 2020 2020 7374 722c 204e  -.        str, N
-0000e400: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000e410: 4361 7465 676f 7279 0a20 2020 2020 2020  Category.       
-0000e420: 2073 7472 2c20 4e6f 6e65 0a20 2020 2020   str, None.     
-0000e430: 2020 2020 2020 204e 616d 650a 2020 2020         Name.    
-0000e440: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000e450: 6361 7465 676f 7279 203d 2073 656c 662e  category = self.
-0000e460: 6765 745f 6361 7465 676f 7279 2864 6129  get_category(da)
-0000e470: 0a20 2020 2020 2020 2063 6174 6567 6f72  .        categor
-0000e480: 6965 7320 3d20 6c69 7374 2873 656c 662e  ies = list(self.
-0000e490: 6361 7465 676f 7269 6573 290a 2020 2020  categories).    
-0000e4a0: 2020 2020 6966 2063 6174 6567 6f72 7920      if category 
-0000e4b0: 213d 2063 6174 6567 6f72 6965 735b 305d  != categories[0]
-0000e4c0: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
-0000e4d0: 7465 676f 7269 6573 203d 2063 6174 6567  tegories = categ
-0000e4e0: 6f72 6965 735b 3a3a 2d31 5d0a 2020 2020  ories[::-1].    
-0000e4f0: 2020 2020 666f 7220 6361 7465 676f 7279      for category
-0000e500: 2069 6e20 6361 7465 676f 7269 6573 3a0a   in categories:.
-0000e510: 2020 2020 2020 2020 2020 2020 6366 5f6e              cf_n
-0000e520: 616d 6520 3d20 7365 6c66 5b63 6174 6567  ame = self[categ
-0000e530: 6f72 795d 2e6d 6174 6368 2864 612c 206c  ory].match(da, l
-0000e540: 6f63 3d6c 6f63 290a 2020 2020 2020 2020  oc=loc).        
-0000e550: 2020 2020 6966 2063 665f 6e61 6d65 3a0a      if cf_name:.
-0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e570: 7265 7475 726e 2063 6174 6567 6f72 792c  return category,
-0000e580: 2063 665f 6e61 6d65 0a20 2020 2020 2020   cf_name.       
-0000e590: 2072 6574 7572 6e20 4e6f 6e65 2c20 4e6f   return None, No
-0000e5a0: 6e65 0a0a 2020 2020 4045 5252 4f52 532e  ne..    @ERRORS.
-0000e5b0: 666f 726d 6174 5f6d 6574 686f 645f 646f  format_method_do
-0000e5c0: 6373 7472 696e 670a 2020 2020 6465 6620  cstring.    def 
-0000e5d0: 7365 6172 6368 5f63 6f6f 7264 2873 656c  search_coord(sel
-0000e5e0: 662c 206f 626a 2c20 6366 5f6e 616d 653d  f, obj, cf_name=
-0000e5f0: 4e6f 6e65 2c20 6c6f 633d 2261 6e79 222c  None, loc="any",
-0000e600: 2067 6574 3d22 6f62 6a22 2c20 7369 6e67   get="obj", sing
-0000e610: 6c65 3d54 7275 652c 2065 7272 6f72 733d  le=True, errors=
-0000e620: 2277 6172 6e22 293a 0a20 2020 2020 2020  "warn"):.       
-0000e630: 2022 2222 5365 6172 6368 2066 6f72 2061   """Search for a
-0000e640: 2063 6f6f 7264 2074 6861 7420 6d61 6368   coord that mach
-0000e650: 6573 2067 6976 656e 206f 7220 616e 7920  es given or any 
-0000e660: 7370 6563 730a 0a20 2020 2020 2020 2050  specs..        P
-0000e670: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0000e680: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000e690: 2020 2020 206f 626a 3a20 4461 7461 4172       obj: DataAr
-0000e6a0: 7261 7920 6f72 2044 6174 6173 6574 0a20  ray or Dataset. 
-0000e6b0: 2020 2020 2020 2063 665f 6e61 6d65 3a20         cf_name: 
-0000e6c0: 7374 722c 2064 6963 740a 2020 2020 2020  str, dict.      
-0000e6d0: 2020 2020 2020 4120 6765 6e65 7269 6320        A generic 
-0000e6e0: 4346 206e 616d 652e 2049 6620 6e6f 7420  CF name. If not 
-0000e6f0: 7072 6f76 6964 6564 2c20 616c 6c20 4346  provided, all CF
-0000e700: 206e 616d 6573 2061 7265 2073 6361 6e65   names are scane
-0000e710: 642e 0a20 2020 2020 2020 206c 6f63 3a20  d..        loc: 
-0000e720: 7374 722c 207b 7b22 616e 7922 2c20 4e6f  str, {{"any", No
-0000e730: 6e65 7d7d 2c20 7b7b 2222 2c20 4661 6c73  ne}}, {{"", Fals
-0000e740: 657d 7d0a 2020 2020 2020 2020 2020 2020  e}}.            
-0000e750: 2d20 7374 723a 206f 6e65 206f 6620 7468  - str: one of th
-0000e760: 6573 6520 6c6f 6361 7469 6f6e 730a 2020  ese locations.  
-0000e770: 2020 2020 2020 2020 2020 2d20 4e6f 6e65            - None
-0000e780: 206f 7220 2261 6e79 223a 2061 6e79 0a20   or "any": any. 
-0000e790: 2020 2020 2020 2020 2020 202d 2046 616c             - Fal
-0000e7a0: 7365 206f 7220 2222 3a20 6e6f 206c 6f63  se or "": no loc
-0000e7b0: 6174 696f 6e0a 2020 2020 2020 2020 6765  ation.        ge
-0000e7c0: 743a 207b 7b22 6f62 6a22 2c20 226e 616d  t: {{"obj", "nam
-0000e7d0: 6522 7d7d 0a20 2020 2020 2020 2020 2020  e"}}.           
-0000e7e0: 2057 6865 6e20 666f 756e 642c 2067 6574   When found, get
-0000e7f0: 2074 6865 206f 626a 6563 7420 666f 756e   the object foun
-0000e800: 6420 6f72 2069 7473 206e 616d 652e 0a20  d or its name.. 
-0000e810: 2020 2020 2020 2073 696e 676c 653a 2062         single: b
-0000e820: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-0000e830: 4966 2054 7275 652c 2072 6574 7572 6e20  If True, return 
-0000e840: 7468 6520 6669 7273 7420 6974 656d 2066  the first item f
-0000e850: 6f75 6e64 206f 7220 4e6f 6e65 2e0a 2020  ound or None..  
-0000e860: 2020 2020 2020 2020 2020 4966 2046 616c            If Fal
-0000e870: 7365 2c20 7265 7475 726e 2061 2070 6f73  se, return a pos
-0000e880: 7369 626c 6520 656d 7074 7920 6c69 7374  sible empty list
-0000e890: 206f 6620 666f 756e 6420 6974 656d 732e   of found items.
-0000e8a0: 0a20 2020 2020 2020 2020 2020 2041 2077  .            A w
-0000e8b0: 6172 6e69 6e67 2069 7320 656d 6974 7465  arning is emitte
-0000e8c0: 6420 7768 656e 2073 6574 2074 6f20 5472  d when set to Tr
-0000e8d0: 7565 2061 6e64 206d 756c 7469 706c 6520  ue and multiple 
-0000e8e0: 6974 656d 2061 7265 2066 6f75 6e64 2e0a  item are found..
-0000e8f0: 2020 2020 2020 2020 7b65 7272 6f72 737d          {errors}
-0000e900: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000e910: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0000e920: 2d0a 2020 2020 2020 2020 4e6f 6e65 206f  -.        None o
-0000e930: 7220 7374 7220 6f72 206f 626a 6563 740a  r str or object.
-0000e940: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-0000e950: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000e960: 0a20 2020 2020 2020 202e 2e20 6970 7974  .        .. ipyt
-0000e970: 686f 6e3a 3a20 7079 7468 6f6e 0a0a 2020  hon:: python..  
-0000e980: 2020 2020 2020 2020 2020 4073 7570 7072            @suppr
-0000e990: 6573 730a 2020 2020 2020 2020 2020 2020  ess.            
-0000e9a0: 6672 6f6d 2078 6f61 2e63 6620 696d 706f  from xoa.cf impo
-0000e9b0: 7274 2067 6574 5f63 665f 7370 6563 730a  rt get_cf_specs.
-0000e9c0: 2020 2020 2020 2020 2020 2020 4073 7570              @sup
-0000e9d0: 7072 6573 730a 2020 2020 2020 2020 2020  press.          
-0000e9e0: 2020 696d 706f 7274 2078 6172 7261 7920    import xarray 
-0000e9f0: 6173 2078 722c 206e 756d 7079 2061 7320  as xr, numpy as 
-0000ea00: 6e70 0a20 2020 2020 2020 2020 2020 206c  np.            l
-0000ea10: 6f6e 203d 2078 722e 4461 7461 4172 7261  on = xr.DataArra
-0000ea20: 7928 5b32 2c20 335d 2c20 6469 6d73 3d27  y([2, 3], dims='
-0000ea30: 666f 6f27 2c0a 2020 2020 2020 2020 2020  foo',.          
-0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea50: 2020 2020 2061 7474 7273 3d7b 7b27 7374       attrs={{'st
-0000ea60: 616e 6461 7264 5f6e 616d 6527 3a20 276c  andard_name': 'l
-0000ea70: 6f6e 6769 7475 6465 277d 7d29 0a20 2020  ongitude'}}).   
-0000ea80: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-0000ea90: 7872 2e44 6174 6141 7272 6179 285b 302c  xr.DataArray([0,
-0000eaa0: 2031 5d2c 2064 696d 733d 2827 666f 6f27   1], dims=('foo'
-0000eab0: 292c 2063 6f6f 7264 733d 5b6c 6f6e 5d29  ), coords=[lon])
-0000eac0: 0a20 2020 2020 2020 2020 2020 2063 6673  .            cfs
-0000ead0: 7065 6373 203d 2067 6574 5f63 665f 7370  pecs = get_cf_sp
-0000eae0: 6563 7328 290a 2020 2020 2020 2020 2020  ecs().          
-0000eaf0: 2020 6366 7370 6563 732e 7365 6172 6368    cfspecs.search
-0000eb00: 5f63 6f6f 7264 2864 6174 612c 2022 6c6f  _coord(data, "lo
-0000eb10: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
-0000eb20: 6366 7370 6563 732e 7365 6172 6368 5f63  cfspecs.search_c
-0000eb30: 6f6f 7264 2864 6174 612c 2022 6c6f 6e22  oord(data, "lon"
-0000eb40: 2c20 6765 743d 2263 665f 6e61 6d65 2229  , get="cf_name")
-0000eb50: 0a20 2020 2020 2020 2020 2020 2063 6673  .            cfs
-0000eb60: 7065 6373 2e73 6561 7263 685f 636f 6f72  pecs.search_coor
-0000eb70: 6428 6461 7461 2c20 226c 6174 222c 2065  d(data, "lat", e
-0000eb80: 7272 6f72 733d 2269 676e 6f72 6522 290a  rrors="ignore").
-0000eb90: 0a20 2020 2020 2020 2053 6565 2061 6c73  .        See als
-0000eba0: 6f0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  o.        ------
-0000ebb0: 2d2d 0a20 2020 2020 2020 2073 6561 7263  --.        searc
-0000ebc0: 685f 6461 7461 5f76 6172 0a20 2020 2020  h_data_var.     
-0000ebd0: 2020 2043 4643 6f6f 7264 5370 6563 732e     CFCoordSpecs.
-0000ebe0: 7365 6172 6368 0a20 2020 2020 2020 2022  search.        "
-0000ebf0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-0000ec00: 6e20 7365 6c66 2e63 6f6f 7264 732e 7365  n self.coords.se
-0000ec10: 6172 6368 280a 2020 2020 2020 2020 2020  arch(.          
-0000ec20: 2020 6f62 6a2c 2063 665f 6e61 6d65 3d63    obj, cf_name=c
-0000ec30: 665f 6e61 6d65 2c20 6c6f 633d 6c6f 632c  f_name, loc=loc,
-0000ec40: 2067 6574 3d67 6574 2c20 7369 6e67 6c65   get=get, single
-0000ec50: 3d73 696e 676c 652c 2065 7272 6f72 733d  =single, errors=
-0000ec60: 6572 726f 7273 0a20 2020 2020 2020 2029  errors.        )
-0000ec70: 0a0a 2020 2020 4045 5252 4f52 532e 666f  ..    @ERRORS.fo
-0000ec80: 726d 6174 5f6d 6574 686f 645f 646f 6373  rmat_method_docs
-0000ec90: 7472 696e 670a 2020 2020 6465 6620 7365  tring.    def se
-0000eca0: 6172 6368 5f64 696d 2873 656c 662c 2064  arch_dim(self, d
-0000ecb0: 612c 2063 665f 6172 673d 4e6f 6e65 2c20  a, cf_arg=None, 
-0000ecc0: 6c6f 633d 2261 6e79 222c 2065 7272 6f72  loc="any", error
-0000ecd0: 733d 2269 676e 6f72 6522 293a 0a20 2020  s="ignore"):.   
-0000ece0: 2020 2020 2022 2222 5365 6172 6368 2066       """Search f
-0000ecf0: 6f72 2061 2064 696d 656e 7369 6f6e 2066  or a dimension f
-0000ed00: 726f 6d20 6974 7320 7479 7065 0a0a 2020  rom its type..  
-0000ed10: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0000ed20: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000ed30: 2d2d 2d0a 2020 2020 2020 2020 6461 3a20  ---.        da: 
-0000ed40: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-0000ed50: 0a20 2020 2020 2020 2063 665f 6172 673a  .        cf_arg:
-0000ed60: 204e 6f6e 652c 2073 7472 2c20 7b7b 2278   None, str, {{"x
-0000ed70: 222c 2022 7922 2c20 227a 222c 2022 7422  ", "y", "z", "t"
-0000ed80: 2c20 2266 227d 7d0a 2020 2020 2020 2020  , "f"}}.        
-0000ed90: 2020 2020 4469 6d65 6e73 696f 6e20 7479      Dimension ty
-0000eda0: 7065 206f 7220 6765 6e65 7269 6320 4346  pe or generic CF
-0000edb0: 206e 616d 650a 2020 2020 2020 2020 6c6f   name.        lo
-0000edc0: 633a 0a20 2020 2020 2020 2020 2020 2053  c:.            S
-0000edd0: 7461 6767 6572 6564 2067 7269 6420 6c6f  taggered grid lo
-0000ede0: 6361 7469 6f6e 0a20 2020 2020 2020 207b  cation.        {
-0000edf0: 6572 726f 7273 7d0a 0a20 2020 2020 2020  errors}..       
-0000ee00: 2052 6574 7572 6e0a 2020 2020 2020 2020   Return.        
-0000ee10: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
-0000ee20: 6f6e 652c 2073 7472 2c20 6469 6374 0a20  one, str, dict. 
-0000ee30: 2020 2020 2020 2020 2020 2044 696d 206e             Dim n
-0000ee40: 616d 6520 4f52 2c20 6469 6374 2077 6974  ame OR, dict wit
-0000ee50: 6820 6469 6d2c 2074 7970 6520 616e 6420  h dim, type and 
-0000ee60: 6366 5f6e 616d 6520 6b65 7973 2069 6620  cf_name keys if 
-0000ee70: 6366 5f61 7267 2069 7320 4e6f 6e65 0a0a  cf_arg is None..
-0000ee80: 2020 2020 2020 2020 5365 6520 616c 736f          See also
-0000ee90: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000eea0: 2d0a 2020 2020 2020 2020 4346 436f 6f72  -.        CFCoor
-0000eeb0: 6453 7065 6373 2e73 6561 7263 685f 6469  dSpecs.search_di
-0000eec0: 6d0a 2020 2020 2020 2020 2222 220a 2020  m.        """.  
-0000eed0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000eee0: 662e 636f 6f72 6473 2e73 6561 7263 685f  f.coords.search_
-0000eef0: 6469 6d28 6461 2c20 6366 5f61 7267 3d63  dim(da, cf_arg=c
-0000ef00: 665f 6172 672c 206c 6f63 3d6c 6f63 2c20  f_arg, loc=loc, 
-0000ef10: 6572 726f 7273 3d65 7272 6f72 7329 0a0a  errors=errors)..
-0000ef20: 2020 2020 4045 5252 4f52 532e 666f 726d      @ERRORS.form
-0000ef30: 6174 5f6d 6574 686f 645f 646f 6373 7472  at_method_docstr
-0000ef40: 696e 670a 2020 2020 6465 6620 7365 6172  ing.    def sear
-0000ef50: 6368 5f63 6f6f 7264 5f66 726f 6d5f 6469  ch_coord_from_di
-0000ef60: 6d28 7365 6c66 2c20 6461 2c20 6469 6d2c  m(self, da, dim,
-0000ef70: 2065 7272 6f72 733d 2269 676e 6f72 6522   errors="ignore"
-0000ef80: 293a 0a20 2020 2020 2020 2022 2222 5365  ):.        """Se
-0000ef90: 6172 6368 2061 2064 6174 6161 7272 6179  arch a dataarray
-0000efa0: 2066 6f72 2061 2063 6f6f 7264 696e 6174   for a coordinat
-0000efb0: 6520 6672 6f6d 2061 2064 696d 656e 7369  e from a dimensi
-0000efc0: 6f6e 206e 616d 650a 0a20 2020 2020 2020  on name..       
-0000efd0: 2049 7420 6669 7273 7420 7365 6172 6368   It first search
-0000efe0: 6573 2066 6f72 2061 2063 6f6f 7264 696e  es for a coordin
-0000eff0: 6174 6520 7769 7468 2074 6865 2073 616d  ate with the sam
-0000f000: 6520 6e61 6d65 2061 6e64 2074 6861 7420  e name and that 
-0000f010: 6973 0a20 2020 2020 2020 2074 6865 206f  is.        the o
-0000f020: 6e6c 7920 6f6e 6520 6861 7669 6e67 2074  nly one having t
-0000f030: 6869 7320 6469 6d65 6e73 696f 6e2e 0a20  his dimension.. 
-0000f040: 2020 2020 2020 2054 6865 6e20 6c6f 6f6b         Then look
-0000f050: 2066 6f72 2063 6f6f 7264 696e 6174 6573   for coordinates
-0000f060: 2077 6974 6820 7468 6520 7361 6d65 2074   with the same t
-0000f070: 7970 6520 6c69 6b65 2078 2c20 792c 2065  ype like x, y, e
-0000f080: 7463 2e0a 0a20 2020 2020 2020 2050 6172  tc...        Par
-0000f090: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0000f0a0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0000f0b0: 2020 2064 613a 2078 6172 7261 792e 4461     da: xarray.Da
-0000f0c0: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
-0000f0d0: 6469 6d3a 2073 7472 0a20 2020 2020 2020  dim: str.       
-0000f0e0: 207b 6572 726f 7273 7d0a 0a20 2020 2020   {errors}..     
-0000f0f0: 2020 2052 6574 7572 6e0a 2020 2020 2020     Return.      
-0000f100: 2020 2d2d 2d2d 2d2d 0a20 2020 2020 2020    ------.       
-0000f110: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
-0000f120: 792c 204e 6f6e 650a 2020 2020 2020 2020  y, None.        
-0000f130: 2020 2020 416e 2063 6f6f 7264 696e 6174      An coordinat
-0000f140: 6520 6172 7261 7920 6f72 204e 6f6e 650a  e array or None.
-0000f150: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f160: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000f170: 636f 6f72 6473 2e73 6561 7263 685f 6672  coords.search_fr
-0000f180: 6f6d 5f64 696d 2864 612c 2064 696d 2c20  om_dim(da, dim, 
-0000f190: 6572 726f 7273 3d65 7272 6f72 7329 0a0a  errors=errors)..
-0000f1a0: 2020 2020 4045 5252 4f52 532e 666f 726d      @ERRORS.form
-0000f1b0: 6174 5f6d 6574 686f 645f 646f 6373 7472  at_method_docstr
-0000f1c0: 696e 670a 2020 2020 6465 6620 7365 6172  ing.    def sear
-0000f1d0: 6368 5f64 6174 615f 7661 7228 7365 6c66  ch_data_var(self
-0000f1e0: 2c20 6f62 6a2c 2063 665f 6e61 6d65 3d4e  , obj, cf_name=N
-0000f1f0: 6f6e 652c 206c 6f63 3d22 616e 7922 2c20  one, loc="any", 
-0000f200: 6765 743d 226f 626a 222c 2073 696e 676c  get="obj", singl
-0000f210: 653d 5472 7565 2c20 6572 726f 7273 3d22  e=True, errors="
-0000f220: 7761 726e 2229 3a0a 2020 2020 2020 2020  warn"):.        
-0000f230: 2222 2253 6561 7263 6820 666f 7220 6120  """Search for a 
-0000f240: 6461 7461 5f76 6172 2074 6861 7420 6d61  data_var that ma
-0000f250: 6368 6573 2067 6976 656e 206f 7220 616e  ches given or an
-0000f260: 7920 7370 6563 730a 0a20 2020 2020 2020  y specs..       
-0000f270: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000f280: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000f290: 2020 2020 2020 206f 626a 3a20 4461 7461         obj: Data
-0000f2a0: 4172 7261 7920 6f72 2044 6174 6173 6574  Array or Dataset
-0000f2b0: 0a20 2020 2020 2020 2063 665f 6e61 6d65  .        cf_name
-0000f2c0: 3a20 7374 722c 2064 6963 740a 2020 2020  : str, dict.    
-0000f2d0: 2020 2020 2020 2020 4120 6765 6e65 7269          A generi
-0000f2e0: 6320 4346 206e 616d 652e 2049 6620 6e6f  c CF name. If no
-0000f2f0: 7420 7072 6f76 6964 6564 2c20 616c 6c20  t provided, all 
-0000f300: 4346 206e 616d 6573 2061 7265 2073 6361  CF names are sca
-0000f310: 6e65 642e 0a20 2020 2020 2020 206c 6f63  ned..        loc
-0000f320: 3a20 7374 722c 207b 7b22 616e 7922 2c20  : str, {{"any", 
-0000f330: 4e6f 6e65 7d7d 2c20 7b7b 2222 2c20 4661  None}}, {{"", Fa
-0000f340: 6c73 657d 7d0a 2020 2020 2020 2020 2020  lse}}.          
-0000f350: 2020 2d20 7374 723a 206f 6e65 206f 6620    - str: one of 
-0000f360: 7468 6573 6520 6c6f 6361 7469 6f6e 730a  these locations.
-0000f370: 2020 2020 2020 2020 2020 2020 2d20 4e6f              - No
-0000f380: 6e65 206f 7220 2261 6e79 223a 2061 6e79  ne or "any": any
-0000f390: 0a20 2020 2020 2020 2020 2020 202d 2046  .            - F
-0000f3a0: 616c 7365 206f 7220 2722 223a 206e 6f20  alse or '"": no 
-0000f3b0: 6c6f 6361 7469 6f6e 0a20 2020 2020 2020  location.       
-0000f3c0: 2067 6574 3a20 7b7b 226f 626a 222c 2022   get: {{"obj", "
-0000f3d0: 6e61 6d65 227d 7d0a 2020 2020 2020 2020  name"}}.        
-0000f3e0: 2020 2020 5768 656e 2066 6f75 6e64 2c20      When found, 
-0000f3f0: 6765 7420 7468 6520 6f62 6a65 6374 2066  get the object f
-0000f400: 6f75 6e64 206f 7220 6974 7320 6e61 6d65  ound or its name
-0000f410: 2e0a 2020 2020 2020 2020 7369 6e67 6c65  ..        single
-0000f420: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
-0000f430: 2020 2049 6620 5472 7565 2c20 7265 7475     If True, retu
-0000f440: 726e 2074 6865 2066 6972 7374 2069 7465  rn the first ite
-0000f450: 6d20 666f 756e 6420 6f72 204e 6f6e 652e  m found or None.
-0000f460: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-0000f470: 4661 6c73 652c 2072 6574 7572 6e20 6120  False, return a 
-0000f480: 706f 7373 6962 6c65 2065 6d70 7479 206c  possible empty l
-0000f490: 6973 7420 6f66 2066 6f75 6e64 2069 7465  ist of found ite
-0000f4a0: 6d73 2e0a 2020 2020 2020 2020 2020 2020  ms..            
-0000f4b0: 4120 7761 726e 696e 6720 6973 2065 6d69  A warning is emi
-0000f4c0: 7474 6564 2077 6865 6e20 7365 7420 746f  tted when set to
-0000f4d0: 2054 7275 6520 616e 6420 6d75 6c74 6970   True and multip
-0000f4e0: 6c65 2069 7465 6d20 6172 6520 666f 756e  le item are foun
-0000f4f0: 642e 0a20 2020 2020 2020 207b 6572 726f  d..        {erro
-0000f500: 7273 7d0a 0a20 2020 2020 2020 2052 6574  rs}..        Ret
-0000f510: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-0000f520: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-0000f530: 6520 6f72 2073 7472 206f 7220 6f62 6a65  e or str or obje
-0000f540: 6374 0a0a 2020 2020 2020 2020 4578 616d  ct..        Exam
-0000f550: 706c 650a 2020 2020 2020 2020 2d2d 2d2d  ple.        ----
-0000f560: 2d2d 2d0a 2020 2020 2020 2020 2e2e 2069  ---.        .. i
-0000f570: 7079 7468 6f6e 3a3a 2070 7974 686f 6e0a  python:: python.
-0000f580: 2020 2020 2020 2020 2020 2020 3a6f 6b77              :okw
-0000f590: 6172 6e69 6e67 3a0a 0a20 2020 2020 2020  arning:..       
-0000f5a0: 2020 2020 2040 7375 7070 7265 7373 0a20       @suppress. 
-0000f5b0: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-0000f5c0: 786f 612e 6366 2069 6d70 6f72 7420 6765  xoa.cf import ge
-0000f5d0: 745f 6366 5f73 7065 6373 0a20 2020 2020  t_cf_specs.     
-0000f5e0: 2020 2020 2020 2040 7375 7070 7265 7373         @suppress
-0000f5f0: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
-0000f600: 6f72 7420 7861 7272 6179 2061 7320 7872  ort xarray as xr
-0000f610: 2c20 6e75 6d70 7920 6173 206e 700a 2020  , numpy as np.  
-0000f620: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-0000f630: 2078 722e 4461 7461 4172 7261 7928 0a20   xr.DataArray(. 
-0000f640: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-0000f650: 302c 2031 5d2c 2064 696d 733d 2827 7827  0, 1], dims=('x'
-0000f660: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000f670: 2020 2061 7474 7273 3d7b 7b27 7374 616e     attrs={{'stan
-0000f680: 6461 7264 5f6e 616d 6527 3a20 2773 6561  dard_name': 'sea
-0000f690: 5f77 6174 6572 5f74 656d 7065 7261 7475  _water_temperatu
-0000f6a0: 7265 277d 7d29 0a20 2020 2020 2020 2020  re'}}).         
-0000f6b0: 2020 2064 7320 3d20 7872 2e44 6174 6173     ds = xr.Datas
-0000f6c0: 6574 287b 7b27 666f 6f27 3a20 6461 7461  et({{'foo': data
-0000f6d0: 7d7d 290a 2020 2020 2020 2020 2020 2020  }}).            
-0000f6e0: 6366 7370 6563 7320 3d20 6765 745f 6366  cfspecs = get_cf
-0000f6f0: 5f73 7065 6373 2829 0a20 2020 2020 2020  _specs().       
-0000f700: 2020 2020 2063 6673 7065 6373 2e73 6561       cfspecs.sea
-0000f710: 7263 685f 6461 7461 5f76 6172 2864 732c  rch_data_var(ds,
-0000f720: 2022 7465 6d70 2229 0a20 2020 2020 2020   "temp").       
-0000f730: 2020 2020 2063 6673 7065 6373 2e73 6561       cfspecs.sea
-0000f740: 7263 685f 6461 7461 5f76 6172 2864 732c  rch_data_var(ds,
-0000f750: 2022 7465 6d70 222c 2067 6574 3d22 6366   "temp", get="cf
-0000f760: 5f6e 616d 6522 290a 2020 2020 2020 2020  _name").        
-0000f770: 2020 2020 6366 7370 6563 732e 7365 6172      cfspecs.sear
-0000f780: 6368 5f64 6174 615f 7661 7228 6473 2c20  ch_data_var(ds, 
-0000f790: 2273 616c 2229 0a0a 2020 2020 2020 2020  "sal")..        
-0000f7a0: 5365 6520 616c 736f 0a20 2020 2020 2020  See also.       
-0000f7b0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020   --------.      
-0000f7c0: 2020 7365 6172 6368 5f63 6f6f 7264 0a20    search_coord. 
-0000f7d0: 2020 2020 2020 2043 4656 6172 5370 6563         CFVarSpec
-0000f7e0: 732e 7365 6172 6368 0a20 2020 2020 2020  s.search.       
-0000f7f0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-0000f800: 7572 6e20 7365 6c66 2e64 6174 615f 7661  urn self.data_va
-0000f810: 7273 2e73 6561 7263 6828 0a20 2020 2020  rs.search(.     
-0000f820: 2020 2020 2020 206f 626a 2c20 6366 5f6e         obj, cf_n
-0000f830: 616d 653d 6366 5f6e 616d 652c 206c 6f63  ame=cf_name, loc
-0000f840: 3d6c 6f63 2c20 6765 743d 6765 742c 2073  =loc, get=get, s
-0000f850: 696e 676c 653d 7369 6e67 6c65 2c20 6572  ingle=single, er
-0000f860: 726f 7273 3d65 7272 6f72 730a 2020 2020  rors=errors.    
-0000f870: 2020 2020 290a 0a20 2020 2040 4552 524f      )..    @ERRO
-0000f880: 5253 2e66 6f72 6d61 745f 6d65 7468 6f64  RS.format_method
-0000f890: 5f64 6f63 7374 7269 6e67 0a20 2020 2064  _docstring.    d
-0000f8a0: 6566 2073 6561 7263 6828 0a20 2020 2020  ef search(.     
-0000f8b0: 2020 2073 656c 662c 206f 626a 2c20 6366     self, obj, cf
-0000f8c0: 5f6e 616d 653d 4e6f 6e65 2c20 6c6f 633d  _name=None, loc=
-0000f8d0: 2261 6e79 222c 2067 6574 3d22 6f62 6a22  "any", get="obj"
-0000f8e0: 2c20 7369 6e67 6c65 3d54 7275 652c 2063  , single=True, c
-0000f8f0: 6174 6567 6f72 6965 733d 4e6f 6e65 2c20  ategories=None, 
-0000f900: 6572 726f 7273 3d22 7761 726e 220a 2020  errors="warn".  
-0000f910: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-0000f920: 5365 6172 6368 2066 6f72 2061 2064 6174  Search for a dat
-0000f930: 6161 7272 6179 2077 6974 6820 6461 7461  aarray with data
-0000f940: 5f76 6172 7320 616e 642f 6f72 2063 6f6f  _vars and/or coo
-0000f950: 7264 730a 0a0a 2020 2020 2020 2020 5061  rds...        Pa
-0000f960: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-0000f970: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0000f980: 2020 2020 6f62 6a3a 2078 6172 7261 792e      obj: xarray.
-0000f990: 4461 7461 4172 7261 792c 2078 6172 7261  DataArray, xarra
-0000f9a0: 792e 4461 7461 7365 740a 2020 2020 2020  y.Dataset.      
-0000f9b0: 2020 2020 2020 4172 7261 7920 6f72 2064        Array or d
-0000f9c0: 6174 6173 6574 2074 6f20 7363 616e 0a20  ataset to scan. 
-0000f9d0: 2020 2020 2020 2063 665f 6e61 6d65 3a20         cf_name: 
-0000f9e0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-0000f9f0: 4765 6e65 7269 6320 4346 206e 616d 6520  Generic CF name 
-0000fa00: 746f 2073 6561 7263 6820 666f 722e 0a20  to search for.. 
-0000fa10: 2020 2020 2020 2063 6174 6567 6f72 6965         categorie
-0000fa20: 733a 2073 7472 2c20 6c69 7374 2c20 4e6f  s: str, list, No
-0000fa30: 6e65 0a20 2020 2020 2020 2020 2020 2045  ne.            E
-0000fa40: 7870 6c69 6374 7920 6361 7465 676f 7269  xplicty categori
-0000fa50: 6573 2077 6974 6820 2263 6f6f 7264 7322  es with "coords"
-0000fa60: 2061 6e64 2022 6461 7461 5f76 6172 7322   and "data_vars"
-0000fa70: 2e0a 2020 2020 2020 2020 7b65 7272 6f72  ..        {error
-0000fa80: 737d 0a0a 2020 2020 2020 2020 5265 7475  s}..        Retu
-0000fa90: 726e 0a20 2020 2020 2020 202d 2d2d 2d2d  rn.        -----
-0000faa0: 2d0a 2020 2020 2020 2020 4e6f 6e65 2c20  -.        None, 
-0000fab0: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-0000fac0: 2c20 6c69 7374 0a0a 2020 2020 2020 2020  , list..        
-0000fad0: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
-0000fae0: 6f74 2063 6174 6567 6f72 6965 733a 0a20  ot categories:. 
-0000faf0: 2020 2020 2020 2020 2020 2063 6174 6567             categ
-0000fb00: 6f72 6965 7320 3d20 7365 6c66 2e63 6174  ories = self.cat
-0000fb10: 6567 6f72 6965 7320 6966 2068 6173 6174  egories if hasat
-0000fb20: 7472 286f 626a 2c20 2264 6174 615f 7661  tr(obj, "data_va
-0000fb30: 7273 2229 2065 6c73 6520 5b22 636f 6f72  rs") else ["coor
-0000fb40: 6473 222c 2022 6461 7461 5f76 6172 7322  ds", "data_vars"
-0000fb50: 5d0a 2020 2020 2020 2020 656c 6966 2069  ].        elif i
-0000fb60: 7369 6e73 7461 6e63 6528 6361 7465 676f  sinstance(catego
-0000fb70: 7269 6573 2c20 7374 7229 3a0a 2020 2020  ries, str):.    
-0000fb80: 2020 2020 2020 2020 6361 7465 676f 7269          categori
-0000fb90: 6573 203d 205b 6361 7465 676f 7269 6573  es = [categories
-0000fba0: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-0000fbb0: 2020 2020 2020 2020 2020 2020 6361 7465              cate
-0000fbc0: 676f 7269 6573 203d 2073 656c 662e 6361  gories = self.ca
-0000fbd0: 7465 676f 7269 6573 0a20 2020 2020 2020  tegories.       
-0000fbe0: 2065 7272 6f72 7320 3d20 4552 524f 5253   errors = ERRORS
-0000fbf0: 5b65 7272 6f72 735d 0a20 2020 2020 2020  [errors].       
-0000fc00: 2069 6620 6e6f 7420 7369 6e67 6c65 3a0a   if not single:.
-0000fc10: 2020 2020 2020 2020 2020 2020 666f 756e              foun
-0000fc20: 6420 3d20 5b5d 0a20 2020 2020 2020 2066  d = [].        f
-0000fc30: 6f72 2063 6174 6567 6f72 7920 696e 2063  or category in c
-0000fc40: 6174 6567 6f72 6965 733a 0a20 2020 2020  ategories:.     
-0000fc50: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
-0000fc60: 665b 6361 7465 676f 7279 5d2e 7365 6172  f[category].sear
-0000fc70: 6368 280a 2020 2020 2020 2020 2020 2020  ch(.            
-0000fc80: 2020 2020 6f62 6a2c 2063 665f 6e61 6d65      obj, cf_name
-0000fc90: 3d63 665f 6e61 6d65 2c20 6c6f 633d 6c6f  =cf_name, loc=lo
-0000fca0: 632c 2067 6574 3d67 6574 2c20 7369 6e67  c, get=get, sing
-0000fcb0: 6c65 3d73 696e 676c 652c 2065 7272 6f72  le=single, error
-0000fcc0: 733d 2269 676e 6f72 6522 0a20 2020 2020  s="ignore".     
-0000fcd0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000fce0: 2020 2020 2069 6620 6e6f 7420 7369 6e67       if not sing
-0000fcf0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-0000fd00: 2020 2020 7265 7320 3d20 5b72 2066 6f72      res = [r for
-0000fd10: 2072 2069 6e20 7265 7320 6966 2072 206e   r in res if r n
-0000fd20: 6f74 2069 6e20 666f 756e 645d 0a20 2020  ot in found].   
-0000fd30: 2020 2020 2020 2020 2020 2020 2066 6f75               fou
-0000fd40: 6e64 2e65 7874 656e 6428 7265 7329 0a20  nd.extend(res). 
-0000fd50: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000fd60: 7265 7320 6973 206e 6f74 204e 6f6e 653a  res is not None:
-0000fd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fd80: 2072 6574 7572 6e20 7265 730a 2020 2020   return res.    
-0000fd90: 2020 2020 6966 206e 6f74 2073 696e 676c      if not singl
-0000fda0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000fdb0: 6574 7572 6e20 666f 756e 640a 2020 2020  eturn found.    
-0000fdc0: 2020 2020 6d73 6720 3d20 2253 6561 7263      msg = "Searc
-0000fdd0: 6820 6661 696c 6564 220a 2020 2020 2020  h failed".      
-0000fde0: 2020 6966 2065 7272 6f72 7320 3d3d 2022    if errors == "
-0000fdf0: 7761 726e 223a 0a20 2020 2020 2020 2020  warn":.         
-0000fe00: 2020 2078 6f61 5f77 6172 6e28 6d73 6729     xoa_warn(msg)
-0000fe10: 0a20 2020 2020 2020 2065 6c69 6620 6572  .        elif er
-0000fe20: 726f 7273 203d 3d20 2272 6169 7365 223a  rors == "raise":
-0000fe30: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000fe40: 7365 2058 6f61 4346 4572 726f 7228 6d73  se XoaCFError(ms
-0000fe50: 6729 0a0a 2020 2020 6465 6620 6765 7428  g)..    def get(
-0000fe60: 7365 6c66 2c20 6f62 6a2c 2063 665f 6e61  self, obj, cf_na
-0000fe70: 6d65 2c20 6765 743d 226f 626a 2229 3a0a  me, get="obj"):.
-0000fe80: 2020 2020 2020 2020 2222 2241 2073 686f          """A sho
-0000fe90: 7274 6375 7420 746f 203a 6d65 7468 3a60  rtcut to :meth:`
-0000fea0: 7365 6172 6368 6020 7769 7468 2061 6e20  search` with an 
-0000feb0: 6578 706c 6963 6974 2067 656e 6572 6963  explicit generic
-0000fec0: 2043 4620 6e61 6d65 0a0a 2020 2020 2020   CF name..      
-0000fed0: 2020 4120 7369 6e67 6c65 2065 6c65 6d65    A single eleme
-0000fee0: 6e74 2069 7320 7365 6172 6368 6564 2066  nt is searched f
-0000fef0: 6f72 2069 6e74 6f20 616c 6c20 3a61 7474  or into all :att
-0000ff00: 723a 6063 6174 6567 6f72 6965 7360 0a20  r:`categories`. 
-0000ff10: 2020 2020 2020 2061 6e64 2065 7272 6f72         and error
-0000ff20: 7320 6172 6520 6967 6e6f 7265 642e 0a20  s are ignored.. 
-0000ff30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000ff40: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
-0000ff50: 6561 7263 6828 6f62 6a2c 2063 665f 6e61  earch(obj, cf_na
-0000ff60: 6d65 2c20 6572 726f 7273 3d22 6967 6e6f  me, errors="igno
-0000ff70: 7265 222c 2073 696e 676c 653d 5472 7565  re", single=True
-0000ff80: 2c20 6765 743d 6765 7429 0a20 2020 2020  , get=get).     
-0000ff90: 2020 2023 2069 6620 6461 2069 7320 4e6f     # if da is No
-0000ffa0: 6e65 3a0a 2020 2020 2020 2020 2320 2020  ne:.        #   
-0000ffb0: 2020 7261 6973 6520 586f 6143 4645 7272    raise XoaCFErr
-0000ffc0: 6f72 2822 5365 6172 6368 2066 6169 6c65  or("Search faile
-0000ffd0: 6420 666f 7220 7468 6520 666f 6c6c 6f77  d for the follow
-0000ffe0: 696e 6720 6366 206e 616d 653a 2022 0a20  ing cf name: ". 
-0000fff0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00010000: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00010010: 6e61 6d65 290a 2020 2020 2020 2020 2320  name).        # 
-00010020: 7265 7475 726e 2064 610a 0a20 2020 2040  return da..    @
-00010030: 4552 524f 5253 2e66 6f72 6d61 745f 6d65  ERRORS.format_me
-00010040: 7468 6f64 5f64 6f63 7374 7269 6e67 0a20  thod_docstring. 
-00010050: 2020 2064 6566 2067 6574 5f64 696d 7328     def get_dims(
-00010060: 0a20 2020 2020 2020 2073 656c 662c 2064  .        self, d
-00010070: 612c 2063 665f 6172 6773 2c20 616c 6c6f  a, cf_args, allo
-00010080: 775f 706f 7369 7469 6f6e 616c 3d46 616c  w_positional=Fal
-00010090: 7365 2c20 706f 7369 7469 6f6e 733d 2774  se, positions='t
-000100a0: 7a79 7827 2c20 7369 6e67 6c65 3d54 7275  zyx', single=Tru
-000100b0: 652c 2065 7272 6f72 733d 2277 6172 6e22  e, errors="warn"
-000100c0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-000100d0: 2222 2247 6574 2074 6865 2064 6174 6120  """Get the data 
-000100e0: 6172 7261 7920 6469 6d65 6e73 696f 6e73  array dimensions
-000100f0: 206e 616d 6573 2066 726f 6d20 7468 6569   names from thei
-00010100: 7220 7479 7065 0a0a 2020 2020 2020 2020  r type..        
-00010110: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00010120: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00010130: 2020 2020 2020 6461 3a20 7861 7272 6179        da: xarray
-00010140: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
-00010150: 2020 2020 2020 2041 7272 6179 2074 6f20         Array to 
-00010160: 7363 616e 0a20 2020 2020 2020 2063 665f  scan.        cf_
-00010170: 6172 6773 3a20 7374 722c 206c 6973 740a  args: str, list.
-00010180: 2020 2020 2020 2020 2020 2020 4c65 7474              Lett
-00010190: 6572 7320 616d 6f6e 6720 2278 222c 2022  ers among "x", "
-000101a0: 7922 2c20 227a 222c 2022 7422 2061 6e64  y", "z", "t" and
-000101b0: 2022 6622 2c0a 2020 2020 2020 2020 2020   "f",.          
-000101c0: 2020 6f72 2067 656e 6572 6963 2043 4620    or generic CF 
-000101d0: 6e61 6d65 732e 0a20 2020 2020 2020 2061  names..        a
-000101e0: 6c6c 6f77 5f70 6f73 6974 696f 6e61 6c3a  llow_positional:
-000101f0: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
-00010200: 2020 4661 6c6c 2062 6163 6b20 746f 2070    Fall back to p
-00010210: 6f73 6974 696f 6e61 6c20 6469 6d65 6e73  ositional dimens
-00010220: 696f 6e20 6f66 2074 7970 6573 2069 7320  ion of types is 
-00010230: 756e 6b6f 776e 2e0a 2020 2020 2020 2020  unkown..        
-00010240: 706f 7369 7469 6f6e 733a 2073 7472 0a20  positions: str. 
-00010250: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00010260: 6c74 2070 6f73 6974 696f 6e20 7065 7220  lt position per 
-00010270: 7479 7065 2073 7461 7274 696e 6720 6672  type starting fr
-00010280: 6f6d 2074 6865 2065 6e64 2e0a 2020 2020  om the end..    
-00010290: 2020 2020 7369 6e67 6c65 3a20 626f 6f6c      single: bool
-000102a0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-000102b0: 5472 7565 2c20 7265 7475 726e 2074 6865  True, return the
-000102c0: 2066 6972 7374 2069 7465 6d20 666f 756e   first item foun
-000102d0: 6420 6f72 204e 6f6e 652e 0a20 2020 2020  d or None..     
-000102e0: 2020 2020 2020 2049 6620 4661 6c73 652c         If False,
-000102f0: 2072 6574 7572 6e20 6120 706f 7373 6962   return a possib
-00010300: 6c65 2065 6d70 7479 206c 6973 7420 6f66  le empty list of
-00010310: 2066 6f75 6e64 2069 7465 6d73 2e0a 2020   found items..  
-00010320: 2020 2020 2020 7b65 7272 6f72 737d 0a0a        {errors}..
-00010330: 2020 2020 2020 2020 5265 7475 726e 0a20          Return. 
-00010340: 2020 2020 2020 202d 2d2d 2d2d 2d0a 2020         ------.  
-00010350: 2020 2020 2020 7475 706c 650a 2020 2020        tuple.    
-00010360: 2020 2020 2020 2020 5475 706c 6520 6f66          Tuple of
-00010370: 2064 696d 656e 7369 6f6e 206e 616d 6520   dimension name 
-00010380: 6f72 204e 6f6e 6520 7768 656e 2074 6865  or None when the
-00010390: 2064 696d 656e 7369 6f6e 2069 6620 6e6f   dimension if no
-000103a0: 7420 666f 756e 640a 0a20 2020 2020 2020  t found..       
-000103b0: 2053 6565 2061 6c73 6f0a 2020 2020 2020   See also.      
-000103c0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020    --------.     
-000103d0: 2020 2043 4643 6f6f 7264 5370 6563 732e     CFCoordSpecs.
-000103e0: 6765 745f 6469 6d73 0a20 2020 2020 2020  get_dims.       
-000103f0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-00010400: 7572 6e20 7365 6c66 2e63 6f6f 7264 732e  urn self.coords.
-00010410: 6765 745f 6469 6d73 280a 2020 2020 2020  get_dims(.      
-00010420: 2020 2020 2020 6461 2c0a 2020 2020 2020        da,.      
-00010430: 2020 2020 2020 6366 5f61 7267 732c 0a20        cf_args,. 
-00010440: 2020 2020 2020 2020 2020 2061 6c6c 6f77             allow
-00010450: 5f70 6f73 6974 696f 6e61 6c3d 616c 6c6f  _positional=allo
-00010460: 775f 706f 7369 7469 6f6e 616c 2c0a 2020  w_positional,.  
-00010470: 2020 2020 2020 2020 2020 706f 7369 7469            positi
-00010480: 6f6e 733d 706f 7369 7469 6f6e 732c 0a20  ons=positions,. 
-00010490: 2020 2020 2020 2020 2020 2073 696e 676c             singl
-000104a0: 653d 7369 6e67 6c65 2c0a 2020 2020 2020  e=single,.      
-000104b0: 2020 2020 2020 6572 726f 7273 3d65 7272        errors=err
-000104c0: 6f72 732c 0a20 2020 2020 2020 2029 0a0a  ors,.        )..
-000104d0: 2020 2020 6465 6620 6765 745f 6178 6973      def get_axis
-000104e0: 2873 656c 662c 2063 6f6f 7264 2c20 6c6f  (self, coord, lo
-000104f0: 7765 723d 4661 6c73 6529 3a0a 2020 2020  wer=False):.    
-00010500: 2020 2020 2222 2247 6574 2074 6865 2064      """Get the d
-00010510: 696d 656e 7369 6f6e 2074 7970 652c 2065  imension type, e
-00010520: 6974 6865 7220 6672 6f6d 2061 7869 7320  ither from axis 
-00010530: 6174 7472 206f 7220 6672 6f6d 206d 6174  attr or from mat
-00010540: 6368 2043 6620 636f 6f72 640a 0a20 2020  ch Cf coord..   
-00010550: 2020 2020 202e 2e20 6e6f 7465 3a3a 2054       .. note:: T
-00010560: 6865 2060 6061 7869 7360 6020 6973 2074  he ``axis`` is t
-00010570: 6865 2075 7070 6572 6361 7365 2076 6572  he uppercase ver
-00010580: 7369 6f6e 206f 6620 7468 6520 6060 6469  sion of the ``di
-00010590: 6d5f 7479 7065 6060 0a0a 2020 2020 2020  m_type``..      
-000105a0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-000105b0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-000105c0: 2020 2020 2020 2020 636f 6f72 643a 2078          coord: x
-000105d0: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
-000105e0: 2020 2020 2020 2020 6c6f 7765 723a 2062          lower: b
-000105f0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-00010600: 4c6f 7765 7220 6361 7365 3f0a 0a20 2020  Lower case?..   
-00010610: 2020 2020 2052 6574 7572 6e0a 2020 2020       Return.    
-00010620: 2020 2020 2d2d 2d2d 2d2d 0a20 2020 2020      ------.     
-00010630: 2020 207b 2278 222c 2022 7922 2c20 227a     {"x", "y", "z
-00010640: 222c 2022 7422 2c20 2266 227d 2c20 4e6f  ", "t", "f"}, No
-00010650: 6e65 0a0a 2020 2020 2020 2020 5365 6520  ne..        See 
-00010660: 616c 736f 0a20 2020 2020 2020 202d 2d2d  also.        ---
-00010670: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6765  -----.        ge
-00010680: 745f 6469 6d5f 7479 7065 0a20 2020 2020  t_dim_type.     
-00010690: 2020 2067 6574 5f64 696d 5f74 7970 6573     get_dim_types
-000106a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000106b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000106c0: 2e63 6f6f 7264 732e 6765 745f 6178 6973  .coords.get_axis
-000106d0: 2863 6f6f 7264 2c20 6c6f 7765 723d 6c6f  (coord, lower=lo
-000106e0: 7765 7229 0a0a 2020 2020 6465 6620 6765  wer)..    def ge
-000106f0: 745f 6469 6d5f 7479 7065 2873 656c 662c  t_dim_type(self,
-00010700: 2064 696d 2c20 6461 3d4e 6f6e 652c 206c   dim, da=None, l
-00010710: 6f77 6572 3d54 7275 6529 3a0a 2020 2020  ower=True):.    
-00010720: 2020 2020 2222 2247 6574 2074 6865 2074      """Get the t
-00010730: 7970 6520 6f66 2061 2064 696d 656e 7369  ype of a dimensi
-00010740: 6f6e 0a0a 2020 2020 2020 2020 5468 7265  on..        Thre
-00010750: 6520 6361 7365 733a 0a0a 2020 2020 2020  e cases:..      
-00010760: 2020 2d20 5468 6973 2064 696d 656e 7369    - This dimensi
-00010770: 6f6e 2069 7320 7265 6769 7374 6572 6564  on is registered
-00010780: 2069 6e20 4346 2064 696d 732e 0a20 2020   in CF dims..   
-00010790: 2020 2020 202d 206f 626a 2068 6173 2064       - obj has d
-000107a0: 696d 2061 7320 6469 6d20 616e 6420 6861  im as dim and ha
-000107b0: 7320 616e 2061 7869 7320 6174 7472 6962  s an axis attrib
-000107c0: 7574 6520 696e 6665 7272 6564 2077 6974  ute inferred wit
-000107d0: 6820 3a6d 6574 683a 6067 6574 5f61 7869  h :meth:`get_axi
-000107e0: 7360 2e0a 2020 2020 2020 2020 2d20 6f62  s`..        - ob
-000107f0: 6a20 6861 7320 6120 636f 6f72 6420 6e61  j has a coord na
-00010800: 6d65 6420 6469 6d20 7769 7468 2061 6e20  med dim with an 
-00010810: 6178 6973 2061 7474 7269 6275 7465 2069  axis attribute i
-00010820: 6e66 6572 7265 6420 7769 7468 203a 6d65  nferred with :me
-00010830: 7468 3a60 6765 745f 6178 6973 602e 0a0a  th:`get_axis`...
-00010840: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00010850: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00010860: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6469  -----.        di
-00010870: 6d3a 2073 7472 0a20 2020 2020 2020 2020  m: str.         
-00010880: 2020 2044 696d 656e 7369 6f6e 206e 616d     Dimension nam
-00010890: 650a 2020 2020 2020 2020 6f62 6a3a 2078  e.        obj: x
-000108a0: 6172 7261 792e 4461 7461 4172 7261 792c  array.DataArray,
-000108b0: 2078 6172 7261 792e 4461 7461 7365 740a   xarray.Dataset.
-000108c0: 2020 2020 2020 2020 2020 2020 4461 7461              Data
-000108d0: 2061 7272 6179 2074 6861 7420 7468 6520   array that the 
-000108e0: 6469 6d65 6e73 696f 6e20 6265 6c6f 6e67  dimension belong
-000108f0: 7320 746f 2c20 746f 2068 656c 7020 696e  s to, to help in
-00010900: 6665 7272 696e 670a 2020 2020 2020 2020  ferring.        
-00010910: 2020 2020 7468 6520 7479 7065 0a20 2020      the type.   
-00010920: 2020 2020 206c 6f77 6572 3a20 626f 6f6c       lower: bool
-00010930: 0a20 2020 2020 2020 2020 2020 2046 6f72  .            For
-00010940: 206c 6f77 6572 2063 6173 650a 0a20 2020   lower case..   
-00010950: 2020 2020 2052 6574 7572 6e0a 2020 2020       Return.    
-00010960: 2020 2020 2d2d 2d2d 2d2d 0a20 2020 2020      ------.     
-00010970: 2020 2073 7472 2c20 4e6f 6e65 0a20 2020     str, None.   
-00010980: 2020 2020 2020 2020 204c 6574 7465 7220           Letter 
-00010990: 6173 206f 6e65 206f 6620 782c 2079 2c20  as one of x, y, 
-000109a0: 7a2c 2074 206f 7220 662c 2069 6620 666f  z, t or f, if fo
-000109b0: 756e 642c 2065 6c73 6520 4e6f 6e65 0a0a  und, else None..
-000109c0: 2020 2020 2020 2020 5365 6520 616c 736f          See also
-000109d0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000109e0: 2d0a 2020 2020 2020 2020 6765 745f 6178  -.        get_ax
-000109f0: 6973 0a20 2020 2020 2020 2022 2222 0a20  is.        """. 
-00010a00: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00010a10: 6c66 2e63 6f6f 7264 732e 6765 745f 6469  lf.coords.get_di
-00010a20: 6d5f 7479 7065 2864 696d 2c20 6461 3d64  m_type(dim, da=d
-00010a30: 612c 206c 6f77 6572 3d6c 6f77 6572 290a  a, lower=lower).
-00010a40: 0a20 2020 2064 6566 2067 6574 5f64 696d  .    def get_dim
-00010a50: 5f74 7970 6573 2873 656c 662c 2064 612c  _types(self, da,
-00010a60: 2075 6e6b 6e6f 776e 3d4e 6f6e 652c 2061   unknown=None, a
-00010a70: 7364 6963 743d 4661 6c73 6529 3a0a 2020  sdict=False):.  
-00010a80: 2020 2020 2020 2222 2247 6574 2061 2074        """Get a t
-00010a90: 7570 6c65 206f 6620 7468 6520 6469 6d65  uple of the dime
-00010aa0: 6e73 696f 6e20 7479 7065 7320 6f66 2061  nsion types of a
-00010ab0: 6e20 6172 7261 790a 0a20 2020 2020 2020  n array..       
-00010ac0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00010ad0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00010ae0: 2020 2020 2020 206f 626a 3a20 7861 7272         obj: xarr
-00010af0: 6179 2e44 6174 6141 7272 6179 2c20 7475  ay.DataArray, tu
-00010b00: 706c 6528 7374 7229 2c20 7861 7272 6179  ple(str), xarray
-00010b10: 2e44 6174 6173 6574 0a20 2020 2020 2020  .Dataset.       
-00010b20: 2020 2020 2044 6174 6120 6172 7261 792c       Data array,
-00010b30: 2064 6174 6173 6574 206f 7220 7475 706c   dataset or tupl
-00010b40: 6520 6f66 2064 696d 656e 7369 6f6e 730a  e of dimensions.
-00010b50: 2020 2020 2020 2020 756e 6b6e 6f77 6e3a          unknown:
-00010b60: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-00010b70: 7565 2074 6f20 6173 7369 676e 2077 6865  ue to assign whe
-00010b80: 6e20 7479 7065 2069 7320 756e 6b6e 6f77  n type is unknow
-00010b90: 6e0a 2020 2020 2020 2020 6173 6469 6374  n.        asdict
-00010ba0: 3a20 626f 6f6c 0a0a 2020 2020 2020 2020  : bool..        
-00010bb0: 5265 7475 726e 0a20 2020 2020 2020 202d  Return.        -
-00010bc0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7475  -----.        tu
-00010bd0: 706c 652c 2064 6963 740a 2020 2020 2020  ple, dict.      
-00010be0: 2020 2020 2020 5475 706c 6520 6f66 2064        Tuple of d
-00010bf0: 696d 656e 7369 6f6e 2074 7970 6573 2061  imension types a
-00010c00: 6e64 206f 6620 6c65 6e67 7468 2060 606f  nd of length ``o
-00010c10: 626a 2e6e 6469 6d60 602e 0a20 2020 2020  bj.ndim``..     
-00010c20: 2020 2020 2020 2041 2064 696d 656e 7369         A dimensi
-00010c30: 6f6e 2074 7970 6520 6973 2065 6974 6865  on type is eithe
-00010c40: 7220 6120 6c65 7474 6572 206f 7220 7468  r a letter or th
-00010c50: 6520 6060 756e 6b6f 776e 6060 2076 616c  e ``unkown`` val
-00010c60: 7565 0a20 2020 2020 2020 2020 2020 2077  ue.            w
-00010c70: 6865 6e20 7468 6520 696e 6665 7265 6e63  hen the inferenc
-00010c80: 6520 6f66 2074 7970 6520 6861 7320 6661  e of type has fa
-00010c90: 696c 6564 2e0a 2020 2020 2020 2020 2020  iled..          
-00010ca0: 2020 4966 2060 6061 7364 6963 7460 6020    If ``asdict`` 
-00010cb0: 6973 2054 7275 652c 2061 2064 6963 7420  is True, a dict 
-00010cc0: 6973 2072 6574 7572 6e65 6420 696e 7374  is returned inst
-00010cd0: 6561 642c 0a20 2020 2020 2020 2020 2020  ead,.           
-00010ce0: 2060 6028 6469 6d2c 2064 696d 5f74 7970   ``(dim, dim_typ
-00010cf0: 6529 6060 2061 7320 6b65 792d 7661 6c75  e)`` as key-valu
-00010d00: 6520 7061 6972 732e 0a0a 2020 2020 2020  e pairs...      
-00010d10: 2020 5365 6520 616c 736f 0a20 2020 2020    See also.     
-00010d20: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
-00010d30: 2020 2020 6765 745f 6469 6d5f 7479 7065      get_dim_type
-00010d40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010d50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00010d60: 2e63 6f6f 7264 732e 6765 745f 6469 6d5f  .coords.get_dim_
-00010d70: 7479 7065 7328 6461 2c20 756e 6b6e 6f77  types(da, unknow
-00010d80: 6e3d 756e 6b6e 6f77 6e2c 2061 7364 6963  n=unknown, asdic
-00010d90: 743d 6173 6469 6374 290a 0a20 2020 2064  t=asdict)..    d
-00010da0: 6566 2070 6172 7365 5f64 696d 7328 7365  ef parse_dims(se
-00010db0: 6c66 2c20 6469 6d73 2c20 6f62 6a29 3a0a  lf, dims, obj):.
-00010dc0: 2020 2020 2020 2020 2222 2243 6f6e 7665          """Conve
-00010dd0: 7274 2066 726f 6d20 6765 6e65 7269 6320  rt from generic 
-00010de0: 6469 6d20 6e61 6d65 7320 746f 2073 7065  dim names to spe
-00010df0: 6369 616c 697a 6564 206e 616d 6573 0a0a  cialized names..
-00010e00: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00010e10: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00010e20: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6469  -----.        di
-00010e30: 6d73 3a20 7374 722c 2074 7570 6c65 2c20  ms: str, tuple, 
-00010e40: 6c69 7374 2c20 6469 6374 0a20 2020 2020  list, dict.     
-00010e50: 2020 206f 626a 3a20 7861 7272 6179 2e44     obj: xarray.D
-00010e60: 6174 6173 6574 2c20 7861 7272 6179 2e44  ataset, xarray.D
-00010e70: 6174 6141 7272 6179 0a0a 2020 2020 2020  ataArray..      
-00010e80: 2020 5265 7475 726e 0a20 2020 2020 2020    Return.       
-00010e90: 202d 2d2d 2d2d 2d0a 2020 2020 2020 2020   ------.        
-00010ea0: 5361 6d65 2074 7970 6520 6173 2064 696d  Same type as dim
-00010eb0: 730a 2020 2020 2020 2020 2222 220a 2020  s.        """.  
-00010ec0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00010ed0: 662e 636f 6f72 6473 2e70 6172 7365 5f64  f.coords.parse_d
-00010ee0: 696d 7328 6469 6d73 2c20 6f62 6a29 0a0a  ims(dims, obj)..
-00010ef0: 2020 2020 6465 6620 696e 6665 725f 636f      def infer_co
-00010f00: 6f72 6473 2873 656c 662c 2064 7329 3a0a  ords(self, ds):.
-00010f10: 2020 2020 2020 2020 2222 2253 6561 7263          """Searc
-00010f20: 6820 666f 7220 6b6e 6f77 6e20 636f 6f72  h for known coor
-00010f30: 6473 2061 6e64 206d 616b 6520 7375 7265  ds and make sure
-00010f40: 2074 6865 7920 6172 6520 7365 7420 6173   they are set as
-00010f50: 2063 6f6f 7264 730a 0a20 2020 2020 2020   coords..       
-00010f60: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00010f70: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00010f80: 2020 2020 2020 2064 733a 2078 6172 7261         ds: xarra
-00010f90: 792e 4461 7461 7365 740a 0a20 2020 2020  y.Dataset..     
-00010fa0: 2020 2052 6574 7572 6e0a 2020 2020 2020     Return.      
-00010fb0: 2020 2d2d 2d2d 2d2d 0a20 2020 2020 2020    ------.       
-00010fc0: 2078 6172 7261 792e 4461 7461 7365 740a   xarray.Dataset.
-00010fd0: 2020 2020 2020 2020 2020 2020 4e65 7720              New 
-00010fe0: 6461 7461 7365 7420 7769 7468 2070 6f74  dataset with pot
-00010ff0: 656e 7469 616c 6c79 2075 7064 6174 6564  entially updated
-00011000: 2063 6f6f 7264 696e 6174 6573 0a20 2020   coordinates.   
-00011010: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011020: 2069 6620 6861 7361 7474 7228 6473 2c20   if hasattr(ds, 
-00011030: 2264 6174 615f 7661 7273 2229 3a0a 2020  "data_vars"):.  
-00011040: 2020 2020 2020 2020 2020 666f 7220 6461            for da
-00011050: 2069 6e20 6473 2e64 6174 615f 7661 7273   in ds.data_vars
-00011060: 2e76 616c 7565 7328 293a 0a20 2020 2020  .values():.     
-00011070: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00011080: 6c66 2e63 6f6f 7264 732e 6d61 7463 6828  lf.coords.match(
-00011090: 6461 293a 0a20 2020 2020 2020 2020 2020  da):.           
-000110a0: 2020 2020 2020 2020 2064 7320 3d20 6473           ds = ds
-000110b0: 2e73 6574 5f63 6f6f 7264 7328 6461 2e6e  .set_coords(da.n
-000110c0: 616d 6529 0a20 2020 2020 2020 2072 6574  ame).        ret
-000110d0: 7572 6e20 6473 2e63 6f70 7928 290a 0a0a  urn ds.copy()...
-000110e0: 636c 6173 7320 5f43 4643 6174 5370 6563  class _CFCatSpec
-000110f0: 735f 286f 626a 6563 7429 3a0a 2020 2020  s_(object):.    
-00011100: 2222 2242 6173 6520 636c 6173 7320 666f  """Base class fo
-00011110: 7220 6c6f 6164 696e 6720 6461 7461 5f76  r loading data_v
-00011120: 6172 7320 616e 6420 636f 6f72 6473 2043  ars and coords C
-00011130: 4620 7370 6563 6966 6963 6174 696f 6e73  F specifications
-00011140: 2222 220a 0a20 2020 2063 6174 6567 6f72  """..    categor
-00011150: 7920 3d20 4e6f 6e65 0a0a 2020 2020 6174  y = None..    at
-00011160: 7472 735f 6578 636c 7564 6520 3d20 5b0a  trs_exclude = [.
-00011170: 2020 2020 2020 2020 226e 616d 6522 2c0a          "name",.
-00011180: 2020 2020 2020 2020 2269 6e68 6572 6974          "inherit
-00011190: 222c 0a20 2020 2020 2020 2022 636f 6f72  ",.        "coor
-000111a0: 6473 222c 0a20 2020 2020 2020 2022 7365  ds",.        "se
-000111b0: 6c65 6374 222c 0a20 2020 2020 2020 2022  lect",.        "
-000111c0: 7365 6172 6368 5f6f 7264 6572 222c 0a20  search_order",. 
-000111d0: 2020 2020 2020 2022 636d 6170 222c 0a20         "cmap",. 
-000111e0: 2020 205d 0a0a 2020 2020 6174 7472 735f     ]..    attrs_
-000111f0: 6669 7273 7420 3d20 5b0a 2020 2020 2020  first = [.      
-00011200: 2020 226e 616d 6522 2c0a 2020 2020 2020    "name",.      
-00011210: 2020 2273 7461 6e64 6172 645f 6e61 6d65    "standard_name
-00011220: 222c 0a20 2020 2020 2020 2022 6c6f 6e67  ",.        "long
-00011230: 5f6e 616d 6522 2c0a 2020 2020 2020 2020  _name",.        
-00011240: 2275 6e69 7473 222c 0a20 2020 205d 0a0a  "units",.    ]..
-00011250: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00011260: 2873 656c 662c 2070 6172 656e 7429 3a0a  (self, parent):.
-00011270: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00011280: 656c 662e 6361 7465 676f 7279 2069 6e20  elf.category in 
-00011290: 7061 7265 6e74 0a20 2020 2020 2020 2073  parent.        s
-000112a0: 656c 662e 7061 7265 6e74 203d 2070 6172  elf.parent = par
-000112b0: 656e 740a 0a20 2020 2040 7072 6f70 6572  ent..    @proper
-000112c0: 7479 0a20 2020 2064 6566 2063 6f6f 7264  ty.    def coord
-000112d0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-000112e0: 2072 6574 7572 6e20 7365 6c66 2e70 6172   return self.par
-000112f0: 656e 742e 636f 6f72 6473 0a0a 2020 2020  ent.coords..    
-00011300: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00011310: 6620 6461 7461 5f76 6172 7328 7365 6c66  f data_vars(self
-00011320: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00011330: 6e20 7365 6c66 2e70 6172 656e 742e 6461  n self.parent.da
-00011340: 7461 5f76 6172 730a 0a20 2020 2040 7072  ta_vars..    @pr
-00011350: 6f70 6572 7479 0a20 2020 2064 6566 2073  operty.    def s
-00011360: 676c 6f63 6174 6f72 2873 656c 6629 3a0a  glocator(self):.
-00011370: 2020 2020 2020 2020 2222 223a 636c 6173          """:clas
-00011380: 733a 6053 474c 6f63 6174 6f72 6020 696e  s:`SGLocator` in
-00011390: 7374 616e 6365 2222 220a 2020 2020 2020  stance""".      
-000113a0: 2020 7265 7475 726e 2073 656c 662e 7061    return self.pa
-000113b0: 7265 6e74 2e73 676c 6f63 6174 6f72 0a0a  rent.sglocator..
-000113c0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-000113d0: 2020 6465 6620 5f64 6963 7428 7365 6c66    def _dict(self
-000113e0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-000113f0: 6e20 7365 6c66 2e70 6172 656e 742e 5f64  n self.parent._d
-00011400: 6963 745b 7365 6c66 2e63 6174 6567 6f72  ict[self.categor
-00011410: 795d 0a0a 2020 2020 6465 6620 5f5f 6765  y]..    def __ge
-00011420: 7469 7465 6d5f 5f28 7365 6c66 2c20 6b65  titem__(self, ke
-00011430: 7929 3a0a 2020 2020 2020 2020 7265 7475  y):.        retu
-00011440: 726e 2073 656c 662e 6765 745f 7370 6563  rn self.get_spec
-00011450: 7328 6b65 7929 0a0a 2020 2020 6465 6620  s(key)..    def 
-00011460: 5f5f 6974 6572 5f5f 2873 656c 6629 3a0a  __iter__(self):.
-00011470: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00011480: 7465 7228 7365 6c66 2e5f 6469 6374 290a  ter(self._dict).
-00011490: 0a20 2020 2064 6566 205f 5f6c 656e 5f5f  .    def __len__
-000114a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000114b0: 7265 7475 726e 206c 656e 2873 656c 662e  return len(self.
-000114c0: 5f64 6963 7429 0a0a 2020 2020 6465 6620  _dict)..    def 
-000114d0: 5f5f 636f 6e74 6169 6e73 5f5f 2873 656c  __contains__(sel
-000114e0: 662c 206b 6579 293a 0a20 2020 2020 2020  f, key):.       
-000114f0: 2072 6574 7572 6e20 6b65 7920 696e 2073   return key in s
-00011500: 656c 662e 5f64 6963 740a 0a20 2020 2023  elf._dict..    #
-00011510: 2064 6566 205f 5f73 7472 5f5f 2873 656c   def __str__(sel
-00011520: 6629 3a0a 2020 2020 2320 2020 2020 7265  f):.    #     re
-00011530: 7475 726e 2070 666f 726d 6174 2873 656c  turn pformat(sel
-00011540: 662e 5f64 6963 7429 0a0a 2020 2020 6465  f._dict)..    de
-00011550: 6620 5f76 616c 6964 6174 655f 6e61 6d65  f _validate_name
-00011560: 5f28 7365 6c66 2c20 6e61 6d65 293a 0a20  _(self, name):. 
-00011570: 2020 2020 2020 2069 6620 6e61 6d65 2069         if name i
-00011580: 6e20 7365 6c66 3a0a 2020 2020 2020 2020  n self:.        
-00011590: 2020 2020 7265 7475 726e 206e 616d 650a      return name.
-000115a0: 0a20 2020 2064 6566 205f 6173 7365 7274  .    def _assert
-000115b0: 5f6b 6e6f 776e 5f28 7365 6c66 2c20 6e61  _known_(self, na
-000115c0: 6d65 2c20 6572 726f 7273 3d22 7261 6973  me, errors="rais
-000115d0: 6522 293a 0a20 2020 2020 2020 2069 6620  e"):.        if 
-000115e0: 6e61 6d65 206e 6f74 2069 6e20 7365 6c66  name not in self
-000115f0: 2e5f 6469 6374 3a0a 2020 2020 2020 2020  ._dict:.        
-00011600: 2020 2020 6966 2065 7272 6f72 7320 3d3d      if errors ==
-00011610: 2022 7261 6973 6522 3a0a 2020 2020 2020   "raise":.      
-00011620: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00011630: 586f 6143 4645 7272 6f72 2866 2249 6e76  XoaCFError(f"Inv
-00011640: 616c 6964 207b 7365 6c66 2e63 6174 6567  alid {self.categ
-00011650: 6f72 797d 2043 4620 7370 6563 7320 6e61  ory} CF specs na
-00011660: 6d65 3a20 2220 2b20 6e61 6d65 290a 2020  me: " + name).  
-00011670: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00011680: 2046 616c 7365 0a20 2020 2020 2020 2072   False.        r
-00011690: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
-000116a0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-000116b0: 6620 6e61 6d65 7328 7365 6c66 293a 0a20  f names(self):. 
-000116c0: 2020 2020 2020 2072 6574 7572 6e20 5b6b         return [k
-000116d0: 6579 2066 6f72 206b 6579 2069 6e20 7365  ey for key in se
-000116e0: 6c66 2e5f 6469 6374 2e6b 6579 7328 2920  lf._dict.keys() 
-000116f0: 6966 206e 6f74 206b 6579 2e73 7461 7274  if not key.start
-00011700: 7377 6974 6828 225f 2229 5d0a 0a20 2020  swith("_")]..   
-00011710: 2064 6566 2069 7465 6d73 2873 656c 6629   def items(self)
-00011720: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00011730: 2073 656c 662e 5f64 6963 742e 6974 656d   self._dict.item
-00011740: 7328 290a 0a20 2020 2064 6566 206b 6579  s()..    def key
-00011750: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-00011760: 2072 6574 7572 6e20 7365 6c66 2e5f 6469   return self._di
-00011770: 6374 2e6b 6579 7328 290a 0a20 2020 2064  ct.keys()..    d
-00011780: 6566 2067 6574 5f73 7065 6373 2873 656c  ef get_specs(sel
-00011790: 662c 206e 616d 652c 2065 7272 6f72 733d  f, name, errors=
-000117a0: 2277 6172 6e22 293a 0a20 2020 2020 2020  "warn"):.       
-000117b0: 2022 2222 4765 7420 7468 6520 7370 6563   """Get the spec
-000117c0: 7320 6f66 2061 2063 6620 6974 656d 0a0a  s of a cf item..
-000117d0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000117e0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-000117f0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6e61  -----.        na
-00011800: 6d65 3a20 7374 720a 2020 2020 2020 2020  me: str.        
-00011810: 6572 726f 7273 3a20 2269 676e 6f72 6522  errors: "ignore"
-00011820: 2c20 2277 6172 6e69 6e67 2220 6f72 2022  , "warning" or "
-00011830: 7261 6973 6522 2e0a 0a20 2020 2020 2020  raise"...       
-00011840: 2052 6574 7572 6e0a 2020 2020 2020 2020   Return.        
-00011850: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2064  ------.        d
-00011860: 6963 7420 6f72 204e 6f6e 650a 2020 2020  ict or None.    
-00011870: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00011880: 6572 726f 7273 203d 2045 5252 4f52 535b  errors = ERRORS[
-00011890: 6572 726f 7273 5d0a 2020 2020 2020 2020  errors].        
-000118a0: 6966 206e 616d 6520 6e6f 7420 696e 2073  if name not in s
-000118b0: 656c 662e 5f64 6963 743a 0a20 2020 2020  elf._dict:.     
-000118c0: 2020 2020 2020 2069 6620 6572 726f 7273         if errors
-000118d0: 203d 3d20 2272 6169 7365 223a 0a20 2020   == "raise":.   
-000118e0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-000118f0: 7365 2058 6f61 4346 4572 726f 7228 2243  se XoaCFError("C
-00011900: 616e 2774 2067 6574 2063 6620 7370 6563  an't get cf spec
-00011910: 7320 6672 6f6d 3a20 2220 2b20 6e61 6d65  s from: " + name
-00011920: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00011930: 2065 7272 6f72 7320 3d3d 2022 7761 726e   errors == "warn
-00011940: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00011950: 2020 2078 6f61 5f77 6172 6e28 2249 6e76     xoa_warn("Inv
-00011960: 616c 6964 2063 6620 6e61 6d65 3a20 2220  alid cf name: " 
-00011970: 2b20 7374 7228 6e61 6d65 2929 0a20 2020  + str(name)).   
-00011980: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00011990: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000119a0: 656c 662e 5f64 6963 745b 6e61 6d65 5d0a  elf._dict[name].
-000119b0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000119c0: 2020 2064 6566 2064 696d 7328 7365 6c66     def dims(self
-000119d0: 293a 0a20 2020 2020 2020 2022 2222 4469  ):.        """Di
-000119e0: 6374 206f 6620 6469 6d20 6e61 6d65 7320  ct of dim names 
-000119f0: 7065 7220 7479 7065 2222 220a 2020 2020  per type""".    
-00011a00: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00011a10: 7061 7265 6e74 2e5f 6469 6374 5b27 6469  parent._dict['di
-00011a20: 6d73 275d 0a0a 2020 2020 6465 6620 7365  ms']..    def se
-00011a30: 745f 7370 6563 7328 7365 6c66 2c20 6974  t_specs(self, it
-00011a40: 656d 2c20 2a2a 7370 6563 7329 3a0a 2020  em, **specs):.  
-00011a50: 2020 2020 2020 2222 2255 7064 6174 6520        """Update 
-00011a60: 6f72 2063 7265 6174 6520 7370 6563 7320  or create specs 
-00011a70: 666f 7220 616e 2069 7465 6d22 2222 0a20  for an item""". 
-00011a80: 2020 2020 2020 2064 6174 6120 3d20 7b73         data = {s
-00011a90: 656c 662e 6361 7465 676f 7279 3a20 7b69  elf.category: {i
-00011aa0: 7465 6d3a 2073 7065 6373 7d7d 0a20 2020  tem: specs}}.   
-00011ab0: 2020 2020 2073 656c 662e 7061 7265 6e74       self.parent
-00011ac0: 2e6c 6f61 645f 6366 6728 6461 7461 290a  .load_cfg(data).
-00011ad0: 0a20 2020 2064 6566 2073 6574 5f73 7065  .    def set_spe
-00011ae0: 6373 5f66 726f 6d5f 6366 6728 7365 6c66  cs_from_cfg(self
-00011af0: 2c20 6366 6729 3a0a 2020 2020 2020 2020  , cfg):.        
-00011b00: 2222 2255 7064 6174 6520 6f72 2063 7265  """Update or cre
-00011b10: 6174 6520 7370 6563 7320 666f 7220 7365  ate specs for se
-00011b20: 7665 7261 6c20 6974 656d 2077 6974 6820  veral item with 
-00011b30: 6120 636f 6e66 6967 2073 7065 6373 2222  a config specs""
-00011b40: 220a 2020 2020 2020 2020 6966 2069 7369  ".        if isi
-00011b50: 6e73 7461 6e63 6528 6366 672c 2064 6963  nstance(cfg, dic
-00011b60: 7429 2061 6e64 2073 656c 662e 6361 7465  t) and self.cate
-00011b70: 676f 7279 206e 6f74 2069 6e20 6366 673a  gory not in cfg:
-00011b80: 0a20 2020 2020 2020 2020 2020 2063 6667  .            cfg
-00011b90: 203d 207b 7365 6c66 2e63 6174 6567 6f72   = {self.categor
-00011ba0: 793a 2063 6667 7d0a 2020 2020 2020 2020  y: cfg}.        
-00011bb0: 7365 6c66 2e70 6172 656e 742e 6c6f 6164  self.parent.load
-00011bc0: 5f63 6667 2863 6667 290a 0a20 2020 2064  _cfg(cfg)..    d
-00011bd0: 6566 2067 6574 5f61 6c6c 6f77 6564 5f6e  ef get_allowed_n
-00011be0: 616d 6573 2873 656c 662c 2063 665f 6e61  ames(self, cf_na
-00011bf0: 6d65 293a 0a20 2020 2020 2020 2022 2222  me):.        """
-00011c00: 4765 7420 7468 6520 6c69 7374 206f 6620  Get the list of 
-00011c10: 616c 6c6f 7765 6420 6e61 6d65 7320 666f  allowed names fo
-00011c20: 7220 6120 6769 7665 6e20 6063 665f 6e61  r a given `cf_na
-00011c30: 6d65 600a 0a20 2020 2020 2020 2049 7420  me`..        It 
-00011c40: 696e 636c 7564 6573 2064 6520 6063 665f  includes de `cf_
-00011c50: 6e61 6d65 6020 6974 7365 6c66 2c20 7468  name` itself, th
-00011c60: 6520 606e 616d 6560 2061 6c74 5f6e 616d  e `name` alt_nam
-00011c70: 6573 6020 7370 6563 6966 6963 6174 696f  es` specificatio
-00011c80: 6e20 7661 6c75 6573 0a0a 2020 2020 2020  n values..      
-00011c90: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00011ca0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-00011cb0: 2020 2020 2020 2020 6366 5f6e 616d 653a          cf_name:
-00011cc0: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
-00011cd0: 2056 616c 6964 2043 4620 6e61 6d65 0a0a   Valid CF name..
-00011ce0: 2020 2020 2020 2020 5265 7475 726e 0a20          Return. 
-00011cf0: 2020 2020 2020 202d 2d2d 2d2d 2d0a 2020         ------.  
-00011d00: 2020 2020 2020 6c69 7374 0a20 2020 2020        list.     
-00011d10: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-00011d20: 7065 6373 203d 2073 656c 665b 6366 5f6e  pecs = self[cf_n
-00011d30: 616d 655d 0a20 2020 2020 2020 2061 6c6c  ame].        all
-00011d40: 6f77 6564 5f6e 616d 6573 203d 205b 6366  owed_names = [cf
-00011d50: 5f6e 616d 655d 0a20 2020 2020 2020 2069  _name].        i
-00011d60: 6620 226e 616d 6522 2069 6e20 7370 6563  f "name" in spec
-00011d70: 7320 616e 6420 7370 6563 735b 226e 616d  s and specs["nam
-00011d80: 6522 5d3a 0a20 2020 2020 2020 2020 2020  e"]:.           
-00011d90: 2061 6c6c 6f77 6564 5f6e 616d 6573 2e61   allowed_names.a
-00011da0: 7070 656e 6428 7370 6563 735b 226e 616d  ppend(specs["nam
-00011db0: 6522 5d29 0a20 2020 2020 2020 2069 6620  e"]).        if 
-00011dc0: 2261 6c74 5f6e 616d 6573 2220 696e 2073  "alt_names" in s
-00011dd0: 7065 6373 3a0a 2020 2020 2020 2020 2020  pecs:.          
-00011de0: 2020 616c 6c6f 7765 645f 6e61 6d65 732e    allowed_names.
-00011df0: 6578 7465 6e64 2873 7065 6373 5b22 616c  extend(specs["al
-00011e00: 745f 6e61 6d65 7322 5d29 0a20 2020 2020  t_names"]).     
-00011e10: 2020 2072 6574 7572 6e20 616c 6c6f 7765     return allowe
-00011e20: 645f 6e61 6d65 730a 0a20 2020 2064 6566  d_names..    def
-00011e30: 2067 6574 5f6c 6f63 5f6d 6170 7069 6e67   get_loc_mapping
-00011e40: 2873 656c 662c 206f 626a 2c20 6366 5f6e  (self, obj, cf_n
-00011e50: 616d 6573 3d4e 6f6e 6529 3a0a 2020 2020  ames=None):.    
-00011e60: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00011e70: 7061 7265 6e74 2e67 6574 5f6c 6f63 5f6d  parent.get_loc_m
-00011e80: 6170 7069 6e67 280a 2020 2020 2020 2020  apping(.        
-00011e90: 2020 2020 6f62 6a2c 2063 665f 6e61 6d65      obj, cf_name
-00011ea0: 733d 6366 5f6e 616d 6573 2c20 6361 7465  s=cf_names, cate
-00011eb0: 676f 7269 6573 3d5b 2263 6f6f 7264 7322  gories=["coords"
-00011ec0: 2c20 2264 6174 615f 7661 7273 225d 0a20  , "data_vars"]. 
-00011ed0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00011ee0: 6620 5f67 6574 5f6f 7264 6572 6564 5f6d  f _get_ordered_m
-00011ef0: 6174 6368 5f73 7065 6373 5f28 7365 6c66  atch_specs_(self
-00011f00: 2c20 6366 5f6e 616d 6529 3a0a 2020 2020  , cf_name):.    
-00011f10: 2020 2020 7370 6563 7320 3d20 7365 6c66      specs = self
-00011f20: 5b63 665f 6e61 6d65 5d0a 2020 2020 2020  [cf_name].      
-00011f30: 2020 6d61 7463 685f 7370 6563 7320 3d20    match_specs = 
-00011f40: 7b7d 0a20 2020 2020 2020 2066 6f72 2073  {}.        for s
-00011f50: 6d20 696e 2073 7065 6373 5b22 7365 6172  m in specs["sear
-00011f60: 6368 5f6f 7264 6572 225d 3a0a 2020 2020  ch_order"]:.    
-00011f70: 2020 2020 2020 2020 666f 7220 6174 7472          for attr
-00011f80: 2069 6e20 280a 2020 2020 2020 2020 2020   in (.          
-00011f90: 2020 2020 2020 226e 616d 6522 2c0a 2020        "name",.  
-00011fa0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00011fb0: 7461 6e64 6172 645f 6e61 6d65 222c 0a20  tandard_name",. 
-00011fc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011fd0: 6c6f 6e67 5f6e 616d 6522 2c0a 2020 2020  long_name",.    
-00011fe0: 2020 2020 2020 2020 2020 2020 2261 7869              "axi
-00011ff0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00012000: 2020 2020 2275 6e69 7473 222c 0a20 2020      "units",.   
-00012010: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
-00012020: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00012030: 7474 725b 305d 2021 3d20 736d 3a0a 2020  ttr[0] != sm:.  
-00012040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012050: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-00012060: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
-00012070: 6174 7472 203d 3d20 226e 616d 6522 2061  attr == "name" a
-00012080: 6e64 2022 6e61 6d65 2220 696e 2073 7065  nd "name" in spe
-00012090: 6373 3a0a 2020 2020 2020 2020 2020 2020  cs:.            
-000120a0: 2020 2020 6966 2061 7474 7220 3d3d 2022      if attr == "
-000120b0: 6e61 6d65 223a 0a20 2020 2020 2020 2020  name":.         
-000120c0: 2020 2020 2020 2020 2020 206d 6174 6368             match
-000120d0: 5f73 7065 6373 5b22 6e61 6d65 225d 203d  _specs["name"] =
-000120e0: 2073 656c 662e 6765 745f 616c 6c6f 7765   self.get_allowe
-000120f0: 645f 6e61 6d65 7328 6366 5f6e 616d 6529  d_names(cf_name)
-00012100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012110: 2065 6c69 6620 2261 7474 7273 2220 696e   elif "attrs" in
-00012120: 2073 7065 6373 2061 6e64 2061 7474 7220   specs and attr 
-00012130: 696e 2073 7065 6373 5b22 6174 7472 7322  in specs["attrs"
-00012140: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00012150: 2020 2020 2020 206d 6174 6368 5f73 7065         match_spe
-00012160: 6373 5b61 7474 725d 203d 2073 7065 6373  cs[attr] = specs
-00012170: 5b22 6174 7472 7322 5d5b 6174 7472 5d0a  ["attrs"][attr].
-00012180: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-00012190: 6174 6368 5f73 7065 6373 0a0a 2020 2020  atch_specs..    
-000121a0: 6465 6620 6d61 7463 6828 7365 6c66 2c20  def match(self, 
-000121b0: 6461 2c20 6366 5f6e 616d 653d 4e6f 6e65  da, cf_name=None
-000121c0: 2c20 6c6f 633d 4e6f 6e65 293a 0a20 2020  , loc=None):.   
-000121d0: 2020 2020 2022 2222 4368 6563 6b20 6966       """Check if
-000121e0: 2064 6120 6174 7472 6962 7574 6573 206d   da attributes m
-000121f0: 6174 6368 2067 6976 656e 206f 7220 616e  atch given or an
-00012200: 7920 7370 6563 730a 0a20 2020 2020 2020  y specs..       
-00012210: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00012220: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00012230: 2020 2020 2020 2064 613a 2078 6172 7261         da: xarra
-00012240: 792e 4461 7461 4172 7261 790a 2020 2020  y.DataArray.    
-00012250: 2020 2020 6366 5f6e 616d 653a 2073 7472      cf_name: str
-00012260: 2c20 6469 6374 2c20 4e6f 6e65 0a20 2020  , dict, None.   
-00012270: 2020 2020 2020 2020 2043 4620 6e61 6d65           CF name
-00012280: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
-00012290: 204e 6f6e 652c 2061 6c6c 206e 616d 6573   None, all names
-000122a0: 2061 7265 2075 7365 642e 0a20 2020 2020   are used..     
-000122b0: 2020 2020 2020 2049 6620 6120 6469 6374         If a dict
-000122c0: 2c20 6e61 6d65 2069 7320 696e 7465 7270  , name is interp
-000122d0: 7265 7465 6420 6173 2061 6e20 6578 706c  reted as an expl
-000122e0: 6963 6974 2073 6574 206f 660a 2020 2020  icit set of.    
-000122f0: 2020 2020 2020 2020 7370 6563 6966 6963          specific
-00012300: 6174 696f 6e73 2e0a 2020 2020 2020 2020  ations..        
-00012310: 6c6f 633a 2073 7472 2c20 7b22 616e 7922  loc: str, {"any"
-00012320: 2c20 4e6f 6e65 7d2c 207b 2222 2c20 4661  , None}, {"", Fa
-00012330: 6c73 657d 0a20 2020 2020 2020 2020 2020  lse}.           
-00012340: 202d 2073 7472 3a20 6f6e 6520 6f66 2074   - str: one of t
-00012350: 6865 7365 206c 6f63 6174 696f 6e73 0a20  hese locations. 
-00012360: 2020 2020 2020 2020 2020 202d 204e 6f6e             - Non
-00012370: 6520 6f72 2022 616e 7922 3a20 616e 790a  e or "any": any.
-00012380: 2020 2020 2020 2020 2020 2020 2d20 4661              - Fa
-00012390: 6c73 6520 6f72 2027 2222 3a20 6e6f 206c  lse or '"": no l
-000123a0: 6f63 6174 696f 6e0a 0a20 2020 2020 2020  ocation..       
-000123b0: 2052 6574 7572 6e0a 2020 2020 2020 2020   Return.        
-000123c0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2062  ------.        b
-000123d0: 6f6f 6c2c 2073 7472 0a20 2020 2020 2020  ool, str.       
-000123e0: 2020 2020 2054 7275 6520 6f72 2046 616c       True or Fal
-000123f0: 7365 2069 6620 6e61 6d65 2069 7320 7072  se if name is pr
-00012400: 6f76 6964 6564 2c20 656c 7365 2066 6f75  ovided, else fou
-00012410: 6e64 206e 616d 6520 6f72 204e 6f6e 650a  nd name or None.
-00012420: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012430: 2020 2020 6966 2063 665f 6e61 6d65 3a0a      if cf_name:.
-00012440: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00012450: 7369 6e73 7461 6e63 6528 6366 5f6e 616d  sinstance(cf_nam
-00012460: 652c 2073 7472 293a 0a20 2020 2020 2020  e, str):.       
-00012470: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
-00012480: 7373 6572 745f 6b6e 6f77 6e5f 2863 665f  ssert_known_(cf_
-00012490: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
-000124a0: 2020 6e61 6d65 7320 3d20 5b63 665f 6e61    names = [cf_na
-000124b0: 6d65 5d0a 2020 2020 2020 2020 656c 7365  me].        else
-000124c0: 3a0a 2020 2020 2020 2020 2020 2020 6e61  :.            na
-000124d0: 6d65 7320 3d20 7365 6c66 2e6e 616d 6573  mes = self.names
-000124e0: 0a20 2020 2020 2020 2066 6f72 206e 616d  .        for nam
-000124f0: 655f 2069 6e20 6e61 6d65 733a 0a0a 2020  e_ in names:..  
-00012500: 2020 2020 2020 2020 2020 2320 4765 7420            # Get 
-00012510: 6d61 7463 6820 7370 6563 730a 2020 2020  match specs.    
-00012520: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00012530: 7461 6e63 6528 6e61 6d65 5f2c 2064 6963  tance(name_, dic
-00012540: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00012550: 2020 2020 6d61 7463 685f 7370 6563 7320      match_specs 
-00012560: 3d20 6e61 6d65 5f0a 2020 2020 2020 2020  = name_.        
-00012570: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00012580: 2020 2020 2020 2020 2020 6d61 7463 685f            match_
-00012590: 7370 6563 7320 3d20 7365 6c66 2e5f 6765  specs = self._ge
-000125a0: 745f 6f72 6465 7265 645f 6d61 7463 685f  t_ordered_match_
-000125b0: 7370 6563 735f 286e 616d 655f 290a 0a20  specs_(name_).. 
-000125c0: 2020 2020 2020 2020 2020 2023 204c 6f6f             # Loo
-000125d0: 7020 6f6e 206d 6174 6368 2073 7065 6373  p on match specs
-000125e0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000125f0: 2061 7474 722c 2072 6566 7320 696e 206d   attr, refs in m
-00012600: 6174 6368 5f73 7065 6373 2e69 7465 6d73  atch_specs.items
-00012610: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00012620: 2020 2020 7661 6c75 6520 3d20 6765 7461      value = geta
-00012630: 7474 7228 6461 2c20 6174 7472 2c20 4e6f  ttr(da, attr, No
-00012640: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-00012650: 2020 2020 6966 2076 616c 7565 2069 7320      if value is 
-00012660: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00012670: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00012680: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00012690: 2020 2066 6f72 2072 6566 2069 6e20 7265     for ref in re
-000126a0: 6673 3a0a 2020 2020 2020 2020 2020 2020  fs:.            
-000126b0: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126d0: 2020 2020 2061 7474 7220 696e 2073 656c       attr in sel
-000126e0: 662e 7367 6c6f 6361 746f 722e 7661 6c69  f.sglocator.vali
-000126f0: 645f 6174 7472 730a 2020 2020 2020 2020  d_attrs.        
-00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012710: 616e 6420 7365 6c66 2e73 676c 6f63 6174  and self.sglocat
-00012720: 6f72 2e6d 6174 6368 5f61 7474 7228 6174  or.match_attr(at
-00012730: 7472 2c20 7661 6c75 652c 2072 6566 2c20  tr, value, ref, 
-00012740: 6c6f 633d 6c6f 6329 0a20 2020 2020 2020  loc=loc).       
-00012750: 2020 2020 2020 2020 2020 2020 2029 206f               ) o
-00012760: 7220 6d61 7463 685f 7374 7269 6e67 2876  r match_string(v
-00012770: 616c 7565 2c20 7265 662c 2069 676e 6f72  alue, ref, ignor
-00012780: 6563 6173 653d 5472 7565 293a 0a20 2020  ecase=True):.   
-00012790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127a0: 2020 2020 2064 612e 656e 636f 6469 6e67       da.encoding
-000127b0: 5b22 6366 5f6e 616d 6522 5d20 3d20 6e61  ["cf_name"] = na
-000127c0: 6d65 5f0a 2020 2020 2020 2020 2020 2020  me_.            
-000127d0: 2020 2020 2020 2020 2020 2020 6461 2e65              da.e
-000127e0: 6e63 6f64 696e 675b 2263 665f 6361 7465  ncoding["cf_cate
-000127f0: 676f 7279 225d 203d 2073 656c 662e 6361  gory"] = self.ca
-00012800: 7465 676f 7279 0a20 2020 2020 2020 2020  tegory.         
-00012810: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00012820: 6574 7572 6e20 5472 7565 2069 6620 6366  eturn True if cf
-00012830: 5f6e 616d 6520 656c 7365 206e 616d 655f  _name else name_
-00012840: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012850: 4661 6c73 6520 6966 2063 665f 6e61 6d65  False if cf_name
-00012860: 2065 6c73 6520 4e6f 6e65 0a0a 2020 2020   else None..    
-00012870: 6465 6620 6d61 7463 685f 6672 6f6d 5f6e  def match_from_n
-00012880: 616d 6528 7365 6c66 2c20 6e61 6d65 2c20  ame(self, name, 
-00012890: 6366 5f6e 616d 653d 4e6f 6e65 2c20 6c6f  cf_name=None, lo
-000128a0: 633d 4e6f 6e65 293a 0a20 2020 2020 2020  c=None):.       
-000128b0: 2022 2222 4765 7420 7468 6520 6765 6e65   """Get the gene
-000128c0: 7269 6320 4346 206e 616d 6520 6f66 2061  ric CF name of a
-000128d0: 6e20 6f62 6a65 6374 206b 6e6f 7769 6e67  n object knowing
-000128e0: 206f 6e6c 7920 6974 7320 6e61 6d65 0a0a   only its name..
-000128f0: 2020 2020 2020 2020 4974 2063 6f6d 7061          It compa
-00012900: 7265 7320 606e 616d 6560 2074 6f20 7468  res `name` to th
-00012910: 6520 606e 616d 6560 2061 6e64 2060 616c  e `name` and `al
-00012920: 745f 6e61 6d65 7360 2063 6f6e 6669 6720  t_names` config 
-00012930: 7661 6c75 6573 2e0a 0a20 2020 2020 2020  values...       
-00012940: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00012950: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00012960: 2020 2020 2020 206e 616d 653a 2073 7472         name: str
-00012970: 0a20 2020 2020 2020 2020 2020 2041 6374  .            Act
-00012980: 7561 6c20 6e61 6d65 0a20 2020 2020 2020  ual name.       
-00012990: 2063 665f 6e61 6d65 3a20 7374 722c 204e   cf_name: str, N
-000129a0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-000129b0: 4120 7461 7267 6574 2067 656e 6572 6963  A target generic
-000129c0: 2043 4620 6e61 6d65 2e20 4966 206e 6f74   CF name. If not
-000129d0: 2070 726f 7669 6465 642c 2061 6c6c 2069   provided, all i
-000129e0: 7465 6d73 2061 7265 2063 6f6e 7369 6465  tems are conside
-000129f0: 7265 642e 0a0a 2020 2020 2020 2020 5265  red...        Re
-00012a00: 7475 726e 0a20 2020 2020 2020 202d 2d2d  turn.        ---
-00012a10: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-00012a20: 2c20 7374 722c 2054 7275 652c 2046 616c  , str, True, Fal
-00012a30: 7365 0a20 2020 2020 2020 2020 2020 2049  se.            I
-00012a40: 6620 6063 665f 6e61 6d65 6020 6973 2070  f `cf_name` is p
-00012a50: 726f 7669 6465 642c 2072 6574 7572 6e73  rovided, returns
-00012a60: 2061 2062 6f6f 6c65 616e 2c20 656c 7365   a boolean, else
-00012a70: 2072 6574 7572 6e73 0a20 2020 2020 2020   returns.       
-00012a80: 2020 2020 2074 6865 206d 6174 6368 696e       the matchin
-00012a90: 6720 4346 206e 616d 6520 6f72 204e 6f6e  g CF name or Non
-00012aa0: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00012ab0: 2020 2020 2020 2065 7870 6c69 6369 7420         explicit 
-00012ac0: 3d20 6366 5f6e 616d 6520 6973 206e 6f74  = cf_name is not
-00012ad0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-00012ae0: 2063 665f 6e61 6d65 3a0a 2020 2020 2020   cf_name:.      
-00012af0: 2020 2020 2020 7365 6c66 2e5f 6173 7365        self._asse
-00012b00: 7274 5f6b 6e6f 776e 5f28 6366 5f6e 616d  rt_known_(cf_nam
-00012b10: 6529 0a20 2020 2020 2020 2020 2020 2063  e).            c
-00012b20: 665f 6e61 6d65 7320 3d20 5b63 665f 6e61  f_names = [cf_na
-00012b30: 6d65 5d0a 2020 2020 2020 2020 656c 7365  me].        else
-00012b40: 3a0a 2020 2020 2020 2020 2020 2020 6366  :.            cf
-00012b50: 5f6e 616d 6573 203d 2073 656c 662e 6e61  _names = self.na
-00012b60: 6d65 730a 0a20 2020 2020 2020 2066 6f72  mes..        for
-00012b70: 2063 665f 6e61 6d65 2069 6e20 6366 5f6e   cf_name in cf_n
-00012b80: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
-00012b90: 2020 666f 7220 616c 6c6f 7765 645f 6e61    for allowed_na
-00012ba0: 6d65 2069 6e20 7365 6c66 2e67 6574 5f61  me in self.get_a
-00012bb0: 6c6c 6f77 6564 5f6e 616d 6573 2863 665f  llowed_names(cf_
-00012bc0: 6e61 6d65 293a 0a20 2020 2020 2020 2020  name):.         
-00012bd0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00012be0: 676c 6f63 6174 6f72 2e6d 6174 6368 5f61  glocator.match_a
-00012bf0: 7474 7228 226e 616d 6522 2c20 6e61 6d65  ttr("name", name
-00012c00: 2c20 616c 6c6f 7765 645f 6e61 6d65 2c20  , allowed_name, 
-00012c10: 6c6f 633d 6c6f 6329 3a0a 2020 2020 2020  loc=loc):.      
-00012c20: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00012c30: 7475 726e 2063 665f 6e61 6d65 2069 6620  turn cf_name if 
-00012c40: 6e6f 7420 6578 706c 6963 6974 2065 6c73  not explicit els
-00012c50: 6520 5472 7565 0a20 2020 2020 2020 2072  e True.        r
-00012c60: 6574 7572 6e20 4e6f 6e65 2069 6620 6e6f  eturn None if no
-00012c70: 7420 6578 706c 6963 6974 2065 6c73 6520  t explicit else 
-00012c80: 4661 6c73 650a 0a20 2020 2040 4552 524f  False..    @ERRO
-00012c90: 5253 2e66 6f72 6d61 745f 6d65 7468 6f64  RS.format_method
-00012ca0: 5f64 6f63 7374 7269 6e67 0a20 2020 2064  _docstring.    d
-00012cb0: 6566 2073 6561 7263 6828 7365 6c66 2c20  ef search(self, 
-00012cc0: 6f62 6a2c 2063 665f 6e61 6d65 3d4e 6f6e  obj, cf_name=Non
-00012cd0: 652c 206c 6f63 3d4e 6f6e 652c 2067 6574  e, loc=None, get
-00012ce0: 3d22 6f62 6a22 2c20 7369 6e67 6c65 3d54  ="obj", single=T
-00012cf0: 7275 652c 2065 7272 6f72 733d 2272 6169  rue, errors="rai
-00012d00: 7365 2229 3a0a 2020 2020 2020 2020 2222  se"):.        ""
-00012d10: 2253 6561 7263 6820 666f 7220 6120 6461  "Search for a da
-00012d20: 7461 5f76 6172 206f 7220 636f 6f72 6420  ta_var or coord 
-00012d30: 7468 6174 206d 6163 6865 7320 6769 7665  that maches give
-00012d40: 6e20 6f72 2061 6e79 2073 7065 6373 0a0a  n or any specs..
-00012d50: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00012d60: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00012d70: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6f62  -----.        ob
-00012d80: 6a3a 2044 6174 6141 7272 6179 206f 7220  j: DataArray or 
-00012d90: 4461 7461 7365 740a 2020 2020 2020 2020  Dataset.        
-00012da0: 6366 5f6e 616d 653a 2073 7472 2c20 6469  cf_name: str, di
-00012db0: 6374 0a20 2020 2020 2020 2020 2020 2041  ct.            A
-00012dc0: 2067 656e 6572 6963 2043 4620 6e61 6d65   generic CF name
-00012dd0: 2e20 4966 206e 6f74 2070 726f 7669 6465  . If not provide
-00012de0: 642c 2061 6c6c 2043 4620 6e61 6d65 7320  d, all CF names 
-00012df0: 6172 6520 7363 616e 6564 2e0a 2020 2020  are scaned..    
-00012e00: 2020 2020 6c6f 633a 2073 7472 2c20 7b7b      loc: str, {{
-00012e10: 2261 6e79 222c 204e 6f6e 657d 7d2c 207b  "any", None}}, {
-00012e20: 7b22 222c 2046 616c 7365 7d7d 0a20 2020  {"", False}}.   
-00012e30: 2020 2020 2020 2020 202d 2073 7472 3a20           - str: 
-00012e40: 6f6e 6520 6f66 2074 6865 7365 206c 6f63  one of these loc
-00012e50: 6174 696f 6e73 0a20 2020 2020 2020 2020  ations.         
-00012e60: 2020 202d 204e 6f6e 6520 6f72 2022 616e     - None or "an
-00012e70: 7922 3a20 616e 790a 2020 2020 2020 2020  y": any.        
-00012e80: 2020 2020 2d20 4661 6c73 6520 6f72 2027      - False or '
-00012e90: 2222 3a20 6e6f 206c 6f63 6174 696f 6e0a  "": no location.
-00012ea0: 2020 2020 2020 2020 6765 743a 207b 7b22          get: {{"
-00012eb0: 6f62 6a22 2c20 2263 665f 6e61 6d65 222c  obj", "cf_name",
-00012ec0: 2022 626f 7468 227d 7d0a 2020 2020 2020   "both"}}.      
-00012ed0: 2020 2020 2020 5768 656e 2066 6f75 6e64        When found
-00012ee0: 2c20 6765 7420 7468 6520 6f62 6a65 6374  , get the object
-00012ef0: 2066 6f75 6e64 206f 7220 6974 7320 6e61   found or its na
-00012f00: 6d65 2e0a 2020 2020 2020 2020 7369 6e67  me..        sing
-00012f10: 6c65 3a20 626f 6f6c 0a20 2020 2020 2020  le: bool.       
-00012f20: 2020 2020 2049 6620 5472 7565 2c20 7265       If True, re
-00012f30: 7475 726e 2074 6865 2066 6972 7374 2069  turn the first i
-00012f40: 7465 6d20 666f 756e 6420 6f72 204e 6f6e  tem found or Non
-00012f50: 652e 0a20 2020 2020 2020 2020 2020 2049  e..            I
-00012f60: 6620 4661 6c73 652c 2072 6574 7572 6e20  f False, return 
-00012f70: 6120 706f 7373 6962 6c65 2065 6d70 7479  a possible empty
-00012f80: 206c 6973 7420 6f66 2066 6f75 6e64 2069   list of found i
-00012f90: 7465 6d73 2e0a 2020 2020 2020 2020 2020  tems..          
-00012fa0: 2020 4120 7761 726e 696e 6720 6973 2065    A warning is e
-00012fb0: 6d69 7474 6564 2077 6865 6e20 7365 7420  mitted when set 
-00012fc0: 746f 2054 7275 6520 616e 6420 6d75 6c74  to True and mult
-00012fd0: 6970 6c65 2069 7465 6d20 6172 6520 666f  iple item are fo
-00012fe0: 756e 642e 0a20 2020 2020 2020 207b 6572  und..        {er
-00012ff0: 726f 7273 7d0a 0a20 2020 2020 2020 2052  rors}..        R
-00013000: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00013010: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
-00013020: 6f6e 6520 6f72 2073 7472 206f 7220 6f62  one or str or ob
-00013030: 6a65 6374 0a20 2020 2020 2020 2022 2222  ject.        """
-00013040: 0a0a 2020 2020 2020 2020 2320 4765 7420  ..        # Get 
-00013050: 7461 7267 6574 206f 626a 6563 7473 0a20  target objects. 
-00013060: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00013070: 6174 6567 6f72 7920 616e 6420 6861 7361  ategory and hasa
-00013080: 7474 7228 6f62 6a2c 2073 656c 662e 6361  ttr(obj, self.ca
-00013090: 7465 676f 7279 293a 0a20 2020 2020 2020  tegory):.       
-000130a0: 2020 2020 206e 616d 6573 203d 2067 6574       names = get
-000130b0: 6174 7472 286f 626a 2c20 7365 6c66 2e63  attr(obj, self.c
-000130c0: 6174 6567 6f72 7929 0a20 2020 2020 2020  ategory).       
-000130d0: 2020 2020 206b 7720 3d20 6469 6374 2864       kw = dict(d
-000130e0: 6174 615f 7661 7273 3d46 616c 7365 2c20  ata_vars=False, 
-000130f0: 636f 6f72 6473 3d46 616c 7365 2c20 6469  coords=False, di
-00013100: 6d73 3d46 616c 7365 290a 2020 2020 2020  ms=False).      
-00013110: 2020 2020 2020 6b77 5b73 656c 662e 6361        kw[self.ca
-00013120: 7465 676f 7279 5d20 3d20 5472 7565 0a20  tegory] = True. 
-00013130: 2020 2020 2020 2020 2020 206e 616d 6573             names
-00013140: 203d 205f 6c69 7374 5f78 725f 6e61 6d65   = _list_xr_name
-00013150: 735f 286f 626a 2c20 2a2a 6b77 290a 2020  s_(obj, **kw).  
-00013160: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00013170: 2020 2020 2020 2020 6e61 6d65 7320 3d20          names = 
-00013180: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00013190: 2020 6c69 7374 286f 626a 290a 2020 2020    list(obj).    
-000131a0: 2020 2020 2020 2020 2020 2020 6966 2068              if h
-000131b0: 6173 6174 7472 286f 626a 2c20 226b 6579  asattr(obj, "key
-000131c0: 7322 290a 2020 2020 2020 2020 2020 2020  s").            
-000131d0: 2020 2020 656c 7365 205f 6c69 7374 5f78      else _list_x
-000131e0: 725f 6e61 6d65 735f 286f 626a 2c20 6461  r_names_(obj, da
-000131f0: 7461 5f76 6172 733d 4661 6c73 652c 2064  ta_vars=False, d
-00013200: 696d 733d 4661 6c73 6529 0a20 2020 2020  ims=False).     
-00013210: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00013220: 2020 2320 4765 7420 6d61 7463 6820 7370    # Get match sp
-00013230: 6563 730a 2020 2020 2020 2020 6966 2063  ecs.        if c
-00013240: 665f 6e61 6d65 3a20 2023 2045 7870 6c69  f_name:  # Expli
-00013250: 6369 7420 6e61 6d65 2073 6f20 7765 206c  cit name so we l
-00013260: 6f6f 7020 6f6e 2073 6561 7263 6820 7370  oop on search sp
-00013270: 6563 730a 2020 2020 2020 2020 2020 2020  ecs.            
-00013280: 6966 2069 7369 6e73 7461 6e63 6528 6366  if isinstance(cf
-00013290: 5f6e 616d 652c 2073 7472 293a 0a20 2020  _name, str):.   
-000132a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000132b0: 6e6f 7420 7365 6c66 2e5f 6173 7365 7274  not self._assert
-000132c0: 5f6b 6e6f 776e 5f28 6366 5f6e 616d 652c  _known_(cf_name,
-000132d0: 2065 7272 6f72 7329 3a0a 2020 2020 2020   errors):.      
-000132e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000132f0: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00013300: 206d 6174 6368 5f73 7065 6373 203d 205b   match_specs = [
-00013310: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-00013320: 7220 6174 7472 2c20 7265 6673 2069 6e20  r attr, refs in 
-00013330: 7365 6c66 2e5f 6765 745f 6f72 6465 7265  self._get_ordere
-00013340: 645f 6d61 7463 685f 7370 6563 735f 2863  d_match_specs_(c
-00013350: 665f 6e61 6d65 292e 6974 656d 7328 293a  f_name).items():
-00013360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013370: 206d 6174 6368 5f73 7065 6373 2e61 7070   match_specs.app
-00013380: 656e 6428 7b61 7474 723a 2072 6566 737d  end({attr: refs}
-00013390: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-000133a0: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
-000133b0: 685f 7370 6563 7320 3d20 5b4e 6f6e 655d  h_specs = [None]
-000133c0: 0a0a 2020 2020 2020 2020 2320 4c6f 6f70  ..        # Loop
-000133d0: 730a 2020 2020 2020 2020 6173 7365 7274  s.        assert
-000133e0: 2067 6574 2069 6e20 280a 2020 2020 2020   get in (.      
-000133f0: 2020 2020 2020 2263 665f 6e61 6d65 222c        "cf_name",
-00013400: 0a20 2020 2020 2020 2020 2020 2022 6f62  .            "ob
-00013410: 6a22 2c0a 2020 2020 2020 2020 2020 2020  j",.            
-00013420: 2262 6f74 6822 2c0a 2020 2020 2020 2020  "both",.        
-00013430: 292c 2066 2227 6765 7427 206d 7573 7420  ), f"'get' must 
-00013440: 6265 2065 6974 6865 7220 2763 665f 6e61  be either 'cf_na
-00013450: 6d65 2720 6f72 2027 6f62 6a27 206f 7220  me' or 'obj' or 
-00013460: 2762 6f74 6827 2c20 4e4f 5420 277b 6765  'both', NOT '{ge
-00013470: 747d 2722 0a20 2020 2020 2020 2066 6f75  t}'".        fou
-00013480: 6e64 203d 205b 5d0a 2020 2020 2020 2020  nd = [].        
-00013490: 666f 756e 645f 6f62 6a73 203d 205b 5d0a  found_objs = [].
-000134a0: 2020 2020 2020 2020 666f 7220 6d61 7463          for matc
-000134b0: 685f 6172 6720 696e 206d 6174 6368 5f73  h_arg in match_s
-000134c0: 7065 6373 3a0a 2020 2020 2020 2020 2020  pecs:.          
-000134d0: 2020 2320 666f 7220 6f62 6a20 696e 206f    # for obj in o
-000134e0: 626a 732e 7661 6c75 6573 2829 3a0a 2020  bjs.values():.  
-000134f0: 2020 2020 2020 2020 2020 666f 7220 7468            for th
-00013500: 6973 5f6e 616d 6520 696e 206e 616d 6573  is_name in names
-00013510: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013520: 2020 7468 6973 5f6f 626a 203d 206f 626a    this_obj = obj
-00013530: 5b74 6869 735f 6e61 6d65 5d0a 2020 2020  [this_name].    
-00013540: 2020 2020 2020 2020 2020 2020 6d20 3d20              m = 
-00013550: 7365 6c66 2e6d 6174 6368 2874 6869 735f  self.match(this_
-00013560: 6f62 6a2c 206d 6174 6368 5f61 7267 2c20  obj, match_arg, 
-00013570: 6c6f 633d 6c6f 6329 0a20 2020 2020 2020  loc=loc).       
-00013580: 2020 2020 2020 2020 2069 6620 6d3a 0a20           if m:. 
-00013590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135a0: 2020 2023 2069 6620 6f62 6a2e 6e61 6d65     # if obj.name
-000135b0: 2069 6e20 666f 756e 645f 6f62 6a73 3a0a   in found_objs:.
-000135c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135d0: 2020 2020 6966 2074 6869 735f 6e61 6d65      if this_name
-000135e0: 2069 6e20 666f 756e 645f 6f62 6a73 3a0a   in found_objs:.
+0000d0d0: 2020 2072 656e 616d 655f 6172 6773 5b6e     rename_args[n
+0000d0e0: 616d 655d 203d 2073 656c 662e 7367 6c6f  ame] = self.sglo
+0000d0f0: 6361 746f 722e 666f 726d 6174 5f61 7474  cator.format_att
+0000d100: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+0000d110: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
+0000d120: 222c 2072 6f6f 745f 6e61 6d65 2c20 6c6f  ", root_name, lo
+0000d130: 6373 5b72 6f6f 745f 6e61 6d65 5d0a 2020  cs[root_name].  
+0000d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d150: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+0000d160: 726e 206f 626a 2e72 656e 616d 6528 7265  rn obj.rename(re
+0000d170: 6e61 6d65 5f61 7267 7329 0a0a 2020 2020  name_args)..    
+0000d180: 6465 6620 7265 6c6f 6328 7365 6c66 2c20  def reloc(self, 
+0000d190: 6f62 6a2c 202a 2a6c 6f63 7329 3a0a 2020  obj, **locs):.  
+0000d1a0: 2020 2020 2020 2222 2243 6f6e 7665 7274        """Convert
+0000d1b0: 2067 6976 656e 2073 7461 6767 6572 6564   given staggered
+0000d1c0: 2067 7269 6420 6c6f 6361 7469 6f6e 7320   grid locations 
+0000d1d0: 746f 206f 7468 6572 206c 6f63 6174 696f  to other locatio
+0000d1e0: 6e73 0a0a 2020 2020 2020 2020 2e2e 206e  ns..        .. n
+0000d1f0: 6f74 653a 3a20 4974 206f 6e6c 7920 6368  ote:: It only ch
+0000d200: 616e 6765 7320 7468 6520 6e61 6d65 732c  anges the names,
+0000d210: 206e 6f74 2074 6865 2061 7474 7269 6275   not the attribu
+0000d220: 7465 732e 0a0a 2020 2020 2020 2020 5061  tes...        Pa
+0000d230: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0000d240: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000d250: 2020 2020 6f62 6a3a 2078 6172 7261 792e      obj: xarray.
+0000d260: 4461 7461 7365 742c 2078 6172 7261 792e  Dataset, xarray.
+0000d270: 4461 7461 4172 7261 790a 2020 2020 2020  DataArray.      
+0000d280: 2020 6c6f 6373 3a20 6469 6374 0a20 2020    locs: dict.   
+0000d290: 2020 2020 2020 2020 202a 2a4b 6579 7320           **Keys 
+0000d2a0: 6172 6520 6c6f 6361 7469 6f6e 732a 2a2c  are locations**,
+0000d2b0: 2076 616c 7565 7320 6172 6520 6e65 7720   values are new 
+0000d2c0: 6c6f 6361 7469 6f6e 732e 0a20 2020 2020  locations..     
+0000d2d0: 2020 2020 2020 2041 2076 616c 7565 206f         A value o
+0000d2e0: 6620 6046 616c 7365 6020 6f72 2060 4e6f  f `False` or `No
+0000d2f0: 6e65 602c 2072 656d 6f76 6520 7468 6520  ne`, remove the 
+0000d300: 6c6f 6361 7469 6f6e 2e0a 0a20 2020 2020  location...     
+0000d310: 2020 2052 6574 7572 6e0a 2020 2020 2020     Return.      
+0000d320: 2020 2d2d 2d2d 2d2d 0a20 2020 2020 2020    ------.       
+0000d330: 2078 6172 7261 792e 4461 7461 7365 742c   xarray.Dataset,
+0000d340: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
+0000d350: 790a 0a20 2020 2020 2020 2053 6565 2061  y..        See a
+0000d360: 6c73 6f0a 2020 2020 2020 2020 2d2d 2d2d  lso.        ----
+0000d370: 2d2d 2d2d 0a20 2020 2020 2020 2074 6f5f  ----.        to_
+0000d380: 6c6f 630a 2020 2020 2020 2020 7367 6c6f  loc.        sglo
+0000d390: 6361 746f 720a 2020 2020 2020 2020 5347  cator.        SG
+0000d3a0: 4c6f 6361 746f 722e 666f 726d 6174 5f61  Locator.format_a
+0000d3b0: 7474 720a 2020 2020 2020 2020 2222 220a  ttr.        """.
+0000d3c0: 2020 2020 2020 2020 7265 6e61 6d65 5f61          rename_a
+0000d3d0: 7267 7320 3d20 7b7d 0a20 2020 2020 2020  rgs = {}.       
+0000d3e0: 206e 616d 6573 203d 205f 6c69 7374 5f78   names = _list_x
+0000d3f0: 725f 6e61 6d65 735f 286f 626a 290a 2020  r_names_(obj).  
+0000d400: 2020 2020 2020 2320 6e61 6d65 7320 3d20        # names = 
+0000d410: 7365 7428 6f62 6a2e 6469 6d73 292e 756e  set(obj.dims).un
+0000d420: 696f 6e28 6f62 6a2e 636f 6f72 6473 290a  ion(obj.coords).
+0000d430: 2020 2020 2020 2020 2320 6966 2068 6173          # if has
+0000d440: 6174 7472 286f 626a 2c20 2264 6174 615f  attr(obj, "data_
+0000d450: 7661 7273 2229 3a0a 2020 2020 2020 2020  vars"):.        
+0000d460: 2320 2020 2020 6e61 6d65 7320 3d20 6e61  #     names = na
+0000d470: 6d65 732e 756e 696f 6e28 6f62 6a2e 6461  mes.union(obj.da
+0000d480: 7461 5f76 6172 7329 0a20 2020 2020 2020  ta_vars).       
+0000d490: 2066 6f72 206e 616d 6520 696e 206e 616d   for name in nam
+0000d4a0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0000d4b0: 6966 206e 616d 6520 6e6f 7420 696e 2072  if name not in r
+0000d4c0: 656e 616d 655f 6172 6773 3a0a 2020 2020  ename_args:.    
+0000d4d0: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+0000d4e0: 5f6e 616d 652c 206f 6c64 5f6c 6f63 203d  _name, old_loc =
+0000d4f0: 2073 656c 662e 7367 6c6f 6361 746f 722e   self.sglocator.
+0000d500: 7061 7273 655f 6174 7472 2822 6e61 6d65  parse_attr("name
+0000d510: 222c 206e 616d 6529 0a20 2020 2020 2020  ", name).       
+0000d520: 2020 2020 2020 2020 2069 6620 6f6c 645f           if old_
+0000d530: 6c6f 6320 616e 6420 6f6c 645f 6c6f 6320  loc and old_loc 
+0000d540: 696e 206c 6f63 733a 0a20 2020 2020 2020  in locs:.       
+0000d550: 2020 2020 2020 2020 2020 2020 2072 656e               ren
+0000d560: 616d 655f 6172 6773 5b6e 616d 655d 203d  ame_args[name] =
+0000d570: 2073 656c 662e 7367 6c6f 6361 746f 722e   self.sglocator.
+0000d580: 666f 726d 6174 5f61 7474 7228 226e 616d  format_attr("nam
+0000d590: 6522 2c20 726f 6f74 5f6e 616d 652c 206c  e", root_name, l
+0000d5a0: 6f63 735b 6f6c 645f 6c6f 635d 290a 0a20  ocs[old_loc]).. 
+0000d5b0: 2020 2020 2020 2072 6574 7572 6e20 6f62         return ob
+0000d5c0: 6a2e 7265 6e61 6d65 2872 656e 616d 655f  j.rename(rename_
+0000d5d0: 6172 6773 290a 0a20 2020 2064 6566 2066  args)..    def f
+0000d5e0: 696c 6c5f 6174 7472 7328 7365 6c66 2c20  ill_attrs(self, 
+0000d5f0: 6f62 6a2c 202a 2a6b 7761 7267 7329 3a0a  obj, **kwargs):.
+0000d600: 2020 2020 2020 2020 2222 2246 696c 6c20          """Fill 
+0000d610: 6d69 7373 696e 6720 6174 7472 6962 7574  missing attribut
+0000d620: 6573 206f 6620 6120 7861 7272 6179 2e44  es of a xarray.D
+0000d630: 6174 6173 6574 206f 7220 7861 7272 6179  ataset or xarray
+0000d640: 2e44 6174 6141 7272 6179 0a0a 2020 2020  .DataArray..    
+0000d650: 2020 2020 2e2e 206e 6f74 653a 3a20 4974      .. note:: It
+0000d660: 2064 6f65 7320 6e6f 7420 7265 6e61 6d65   does not rename
+0000d670: 2061 6e79 7468 696e 670a 0a20 2020 2020   anything..     
+0000d680: 2020 2053 6565 2061 6c73 6f0a 2020 2020     See also.    
+0000d690: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0000d6a0: 2020 2020 2066 6f72 6d61 745f 6461 7461       format_data
+0000d6b0: 6172 7261 790a 2020 2020 2020 2020 666f  array.        fo
+0000d6c0: 726d 6174 5f64 6174 6173 6574 0a20 2020  rmat_dataset.   
+0000d6d0: 2020 2020 2061 7574 6f5f 666f 726d 6174       auto_format
+0000d6e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d6f0: 2020 2020 206b 7761 7267 732e 7570 6461       kwargs.upda
+0000d700: 7465 2872 656e 616d 653d 4661 6c73 652c  te(rename=False,
+0000d710: 2072 6570 6c61 6365 5f61 7474 7273 3d46   replace_attrs=F
+0000d720: 616c 7365 290a 2020 2020 2020 2020 6966  alse).        if
+0000d730: 2068 6173 6174 7472 286f 626a 2c20 2264   hasattr(obj, "d
+0000d740: 6174 615f 7661 7273 2229 3a0a 2020 2020  ata_vars"):.    
+0000d750: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000d760: 656c 662e 666f 726d 6174 5f64 6174 6173  elf.format_datas
+0000d770: 6574 286f 626a 2c20 666f 726d 6174 5f63  et(obj, format_c
+0000d780: 6f6f 7264 733d 5472 7565 2c20 2a2a 6b77  oords=True, **kw
+0000d790: 6172 6773 290a 2020 2020 2020 2020 7265  args).        re
+0000d7a0: 7475 726e 2073 656c 662e 666f 726d 6174  turn self.format
+0000d7b0: 5f64 6174 615f 7661 7228 6f62 6a2c 202a  _data_var(obj, *
+0000d7c0: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
+0000d7d0: 6620 6d61 7463 685f 636f 6f72 6428 7365  f match_coord(se
+0000d7e0: 6c66 2c20 6461 2c20 6366 5f6e 616d 653d  lf, da, cf_name=
+0000d7f0: 4e6f 6e65 2c20 6c6f 633d 2261 6e79 2229  None, loc="any")
+0000d800: 3a0a 2020 2020 2020 2020 2222 2243 6865  :.        """Che
+0000d810: 636b 2069 6620 616e 2061 7272 6179 206d  ck if an array m
+0000d820: 6174 6368 6573 2061 2067 6976 656e 206f  atches a given o
+0000d830: 7220 616e 7920 636f 6f72 6420 7370 6563  r any coord spec
+0000d840: 730a 0a20 2020 2020 2020 2050 6172 616d  s..        Param
+0000d850: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0000d860: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000d870: 2064 613a 2078 6172 7261 792e 4461 7461   da: xarray.Data
+0000d880: 4172 7261 790a 2020 2020 2020 2020 6366  Array.        cf
+0000d890: 5f6e 616d 653a 2073 7472 2c20 6469 6374  _name: str, dict
+0000d8a0: 2c20 4e6f 6e65 0a20 2020 2020 2020 2020  , None.         
+0000d8b0: 2020 2043 6620 6e61 6d65 2e0a 2020 2020     Cf name..    
+0000d8c0: 2020 2020 2020 2020 4966 204e 6f6e 652c          If None,
+0000d8d0: 2061 6c6c 206e 616d 6573 2061 7265 2075   all names are u
+0000d8e0: 7365 642e 0a20 2020 2020 2020 2020 2020  sed..           
+0000d8f0: 2049 6620 6120 6469 6374 2c20 6e61 6d65   If a dict, name
+0000d900: 2069 7320 696e 7465 7270 7265 7465 6420   is interpreted 
+0000d910: 6173 2061 6e20 6578 706c 6963 6974 2073  as an explicit s
+0000d920: 6574 206f 660a 2020 2020 2020 2020 2020  et of.          
+0000d930: 2020 7370 6563 6966 6963 6174 696f 6e73    specifications
+0000d940: 2e0a 2020 2020 2020 2020 6c6f 633a 2073  ..        loc: s
+0000d950: 7472 2c20 7b22 616e 7922 2c20 4e6f 6e65  tr, {"any", None
+0000d960: 7d2c 207b 2222 2c20 4661 6c73 657d 0a20  }, {"", False}. 
+0000d970: 2020 2020 2020 2020 2020 202d 2073 7472             - str
+0000d980: 3a20 6f6e 6520 6f66 2074 6865 7365 206c  : one of these l
+0000d990: 6f63 6174 696f 6e73 0a20 2020 2020 2020  ocations.       
+0000d9a0: 2020 2020 202d 204e 6f6e 6520 6f72 2022       - None or "
+0000d9b0: 616e 7922 3a20 616e 790a 2020 2020 2020  any": any.      
+0000d9c0: 2020 2020 2020 2d20 4661 6c73 6520 6f72        - False or
+0000d9d0: 2027 2222 3a20 6e6f 206c 6f63 6174 696f   '"": no locatio
+0000d9e0: 6e0a 0a20 2020 2020 2020 2052 6574 7572  n..        Retur
+0000d9f0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+0000da00: 2d2d 0a20 2020 2020 2020 2062 6f6f 6c2c  --.        bool,
+0000da10: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
+0000da20: 2054 7275 6520 6f72 2046 616c 7365 2069   True or False i
+0000da30: 6620 6e61 6d65 2069 7320 7072 6f76 6964  f name is provid
+0000da40: 6564 2c20 656c 7365 2066 6f75 6e64 206e  ed, else found n
+0000da50: 616d 6520 6f72 204e 6f6e 650a 0a20 2020  ame or None..   
+0000da60: 2020 2020 2053 6565 2061 6c73 6f0a 2020       See also.  
+0000da70: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20        --------. 
+0000da80: 2020 2020 2020 2043 4643 6f6f 7264 5370         CFCoordSp
+0000da90: 6563 732e 6d61 7463 680a 2020 2020 2020  ecs.match.      
+0000daa0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+0000dab0: 7475 726e 2073 656c 662e 636f 6f72 6473  turn self.coords
+0000dac0: 2e6d 6174 6368 2864 612c 2063 665f 6e61  .match(da, cf_na
+0000dad0: 6d65 3d63 665f 6e61 6d65 2c20 6c6f 633d  me=cf_name, loc=
+0000dae0: 6c6f 6329 0a0a 2020 2020 6465 6620 6d61  loc)..    def ma
+0000daf0: 7463 685f 6461 7461 5f76 6172 2873 656c  tch_data_var(sel
+0000db00: 662c 2064 612c 2063 665f 6e61 6d65 3d4e  f, da, cf_name=N
+0000db10: 6f6e 652c 206c 6f63 3d22 616e 7922 293a  one, loc="any"):
+0000db20: 0a20 2020 2020 2020 2022 2222 4368 6563  .        """Chec
+0000db30: 6b20 6966 2061 6e20 6172 7261 7920 6d61  k if an array ma
+0000db40: 7463 6865 7320 6769 7665 6e20 6f72 2061  tches given or a
+0000db50: 6e79 2064 6174 615f 7661 7220 7370 6563  ny data_var spec
+0000db60: 730a 0a20 2020 2020 2020 2050 6172 616d  s..        Param
+0000db70: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0000db80: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000db90: 2064 613a 2078 6172 7261 792e 4461 7461   da: xarray.Data
+0000dba0: 4172 7261 790a 2020 2020 2020 2020 6e61  Array.        na
+0000dbb0: 6d65 3a20 7374 722c 2064 6963 742c 204e  me: str, dict, N
+0000dbc0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000dbd0: 4366 206e 616d 652e 0a20 2020 2020 2020  Cf name..       
+0000dbe0: 2020 2020 2049 6620 4e6f 6e65 2c20 616c       If None, al
+0000dbf0: 6c20 6e61 6d65 7320 6172 6520 7573 6564  l names are used
+0000dc00: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+0000dc10: 2061 2064 6963 742c 206e 616d 6520 6973   a dict, name is
+0000dc20: 2069 6e74 6572 7072 6574 6564 2061 7320   interpreted as 
+0000dc30: 616e 2065 7870 6c69 6369 7420 7365 7420  an explicit set 
+0000dc40: 6f66 0a20 2020 2020 2020 2020 2020 2073  of.            s
+0000dc50: 7065 6369 6669 6361 7469 6f6e 732e 0a20  pecifications.. 
+0000dc60: 2020 2020 2020 206c 6f63 3a20 7374 722c         loc: str,
+0000dc70: 207b 2261 6e79 222c 204e 6f6e 657d 2c20   {"any", None}, 
+0000dc80: 7b22 222c 2046 616c 7365 7d0a 2020 2020  {"", False}.    
+0000dc90: 2020 2020 2020 2020 2d20 7374 723a 206f          - str: o
+0000dca0: 6e65 206f 6620 7468 6573 6520 6c6f 6361  ne of these loca
+0000dcb0: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+0000dcc0: 2020 2d20 4e6f 6e65 206f 7220 2261 6e79    - None or "any
+0000dcd0: 223a 2061 6e79 0a20 2020 2020 2020 2020  ": any.         
+0000dce0: 2020 202d 2046 616c 7365 206f 7220 2722     - False or '"
+0000dcf0: 223a 206e 6f20 6c6f 6361 7469 6f6e 0a0a  ": no location..
+0000dd00: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+0000dd10: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0000dd20: 2020 2020 2020 2020 626f 6f6c 2c20 7374          bool, st
+0000dd30: 720a 2020 2020 2020 2020 2020 2020 5472  r.            Tr
+0000dd40: 7565 206f 7220 4661 6c73 6520 6966 206e  ue or False if n
+0000dd50: 616d 6520 6973 2070 726f 7669 6465 642c  ame is provided,
+0000dd60: 2065 6c73 6520 666f 756e 6420 6e61 6d65   else found name
+0000dd70: 206f 7220 4e6f 6e65 0a0a 2020 2020 2020   or None..      
+0000dd80: 2020 5365 6520 616c 736f 0a20 2020 2020    See also.     
+0000dd90: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+0000dda0: 2020 2020 4346 5661 7253 7065 6373 2e6d      CFVarSpecs.m
+0000ddb0: 6174 6368 0a20 2020 2020 2020 2022 2222  atch.        """
+0000ddc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000ddd0: 7365 6c66 2e64 6174 615f 7661 7273 2e6d  self.data_vars.m
+0000dde0: 6174 6368 2864 612c 2063 665f 6e61 6d65  atch(da, cf_name
+0000ddf0: 3d63 665f 6e61 6d65 2c20 6c6f 633d 6c6f  =cf_name, loc=lo
+0000de00: 6329 0a0a 2020 2020 6465 6620 6d61 7463  c)..    def matc
+0000de10: 685f 6469 6d28 7365 6c66 2c20 6469 6d2c  h_dim(self, dim,
+0000de20: 2063 665f 6e61 6d65 3d4e 6f6e 652c 206c   cf_name=None, l
+0000de30: 6f63 3d4e 6f6e 6529 3a0a 2020 2020 2020  oc=None):.      
+0000de40: 2020 2222 2243 6865 636b 2069 6620 6120    """Check if a 
+0000de50: 6469 6d65 6e73 696f 6e20 6e61 6d65 206d  dimension name m
+0000de60: 6174 6368 6573 2067 6976 656e 206f 7220  atches given or 
+0000de70: 616e 7920 636f 6f72 6420 7370 6563 730a  any coord specs.
+0000de80: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0000de90: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+0000dea0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2064  ------.        d
+0000deb0: 696d 3a20 7374 720a 2020 2020 2020 2020  im: str.        
+0000dec0: 2020 2020 4469 6d65 6e73 696f 6e20 6e61      Dimension na
+0000ded0: 6d65 0a20 2020 2020 2020 2063 665f 6e61  me.        cf_na
+0000dee0: 6d65 3a20 7374 722c 204e 6f6e 650a 2020  me: str, None.  
+0000def0: 2020 2020 2020 2020 2020 4366 206e 616d            Cf nam
+0000df00: 652e 0a20 2020 2020 2020 206c 6f63 3a20  e..        loc: 
+0000df10: 7374 722c 207b 2261 6e79 222c 204e 6f6e  str, {"any", Non
+0000df20: 657d 2c20 7b22 222c 2046 616c 7365 7d0a  e}, {"", False}.
+0000df30: 2020 2020 2020 2020 2020 2020 2d20 7374              - st
+0000df40: 723a 206f 6e65 206f 6620 7468 6573 6520  r: one of these 
+0000df50: 6c6f 6361 7469 6f6e 730a 2020 2020 2020  locations.      
+0000df60: 2020 2020 2020 2d20 4e6f 6e65 206f 7220        - None or 
+0000df70: 2261 6e79 223a 2061 6e79 0a20 2020 2020  "any": any.     
+0000df80: 2020 2020 2020 202d 2046 616c 7365 206f         - False o
+0000df90: 7220 2722 223a 206e 6f20 6c6f 6361 7469  r '"": no locati
+0000dfa0: 6f6e 0a0a 2020 2020 2020 2020 5265 7475  on..        Retu
+0000dfb0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0000dfc0: 2d2d 2d0a 2020 2020 2020 2020 626f 6f6c  ---.        bool
+0000dfd0: 2c20 7374 720a 2020 2020 2020 2020 2020  , str.          
+0000dfe0: 2020 5472 7565 206f 7220 4661 6c73 6520    True or False 
+0000dff0: 6966 206e 616d 6520 6973 2070 726f 7669  if name is provi
+0000e000: 6465 642c 2065 6c73 6520 666f 756e 6420  ded, else found 
+0000e010: 6e61 6d65 206f 7220 4e6f 6e65 0a0a 2020  name or None..  
+0000e020: 2020 2020 2020 5365 6520 616c 736f 0a20        See also. 
+0000e030: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0a         --------.
+0000e040: 2020 2020 2020 2020 4346 5661 7253 7065          CFVarSpe
+0000e050: 6373 2e6d 6174 6368 5f66 726f 6d5f 6e61  cs.match_from_na
+0000e060: 6d65 0a20 2020 2020 2020 2022 2222 0a20  me.        """. 
+0000e070: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000e080: 6c66 2e63 6f6f 7264 732e 6d61 7463 685f  lf.coords.match_
+0000e090: 6672 6f6d 5f6e 616d 6528 6469 6d2c 2063  from_name(dim, c
+0000e0a0: 665f 6e61 6d65 3d63 665f 6e61 6d65 2c20  f_name=cf_name, 
+0000e0b0: 6c6f 633d 6c6f 6329 0a0a 2020 2020 4073  loc=loc)..    @s
+0000e0c0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+0000e0d0: 6465 6620 6765 745f 6361 7465 676f 7279  def get_category
+0000e0e0: 2864 6129 3a0a 2020 2020 2020 2020 2222  (da):.        ""
+0000e0f0: 2247 7565 7373 2069 6620 6120 6461 7461  "Guess if a data
+0000e100: 6172 7261 7920 6265 6c6f 6e67 7320 746f  array belongs to
+0000e110: 2064 6174 615f 7661 7273 206f 7220 636f   data_vars or co
+0000e120: 6f72 6473 0a0a 2020 2020 2020 2020 4974  ords..        It
+0000e130: 2062 656c 6f6e 6773 2074 6f20 636f 6f72   belongs to coor
+0000e140: 6473 2069 6620 6f6e 6520 6f66 2069 7473  ds if one of its
+0000e150: 2064 696d 656e 7369 6f6e 7320 6f72 0a20   dimensions or. 
+0000e160: 2020 2020 2020 2063 6f6f 7264 696e 6174         coordinat
+0000e170: 6573 2068 6173 2069 7473 206e 616d 652e  es has its name.
+0000e180: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0000e190: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+0000e1a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000e1b0: 6461 3a20 7861 7272 6179 2e44 6174 6141  da: xarray.DataA
+0000e1c0: 7272 6179 0a0a 2020 2020 2020 2020 5265  rray..        Re
+0000e1d0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+0000e1e0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7374  -----.        st
+0000e1f0: 720a 2020 2020 2020 2020 2222 220a 2020  r.        """.  
+0000e200: 2020 2020 2020 2320 6966 2064 612e 6e61        # if da.na
+0000e210: 6d65 2069 7320 6e6f 7420 4e6f 6e65 2061  me is not None a
+0000e220: 6e64 2028 6461 2e6e 616d 6520 696e 2064  nd (da.name in d
+0000e230: 612e 6469 6d73 206f 7220 6461 2e6e 616d  a.dims or da.nam
+0000e240: 6520 696e 2064 612e 636f 6f72 6473 293a  e in da.coords):
+0000e250: 0a20 2020 2020 2020 2069 6620 6461 2e6e  .        if da.n
+0000e260: 616d 6520 6973 206e 6f74 204e 6f6e 6520  ame is not None 
+0000e270: 616e 6420 5f6c 6973 745f 7872 5f6e 616d  and _list_xr_nam
+0000e280: 6573 5f28 6461 2c20 6461 7461 5f76 6172  es_(da, data_var
+0000e290: 733d 4661 6c73 6529 3a0a 2020 2020 2020  s=False):.      
+0000e2a0: 2020 2020 2020 7265 7475 726e 2022 636f        return "co
+0000e2b0: 6f72 6473 220a 2020 2020 2020 2020 7265  ords".        re
+0000e2c0: 7475 726e 2022 6461 7461 5f76 6172 7322  turn "data_vars"
+0000e2d0: 0a0a 2020 2020 6465 6620 6d61 7463 6828  ..    def match(
+0000e2e0: 7365 6c66 2c20 6461 2c20 6c6f 633d 2261  self, da, loc="a
+0000e2f0: 6e79 2229 3a0a 2020 2020 2020 2020 2222  ny"):.        ""
+0000e300: 2243 6865 636b 2069 6620 616e 2061 7272  "Check if an arr
+0000e310: 6179 206d 6174 6368 6573 2061 6e79 2064  ay matches any d
+0000e320: 6174 615f 7661 7220 6f72 2063 6f6f 7264  ata_var or coord
+0000e330: 2073 7065 6373 0a0a 2020 2020 2020 2020   specs..        
+0000e340: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+0000e350: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000e360: 2020 2020 2020 6461 3a20 7861 7272 6179        da: xarray
+0000e370: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
+0000e380: 2020 206c 6f63 3a20 7374 722c 207b 2261     loc: str, {"a
+0000e390: 6e79 222c 204e 6f6e 657d 2c20 7b22 222c  ny", None}, {"",
+0000e3a0: 2046 616c 7365 7d0a 2020 2020 2020 2020   False}.        
+0000e3b0: 2020 2020 2d20 7374 723a 206f 6e65 206f      - str: one o
+0000e3c0: 6620 7468 6573 6520 6c6f 6361 7469 6f6e  f these location
+0000e3d0: 730a 2020 2020 2020 2020 2020 2020 2d20  s.            - 
+0000e3e0: 4e6f 6e65 206f 7220 2261 6e79 223a 2061  None or "any": a
+0000e3f0: 6e79 0a20 2020 2020 2020 2020 2020 202d  ny.            -
+0000e400: 2046 616c 7365 206f 7220 2722 223a 206e   False or '"": n
+0000e410: 6f20 6c6f 6361 7469 6f6e 0a0a 2020 2020  o location..    
+0000e420: 2020 2020 5265 7475 726e 0a20 2020 2020      Return.     
+0000e430: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
+0000e440: 2020 7374 722c 204e 6f6e 650a 2020 2020    str, None.    
+0000e450: 2020 2020 2020 2020 4361 7465 676f 7279          Category
+0000e460: 0a20 2020 2020 2020 2073 7472 2c20 4e6f  .        str, No
+0000e470: 6e65 0a20 2020 2020 2020 2020 2020 204e  ne.            N
+0000e480: 616d 650a 2020 2020 2020 2020 2222 220a  ame.        """.
+0000e490: 2020 2020 2020 2020 6361 7465 676f 7279          category
+0000e4a0: 203d 2073 656c 662e 6765 745f 6361 7465   = self.get_cate
+0000e4b0: 676f 7279 2864 6129 0a20 2020 2020 2020  gory(da).       
+0000e4c0: 2063 6174 6567 6f72 6965 7320 3d20 6c69   categories = li
+0000e4d0: 7374 2873 656c 662e 6361 7465 676f 7269  st(self.categori
+0000e4e0: 6573 290a 2020 2020 2020 2020 6966 2063  es).        if c
+0000e4f0: 6174 6567 6f72 7920 213d 2063 6174 6567  ategory != categ
+0000e500: 6f72 6965 735b 305d 3a0a 2020 2020 2020  ories[0]:.      
+0000e510: 2020 2020 2020 6361 7465 676f 7269 6573        categories
+0000e520: 203d 2063 6174 6567 6f72 6965 735b 3a3a   = categories[::
+0000e530: 2d31 5d0a 2020 2020 2020 2020 666f 7220  -1].        for 
+0000e540: 6361 7465 676f 7279 2069 6e20 6361 7465  category in cate
+0000e550: 676f 7269 6573 3a0a 2020 2020 2020 2020  gories:.        
+0000e560: 2020 2020 6366 5f6e 616d 6520 3d20 7365      cf_name = se
+0000e570: 6c66 5b63 6174 6567 6f72 795d 2e6d 6174  lf[category].mat
+0000e580: 6368 2864 612c 206c 6f63 3d6c 6f63 290a  ch(da, loc=loc).
+0000e590: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+0000e5a0: 665f 6e61 6d65 3a0a 2020 2020 2020 2020  f_name:.        
+0000e5b0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+0000e5c0: 6174 6567 6f72 792c 2063 665f 6e61 6d65  ategory, cf_name
+0000e5d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000e5e0: 4e6f 6e65 2c20 4e6f 6e65 0a0a 2020 2020  None, None..    
+0000e5f0: 4045 5252 4f52 532e 666f 726d 6174 5f6d  @ERRORS.format_m
+0000e600: 6574 686f 645f 646f 6373 7472 696e 670a  ethod_docstring.
+0000e610: 2020 2020 6465 6620 7365 6172 6368 5f63      def search_c
+0000e620: 6f6f 7264 2873 656c 662c 206f 626a 2c20  oord(self, obj, 
+0000e630: 6366 5f6e 616d 653d 4e6f 6e65 2c20 6c6f  cf_name=None, lo
+0000e640: 633d 2261 6e79 222c 2067 6574 3d22 6f62  c="any", get="ob
+0000e650: 6a22 2c20 7369 6e67 6c65 3d54 7275 652c  j", single=True,
+0000e660: 2065 7272 6f72 733d 2277 6172 6e22 293a   errors="warn"):
+0000e670: 0a20 2020 2020 2020 2022 2222 5365 6172  .        """Sear
+0000e680: 6368 2066 6f72 2061 2063 6f6f 7264 2074  ch for a coord t
+0000e690: 6861 7420 6d61 6368 6573 2067 6976 656e  hat maches given
+0000e6a0: 206f 7220 616e 7920 7370 6563 730a 0a20   or any specs.. 
+0000e6b0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000e6c0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000e6d0: 2d2d 2d2d 0a20 2020 2020 2020 206f 626a  ----.        obj
+0000e6e0: 3a20 4461 7461 4172 7261 7920 6f72 2044  : DataArray or D
+0000e6f0: 6174 6173 6574 0a20 2020 2020 2020 2063  ataset.        c
+0000e700: 665f 6e61 6d65 3a20 7374 722c 2064 6963  f_name: str, dic
+0000e710: 740a 2020 2020 2020 2020 2020 2020 4120  t.            A 
+0000e720: 6765 6e65 7269 6320 4346 206e 616d 652e  generic CF name.
+0000e730: 2049 6620 6e6f 7420 7072 6f76 6964 6564   If not provided
+0000e740: 2c20 616c 6c20 4346 206e 616d 6573 2061  , all CF names a
+0000e750: 7265 2073 6361 6e65 642e 0a20 2020 2020  re scaned..     
+0000e760: 2020 206c 6f63 3a20 7374 722c 207b 7b22     loc: str, {{"
+0000e770: 616e 7922 2c20 4e6f 6e65 7d7d 2c20 7b7b  any", None}}, {{
+0000e780: 2222 2c20 4661 6c73 657d 7d0a 2020 2020  "", False}}.    
+0000e790: 2020 2020 2020 2020 2d20 7374 723a 206f          - str: o
+0000e7a0: 6e65 206f 6620 7468 6573 6520 6c6f 6361  ne of these loca
+0000e7b0: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+0000e7c0: 2020 2d20 4e6f 6e65 206f 7220 2261 6e79    - None or "any
+0000e7d0: 223a 2061 6e79 0a20 2020 2020 2020 2020  ": any.         
+0000e7e0: 2020 202d 2046 616c 7365 206f 7220 2222     - False or ""
+0000e7f0: 3a20 6e6f 206c 6f63 6174 696f 6e0a 2020  : no location.  
+0000e800: 2020 2020 2020 6765 743a 207b 7b22 6f62        get: {{"ob
+0000e810: 6a22 2c20 226e 616d 6522 7d7d 0a20 2020  j", "name"}}.   
+0000e820: 2020 2020 2020 2020 2057 6865 6e20 666f           When fo
+0000e830: 756e 642c 2067 6574 2074 6865 206f 626a  und, get the obj
+0000e840: 6563 7420 666f 756e 6420 6f72 2069 7473  ect found or its
+0000e850: 206e 616d 652e 0a20 2020 2020 2020 2073   name..        s
+0000e860: 696e 676c 653a 2062 6f6f 6c0a 2020 2020  ingle: bool.    
+0000e870: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+0000e880: 2072 6574 7572 6e20 7468 6520 6669 7273   return the firs
+0000e890: 7420 6974 656d 2066 6f75 6e64 206f 7220  t item found or 
+0000e8a0: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
+0000e8b0: 2020 4966 2046 616c 7365 2c20 7265 7475    If False, retu
+0000e8c0: 726e 2061 2070 6f73 7369 626c 6520 656d  rn a possible em
+0000e8d0: 7074 7920 6c69 7374 206f 6620 666f 756e  pty list of foun
+0000e8e0: 6420 6974 656d 732e 0a20 2020 2020 2020  d items..       
+0000e8f0: 2020 2020 2041 2077 6172 6e69 6e67 2069       A warning i
+0000e900: 7320 656d 6974 7465 6420 7768 656e 2073  s emitted when s
+0000e910: 6574 2074 6f20 5472 7565 2061 6e64 206d  et to True and m
+0000e920: 756c 7469 706c 6520 6974 656d 2061 7265  ultiple item are
+0000e930: 2066 6f75 6e64 2e0a 2020 2020 2020 2020   found..        
+0000e940: 7b65 7272 6f72 737d 0a0a 2020 2020 2020  {errors}..      
+0000e950: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+0000e960: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+0000e970: 2020 4e6f 6e65 206f 7220 7374 7220 6f72    None or str or
+0000e980: 206f 626a 6563 740a 0a20 2020 2020 2020   object..       
+0000e990: 2045 7861 6d70 6c65 0a20 2020 2020 2020   Example.       
+0000e9a0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+0000e9b0: 202e 2e20 6970 7974 686f 6e3a 3a20 7079   .. ipython:: py
+0000e9c0: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
+0000e9d0: 2020 4073 7570 7072 6573 730a 2020 2020    @suppress.    
+0000e9e0: 2020 2020 2020 2020 6672 6f6d 2078 6f61          from xoa
+0000e9f0: 2e63 6620 696d 706f 7274 2067 6574 5f63  .cf import get_c
+0000ea00: 665f 7370 6563 730a 2020 2020 2020 2020  f_specs.        
+0000ea10: 2020 2020 4073 7570 7072 6573 730a 2020      @suppress.  
+0000ea20: 2020 2020 2020 2020 2020 696d 706f 7274            import
+0000ea30: 2078 6172 7261 7920 6173 2078 722c 206e   xarray as xr, n
+0000ea40: 756d 7079 2061 7320 6e70 0a20 2020 2020  umpy as np.     
+0000ea50: 2020 2020 2020 206c 6f6e 203d 2078 722e         lon = xr.
+0000ea60: 4461 7461 4172 7261 7928 5b32 2c20 335d  DataArray([2, 3]
+0000ea70: 2c20 6469 6d73 3d27 666f 6f27 2c0a 2020  , dims='foo',.  
+0000ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea90: 2020 2020 2020 2020 2020 2020 2061 7474               att
+0000eaa0: 7273 3d7b 7b27 7374 616e 6461 7264 5f6e  rs={{'standard_n
+0000eab0: 616d 6527 3a20 276c 6f6e 6769 7475 6465  ame': 'longitude
+0000eac0: 277d 7d29 0a20 2020 2020 2020 2020 2020  '}}).           
+0000ead0: 2064 6174 6120 3d20 7872 2e44 6174 6141   data = xr.DataA
+0000eae0: 7272 6179 285b 302c 2031 5d2c 2064 696d  rray([0, 1], dim
+0000eaf0: 733d 2827 666f 6f27 292c 2063 6f6f 7264  s=('foo'), coord
+0000eb00: 733d 5b6c 6f6e 5d29 0a20 2020 2020 2020  s=[lon]).       
+0000eb10: 2020 2020 2063 6673 7065 6373 203d 2067       cfspecs = g
+0000eb20: 6574 5f63 665f 7370 6563 7328 290a 2020  et_cf_specs().  
+0000eb30: 2020 2020 2020 2020 2020 6366 7370 6563            cfspec
+0000eb40: 732e 7365 6172 6368 5f63 6f6f 7264 2864  s.search_coord(d
+0000eb50: 6174 612c 2022 6c6f 6e22 290a 2020 2020  ata, "lon").    
+0000eb60: 2020 2020 2020 2020 6366 7370 6563 732e          cfspecs.
+0000eb70: 7365 6172 6368 5f63 6f6f 7264 2864 6174  search_coord(dat
+0000eb80: 612c 2022 6c6f 6e22 2c20 6765 743d 2263  a, "lon", get="c
+0000eb90: 665f 6e61 6d65 2229 0a20 2020 2020 2020  f_name").       
+0000eba0: 2020 2020 2063 6673 7065 6373 2e73 6561       cfspecs.sea
+0000ebb0: 7263 685f 636f 6f72 6428 6461 7461 2c20  rch_coord(data, 
+0000ebc0: 226c 6174 222c 2065 7272 6f72 733d 2269  "lat", errors="i
+0000ebd0: 676e 6f72 6522 290a 0a20 2020 2020 2020  gnore")..       
+0000ebe0: 2053 6565 2061 6c73 6f0a 2020 2020 2020   See also.      
+0000ebf0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020    --------.     
+0000ec00: 2020 2073 6561 7263 685f 6461 7461 5f76     search_data_v
+0000ec10: 6172 0a20 2020 2020 2020 2043 4643 6f6f  ar.        CFCoo
+0000ec20: 7264 5370 6563 732e 7365 6172 6368 0a20  rdSpecs.search. 
+0000ec30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000ec40: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
+0000ec50: 6f6f 7264 732e 7365 6172 6368 280a 2020  oords.search(.  
+0000ec60: 2020 2020 2020 2020 2020 6f62 6a2c 2063            obj, c
+0000ec70: 665f 6e61 6d65 3d63 665f 6e61 6d65 2c20  f_name=cf_name, 
+0000ec80: 6c6f 633d 6c6f 632c 2067 6574 3d67 6574  loc=loc, get=get
+0000ec90: 2c20 7369 6e67 6c65 3d73 696e 676c 652c  , single=single,
+0000eca0: 2065 7272 6f72 733d 6572 726f 7273 0a20   errors=errors. 
+0000ecb0: 2020 2020 2020 2029 0a0a 2020 2020 4045         )..    @E
+0000ecc0: 5252 4f52 532e 666f 726d 6174 5f6d 6574  RRORS.format_met
+0000ecd0: 686f 645f 646f 6373 7472 696e 670a 2020  hod_docstring.  
+0000ece0: 2020 6465 6620 7365 6172 6368 5f64 696d    def search_dim
+0000ecf0: 2873 656c 662c 2064 612c 2063 665f 6172  (self, da, cf_ar
+0000ed00: 673d 4e6f 6e65 2c20 6c6f 633d 2261 6e79  g=None, loc="any
+0000ed10: 222c 2065 7272 6f72 733d 2269 676e 6f72  ", errors="ignor
+0000ed20: 6522 293a 0a20 2020 2020 2020 2022 2222  e"):.        """
+0000ed30: 5365 6172 6368 2066 6f72 2061 2064 696d  Search for a dim
+0000ed40: 656e 7369 6f6e 2066 726f 6d20 6974 7320  ension from its 
+0000ed50: 7479 7065 0a0a 2020 2020 2020 2020 5061  type..        Pa
+0000ed60: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0000ed70: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000ed80: 2020 2020 6461 3a20 7861 7272 6179 2e44      da: xarray.D
+0000ed90: 6174 6141 7272 6179 0a20 2020 2020 2020  ataArray.       
+0000eda0: 2063 665f 6172 673a 204e 6f6e 652c 2073   cf_arg: None, s
+0000edb0: 7472 2c20 7b7b 2278 222c 2022 7922 2c20  tr, {{"x", "y", 
+0000edc0: 227a 222c 2022 7422 2c20 2266 227d 7d0a  "z", "t", "f"}}.
+0000edd0: 2020 2020 2020 2020 2020 2020 4469 6d65              Dime
+0000ede0: 6e73 696f 6e20 7479 7065 206f 7220 6765  nsion type or ge
+0000edf0: 6e65 7269 6320 4346 206e 616d 650a 2020  neric CF name.  
+0000ee00: 2020 2020 2020 6c6f 633a 0a20 2020 2020        loc:.     
+0000ee10: 2020 2020 2020 2053 7461 6767 6572 6564         Staggered
+0000ee20: 2067 7269 6420 6c6f 6361 7469 6f6e 0a20   grid location. 
+0000ee30: 2020 2020 2020 207b 6572 726f 7273 7d0a         {errors}.
+0000ee40: 0a20 2020 2020 2020 2052 6574 7572 6e0a  .        Return.
+0000ee50: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0a20          ------. 
+0000ee60: 2020 2020 2020 204e 6f6e 652c 2073 7472         None, str
+0000ee70: 2c20 6469 6374 0a20 2020 2020 2020 2020  , dict.         
+0000ee80: 2020 2044 696d 206e 616d 6520 4f52 2c20     Dim name OR, 
+0000ee90: 6469 6374 2077 6974 6820 6469 6d2c 2074  dict with dim, t
+0000eea0: 7970 6520 616e 6420 6366 5f6e 616d 6520  ype and cf_name 
+0000eeb0: 6b65 7973 2069 6620 6366 5f61 7267 2069  keys if cf_arg i
+0000eec0: 7320 4e6f 6e65 0a0a 2020 2020 2020 2020  s None..        
+0000eed0: 5365 6520 616c 736f 0a20 2020 2020 2020  See also.       
+0000eee0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020   --------.      
+0000eef0: 2020 4346 436f 6f72 6453 7065 6373 2e73    CFCoordSpecs.s
+0000ef00: 6561 7263 685f 6469 6d0a 2020 2020 2020  earch_dim.      
+0000ef10: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+0000ef20: 7475 726e 2073 656c 662e 636f 6f72 6473  turn self.coords
+0000ef30: 2e73 6561 7263 685f 6469 6d28 6461 2c20  .search_dim(da, 
+0000ef40: 6366 5f61 7267 3d63 665f 6172 672c 206c  cf_arg=cf_arg, l
+0000ef50: 6f63 3d6c 6f63 2c20 6572 726f 7273 3d65  oc=loc, errors=e
+0000ef60: 7272 6f72 7329 0a0a 2020 2020 4045 5252  rrors)..    @ERR
+0000ef70: 4f52 532e 666f 726d 6174 5f6d 6574 686f  ORS.format_metho
+0000ef80: 645f 646f 6373 7472 696e 670a 2020 2020  d_docstring.    
+0000ef90: 6465 6620 7365 6172 6368 5f63 6f6f 7264  def search_coord
+0000efa0: 5f66 726f 6d5f 6469 6d28 7365 6c66 2c20  _from_dim(self, 
+0000efb0: 6461 2c20 6469 6d2c 2065 7272 6f72 733d  da, dim, errors=
+0000efc0: 2269 676e 6f72 6522 293a 0a20 2020 2020  "ignore"):.     
+0000efd0: 2020 2022 2222 5365 6172 6368 2061 2064     """Search a d
+0000efe0: 6174 6161 7272 6179 2066 6f72 2061 2063  ataarray for a c
+0000eff0: 6f6f 7264 696e 6174 6520 6672 6f6d 2061  oordinate from a
+0000f000: 2064 696d 656e 7369 6f6e 206e 616d 650a   dimension name.
+0000f010: 0a20 2020 2020 2020 2049 7420 6669 7273  .        It firs
+0000f020: 7420 7365 6172 6368 6573 2066 6f72 2061  t searches for a
+0000f030: 2063 6f6f 7264 696e 6174 6520 7769 7468   coordinate with
+0000f040: 2074 6865 2073 616d 6520 6e61 6d65 2061   the same name a
+0000f050: 6e64 2074 6861 7420 6973 0a20 2020 2020  nd that is.     
+0000f060: 2020 2074 6865 206f 6e6c 7920 6f6e 6520     the only one 
+0000f070: 6861 7669 6e67 2074 6869 7320 6469 6d65  having this dime
+0000f080: 6e73 696f 6e2e 0a20 2020 2020 2020 2054  nsion..        T
+0000f090: 6865 6e20 6c6f 6f6b 2066 6f72 2063 6f6f  hen look for coo
+0000f0a0: 7264 696e 6174 6573 2077 6974 6820 7468  rdinates with th
+0000f0b0: 6520 7361 6d65 2074 7970 6520 6c69 6b65  e same type like
+0000f0c0: 2078 2c20 792c 2065 7463 2e0a 0a20 2020   x, y, etc...   
+0000f0d0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+0000f0e0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0000f0f0: 2d2d 0a20 2020 2020 2020 2064 613a 2078  --.        da: x
+0000f100: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
+0000f110: 2020 2020 2020 2020 6469 6d3a 2073 7472          dim: str
+0000f120: 0a20 2020 2020 2020 207b 6572 726f 7273  .        {errors
+0000f130: 7d0a 0a20 2020 2020 2020 2052 6574 7572  }..        Retur
+0000f140: 6e0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  n.        ------
+0000f150: 0a20 2020 2020 2020 2078 6172 7261 792e  .        xarray.
+0000f160: 4461 7461 4172 7261 792c 204e 6f6e 650a  DataArray, None.
+0000f170: 2020 2020 2020 2020 2020 2020 416e 2063              An c
+0000f180: 6f6f 7264 696e 6174 6520 6172 7261 7920  oordinate array 
+0000f190: 6f72 204e 6f6e 650a 2020 2020 2020 2020  or None.        
+0000f1a0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+0000f1b0: 726e 2073 656c 662e 636f 6f72 6473 2e73  rn self.coords.s
+0000f1c0: 6561 7263 685f 6672 6f6d 5f64 696d 2864  earch_from_dim(d
+0000f1d0: 612c 2064 696d 2c20 6572 726f 7273 3d65  a, dim, errors=e
+0000f1e0: 7272 6f72 7329 0a0a 2020 2020 4045 5252  rrors)..    @ERR
+0000f1f0: 4f52 532e 666f 726d 6174 5f6d 6574 686f  ORS.format_metho
+0000f200: 645f 646f 6373 7472 696e 670a 2020 2020  d_docstring.    
+0000f210: 6465 6620 7365 6172 6368 5f64 6174 615f  def search_data_
+0000f220: 7661 7228 7365 6c66 2c20 6f62 6a2c 2063  var(self, obj, c
+0000f230: 665f 6e61 6d65 3d4e 6f6e 652c 206c 6f63  f_name=None, loc
+0000f240: 3d22 616e 7922 2c20 6765 743d 226f 626a  ="any", get="obj
+0000f250: 222c 2073 696e 676c 653d 5472 7565 2c20  ", single=True, 
+0000f260: 6572 726f 7273 3d22 7761 726e 2229 3a0a  errors="warn"):.
+0000f270: 2020 2020 2020 2020 2222 2253 6561 7263          """Searc
+0000f280: 6820 666f 7220 6120 6461 7461 5f76 6172  h for a data_var
+0000f290: 2074 6861 7420 6d61 6368 6573 2067 6976   that maches giv
+0000f2a0: 656e 206f 7220 616e 7920 7370 6563 730a  en or any specs.
+0000f2b0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0000f2c0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+0000f2d0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 206f  ------.        o
+0000f2e0: 626a 3a20 4461 7461 4172 7261 7920 6f72  bj: DataArray or
+0000f2f0: 2044 6174 6173 6574 0a20 2020 2020 2020   Dataset.       
+0000f300: 2063 665f 6e61 6d65 3a20 7374 722c 2064   cf_name: str, d
+0000f310: 6963 740a 2020 2020 2020 2020 2020 2020  ict.            
+0000f320: 4120 6765 6e65 7269 6320 4346 206e 616d  A generic CF nam
+0000f330: 652e 2049 6620 6e6f 7420 7072 6f76 6964  e. If not provid
+0000f340: 6564 2c20 616c 6c20 4346 206e 616d 6573  ed, all CF names
+0000f350: 2061 7265 2073 6361 6e65 642e 0a20 2020   are scaned..   
+0000f360: 2020 2020 206c 6f63 3a20 7374 722c 207b       loc: str, {
+0000f370: 7b22 616e 7922 2c20 4e6f 6e65 7d7d 2c20  {"any", None}}, 
+0000f380: 7b7b 2222 2c20 4661 6c73 657d 7d0a 2020  {{"", False}}.  
+0000f390: 2020 2020 2020 2020 2020 2d20 7374 723a            - str:
+0000f3a0: 206f 6e65 206f 6620 7468 6573 6520 6c6f   one of these lo
+0000f3b0: 6361 7469 6f6e 730a 2020 2020 2020 2020  cations.        
+0000f3c0: 2020 2020 2d20 4e6f 6e65 206f 7220 2261      - None or "a
+0000f3d0: 6e79 223a 2061 6e79 0a20 2020 2020 2020  ny": any.       
+0000f3e0: 2020 2020 202d 2046 616c 7365 206f 7220       - False or 
+0000f3f0: 2722 223a 206e 6f20 6c6f 6361 7469 6f6e  '"": no location
+0000f400: 0a20 2020 2020 2020 2067 6574 3a20 7b7b  .        get: {{
+0000f410: 226f 626a 222c 2022 6e61 6d65 227d 7d0a  "obj", "name"}}.
+0000f420: 2020 2020 2020 2020 2020 2020 5768 656e              When
+0000f430: 2066 6f75 6e64 2c20 6765 7420 7468 6520   found, get the 
+0000f440: 6f62 6a65 6374 2066 6f75 6e64 206f 7220  object found or 
+0000f450: 6974 7320 6e61 6d65 2e0a 2020 2020 2020  its name..      
+0000f460: 2020 7369 6e67 6c65 3a20 626f 6f6c 0a20    single: bool. 
+0000f470: 2020 2020 2020 2020 2020 2049 6620 5472             If Tr
+0000f480: 7565 2c20 7265 7475 726e 2074 6865 2066  ue, return the f
+0000f490: 6972 7374 2069 7465 6d20 666f 756e 6420  irst item found 
+0000f4a0: 6f72 204e 6f6e 652e 0a20 2020 2020 2020  or None..       
+0000f4b0: 2020 2020 2049 6620 4661 6c73 652c 2072       If False, r
+0000f4c0: 6574 7572 6e20 6120 706f 7373 6962 6c65  eturn a possible
+0000f4d0: 2065 6d70 7479 206c 6973 7420 6f66 2066   empty list of f
+0000f4e0: 6f75 6e64 2069 7465 6d73 2e0a 2020 2020  ound items..    
+0000f4f0: 2020 2020 2020 2020 4120 7761 726e 696e          A warnin
+0000f500: 6720 6973 2065 6d69 7474 6564 2077 6865  g is emitted whe
+0000f510: 6e20 7365 7420 746f 2054 7275 6520 616e  n set to True an
+0000f520: 6420 6d75 6c74 6970 6c65 2069 7465 6d20  d multiple item 
+0000f530: 6172 6520 666f 756e 642e 0a20 2020 2020  are found..     
+0000f540: 2020 207b 6572 726f 7273 7d0a 0a20 2020     {errors}..   
+0000f550: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+0000f560: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+0000f570: 2020 2020 204e 6f6e 6520 6f72 2073 7472       None or str
+0000f580: 206f 7220 6f62 6a65 6374 0a0a 2020 2020   or object..    
+0000f590: 2020 2020 4578 616d 706c 650a 2020 2020      Example.    
+0000f5a0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0000f5b0: 2020 2020 2e2e 2069 7079 7468 6f6e 3a3a      .. ipython::
+0000f5c0: 2070 7974 686f 6e0a 2020 2020 2020 2020   python.        
+0000f5d0: 2020 2020 3a6f 6b77 6172 6e69 6e67 3a0a      :okwarning:.
+0000f5e0: 0a20 2020 2020 2020 2020 2020 2040 7375  .            @su
+0000f5f0: 7070 7265 7373 0a20 2020 2020 2020 2020  ppress.         
+0000f600: 2020 2066 726f 6d20 786f 612e 6366 2069     from xoa.cf i
+0000f610: 6d70 6f72 7420 6765 745f 6366 5f73 7065  mport get_cf_spe
+0000f620: 6373 0a20 2020 2020 2020 2020 2020 2040  cs.            @
+0000f630: 7375 7070 7265 7373 0a20 2020 2020 2020  suppress.       
+0000f640: 2020 2020 2069 6d70 6f72 7420 7861 7272       import xarr
+0000f650: 6179 2061 7320 7872 2c20 6e75 6d70 7920  ay as xr, numpy 
+0000f660: 6173 206e 700a 2020 2020 2020 2020 2020  as np.          
+0000f670: 2020 6461 7461 203d 2078 722e 4461 7461    data = xr.Data
+0000f680: 4172 7261 7928 0a20 2020 2020 2020 2020  Array(.         
+0000f690: 2020 2020 2020 205b 302c 2031 5d2c 2064         [0, 1], d
+0000f6a0: 696d 733d 2827 7827 292c 0a20 2020 2020  ims=('x'),.     
+0000f6b0: 2020 2020 2020 2020 2020 2061 7474 7273             attrs
+0000f6c0: 3d7b 7b27 7374 616e 6461 7264 5f6e 616d  ={{'standard_nam
+0000f6d0: 6527 3a20 2773 6561 5f77 6174 6572 5f74  e': 'sea_water_t
+0000f6e0: 656d 7065 7261 7475 7265 277d 7d29 0a20  emperature'}}). 
+0000f6f0: 2020 2020 2020 2020 2020 2064 7320 3d20             ds = 
+0000f700: 7872 2e44 6174 6173 6574 287b 7b27 666f  xr.Dataset({{'fo
+0000f710: 6f27 3a20 6461 7461 7d7d 290a 2020 2020  o': data}}).    
+0000f720: 2020 2020 2020 2020 6366 7370 6563 7320          cfspecs 
+0000f730: 3d20 6765 745f 6366 5f73 7065 6373 2829  = get_cf_specs()
+0000f740: 0a20 2020 2020 2020 2020 2020 2063 6673  .            cfs
+0000f750: 7065 6373 2e73 6561 7263 685f 6461 7461  pecs.search_data
+0000f760: 5f76 6172 2864 732c 2022 7465 6d70 2229  _var(ds, "temp")
+0000f770: 0a20 2020 2020 2020 2020 2020 2063 6673  .            cfs
+0000f780: 7065 6373 2e73 6561 7263 685f 6461 7461  pecs.search_data
+0000f790: 5f76 6172 2864 732c 2022 7465 6d70 222c  _var(ds, "temp",
+0000f7a0: 2067 6574 3d22 6366 5f6e 616d 6522 290a   get="cf_name").
+0000f7b0: 2020 2020 2020 2020 2020 2020 6366 7370              cfsp
+0000f7c0: 6563 732e 7365 6172 6368 5f64 6174 615f  ecs.search_data_
+0000f7d0: 7661 7228 6473 2c20 2273 616c 2229 0a0a  var(ds, "sal")..
+0000f7e0: 2020 2020 2020 2020 5365 6520 616c 736f          See also
+0000f7f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000f800: 2d0a 2020 2020 2020 2020 7365 6172 6368  -.        search
+0000f810: 5f63 6f6f 7264 0a20 2020 2020 2020 2043  _coord.        C
+0000f820: 4656 6172 5370 6563 732e 7365 6172 6368  FVarSpecs.search
+0000f830: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f840: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000f850: 2e64 6174 615f 7661 7273 2e73 6561 7263  .data_vars.searc
+0000f860: 6828 0a20 2020 2020 2020 2020 2020 206f  h(.            o
+0000f870: 626a 2c20 6366 5f6e 616d 653d 6366 5f6e  bj, cf_name=cf_n
+0000f880: 616d 652c 206c 6f63 3d6c 6f63 2c20 6765  ame, loc=loc, ge
+0000f890: 743d 6765 742c 2073 696e 676c 653d 7369  t=get, single=si
+0000f8a0: 6e67 6c65 2c20 6572 726f 7273 3d65 7272  ngle, errors=err
+0000f8b0: 6f72 730a 2020 2020 2020 2020 290a 0a20  ors.        ).. 
+0000f8c0: 2020 2040 4552 524f 5253 2e66 6f72 6d61     @ERRORS.forma
+0000f8d0: 745f 6d65 7468 6f64 5f64 6f63 7374 7269  t_method_docstri
+0000f8e0: 6e67 0a20 2020 2064 6566 2073 6561 7263  ng.    def searc
+0000f8f0: 6828 0a20 2020 2020 2020 2073 656c 662c  h(.        self,
+0000f900: 206f 626a 2c20 6366 5f6e 616d 653d 4e6f   obj, cf_name=No
+0000f910: 6e65 2c20 6c6f 633d 2261 6e79 222c 2067  ne, loc="any", g
+0000f920: 6574 3d22 6f62 6a22 2c20 7369 6e67 6c65  et="obj", single
+0000f930: 3d54 7275 652c 2063 6174 6567 6f72 6965  =True, categorie
+0000f940: 733d 4e6f 6e65 2c20 6572 726f 7273 3d22  s=None, errors="
+0000f950: 7761 726e 220a 2020 2020 293a 0a20 2020  warn".    ):.   
+0000f960: 2020 2020 2022 2222 5365 6172 6368 2066       """Search f
+0000f970: 6f72 2061 2064 6174 6161 7272 6179 2077  or a dataarray w
+0000f980: 6974 6820 6461 7461 5f76 6172 7320 616e  ith data_vars an
+0000f990: 642f 6f72 2063 6f6f 7264 730a 0a0a 2020  d/or coords...  
+0000f9a0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+0000f9b0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000f9c0: 2d2d 2d0a 2020 2020 2020 2020 6f62 6a3a  ---.        obj:
+0000f9d0: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
+0000f9e0: 792c 2078 6172 7261 792e 4461 7461 7365  y, xarray.Datase
+0000f9f0: 740a 2020 2020 2020 2020 2020 2020 4172  t.            Ar
+0000fa00: 7261 7920 6f72 2064 6174 6173 6574 2074  ray or dataset t
+0000fa10: 6f20 7363 616e 0a20 2020 2020 2020 2063  o scan.        c
+0000fa20: 665f 6e61 6d65 3a20 7374 720a 2020 2020  f_name: str.    
+0000fa30: 2020 2020 2020 2020 4765 6e65 7269 6320          Generic 
+0000fa40: 4346 206e 616d 6520 746f 2073 6561 7263  CF name to searc
+0000fa50: 6820 666f 722e 0a20 2020 2020 2020 2063  h for..        c
+0000fa60: 6174 6567 6f72 6965 733a 2073 7472 2c20  ategories: str, 
+0000fa70: 6c69 7374 2c20 4e6f 6e65 0a20 2020 2020  list, None.     
+0000fa80: 2020 2020 2020 2045 7870 6c69 6374 7920         Explicty 
+0000fa90: 6361 7465 676f 7269 6573 2077 6974 6820  categories with 
+0000faa0: 2263 6f6f 7264 7322 2061 6e64 2022 6461  "coords" and "da
+0000fab0: 7461 5f76 6172 7322 2e0a 2020 2020 2020  ta_vars"..      
+0000fac0: 2020 7b65 7272 6f72 737d 0a0a 2020 2020    {errors}..    
+0000fad0: 2020 2020 5265 7475 726e 0a20 2020 2020      Return.     
+0000fae0: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
+0000faf0: 2020 4e6f 6e65 2c20 7861 7272 6179 2e44    None, xarray.D
+0000fb00: 6174 6141 7272 6179 2c20 6c69 7374 0a0a  ataArray, list..
+0000fb10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000fb20: 2020 2020 6966 206e 6f74 2063 6174 6567      if not categ
+0000fb30: 6f72 6965 733a 0a20 2020 2020 2020 2020  ories:.         
+0000fb40: 2020 2063 6174 6567 6f72 6965 7320 3d20     categories = 
+0000fb50: 7365 6c66 2e63 6174 6567 6f72 6965 7320  self.categories 
+0000fb60: 6966 2068 6173 6174 7472 286f 626a 2c20  if hasattr(obj, 
+0000fb70: 2264 6174 615f 7661 7273 2229 2065 6c73  "data_vars") els
+0000fb80: 6520 5b22 636f 6f72 6473 222c 2022 6461  e ["coords", "da
+0000fb90: 7461 5f76 6172 7322 5d0a 2020 2020 2020  ta_vars"].      
+0000fba0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+0000fbb0: 6528 6361 7465 676f 7269 6573 2c20 7374  e(categories, st
+0000fbc0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0000fbd0: 6361 7465 676f 7269 6573 203d 205b 6361  categories = [ca
+0000fbe0: 7465 676f 7269 6573 5d0a 2020 2020 2020  tegories].      
+0000fbf0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000fc00: 2020 2020 6361 7465 676f 7269 6573 203d      categories =
+0000fc10: 2073 656c 662e 6361 7465 676f 7269 6573   self.categories
+0000fc20: 0a20 2020 2020 2020 2065 7272 6f72 7320  .        errors 
+0000fc30: 3d20 4552 524f 5253 5b65 7272 6f72 735d  = ERRORS[errors]
+0000fc40: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000fc50: 7369 6e67 6c65 3a0a 2020 2020 2020 2020  single:.        
+0000fc60: 2020 2020 666f 756e 6420 3d20 5b5d 0a20      found = []. 
+0000fc70: 2020 2020 2020 2066 6f72 2063 6174 6567         for categ
+0000fc80: 6f72 7920 696e 2063 6174 6567 6f72 6965  ory in categorie
+0000fc90: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+0000fca0: 6573 203d 2073 656c 665b 6361 7465 676f  es = self[catego
+0000fcb0: 7279 5d2e 7365 6172 6368 280a 2020 2020  ry].search(.    
+0000fcc0: 2020 2020 2020 2020 2020 2020 6f62 6a2c              obj,
+0000fcd0: 2063 665f 6e61 6d65 3d63 665f 6e61 6d65   cf_name=cf_name
+0000fce0: 2c20 6c6f 633d 6c6f 632c 2067 6574 3d67  , loc=loc, get=g
+0000fcf0: 6574 2c20 7369 6e67 6c65 3d73 696e 676c  et, single=singl
+0000fd00: 652c 2065 7272 6f72 733d 2269 676e 6f72  e, errors="ignor
+0000fd10: 6522 0a20 2020 2020 2020 2020 2020 2029  e".            )
+0000fd20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000fd30: 6e6f 7420 7369 6e67 6c65 3a0a 2020 2020  not single:.    
+0000fd40: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+0000fd50: 3d20 5b72 2066 6f72 2072 2069 6e20 7265  = [r for r in re
+0000fd60: 7320 6966 2072 2e6e 616d 6520 6e6f 7420  s if r.name not 
+0000fd70: 696e 205b 662e 6e61 6d65 2066 6f72 2066  in [f.name for f
+0000fd80: 2069 6e20 666f 756e 645d 5d0a 2020 2020   in found]].    
+0000fd90: 2020 2020 2020 2020 2020 2020 666f 756e              foun
+0000fda0: 642e 6578 7465 6e64 2872 6573 290a 2020  d.extend(res).  
+0000fdb0: 2020 2020 2020 2020 2020 656c 6966 2072            elif r
+0000fdc0: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fde0: 7265 7475 726e 2072 6573 0a20 2020 2020  return res.     
+0000fdf0: 2020 2069 6620 6e6f 7420 7369 6e67 6c65     if not single
+0000fe00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000fe10: 7475 726e 2066 6f75 6e64 0a20 2020 2020  turn found.     
+0000fe20: 2020 206d 7367 203d 2022 5365 6172 6368     msg = "Search
+0000fe30: 2066 6169 6c65 6422 0a20 2020 2020 2020   failed".       
+0000fe40: 2069 6620 6572 726f 7273 203d 3d20 2277   if errors == "w
+0000fe50: 6172 6e22 3a0a 2020 2020 2020 2020 2020  arn":.          
+0000fe60: 2020 786f 615f 7761 726e 286d 7367 290a    xoa_warn(msg).
+0000fe70: 2020 2020 2020 2020 656c 6966 2065 7272          elif err
+0000fe80: 6f72 7320 3d3d 2022 7261 6973 6522 3a0a  ors == "raise":.
+0000fe90: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000fea0: 6520 586f 6143 4645 7272 6f72 286d 7367  e XoaCFError(msg
+0000feb0: 290a 0a20 2020 2064 6566 2067 6574 2873  )..    def get(s
+0000fec0: 656c 662c 206f 626a 2c20 6366 5f6e 616d  elf, obj, cf_nam
+0000fed0: 652c 2067 6574 3d22 6f62 6a22 293a 0a20  e, get="obj"):. 
+0000fee0: 2020 2020 2020 2022 2222 4120 7368 6f72         """A shor
+0000fef0: 7463 7574 2074 6f20 3a6d 6574 683a 6073  tcut to :meth:`s
+0000ff00: 6561 7263 6860 2077 6974 6820 616e 2065  earch` with an e
+0000ff10: 7870 6c69 6369 7420 6765 6e65 7269 6320  xplicit generic 
+0000ff20: 4346 206e 616d 650a 0a20 2020 2020 2020  CF name..       
+0000ff30: 2041 2073 696e 676c 6520 656c 656d 656e   A single elemen
+0000ff40: 7420 6973 2073 6561 7263 6865 6420 666f  t is searched fo
+0000ff50: 7220 696e 746f 2061 6c6c 203a 6174 7472  r into all :attr
+0000ff60: 3a60 6361 7465 676f 7269 6573 600a 2020  :`categories`.  
+0000ff70: 2020 2020 2020 616e 6420 6572 726f 7273        and errors
+0000ff80: 2061 7265 2069 676e 6f72 6564 2e0a 2020   are ignored..  
+0000ff90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000ffa0: 2020 7265 7475 726e 2073 656c 662e 7365    return self.se
+0000ffb0: 6172 6368 286f 626a 2c20 6366 5f6e 616d  arch(obj, cf_nam
+0000ffc0: 652c 2065 7272 6f72 733d 2269 676e 6f72  e, errors="ignor
+0000ffd0: 6522 2c20 7369 6e67 6c65 3d54 7275 652c  e", single=True,
+0000ffe0: 2067 6574 3d67 6574 290a 2020 2020 2020   get=get).      
+0000fff0: 2020 2320 6966 2064 6120 6973 204e 6f6e    # if da is Non
+00010000: 653a 0a20 2020 2020 2020 2023 2020 2020  e:.        #    
+00010010: 2072 6169 7365 2058 6f61 4346 4572 726f   raise XoaCFErro
+00010020: 7228 2253 6561 7263 6820 6661 696c 6564  r("Search failed
+00010030: 2066 6f72 2074 6865 2066 6f6c 6c6f 7769   for the followi
+00010040: 6e67 2063 6620 6e61 6d65 3a20 220a 2020  ng cf name: ".  
+00010050: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+00010060: 2020 2020 2020 2020 2020 2020 202b 206e               + n
+00010070: 616d 6529 0a20 2020 2020 2020 2023 2072  ame).        # r
+00010080: 6574 7572 6e20 6461 0a0a 2020 2020 4045  eturn da..    @E
+00010090: 5252 4f52 532e 666f 726d 6174 5f6d 6574  RRORS.format_met
+000100a0: 686f 645f 646f 6373 7472 696e 670a 2020  hod_docstring.  
+000100b0: 2020 6465 6620 6765 745f 6469 6d73 280a    def get_dims(.
+000100c0: 2020 2020 2020 2020 7365 6c66 2c20 6461          self, da
+000100d0: 2c20 6366 5f61 7267 732c 2061 6c6c 6f77  , cf_args, allow
+000100e0: 5f70 6f73 6974 696f 6e61 6c3d 4661 6c73  _positional=Fals
+000100f0: 652c 2070 6f73 6974 696f 6e73 3d27 747a  e, positions='tz
+00010100: 7978 272c 2073 696e 676c 653d 5472 7565  yx', single=True
+00010110: 2c20 6572 726f 7273 3d22 7761 726e 220a  , errors="warn".
+00010120: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+00010130: 2222 4765 7420 7468 6520 6461 7461 2061  ""Get the data a
+00010140: 7272 6179 2064 696d 656e 7369 6f6e 7320  rray dimensions 
+00010150: 6e61 6d65 7320 6672 6f6d 2074 6865 6972  names from their
+00010160: 2074 7970 650a 0a20 2020 2020 2020 2050   type..        P
+00010170: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00010180: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00010190: 2020 2020 2064 613a 2078 6172 7261 792e       da: xarray.
+000101a0: 4461 7461 4172 7261 790a 2020 2020 2020  DataArray.      
+000101b0: 2020 2020 2020 4172 7261 7920 746f 2073        Array to s
+000101c0: 6361 6e0a 2020 2020 2020 2020 6366 5f61  can.        cf_a
+000101d0: 7267 733a 2073 7472 2c20 6c69 7374 0a20  rgs: str, list. 
+000101e0: 2020 2020 2020 2020 2020 204c 6574 7465             Lette
+000101f0: 7273 2061 6d6f 6e67 2022 7822 2c20 2279  rs among "x", "y
+00010200: 222c 2022 7a22 2c20 2274 2220 616e 6420  ", "z", "t" and 
+00010210: 2266 222c 0a20 2020 2020 2020 2020 2020  "f",.           
+00010220: 206f 7220 6765 6e65 7269 6320 4346 206e   or generic CF n
+00010230: 616d 6573 2e0a 2020 2020 2020 2020 616c  ames..        al
+00010240: 6c6f 775f 706f 7369 7469 6f6e 616c 3a20  low_positional: 
+00010250: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
+00010260: 2046 616c 6c20 6261 636b 2074 6f20 706f   Fall back to po
+00010270: 7369 7469 6f6e 616c 2064 696d 656e 7369  sitional dimensi
+00010280: 6f6e 206f 6620 7479 7065 7320 6973 2075  on of types is u
+00010290: 6e6b 6f77 6e2e 0a20 2020 2020 2020 2070  nkown..        p
+000102a0: 6f73 6974 696f 6e73 3a20 7374 720a 2020  ositions: str.  
+000102b0: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+000102c0: 7420 706f 7369 7469 6f6e 2070 6572 2074  t position per t
+000102d0: 7970 6520 7374 6172 7469 6e67 2066 726f  ype starting fro
+000102e0: 6d20 7468 6520 656e 642e 0a20 2020 2020  m the end..     
+000102f0: 2020 2073 696e 676c 653a 2062 6f6f 6c0a     single: bool.
+00010300: 2020 2020 2020 2020 2020 2020 4966 2054              If T
+00010310: 7275 652c 2072 6574 7572 6e20 7468 6520  rue, return the 
+00010320: 6669 7273 7420 6974 656d 2066 6f75 6e64  first item found
+00010330: 206f 7220 4e6f 6e65 2e0a 2020 2020 2020   or None..      
+00010340: 2020 2020 2020 4966 2046 616c 7365 2c20        If False, 
+00010350: 7265 7475 726e 2061 2070 6f73 7369 626c  return a possibl
+00010360: 6520 656d 7074 7920 6c69 7374 206f 6620  e empty list of 
+00010370: 666f 756e 6420 6974 656d 732e 0a20 2020  found items..   
+00010380: 2020 2020 207b 6572 726f 7273 7d0a 0a20       {errors}.. 
+00010390: 2020 2020 2020 2052 6574 7572 6e0a 2020         Return.  
+000103a0: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
+000103b0: 2020 2020 2074 7570 6c65 0a20 2020 2020       tuple.     
+000103c0: 2020 2020 2020 2054 7570 6c65 206f 6620         Tuple of 
+000103d0: 6469 6d65 6e73 696f 6e20 6e61 6d65 206f  dimension name o
+000103e0: 7220 4e6f 6e65 2077 6865 6e20 7468 6520  r None when the 
+000103f0: 6469 6d65 6e73 696f 6e20 6966 206e 6f74  dimension if not
+00010400: 2066 6f75 6e64 0a0a 2020 2020 2020 2020   found..        
+00010410: 5365 6520 616c 736f 0a20 2020 2020 2020  See also.       
+00010420: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020   --------.      
+00010430: 2020 4346 436f 6f72 6453 7065 6373 2e67    CFCoordSpecs.g
+00010440: 6574 5f64 696d 730a 2020 2020 2020 2020  et_dims.        
+00010450: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00010460: 726e 2073 656c 662e 636f 6f72 6473 2e67  rn self.coords.g
+00010470: 6574 5f64 696d 7328 0a20 2020 2020 2020  et_dims(.       
+00010480: 2020 2020 2064 612c 0a20 2020 2020 2020       da,.       
+00010490: 2020 2020 2063 665f 6172 6773 2c0a 2020       cf_args,.  
+000104a0: 2020 2020 2020 2020 2020 616c 6c6f 775f            allow_
+000104b0: 706f 7369 7469 6f6e 616c 3d61 6c6c 6f77  positional=allow
+000104c0: 5f70 6f73 6974 696f 6e61 6c2c 0a20 2020  _positional,.   
+000104d0: 2020 2020 2020 2020 2070 6f73 6974 696f           positio
+000104e0: 6e73 3d70 6f73 6974 696f 6e73 2c0a 2020  ns=positions,.  
+000104f0: 2020 2020 2020 2020 2020 7369 6e67 6c65            single
+00010500: 3d73 696e 676c 652c 0a20 2020 2020 2020  =single,.       
+00010510: 2020 2020 2065 7272 6f72 733d 6572 726f       errors=erro
+00010520: 7273 2c0a 2020 2020 2020 2020 290a 0a20  rs,.        ).. 
+00010530: 2020 2064 6566 2067 6574 5f61 7869 7328     def get_axis(
+00010540: 7365 6c66 2c20 636f 6f72 642c 206c 6f77  self, coord, low
+00010550: 6572 3d46 616c 7365 293a 0a20 2020 2020  er=False):.     
+00010560: 2020 2022 2222 4765 7420 7468 6520 6469     """Get the di
+00010570: 6d65 6e73 696f 6e20 7479 7065 2c20 6569  mension type, ei
+00010580: 7468 6572 2066 726f 6d20 6178 6973 2061  ther from axis a
+00010590: 7474 7220 6f72 2066 726f 6d20 6d61 7463  ttr or from matc
+000105a0: 6820 4366 2063 6f6f 7264 0a0a 2020 2020  h Cf coord..    
+000105b0: 2020 2020 2e2e 206e 6f74 653a 3a20 5468      .. note:: Th
+000105c0: 6520 6060 6178 6973 6060 2069 7320 7468  e ``axis`` is th
+000105d0: 6520 7570 7065 7263 6173 6520 7665 7273  e uppercase vers
+000105e0: 696f 6e20 6f66 2074 6865 2060 6064 696d  ion of the ``dim
+000105f0: 5f74 7970 6560 600a 0a20 2020 2020 2020  _type``..       
+00010600: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00010610: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00010620: 2020 2020 2020 2063 6f6f 7264 3a20 7861         coord: xa
+00010630: 7272 6179 2e44 6174 6141 7272 6179 0a20  rray.DataArray. 
+00010640: 2020 2020 2020 206c 6f77 6572 3a20 626f         lower: bo
+00010650: 6f6c 0a20 2020 2020 2020 2020 2020 204c  ol.            L
+00010660: 6f77 6572 2063 6173 653f 0a0a 2020 2020  ower case?..    
+00010670: 2020 2020 5265 7475 726e 0a20 2020 2020      Return.     
+00010680: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
+00010690: 2020 7b22 7822 2c20 2279 222c 2022 7a22    {"x", "y", "z"
+000106a0: 2c20 2274 222c 2022 6622 7d2c 204e 6f6e  , "t", "f"}, Non
+000106b0: 650a 0a20 2020 2020 2020 2053 6565 2061  e..        See a
+000106c0: 6c73 6f0a 2020 2020 2020 2020 2d2d 2d2d  lso.        ----
+000106d0: 2d2d 2d2d 0a20 2020 2020 2020 2067 6574  ----.        get
+000106e0: 5f64 696d 5f74 7970 650a 2020 2020 2020  _dim_type.      
+000106f0: 2020 6765 745f 6469 6d5f 7479 7065 730a    get_dim_types.
+00010700: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010710: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00010720: 636f 6f72 6473 2e67 6574 5f61 7869 7328  coords.get_axis(
+00010730: 636f 6f72 642c 206c 6f77 6572 3d6c 6f77  coord, lower=low
+00010740: 6572 290a 0a20 2020 2064 6566 2067 6574  er)..    def get
+00010750: 5f64 696d 5f74 7970 6528 7365 6c66 2c20  _dim_type(self, 
+00010760: 6469 6d2c 2064 613d 4e6f 6e65 2c20 6c6f  dim, da=None, lo
+00010770: 7765 723d 5472 7565 293a 0a20 2020 2020  wer=True):.     
+00010780: 2020 2022 2222 4765 7420 7468 6520 7479     """Get the ty
+00010790: 7065 206f 6620 6120 6469 6d65 6e73 696f  pe of a dimensio
+000107a0: 6e0a 0a20 2020 2020 2020 2054 6872 6565  n..        Three
+000107b0: 2063 6173 6573 3a0a 0a20 2020 2020 2020   cases:..       
+000107c0: 202d 2054 6869 7320 6469 6d65 6e73 696f   - This dimensio
+000107d0: 6e20 6973 2072 6567 6973 7465 7265 6420  n is registered 
+000107e0: 696e 2043 4620 6469 6d73 2e0a 2020 2020  in CF dims..    
+000107f0: 2020 2020 2d20 6f62 6a20 6861 7320 6469      - obj has di
+00010800: 6d20 6173 2064 696d 2061 6e64 2068 6173  m as dim and has
+00010810: 2061 6e20 6178 6973 2061 7474 7269 6275   an axis attribu
+00010820: 7465 2069 6e66 6572 7265 6420 7769 7468  te inferred with
+00010830: 203a 6d65 7468 3a60 6765 745f 6178 6973   :meth:`get_axis
+00010840: 602e 0a20 2020 2020 2020 202d 206f 626a  `..        - obj
+00010850: 2068 6173 2061 2063 6f6f 7264 206e 616d   has a coord nam
+00010860: 6564 2064 696d 2077 6974 6820 616e 2061  ed dim with an a
+00010870: 7869 7320 6174 7472 6962 7574 6520 696e  xis attribute in
+00010880: 6665 7272 6564 2077 6974 6820 3a6d 6574  ferred with :met
+00010890: 683a 6067 6574 5f61 7869 7360 2e0a 0a20  h:`get_axis`... 
+000108a0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+000108b0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000108c0: 2d2d 2d2d 0a20 2020 2020 2020 2064 696d  ----.        dim
+000108d0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+000108e0: 2020 4469 6d65 6e73 696f 6e20 6e61 6d65    Dimension name
+000108f0: 0a20 2020 2020 2020 206f 626a 3a20 7861  .        obj: xa
+00010900: 7272 6179 2e44 6174 6141 7272 6179 2c20  rray.DataArray, 
+00010910: 7861 7272 6179 2e44 6174 6173 6574 0a20  xarray.Dataset. 
+00010920: 2020 2020 2020 2020 2020 2044 6174 6120             Data 
+00010930: 6172 7261 7920 7468 6174 2074 6865 2064  array that the d
+00010940: 696d 656e 7369 6f6e 2062 656c 6f6e 6773  imension belongs
+00010950: 2074 6f2c 2074 6f20 6865 6c70 2069 6e66   to, to help inf
+00010960: 6572 7269 6e67 0a20 2020 2020 2020 2020  erring.         
+00010970: 2020 2074 6865 2074 7970 650a 2020 2020     the type.    
+00010980: 2020 2020 6c6f 7765 723a 2062 6f6f 6c0a      lower: bool.
+00010990: 2020 2020 2020 2020 2020 2020 466f 7220              For 
+000109a0: 6c6f 7765 7220 6361 7365 0a0a 2020 2020  lower case..    
+000109b0: 2020 2020 5265 7475 726e 0a20 2020 2020      Return.     
+000109c0: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
+000109d0: 2020 7374 722c 204e 6f6e 650a 2020 2020    str, None.    
+000109e0: 2020 2020 2020 2020 4c65 7474 6572 2061          Letter a
+000109f0: 7320 6f6e 6520 6f66 2078 2c20 792c 207a  s one of x, y, z
+00010a00: 2c20 7420 6f72 2066 2c20 6966 2066 6f75  , t or f, if fou
+00010a10: 6e64 2c20 656c 7365 204e 6f6e 650a 0a20  nd, else None.. 
+00010a20: 2020 2020 2020 2053 6565 2061 6c73 6f0a         See also.
+00010a30: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00010a40: 0a20 2020 2020 2020 2067 6574 5f61 7869  .        get_axi
+00010a50: 730a 2020 2020 2020 2020 2222 220a 2020  s.        """.  
+00010a60: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00010a70: 662e 636f 6f72 6473 2e67 6574 5f64 696d  f.coords.get_dim
+00010a80: 5f74 7970 6528 6469 6d2c 2064 613d 6461  _type(dim, da=da
+00010a90: 2c20 6c6f 7765 723d 6c6f 7765 7229 0a0a  , lower=lower)..
+00010aa0: 2020 2020 6465 6620 6765 745f 6469 6d5f      def get_dim_
+00010ab0: 7479 7065 7328 7365 6c66 2c20 6461 2c20  types(self, da, 
+00010ac0: 756e 6b6e 6f77 6e3d 4e6f 6e65 2c20 6173  unknown=None, as
+00010ad0: 6469 6374 3d46 616c 7365 293a 0a20 2020  dict=False):.   
+00010ae0: 2020 2020 2022 2222 4765 7420 6120 7475       """Get a tu
+00010af0: 706c 6520 6f66 2074 6865 2064 696d 656e  ple of the dimen
+00010b00: 7369 6f6e 2074 7970 6573 206f 6620 616e  sion types of an
+00010b10: 2061 7272 6179 0a0a 2020 2020 2020 2020   array..        
+00010b20: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00010b30: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00010b40: 2020 2020 2020 6f62 6a3a 2078 6172 7261        obj: xarra
+00010b50: 792e 4461 7461 4172 7261 792c 2074 7570  y.DataArray, tup
+00010b60: 6c65 2873 7472 292c 2078 6172 7261 792e  le(str), xarray.
+00010b70: 4461 7461 7365 740a 2020 2020 2020 2020  Dataset.        
+00010b80: 2020 2020 4461 7461 2061 7272 6179 2c20      Data array, 
+00010b90: 6461 7461 7365 7420 6f72 2074 7570 6c65  dataset or tuple
+00010ba0: 206f 6620 6469 6d65 6e73 696f 6e73 0a20   of dimensions. 
+00010bb0: 2020 2020 2020 2075 6e6b 6e6f 776e 3a0a         unknown:.
+00010bc0: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
+00010bd0: 6520 746f 2061 7373 6967 6e20 7768 656e  e to assign when
+00010be0: 2074 7970 6520 6973 2075 6e6b 6e6f 776e   type is unknown
+00010bf0: 0a20 2020 2020 2020 2061 7364 6963 743a  .        asdict:
+00010c00: 2062 6f6f 6c0a 0a20 2020 2020 2020 2052   bool..        R
+00010c10: 6574 7572 6e0a 2020 2020 2020 2020 2d2d  eturn.        --
+00010c20: 2d2d 2d2d 0a20 2020 2020 2020 2074 7570  ----.        tup
+00010c30: 6c65 2c20 6469 6374 0a20 2020 2020 2020  le, dict.       
+00010c40: 2020 2020 2054 7570 6c65 206f 6620 6469       Tuple of di
+00010c50: 6d65 6e73 696f 6e20 7479 7065 7320 616e  mension types an
+00010c60: 6420 6f66 206c 656e 6774 6820 6060 6f62  d of length ``ob
+00010c70: 6a2e 6e64 696d 6060 2e0a 2020 2020 2020  j.ndim``..      
+00010c80: 2020 2020 2020 4120 6469 6d65 6e73 696f        A dimensio
+00010c90: 6e20 7479 7065 2069 7320 6569 7468 6572  n type is either
+00010ca0: 2061 206c 6574 7465 7220 6f72 2074 6865   a letter or the
+00010cb0: 2060 6075 6e6b 6f77 6e60 6020 7661 6c75   ``unkown`` valu
+00010cc0: 650a 2020 2020 2020 2020 2020 2020 7768  e.            wh
+00010cd0: 656e 2074 6865 2069 6e66 6572 656e 6365  en the inference
+00010ce0: 206f 6620 7479 7065 2068 6173 2066 6169   of type has fai
+00010cf0: 6c65 642e 0a20 2020 2020 2020 2020 2020  led..           
+00010d00: 2049 6620 6060 6173 6469 6374 6060 2069   If ``asdict`` i
+00010d10: 7320 5472 7565 2c20 6120 6469 6374 2069  s True, a dict i
+00010d20: 7320 7265 7475 726e 6564 2069 6e73 7465  s returned inste
+00010d30: 6164 2c0a 2020 2020 2020 2020 2020 2020  ad,.            
+00010d40: 6060 2864 696d 2c20 6469 6d5f 7479 7065  ``(dim, dim_type
+00010d50: 2960 6020 6173 206b 6579 2d76 616c 7565  )`` as key-value
+00010d60: 2070 6169 7273 2e0a 0a20 2020 2020 2020   pairs...       
+00010d70: 2053 6565 2061 6c73 6f0a 2020 2020 2020   See also.      
+00010d80: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020    --------.     
+00010d90: 2020 2067 6574 5f64 696d 5f74 7970 650a     get_dim_type.
+00010da0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010db0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00010dc0: 636f 6f72 6473 2e67 6574 5f64 696d 5f74  coords.get_dim_t
+00010dd0: 7970 6573 2864 612c 2075 6e6b 6e6f 776e  ypes(da, unknown
+00010de0: 3d75 6e6b 6e6f 776e 2c20 6173 6469 6374  =unknown, asdict
+00010df0: 3d61 7364 6963 7429 0a0a 2020 2020 6465  =asdict)..    de
+00010e00: 6620 7061 7273 655f 6469 6d73 2873 656c  f parse_dims(sel
+00010e10: 662c 2064 696d 732c 206f 626a 293a 0a20  f, dims, obj):. 
+00010e20: 2020 2020 2020 2022 2222 436f 6e76 6572         """Conver
+00010e30: 7420 6672 6f6d 2067 656e 6572 6963 2064  t from generic d
+00010e40: 696d 206e 616d 6573 2074 6f20 7370 6563  im names to spec
+00010e50: 6961 6c69 7a65 6420 6e61 6d65 730a 0a20  ialized names.. 
+00010e60: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00010e70: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00010e80: 2d2d 2d2d 0a20 2020 2020 2020 2064 696d  ----.        dim
+00010e90: 733a 2073 7472 2c20 7475 706c 652c 206c  s: str, tuple, l
+00010ea0: 6973 742c 2064 6963 740a 2020 2020 2020  ist, dict.      
+00010eb0: 2020 6f62 6a3a 2078 6172 7261 792e 4461    obj: xarray.Da
+00010ec0: 7461 7365 742c 2078 6172 7261 792e 4461  taset, xarray.Da
+00010ed0: 7461 4172 7261 790a 0a20 2020 2020 2020  taArray..       
+00010ee0: 2052 6574 7572 6e0a 2020 2020 2020 2020   Return.        
+00010ef0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2053  ------.        S
+00010f00: 616d 6520 7479 7065 2061 7320 6469 6d73  ame type as dims
+00010f10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010f20: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00010f30: 2e63 6f6f 7264 732e 7061 7273 655f 6469  .coords.parse_di
+00010f40: 6d73 2864 696d 732c 206f 626a 290a 0a20  ms(dims, obj).. 
+00010f50: 2020 2064 6566 2069 6e66 6572 5f63 6f6f     def infer_coo
+00010f60: 7264 7328 7365 6c66 2c20 6473 293a 0a20  rds(self, ds):. 
+00010f70: 2020 2020 2020 2022 2222 5365 6172 6368         """Search
+00010f80: 2066 6f72 206b 6e6f 776e 2063 6f6f 7264   for known coord
+00010f90: 7320 616e 6420 6d61 6b65 2073 7572 6520  s and make sure 
+00010fa0: 7468 6579 2061 7265 2073 6574 2061 7320  they are set as 
+00010fb0: 636f 6f72 6473 0a0a 2020 2020 2020 2020  coords..        
+00010fc0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00010fd0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00010fe0: 2020 2020 2020 6473 3a20 7861 7272 6179        ds: xarray
+00010ff0: 2e44 6174 6173 6574 0a0a 2020 2020 2020  .Dataset..      
+00011000: 2020 5265 7475 726e 0a20 2020 2020 2020    Return.       
+00011010: 202d 2d2d 2d2d 2d0a 2020 2020 2020 2020   ------.        
+00011020: 7861 7272 6179 2e44 6174 6173 6574 0a20  xarray.Dataset. 
+00011030: 2020 2020 2020 2020 2020 204e 6577 2064             New d
+00011040: 6174 6173 6574 2077 6974 6820 706f 7465  ataset with pote
+00011050: 6e74 6961 6c6c 7920 7570 6461 7465 6420  ntially updated 
+00011060: 636f 6f72 6469 6e61 7465 730a 2020 2020  coordinates.    
+00011070: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011080: 6966 2068 6173 6174 7472 2864 732c 2022  if hasattr(ds, "
+00011090: 6461 7461 5f76 6172 7322 293a 0a20 2020  data_vars"):.   
+000110a0: 2020 2020 2020 2020 2066 6f72 2064 6120           for da 
+000110b0: 696e 2064 732e 6461 7461 5f76 6172 732e  in ds.data_vars.
+000110c0: 7661 6c75 6573 2829 3a0a 2020 2020 2020  values():.      
+000110d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000110e0: 662e 636f 6f72 6473 2e6d 6174 6368 2864  f.coords.match(d
+000110f0: 6129 3a0a 2020 2020 2020 2020 2020 2020  a):.            
+00011100: 2020 2020 2020 2020 6473 203d 2064 732e          ds = ds.
+00011110: 7365 745f 636f 6f72 6473 2864 612e 6e61  set_coords(da.na
+00011120: 6d65 290a 2020 2020 2020 2020 7265 7475  me).        retu
+00011130: 726e 2064 732e 636f 7079 2829 0a0a 0a63  rn ds.copy()...c
+00011140: 6c61 7373 205f 4346 4361 7453 7065 6373  lass _CFCatSpecs
+00011150: 5f28 6f62 6a65 6374 293a 0a20 2020 2022  _(object):.    "
+00011160: 2222 4261 7365 2063 6c61 7373 2066 6f72  ""Base class for
+00011170: 206c 6f61 6469 6e67 2064 6174 615f 7661   loading data_va
+00011180: 7273 2061 6e64 2063 6f6f 7264 7320 4346  rs and coords CF
+00011190: 2073 7065 6369 6669 6361 7469 6f6e 7322   specifications"
+000111a0: 2222 0a0a 2020 2020 6361 7465 676f 7279  ""..    category
+000111b0: 203d 204e 6f6e 650a 0a20 2020 2061 7474   = None..    att
+000111c0: 7273 5f65 7863 6c75 6465 203d 205b 0a20  rs_exclude = [. 
+000111d0: 2020 2020 2020 2022 6e61 6d65 222c 0a20         "name",. 
+000111e0: 2020 2020 2020 2022 696e 6865 7269 7422         "inherit"
+000111f0: 2c0a 2020 2020 2020 2020 2263 6f6f 7264  ,.        "coord
+00011200: 7322 2c0a 2020 2020 2020 2020 2273 656c  s",.        "sel
+00011210: 6563 7422 2c0a 2020 2020 2020 2020 2273  ect",.        "s
+00011220: 6561 7263 685f 6f72 6465 7222 2c0a 2020  earch_order",.  
+00011230: 2020 2020 2020 2263 6d61 7022 2c0a 2020        "cmap",.  
+00011240: 2020 5d0a 0a20 2020 2061 7474 7273 5f66    ]..    attrs_f
+00011250: 6972 7374 203d 205b 0a20 2020 2020 2020  irst = [.       
+00011260: 2022 6e61 6d65 222c 0a20 2020 2020 2020   "name",.       
+00011270: 2022 7374 616e 6461 7264 5f6e 616d 6522   "standard_name"
+00011280: 2c0a 2020 2020 2020 2020 226c 6f6e 675f  ,.        "long_
+00011290: 6e61 6d65 222c 0a20 2020 2020 2020 2022  name",.        "
+000112a0: 756e 6974 7322 2c0a 2020 2020 5d0a 0a20  units",.    ].. 
+000112b0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000112c0: 7365 6c66 2c20 7061 7265 6e74 293a 0a20  self, parent):. 
+000112d0: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+000112e0: 6c66 2e63 6174 6567 6f72 7920 696e 2070  lf.category in p
+000112f0: 6172 656e 740a 2020 2020 2020 2020 7365  arent.        se
+00011300: 6c66 2e70 6172 656e 7420 3d20 7061 7265  lf.parent = pare
+00011310: 6e74 0a0a 2020 2020 4070 726f 7065 7274  nt..    @propert
+00011320: 790a 2020 2020 6465 6620 636f 6f72 6473  y.    def coords
+00011330: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00011340: 7265 7475 726e 2073 656c 662e 7061 7265  return self.pare
+00011350: 6e74 2e63 6f6f 7264 730a 0a20 2020 2040  nt.coords..    @
+00011360: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00011370: 2064 6174 615f 7661 7273 2873 656c 6629   data_vars(self)
+00011380: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00011390: 2073 656c 662e 7061 7265 6e74 2e64 6174   self.parent.dat
+000113a0: 615f 7661 7273 0a0a 2020 2020 4070 726f  a_vars..    @pro
+000113b0: 7065 7274 790a 2020 2020 6465 6620 7367  perty.    def sg
+000113c0: 6c6f 6361 746f 7228 7365 6c66 293a 0a20  locator(self):. 
+000113d0: 2020 2020 2020 2022 2222 3a63 6c61 7373         """:class
+000113e0: 3a60 5347 4c6f 6361 746f 7260 2069 6e73  :`SGLocator` ins
+000113f0: 7461 6e63 6522 2222 0a20 2020 2020 2020  tance""".       
+00011400: 2072 6574 7572 6e20 7365 6c66 2e70 6172   return self.par
+00011410: 656e 742e 7367 6c6f 6361 746f 720a 0a20  ent.sglocator.. 
+00011420: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00011430: 2064 6566 205f 6469 6374 2873 656c 6629   def _dict(self)
+00011440: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00011450: 2073 656c 662e 7061 7265 6e74 2e5f 6469   self.parent._di
+00011460: 6374 5b73 656c 662e 6361 7465 676f 7279  ct[self.category
+00011470: 5d0a 0a20 2020 2064 6566 205f 5f67 6574  ]..    def __get
+00011480: 6974 656d 5f5f 2873 656c 662c 206b 6579  item__(self, key
+00011490: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+000114a0: 6e20 7365 6c66 2e67 6574 5f73 7065 6373  n self.get_specs
+000114b0: 286b 6579 290a 0a20 2020 2064 6566 205f  (key)..    def _
+000114c0: 5f69 7465 725f 5f28 7365 6c66 293a 0a20  _iter__(self):. 
+000114d0: 2020 2020 2020 2072 6574 7572 6e20 6974         return it
+000114e0: 6572 2873 656c 662e 5f64 6963 7429 0a0a  er(self._dict)..
+000114f0: 2020 2020 6465 6620 5f5f 6c65 6e5f 5f28      def __len__(
+00011500: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+00011510: 6574 7572 6e20 6c65 6e28 7365 6c66 2e5f  eturn len(self._
+00011520: 6469 6374 290a 0a20 2020 2064 6566 205f  dict)..    def _
+00011530: 5f63 6f6e 7461 696e 735f 5f28 7365 6c66  _contains__(self
+00011540: 2c20 6b65 7929 3a0a 2020 2020 2020 2020  , key):.        
+00011550: 7265 7475 726e 206b 6579 2069 6e20 7365  return key in se
+00011560: 6c66 2e5f 6469 6374 0a0a 2020 2020 2320  lf._dict..    # 
+00011570: 6465 6620 5f5f 7374 725f 5f28 7365 6c66  def __str__(self
+00011580: 293a 0a20 2020 2023 2020 2020 2072 6574  ):.    #     ret
+00011590: 7572 6e20 7066 6f72 6d61 7428 7365 6c66  urn pformat(self
+000115a0: 2e5f 6469 6374 290a 0a20 2020 2064 6566  ._dict)..    def
+000115b0: 205f 7661 6c69 6461 7465 5f6e 616d 655f   _validate_name_
+000115c0: 2873 656c 662c 206e 616d 6529 3a0a 2020  (self, name):.  
+000115d0: 2020 2020 2020 6966 206e 616d 6520 696e        if name in
+000115e0: 2073 656c 663a 0a20 2020 2020 2020 2020   self:.         
+000115f0: 2020 2072 6574 7572 6e20 6e61 6d65 0a0a     return name..
+00011600: 2020 2020 6465 6620 5f61 7373 6572 745f      def _assert_
+00011610: 6b6e 6f77 6e5f 2873 656c 662c 206e 616d  known_(self, nam
+00011620: 652c 2065 7272 6f72 733d 2272 6169 7365  e, errors="raise
+00011630: 2229 3a0a 2020 2020 2020 2020 6966 206e  "):.        if n
+00011640: 616d 6520 6e6f 7420 696e 2073 656c 662e  ame not in self.
+00011650: 5f64 6963 743a 0a20 2020 2020 2020 2020  _dict:.         
+00011660: 2020 2069 6620 6572 726f 7273 203d 3d20     if errors == 
+00011670: 2272 6169 7365 223a 0a20 2020 2020 2020  "raise":.       
+00011680: 2020 2020 2020 2020 2072 6169 7365 2058           raise X
+00011690: 6f61 4346 4572 726f 7228 6622 496e 7661  oaCFError(f"Inva
+000116a0: 6c69 6420 7b73 656c 662e 6361 7465 676f  lid {self.catego
+000116b0: 7279 7d20 4346 2073 7065 6373 206e 616d  ry} CF specs nam
+000116c0: 653a 2022 202b 206e 616d 6529 0a20 2020  e: " + name).   
+000116d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000116e0: 4661 6c73 650a 2020 2020 2020 2020 7265  False.        re
+000116f0: 7475 726e 2054 7275 650a 0a20 2020 2040  turn True..    @
+00011700: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00011710: 206e 616d 6573 2873 656c 6629 3a0a 2020   names(self):.  
+00011720: 2020 2020 2020 7265 7475 726e 205b 6b65        return [ke
+00011730: 7920 666f 7220 6b65 7920 696e 2073 656c  y for key in sel
+00011740: 662e 5f64 6963 742e 6b65 7973 2829 2069  f._dict.keys() i
+00011750: 6620 6e6f 7420 6b65 792e 7374 6172 7473  f not key.starts
+00011760: 7769 7468 2822 5f22 295d 0a0a 2020 2020  with("_")]..    
+00011770: 6465 6620 6974 656d 7328 7365 6c66 293a  def items(self):
+00011780: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011790: 7365 6c66 2e5f 6469 6374 2e69 7465 6d73  self._dict.items
+000117a0: 2829 0a0a 2020 2020 6465 6620 6b65 7973  ()..    def keys
+000117b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000117c0: 7265 7475 726e 2073 656c 662e 5f64 6963  return self._dic
+000117d0: 742e 6b65 7973 2829 0a0a 2020 2020 6465  t.keys()..    de
+000117e0: 6620 6765 745f 7370 6563 7328 7365 6c66  f get_specs(self
+000117f0: 2c20 6e61 6d65 2c20 6572 726f 7273 3d22  , name, errors="
+00011800: 7761 726e 2229 3a0a 2020 2020 2020 2020  warn"):.        
+00011810: 2222 2247 6574 2074 6865 2073 7065 6373  """Get the specs
+00011820: 206f 6620 6120 6366 2069 7465 6d0a 0a20   of a cf item.. 
+00011830: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00011840: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00011850: 2d2d 2d2d 0a20 2020 2020 2020 206e 616d  ----.        nam
+00011860: 653a 2073 7472 0a20 2020 2020 2020 2065  e: str.        e
+00011870: 7272 6f72 733a 2022 6967 6e6f 7265 222c  rrors: "ignore",
+00011880: 2022 7761 726e 696e 6722 206f 7220 2272   "warning" or "r
+00011890: 6169 7365 222e 0a0a 2020 2020 2020 2020  aise"...        
+000118a0: 5265 7475 726e 0a20 2020 2020 2020 202d  Return.        -
+000118b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6469  -----.        di
+000118c0: 6374 206f 7220 4e6f 6e65 0a20 2020 2020  ct or None.     
+000118d0: 2020 2022 2222 0a20 2020 2020 2020 2065     """.        e
+000118e0: 7272 6f72 7320 3d20 4552 524f 5253 5b65  rrors = ERRORS[e
+000118f0: 7272 6f72 735d 0a20 2020 2020 2020 2069  rrors].        i
+00011900: 6620 6e61 6d65 206e 6f74 2069 6e20 7365  f name not in se
+00011910: 6c66 2e5f 6469 6374 3a0a 2020 2020 2020  lf._dict:.      
+00011920: 2020 2020 2020 6966 2065 7272 6f72 7320        if errors 
+00011930: 3d3d 2022 7261 6973 6522 3a0a 2020 2020  == "raise":.    
+00011940: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00011950: 6520 586f 6143 4645 7272 6f72 2822 4361  e XoaCFError("Ca
+00011960: 6e27 7420 6765 7420 6366 2073 7065 6373  n't get cf specs
+00011970: 2066 726f 6d3a 2022 202b 206e 616d 6529   from: " + name)
+00011980: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011990: 6572 726f 7273 203d 3d20 2277 6172 6e22  errors == "warn"
+000119a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000119b0: 2020 786f 615f 7761 726e 2822 496e 7661    xoa_warn("Inva
+000119c0: 6c69 6420 6366 206e 616d 653a 2022 202b  lid cf name: " +
+000119d0: 2073 7472 286e 616d 6529 290a 2020 2020   str(name)).    
+000119e0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+000119f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00011a00: 6c66 2e5f 6469 6374 5b6e 616d 655d 0a0a  lf._dict[name]..
+00011a10: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00011a20: 2020 6465 6620 6469 6d73 2873 656c 6629    def dims(self)
+00011a30: 3a0a 2020 2020 2020 2020 2222 2244 6963  :.        """Dic
+00011a40: 7420 6f66 2064 696d 206e 616d 6573 2070  t of dim names p
+00011a50: 6572 2074 7970 6522 2222 0a20 2020 2020  er type""".     
+00011a60: 2020 2072 6574 7572 6e20 7365 6c66 2e70     return self.p
+00011a70: 6172 656e 742e 5f64 6963 745b 2764 696d  arent._dict['dim
+00011a80: 7327 5d0a 0a20 2020 2064 6566 2073 6574  s']..    def set
+00011a90: 5f73 7065 6373 2873 656c 662c 2069 7465  _specs(self, ite
+00011aa0: 6d2c 202a 2a73 7065 6373 293a 0a20 2020  m, **specs):.   
+00011ab0: 2020 2020 2022 2222 5570 6461 7465 206f       """Update o
+00011ac0: 7220 6372 6561 7465 2073 7065 6373 2066  r create specs f
+00011ad0: 6f72 2061 6e20 6974 656d 2222 220a 2020  or an item""".  
+00011ae0: 2020 2020 2020 6461 7461 203d 207b 7365        data = {se
+00011af0: 6c66 2e63 6174 6567 6f72 793a 207b 6974  lf.category: {it
+00011b00: 656d 3a20 7370 6563 737d 7d0a 2020 2020  em: specs}}.    
+00011b10: 2020 2020 7365 6c66 2e70 6172 656e 742e      self.parent.
+00011b20: 6c6f 6164 5f63 6667 2864 6174 6129 0a0a  load_cfg(data)..
+00011b30: 2020 2020 6465 6620 7365 745f 7370 6563      def set_spec
+00011b40: 735f 6672 6f6d 5f63 6667 2873 656c 662c  s_from_cfg(self,
+00011b50: 2063 6667 293a 0a20 2020 2020 2020 2022   cfg):.        "
+00011b60: 2222 5570 6461 7465 206f 7220 6372 6561  ""Update or crea
+00011b70: 7465 2073 7065 6373 2066 6f72 2073 6576  te specs for sev
+00011b80: 6572 616c 2069 7465 6d20 7769 7468 2061  eral item with a
+00011b90: 2063 6f6e 6669 6720 7370 6563 7322 2222   config specs"""
+00011ba0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00011bb0: 7374 616e 6365 2863 6667 2c20 6469 6374  stance(cfg, dict
+00011bc0: 2920 616e 6420 7365 6c66 2e63 6174 6567  ) and self.categ
+00011bd0: 6f72 7920 6e6f 7420 696e 2063 6667 3a0a  ory not in cfg:.
+00011be0: 2020 2020 2020 2020 2020 2020 6366 6720              cfg 
+00011bf0: 3d20 7b73 656c 662e 6361 7465 676f 7279  = {self.category
+00011c00: 3a20 6366 677d 0a20 2020 2020 2020 2073  : cfg}.        s
+00011c10: 656c 662e 7061 7265 6e74 2e6c 6f61 645f  elf.parent.load_
+00011c20: 6366 6728 6366 6729 0a0a 2020 2020 6465  cfg(cfg)..    de
+00011c30: 6620 6765 745f 616c 6c6f 7765 645f 6e61  f get_allowed_na
+00011c40: 6d65 7328 7365 6c66 2c20 6366 5f6e 616d  mes(self, cf_nam
+00011c50: 6529 3a0a 2020 2020 2020 2020 2222 2247  e):.        """G
+00011c60: 6574 2074 6865 206c 6973 7420 6f66 2061  et the list of a
+00011c70: 6c6c 6f77 6564 206e 616d 6573 2066 6f72  llowed names for
+00011c80: 2061 2067 6976 656e 2060 6366 5f6e 616d   a given `cf_nam
+00011c90: 6560 0a0a 2020 2020 2020 2020 4974 2069  e`..        It i
+00011ca0: 6e63 6c75 6465 7320 6465 2060 6366 5f6e  ncludes de `cf_n
+00011cb0: 616d 6560 2069 7473 656c 662c 2074 6865  ame` itself, the
+00011cc0: 2060 6e61 6d65 6020 616c 745f 6e61 6d65   `name` alt_name
+00011cd0: 7360 2073 7065 6369 6669 6361 7469 6f6e  s` specification
+00011ce0: 2076 616c 7565 730a 0a20 2020 2020 2020   values..       
+00011cf0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00011d00: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00011d10: 2020 2020 2020 2063 665f 6e61 6d65 3a20         cf_name: 
+00011d20: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00011d30: 5661 6c69 6420 4346 206e 616d 650a 0a20  Valid CF name.. 
+00011d40: 2020 2020 2020 2052 6574 7572 6e0a 2020         Return.  
+00011d50: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
+00011d60: 2020 2020 206c 6973 740a 2020 2020 2020       list.      
+00011d70: 2020 2222 220a 2020 2020 2020 2020 7370    """.        sp
+00011d80: 6563 7320 3d20 7365 6c66 5b63 665f 6e61  ecs = self[cf_na
+00011d90: 6d65 5d0a 2020 2020 2020 2020 616c 6c6f  me].        allo
+00011da0: 7765 645f 6e61 6d65 7320 3d20 5b63 665f  wed_names = [cf_
+00011db0: 6e61 6d65 5d0a 2020 2020 2020 2020 6966  name].        if
+00011dc0: 2022 6e61 6d65 2220 696e 2073 7065 6373   "name" in specs
+00011dd0: 2061 6e64 2073 7065 6373 5b22 6e61 6d65   and specs["name
+00011de0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+00011df0: 616c 6c6f 7765 645f 6e61 6d65 732e 6170  allowed_names.ap
+00011e00: 7065 6e64 2873 7065 6373 5b22 6e61 6d65  pend(specs["name
+00011e10: 225d 290a 2020 2020 2020 2020 6966 2022  "]).        if "
+00011e20: 616c 745f 6e61 6d65 7322 2069 6e20 7370  alt_names" in sp
+00011e30: 6563 733a 0a20 2020 2020 2020 2020 2020  ecs:.           
+00011e40: 2061 6c6c 6f77 6564 5f6e 616d 6573 2e65   allowed_names.e
+00011e50: 7874 656e 6428 7370 6563 735b 2261 6c74  xtend(specs["alt
+00011e60: 5f6e 616d 6573 225d 290a 2020 2020 2020  _names"]).      
+00011e70: 2020 7265 7475 726e 2061 6c6c 6f77 6564    return allowed
+00011e80: 5f6e 616d 6573 0a0a 2020 2020 6465 6620  _names..    def 
+00011e90: 6765 745f 6c6f 635f 6d61 7070 696e 6728  get_loc_mapping(
+00011ea0: 7365 6c66 2c20 6f62 6a2c 2063 665f 6e61  self, obj, cf_na
+00011eb0: 6d65 733d 4e6f 6e65 293a 0a20 2020 2020  mes=None):.     
+00011ec0: 2020 2072 6574 7572 6e20 7365 6c66 2e70     return self.p
+00011ed0: 6172 656e 742e 6765 745f 6c6f 635f 6d61  arent.get_loc_ma
+00011ee0: 7070 696e 6728 0a20 2020 2020 2020 2020  pping(.         
+00011ef0: 2020 206f 626a 2c20 6366 5f6e 616d 6573     obj, cf_names
+00011f00: 3d63 665f 6e61 6d65 732c 2063 6174 6567  =cf_names, categ
+00011f10: 6f72 6965 733d 5b22 636f 6f72 6473 222c  ories=["coords",
+00011f20: 2022 6461 7461 5f76 6172 7322 5d0a 2020   "data_vars"].  
+00011f30: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00011f40: 205f 6765 745f 6f72 6465 7265 645f 6d61   _get_ordered_ma
+00011f50: 7463 685f 7370 6563 735f 2873 656c 662c  tch_specs_(self,
+00011f60: 2063 665f 6e61 6d65 293a 0a20 2020 2020   cf_name):.     
+00011f70: 2020 2073 7065 6373 203d 2073 656c 665b     specs = self[
+00011f80: 6366 5f6e 616d 655d 0a20 2020 2020 2020  cf_name].       
+00011f90: 206d 6174 6368 5f73 7065 6373 203d 207b   match_specs = {
+00011fa0: 7d0a 2020 2020 2020 2020 666f 7220 736d  }.        for sm
+00011fb0: 2069 6e20 7370 6563 735b 2273 6561 7263   in specs["searc
+00011fc0: 685f 6f72 6465 7222 5d3a 0a20 2020 2020  h_order"]:.     
+00011fd0: 2020 2020 2020 2066 6f72 2061 7474 7220         for attr 
+00011fe0: 696e 2028 0a20 2020 2020 2020 2020 2020  in (.           
+00011ff0: 2020 2020 2022 6e61 6d65 222c 0a20 2020       "name",.   
+00012000: 2020 2020 2020 2020 2020 2020 2022 7374               "st
+00012010: 616e 6461 7264 5f6e 616d 6522 2c0a 2020  andard_name",.  
+00012020: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00012030: 6f6e 675f 6e61 6d65 222c 0a20 2020 2020  ong_name",.     
+00012040: 2020 2020 2020 2020 2020 2022 6178 6973             "axis
+00012050: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00012060: 2020 2022 756e 6974 7322 2c0a 2020 2020     "units",.    
+00012070: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+00012080: 2020 2020 2020 2020 2020 2069 6620 6174             if at
+00012090: 7472 5b30 5d20 213d 2073 6d3a 0a20 2020  tr[0] != sm:.   
+000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120b0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+000120c0: 2020 2020 2020 2020 2020 2320 6966 2061            # if a
+000120d0: 7474 7220 3d3d 2022 6e61 6d65 2220 616e  ttr == "name" an
+000120e0: 6420 226e 616d 6522 2069 6e20 7370 6563  d "name" in spec
+000120f0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00012100: 2020 2069 6620 6174 7472 203d 3d20 226e     if attr == "n
+00012110: 616d 6522 3a0a 2020 2020 2020 2020 2020  ame":.          
+00012120: 2020 2020 2020 2020 2020 6d61 7463 685f            match_
+00012130: 7370 6563 735b 226e 616d 6522 5d20 3d20  specs["name"] = 
+00012140: 7365 6c66 2e67 6574 5f61 6c6c 6f77 6564  self.get_allowed
+00012150: 5f6e 616d 6573 2863 665f 6e61 6d65 290a  _names(cf_name).
+00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012170: 656c 6966 2022 6174 7472 7322 2069 6e20  elif "attrs" in 
+00012180: 7370 6563 7320 616e 6420 6174 7472 2069  specs and attr i
+00012190: 6e20 7370 6563 735b 2261 7474 7273 225d  n specs["attrs"]
+000121a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000121b0: 2020 2020 2020 6d61 7463 685f 7370 6563        match_spec
+000121c0: 735b 6174 7472 5d20 3d20 7370 6563 735b  s[attr] = specs[
+000121d0: 2261 7474 7273 225d 5b61 7474 725d 0a20  "attrs"][attr]. 
+000121e0: 2020 2020 2020 2072 6574 7572 6e20 6d61         return ma
+000121f0: 7463 685f 7370 6563 730a 0a20 2020 2064  tch_specs..    d
+00012200: 6566 206d 6174 6368 2873 656c 662c 2064  ef match(self, d
+00012210: 612c 2063 665f 6e61 6d65 3d4e 6f6e 652c  a, cf_name=None,
+00012220: 206c 6f63 3d4e 6f6e 6529 3a0a 2020 2020   loc=None):.    
+00012230: 2020 2020 2222 2243 6865 636b 2069 6620      """Check if 
+00012240: 6461 2061 7474 7269 6275 7465 7320 6d61  da attributes ma
+00012250: 7463 6820 6769 7665 6e20 6f72 2061 6e79  tch given or any
+00012260: 2073 7065 6373 0a0a 2020 2020 2020 2020   specs..        
+00012270: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00012280: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00012290: 2020 2020 2020 6461 3a20 7861 7272 6179        da: xarray
+000122a0: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
+000122b0: 2020 2063 665f 6e61 6d65 3a20 7374 722c     cf_name: str,
+000122c0: 2064 6963 742c 204e 6f6e 650a 2020 2020   dict, None.    
+000122d0: 2020 2020 2020 2020 4346 206e 616d 652e          CF name.
+000122e0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+000122f0: 4e6f 6e65 2c20 616c 6c20 6e61 6d65 7320  None, all names 
+00012300: 6172 6520 7573 6564 2e0a 2020 2020 2020  are used..      
+00012310: 2020 2020 2020 4966 2061 2064 6963 742c        If a dict,
+00012320: 206e 616d 6520 6973 2069 6e74 6572 7072   name is interpr
+00012330: 6574 6564 2061 7320 616e 2065 7870 6c69  eted as an expli
+00012340: 6369 7420 7365 7420 6f66 0a20 2020 2020  cit set of.     
+00012350: 2020 2020 2020 2073 7065 6369 6669 6361         specifica
+00012360: 7469 6f6e 732e 0a20 2020 2020 2020 206c  tions..        l
+00012370: 6f63 3a20 7374 722c 207b 2261 6e79 222c  oc: str, {"any",
+00012380: 204e 6f6e 657d 2c20 7b22 222c 2046 616c   None}, {"", Fal
+00012390: 7365 7d0a 2020 2020 2020 2020 2020 2020  se}.            
+000123a0: 2d20 7374 723a 206f 6e65 206f 6620 7468  - str: one of th
+000123b0: 6573 6520 6c6f 6361 7469 6f6e 730a 2020  ese locations.  
+000123c0: 2020 2020 2020 2020 2020 2d20 4e6f 6e65            - None
+000123d0: 206f 7220 2261 6e79 223a 2061 6e79 0a20   or "any": any. 
+000123e0: 2020 2020 2020 2020 2020 202d 2046 616c             - Fal
+000123f0: 7365 206f 7220 2722 223a 206e 6f20 6c6f  se or '"": no lo
+00012400: 6361 7469 6f6e 0a0a 2020 2020 2020 2020  cation..        
+00012410: 5265 7475 726e 0a20 2020 2020 2020 202d  Return.        -
+00012420: 2d2d 2d2d 2d0a 2020 2020 2020 2020 626f  -----.        bo
+00012430: 6f6c 2c20 7374 720a 2020 2020 2020 2020  ol, str.        
+00012440: 2020 2020 5472 7565 206f 7220 4661 6c73      True or Fals
+00012450: 6520 6966 206e 616d 6520 6973 2070 726f  e if name is pro
+00012460: 7669 6465 642c 2065 6c73 6520 666f 756e  vided, else foun
+00012470: 6420 6e61 6d65 206f 7220 4e6f 6e65 0a20  d name or None. 
+00012480: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012490: 2020 2069 6620 6366 5f6e 616d 653a 0a20     if cf_name:. 
+000124a0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+000124b0: 696e 7374 616e 6365 2863 665f 6e61 6d65  instance(cf_name
+000124c0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+000124d0: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
+000124e0: 7365 7274 5f6b 6e6f 776e 5f28 6366 5f6e  sert_known_(cf_n
+000124f0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+00012500: 206e 616d 6573 203d 205b 6366 5f6e 616d   names = [cf_nam
+00012510: 655d 0a20 2020 2020 2020 2065 6c73 653a  e].        else:
+00012520: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+00012530: 6573 203d 2073 656c 662e 6e61 6d65 730a  es = self.names.
+00012540: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
+00012550: 5f20 696e 206e 616d 6573 3a0a 0a20 2020  _ in names:..   
+00012560: 2020 2020 2020 2020 2023 2047 6574 206d           # Get m
+00012570: 6174 6368 2073 7065 6373 0a20 2020 2020  atch specs.     
+00012580: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00012590: 616e 6365 286e 616d 655f 2c20 6469 6374  ance(name_, dict
+000125a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000125b0: 2020 206d 6174 6368 5f73 7065 6373 203d     match_specs =
+000125c0: 206e 616d 655f 0a20 2020 2020 2020 2020   name_.         
+000125d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000125e0: 2020 2020 2020 2020 206d 6174 6368 5f73           match_s
+000125f0: 7065 6373 203d 2073 656c 662e 5f67 6574  pecs = self._get
+00012600: 5f6f 7264 6572 6564 5f6d 6174 6368 5f73  _ordered_match_s
+00012610: 7065 6373 5f28 6e61 6d65 5f29 0a0a 2020  pecs_(name_)..  
+00012620: 2020 2020 2020 2020 2020 2320 4c6f 6f70            # Loop
+00012630: 206f 6e20 6d61 7463 6820 7370 6563 730a   on match specs.
+00012640: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00012650: 6174 7472 2c20 7265 6673 2069 6e20 6d61  attr, refs in ma
+00012660: 7463 685f 7370 6563 732e 6974 656d 7328  tch_specs.items(
+00012670: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00012680: 2020 2076 616c 7565 203d 2067 6574 6174     value = getat
+00012690: 7472 2864 612c 2061 7474 722c 204e 6f6e  tr(da, attr, Non
+000126a0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+000126b0: 2020 2069 6620 7661 6c75 6520 6973 204e     if value is N
+000126c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000126d0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+000126e0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000126f0: 2020 666f 7220 7265 6620 696e 2072 6566    for ref in ref
+00012700: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00012710: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
+00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012730: 2020 2020 6174 7472 2069 6e20 7365 6c66      attr in self
+00012740: 2e73 676c 6f63 6174 6f72 2e76 616c 6964  .sglocator.valid
+00012750: 5f61 7474 7273 0a20 2020 2020 2020 2020  _attrs.         
+00012760: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00012770: 6e64 2073 656c 662e 7367 6c6f 6361 746f  nd self.sglocato
+00012780: 722e 6d61 7463 685f 6174 7472 2861 7474  r.match_attr(att
+00012790: 722c 2076 616c 7565 2c20 7265 662c 206c  r, value, ref, l
+000127a0: 6f63 3d6c 6f63 290a 2020 2020 2020 2020  oc=loc).        
+000127b0: 2020 2020 2020 2020 2020 2020 2920 6f72              ) or
+000127c0: 206d 6174 6368 5f73 7472 696e 6728 7661   match_string(va
+000127d0: 6c75 652c 2072 6566 2c20 6967 6e6f 7265  lue, ref, ignore
+000127e0: 6361 7365 3d54 7275 6529 3a0a 2020 2020  case=True):.    
+000127f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012800: 2020 2020 6461 2e65 6e63 6f64 696e 675b      da.encoding[
+00012810: 2263 665f 6e61 6d65 225d 203d 206e 616d  "cf_name"] = nam
+00012820: 655f 0a20 2020 2020 2020 2020 2020 2020  e_.             
+00012830: 2020 2020 2020 2020 2020 2064 612e 656e             da.en
+00012840: 636f 6469 6e67 5b22 6366 5f63 6174 6567  coding["cf_categ
+00012850: 6f72 7922 5d20 3d20 7365 6c66 2e63 6174  ory"] = self.cat
+00012860: 6567 6f72 790a 2020 2020 2020 2020 2020  egory.          
+00012870: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00012880: 7475 726e 2054 7275 6520 6966 2063 665f  turn True if cf_
+00012890: 6e61 6d65 2065 6c73 6520 6e61 6d65 5f0a  name else name_.
+000128a0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+000128b0: 616c 7365 2069 6620 6366 5f6e 616d 6520  alse if cf_name 
+000128c0: 656c 7365 204e 6f6e 650a 0a20 2020 2064  else None..    d
+000128d0: 6566 206d 6174 6368 5f66 726f 6d5f 6e61  ef match_from_na
+000128e0: 6d65 2873 656c 662c 206e 616d 652c 2063  me(self, name, c
+000128f0: 665f 6e61 6d65 3d4e 6f6e 652c 206c 6f63  f_name=None, loc
+00012900: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00012910: 2222 2247 6574 2074 6865 2067 656e 6572  """Get the gener
+00012920: 6963 2043 4620 6e61 6d65 206f 6620 616e  ic CF name of an
+00012930: 206f 626a 6563 7420 6b6e 6f77 696e 6720   object knowing 
+00012940: 6f6e 6c79 2069 7473 206e 616d 650a 0a20  only its name.. 
+00012950: 2020 2020 2020 2049 7420 636f 6d70 6172         It compar
+00012960: 6573 2060 6e61 6d65 6020 746f 2074 6865  es `name` to the
+00012970: 2060 6e61 6d65 6020 616e 6420 6061 6c74   `name` and `alt
+00012980: 5f6e 616d 6573 6020 636f 6e66 6967 2076  _names` config v
+00012990: 616c 7565 732e 0a0a 2020 2020 2020 2020  alues...        
+000129a0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+000129b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000129c0: 2020 2020 2020 6e61 6d65 3a20 7374 720a        name: str.
+000129d0: 2020 2020 2020 2020 2020 2020 4163 7475              Actu
+000129e0: 616c 206e 616d 650a 2020 2020 2020 2020  al name.        
+000129f0: 6366 5f6e 616d 653a 2073 7472 2c20 4e6f  cf_name: str, No
+00012a00: 6e65 0a20 2020 2020 2020 2020 2020 2041  ne.            A
+00012a10: 2074 6172 6765 7420 6765 6e65 7269 6320   target generic 
+00012a20: 4346 206e 616d 652e 2049 6620 6e6f 7420  CF name. If not 
+00012a30: 7072 6f76 6964 6564 2c20 616c 6c20 6974  provided, all it
+00012a40: 656d 7320 6172 6520 636f 6e73 6964 6572  ems are consider
+00012a50: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
+00012a60: 7572 6e0a 2020 2020 2020 2020 2d2d 2d2d  urn.        ----
+00012a70: 2d2d 0a20 2020 2020 2020 204e 6f6e 652c  --.        None,
+00012a80: 2073 7472 2c20 5472 7565 2c20 4661 6c73   str, True, Fals
+00012a90: 650a 2020 2020 2020 2020 2020 2020 4966  e.            If
+00012aa0: 2060 6366 5f6e 616d 6560 2069 7320 7072   `cf_name` is pr
+00012ab0: 6f76 6964 6564 2c20 7265 7475 726e 7320  ovided, returns 
+00012ac0: 6120 626f 6f6c 6561 6e2c 2065 6c73 6520  a boolean, else 
+00012ad0: 7265 7475 726e 730a 2020 2020 2020 2020  returns.        
+00012ae0: 2020 2020 7468 6520 6d61 7463 6869 6e67      the matching
+00012af0: 2043 4620 6e61 6d65 206f 7220 4e6f 6e65   CF name or None
+00012b00: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00012b10: 2020 2020 2020 6578 706c 6963 6974 203d        explicit =
+00012b20: 2063 665f 6e61 6d65 2069 7320 6e6f 7420   cf_name is not 
+00012b30: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
+00012b40: 6366 5f6e 616d 653a 0a20 2020 2020 2020  cf_name:.       
+00012b50: 2020 2020 2073 656c 662e 5f61 7373 6572       self._asser
+00012b60: 745f 6b6e 6f77 6e5f 2863 665f 6e61 6d65  t_known_(cf_name
+00012b70: 290a 2020 2020 2020 2020 2020 2020 6366  ).            cf
+00012b80: 5f6e 616d 6573 203d 205b 6366 5f6e 616d  _names = [cf_nam
+00012b90: 655d 0a20 2020 2020 2020 2065 6c73 653a  e].        else:
+00012ba0: 0a20 2020 2020 2020 2020 2020 2063 665f  .            cf_
+00012bb0: 6e61 6d65 7320 3d20 7365 6c66 2e6e 616d  names = self.nam
+00012bc0: 6573 0a0a 2020 2020 2020 2020 666f 7220  es..        for 
+00012bd0: 6366 5f6e 616d 6520 696e 2063 665f 6e61  cf_name in cf_na
+00012be0: 6d65 733a 0a20 2020 2020 2020 2020 2020  mes:.           
+00012bf0: 2066 6f72 2061 6c6c 6f77 6564 5f6e 616d   for allowed_nam
+00012c00: 6520 696e 2073 656c 662e 6765 745f 616c  e in self.get_al
+00012c10: 6c6f 7765 645f 6e61 6d65 7328 6366 5f6e  lowed_names(cf_n
+00012c20: 616d 6529 3a0a 2020 2020 2020 2020 2020  ame):.          
+00012c30: 2020 2020 2020 6966 2073 656c 662e 7367        if self.sg
+00012c40: 6c6f 6361 746f 722e 6d61 7463 685f 6174  locator.match_at
+00012c50: 7472 2822 6e61 6d65 222c 206e 616d 652c  tr("name", name,
+00012c60: 2061 6c6c 6f77 6564 5f6e 616d 652c 206c   allowed_name, l
+00012c70: 6f63 3d6c 6f63 293a 0a20 2020 2020 2020  oc=loc):.       
+00012c80: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00012c90: 7572 6e20 6366 5f6e 616d 6520 6966 206e  urn cf_name if n
+00012ca0: 6f74 2065 7870 6c69 6369 7420 656c 7365  ot explicit else
+00012cb0: 2054 7275 650a 2020 2020 2020 2020 7265   True.        re
+00012cc0: 7475 726e 204e 6f6e 6520 6966 206e 6f74  turn None if not
+00012cd0: 2065 7870 6c69 6369 7420 656c 7365 2046   explicit else F
+00012ce0: 616c 7365 0a0a 2020 2020 4045 5252 4f52  alse..    @ERROR
+00012cf0: 532e 666f 726d 6174 5f6d 6574 686f 645f  S.format_method_
+00012d00: 646f 6373 7472 696e 670a 2020 2020 6465  docstring.    de
+00012d10: 6620 7365 6172 6368 2873 656c 662c 206f  f search(self, o
+00012d20: 626a 2c20 6366 5f6e 616d 653d 4e6f 6e65  bj, cf_name=None
+00012d30: 2c20 6c6f 633d 4e6f 6e65 2c20 6765 743d  , loc=None, get=
+00012d40: 226f 626a 222c 2073 696e 676c 653d 5472  "obj", single=Tr
+00012d50: 7565 2c20 6572 726f 7273 3d22 7261 6973  ue, errors="rais
+00012d60: 6522 293a 0a20 2020 2020 2020 2022 2222  e"):.        """
+00012d70: 5365 6172 6368 2066 6f72 2061 2064 6174  Search for a dat
+00012d80: 615f 7661 7220 6f72 2063 6f6f 7264 2074  a_var or coord t
+00012d90: 6861 7420 6d61 6368 6573 2067 6976 656e  hat maches given
+00012da0: 206f 7220 616e 7920 7370 6563 730a 0a20   or any specs.. 
+00012db0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00012dc0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00012dd0: 2d2d 2d2d 0a20 2020 2020 2020 206f 626a  ----.        obj
+00012de0: 3a20 4461 7461 4172 7261 7920 6f72 2044  : DataArray or D
+00012df0: 6174 6173 6574 0a20 2020 2020 2020 2063  ataset.        c
+00012e00: 665f 6e61 6d65 3a20 7374 722c 2064 6963  f_name: str, dic
+00012e10: 740a 2020 2020 2020 2020 2020 2020 4120  t.            A 
+00012e20: 6765 6e65 7269 6320 4346 206e 616d 652e  generic CF name.
+00012e30: 2049 6620 6e6f 7420 7072 6f76 6964 6564   If not provided
+00012e40: 2c20 616c 6c20 4346 206e 616d 6573 2061  , all CF names a
+00012e50: 7265 2073 6361 6e65 642e 0a20 2020 2020  re scaned..     
+00012e60: 2020 206c 6f63 3a20 7374 722c 207b 7b22     loc: str, {{"
+00012e70: 616e 7922 2c20 4e6f 6e65 7d7d 2c20 7b7b  any", None}}, {{
+00012e80: 2222 2c20 4661 6c73 657d 7d0a 2020 2020  "", False}}.    
+00012e90: 2020 2020 2020 2020 2d20 7374 723a 206f          - str: o
+00012ea0: 6e65 206f 6620 7468 6573 6520 6c6f 6361  ne of these loca
+00012eb0: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+00012ec0: 2020 2d20 4e6f 6e65 206f 7220 2261 6e79    - None or "any
+00012ed0: 223a 2061 6e79 0a20 2020 2020 2020 2020  ": any.         
+00012ee0: 2020 202d 2046 616c 7365 206f 7220 2722     - False or '"
+00012ef0: 223a 206e 6f20 6c6f 6361 7469 6f6e 0a20  ": no location. 
+00012f00: 2020 2020 2020 2067 6574 3a20 7b7b 226f         get: {{"o
+00012f10: 626a 222c 2022 6366 5f6e 616d 6522 2c20  bj", "cf_name", 
+00012f20: 2262 6f74 6822 7d7d 0a20 2020 2020 2020  "both"}}.       
+00012f30: 2020 2020 2057 6865 6e20 666f 756e 642c       When found,
+00012f40: 2067 6574 2074 6865 206f 626a 6563 7420   get the object 
+00012f50: 666f 756e 6420 6f72 2069 7473 206e 616d  found or its nam
+00012f60: 652e 0a20 2020 2020 2020 2073 696e 676c  e..        singl
+00012f70: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00012f80: 2020 2020 4966 2054 7275 652c 2072 6574      If True, ret
+00012f90: 7572 6e20 7468 6520 6669 7273 7420 6974  urn the first it
+00012fa0: 656d 2066 6f75 6e64 206f 7220 4e6f 6e65  em found or None
+00012fb0: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+00012fc0: 2046 616c 7365 2c20 7265 7475 726e 2061   False, return a
+00012fd0: 2070 6f73 7369 626c 6520 656d 7074 7920   possible empty 
+00012fe0: 6c69 7374 206f 6620 666f 756e 6420 6974  list of found it
+00012ff0: 656d 732e 0a20 2020 2020 2020 2020 2020  ems..           
+00013000: 2041 2077 6172 6e69 6e67 2069 7320 656d   A warning is em
+00013010: 6974 7465 6420 7768 656e 2073 6574 2074  itted when set t
+00013020: 6f20 5472 7565 2061 6e64 206d 756c 7469  o True and multi
+00013030: 706c 6520 6974 656d 2061 7265 2066 6f75  ple item are fou
+00013040: 6e64 2e0a 2020 2020 2020 2020 7b65 7272  nd..        {err
+00013050: 6f72 737d 0a0a 2020 2020 2020 2020 5265  ors}..        Re
+00013060: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00013070: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
+00013080: 6e65 206f 7220 7374 7220 6f72 206f 626a  ne or str or obj
+00013090: 6563 740a 2020 2020 2020 2020 2222 220a  ect.        """.
+000130a0: 0a20 2020 2020 2020 2023 2047 6574 2074  .        # Get t
+000130b0: 6172 6765 7420 6f62 6a65 6374 730a 2020  arget objects.  
+000130c0: 2020 2020 2020 6966 2073 656c 662e 6361        if self.ca
+000130d0: 7465 676f 7279 2061 6e64 2068 6173 6174  tegory and hasat
+000130e0: 7472 286f 626a 2c20 7365 6c66 2e63 6174  tr(obj, self.cat
+000130f0: 6567 6f72 7929 3a0a 2020 2020 2020 2020  egory):.        
+00013100: 2020 2020 6e61 6d65 7320 3d20 6765 7461      names = geta
+00013110: 7474 7228 6f62 6a2c 2073 656c 662e 6361  ttr(obj, self.ca
+00013120: 7465 676f 7279 290a 2020 2020 2020 2020  tegory).        
+00013130: 2020 2020 6b77 203d 2064 6963 7428 6461      kw = dict(da
+00013140: 7461 5f76 6172 733d 4661 6c73 652c 2063  ta_vars=False, c
+00013150: 6f6f 7264 733d 4661 6c73 652c 2064 696d  oords=False, dim
+00013160: 733d 4661 6c73 6529 0a20 2020 2020 2020  s=False).       
+00013170: 2020 2020 206b 775b 7365 6c66 2e63 6174       kw[self.cat
+00013180: 6567 6f72 795d 203d 2054 7275 650a 2020  egory] = True.  
+00013190: 2020 2020 2020 2020 2020 6e61 6d65 7320            names 
+000131a0: 3d20 5f6c 6973 745f 7872 5f6e 616d 6573  = _list_xr_names
+000131b0: 5f28 6f62 6a2c 202a 2a6b 7729 0a20 2020  _(obj, **kw).   
+000131c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000131d0: 2020 2020 2020 206e 616d 6573 203d 2028         names = (
+000131e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000131f0: 206c 6973 7428 6f62 6a29 0a20 2020 2020   list(obj).     
+00013200: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+00013210: 7361 7474 7228 6f62 6a2c 2022 6b65 7973  sattr(obj, "keys
+00013220: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00013230: 2020 2065 6c73 6520 5f6c 6973 745f 7872     else _list_xr
+00013240: 5f6e 616d 6573 5f28 6f62 6a2c 2064 6174  _names_(obj, dat
+00013250: 615f 7661 7273 3d46 616c 7365 2c20 6469  a_vars=False, di
+00013260: 6d73 3d46 616c 7365 290a 2020 2020 2020  ms=False).      
+00013270: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00013280: 2023 2047 6574 206d 6174 6368 2073 7065   # Get match spe
+00013290: 6373 0a20 2020 2020 2020 2069 6620 6366  cs.        if cf
+000132a0: 5f6e 616d 653a 2020 2320 4578 706c 6963  _name:  # Explic
+000132b0: 6974 206e 616d 6520 736f 2077 6520 6c6f  it name so we lo
+000132c0: 6f70 206f 6e20 7365 6172 6368 2073 7065  op on search spe
+000132d0: 6373 0a20 2020 2020 2020 2020 2020 2069  cs.            i
+000132e0: 6620 6973 696e 7374 616e 6365 2863 665f  f isinstance(cf_
+000132f0: 6e61 6d65 2c20 7374 7229 3a0a 2020 2020  name, str):.    
+00013300: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00013310: 6f74 2073 656c 662e 5f61 7373 6572 745f  ot self._assert_
+00013320: 6b6e 6f77 6e5f 2863 665f 6e61 6d65 2c20  known_(cf_name, 
+00013330: 6572 726f 7273 293a 0a20 2020 2020 2020  errors):.       
+00013340: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00013350: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
+00013360: 6d61 7463 685f 7370 6563 7320 3d20 5b5d  match_specs = []
+00013370: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00013380: 2061 7474 722c 2072 6566 7320 696e 2073   attr, refs in s
+00013390: 656c 662e 5f67 6574 5f6f 7264 6572 6564  elf._get_ordered
+000133a0: 5f6d 6174 6368 5f73 7065 6373 5f28 6366  _match_specs_(cf
+000133b0: 5f6e 616d 6529 2e69 7465 6d73 2829 3a0a  _name).items():.
+000133c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133d0: 6d61 7463 685f 7370 6563 732e 6170 7065  match_specs.appe
+000133e0: 6e64 287b 6174 7472 3a20 7265 6673 7d29  nd({attr: refs})
+000133f0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00013400: 2020 2020 2020 2020 2020 206d 6174 6368             match
+00013410: 5f73 7065 6373 203d 205b 4e6f 6e65 5d0a  _specs = [None].
+00013420: 0a20 2020 2020 2020 2023 204c 6f6f 7073  .        # Loops
+00013430: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00013440: 6765 7420 696e 2028 0a20 2020 2020 2020  get in (.       
+00013450: 2020 2020 2022 6366 5f6e 616d 6522 2c0a       "cf_name",.
+00013460: 2020 2020 2020 2020 2020 2020 226f 626a              "obj
+00013470: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00013480: 626f 7468 222c 0a20 2020 2020 2020 2029  both",.        )
+00013490: 2c20 6622 2767 6574 2720 6d75 7374 2062  , f"'get' must b
+000134a0: 6520 6569 7468 6572 2027 6366 5f6e 616d  e either 'cf_nam
+000134b0: 6527 206f 7220 276f 626a 2720 6f72 2027  e' or 'obj' or '
+000134c0: 626f 7468 272c 204e 4f54 2027 7b67 6574  both', NOT '{get
+000134d0: 7d27 220a 2020 2020 2020 2020 666f 756e  }'".        foun
+000134e0: 6420 3d20 5b5d 0a20 2020 2020 2020 2066  d = [].        f
+000134f0: 6f75 6e64 5f6f 626a 7320 3d20 5b5d 0a20  ound_objs = []. 
+00013500: 2020 2020 2020 2066 6f72 206d 6174 6368         for match
+00013510: 5f61 7267 2069 6e20 6d61 7463 685f 7370  _arg in match_sp
+00013520: 6563 733a 0a20 2020 2020 2020 2020 2020  ecs:.           
+00013530: 2023 2066 6f72 206f 626a 2069 6e20 6f62   # for obj in ob
+00013540: 6a73 2e76 616c 7565 7328 293a 0a20 2020  js.values():.   
+00013550: 2020 2020 2020 2020 2066 6f72 2074 6869           for thi
+00013560: 735f 6e61 6d65 2069 6e20 6e61 6d65 733a  s_name in names:
+00013570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013580: 2074 6869 735f 6f62 6a20 3d20 6f62 6a5b   this_obj = obj[
+00013590: 7468 6973 5f6e 616d 655d 0a20 2020 2020  this_name].     
+000135a0: 2020 2020 2020 2020 2020 206d 203d 2073             m = s
+000135b0: 656c 662e 6d61 7463 6828 7468 6973 5f6f  elf.match(this_o
+000135c0: 626a 2c20 6d61 7463 685f 6172 672c 206c  bj, match_arg, l
+000135d0: 6f63 3d6c 6f63 290a 2020 2020 2020 2020  oc=loc).        
+000135e0: 2020 2020 2020 2020 6966 206d 3a0a 2020          if m:.  
 000135f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013600: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00013610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013620: 2020 2020 2066 6f75 6e64 5f6f 626a 732e       found_objs.
-00013630: 6170 7065 6e64 2874 6869 735f 6e61 6d65  append(this_name
-00013640: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013650: 2020 2020 2020 6366 5f6e 616d 6520 3d20        cf_name = 
-00013660: 6366 5f6e 616d 6520 6966 2063 665f 6e61  cf_name if cf_na
-00013670: 6d65 2065 6c73 6520 6d0a 2020 2020 2020  me else m.      
-00013680: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00013690: 2067 6574 203d 3d20 2262 6f74 6822 3a0a   get == "both":.
-000136a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136b0: 2020 2020 2020 2020 666f 756e 642e 6170          found.ap
-000136c0: 7065 6e64 2828 7468 6973 5f6f 626a 2c20  pend((this_obj, 
-000136d0: 6366 5f6e 616d 6529 290a 2020 2020 2020  cf_name)).      
-000136e0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000136f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00013700: 2020 2020 2020 2020 2020 2020 666f 756e              foun
-00013710: 642e 6170 7065 6e64 2874 6869 735f 6f62  d.append(this_ob
-00013720: 6a20 6966 2067 6574 203d 3d20 226f 626a  j if get == "obj
-00013730: 2220 656c 7365 2063 665f 6e61 6d65 290a  " else cf_name).
-00013740: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
-00013750: 6e0a 2020 2020 2020 2020 6966 206e 6f74  n.        if not
-00013760: 2073 696e 676c 653a 0a20 2020 2020 2020   single:.       
-00013770: 2020 2020 2072 6574 7572 6e20 666f 756e       return foun
-00013780: 640a 2020 2020 2020 2020 6572 726f 7273  d.        errors
-00013790: 203d 2045 5252 4f52 535b 6572 726f 7273   = ERRORS[errors
-000137a0: 5d0a 2020 2020 2020 2020 6966 2065 7272  ].        if err
-000137b0: 6f72 7320 213d 2022 6967 6e6f 7265 2220  ors != "ignore" 
-000137c0: 616e 6420 6c65 6e28 666f 756e 6429 203e  and len(found) >
-000137d0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-000137e0: 6d73 6720 3d20 224d 756c 7469 706c 6520  msg = "Multiple 
-000137f0: 6974 656d 7320 666f 756e 6420 7768 696c  items found whil
-00013800: 6520 796f 7520 7265 7175 6573 7465 6420  e you requested 
-00013810: 6120 7369 6e67 6c65 206f 6e65 220a 2020  a single one".  
-00013820: 2020 2020 2020 2020 2020 6966 2065 7272            if err
-00013830: 6f72 7320 3d3d 2022 7261 6973 6522 3a0a  ors == "raise":.
-00013840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013850: 7261 6973 6520 586f 6143 4645 7272 6f72  raise XoaCFError
-00013860: 286d 7367 290a 2020 2020 2020 2020 2020  (msg).          
-00013870: 2020 786f 615f 7761 726e 286d 7367 290a    xoa_warn(msg).
-00013880: 2020 2020 2020 2020 6966 2066 6f75 6e64          if found
-00013890: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000138a0: 7475 726e 2066 6f75 6e64 5b30 5d0a 2020  turn found[0].  
-000138b0: 2020 2020 2020 6966 2065 7272 6f72 7320        if errors 
-000138c0: 213d 2022 6967 6e6f 7265 223a 0a20 2020  != "ignore":.   
-000138d0: 2020 2020 2020 2020 206d 7367 203d 2022           msg = "
-000138e0: 4e6f 206d 6174 6368 696e 6720 6974 656d  No matching item
-000138f0: 2066 6f75 6e64 220a 2020 2020 2020 2020   found".        
-00013900: 2020 2020 6966 2065 7272 6f72 7320 3d3d      if errors ==
-00013910: 2022 7261 6973 6522 3a0a 2020 2020 2020   "raise":.      
-00013920: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00013930: 586f 6143 4645 7272 6f72 286d 7367 290a  XoaCFError(msg).
-00013940: 2020 2020 2020 2020 2020 2020 786f 615f              xoa_
-00013950: 7761 726e 286d 7367 290a 0a20 2020 2064  warn(msg)..    d
-00013960: 6566 2067 6574 2873 656c 662c 206f 626a  ef get(self, obj
-00013970: 2c20 6366 5f6e 616d 6529 3a0a 2020 2020  , cf_name):.    
-00013980: 2020 2020 2222 2243 616c 6c20 746f 203a      """Call to :
-00013990: 6d65 7468 3a60 7365 6172 6368 6020 7769  meth:`search` wi
-000139a0: 7468 2061 6e20 6578 706c 6963 6974 206e  th an explicit n
-000139b0: 616d 6520 616e 6420 6967 6e6f 7269 6e67  ame and ignoring
-000139c0: 2065 7272 6f72 7322 2222 0a20 2020 2020   errors""".     
-000139d0: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
-000139e0: 6561 7263 6828 6f62 6a2c 2063 665f 6e61  earch(obj, cf_na
-000139f0: 6d65 2c20 6572 726f 7273 3d22 6967 6e6f  me, errors="igno
-00013a00: 7265 2229 0a0a 2020 2020 4045 5252 4f52  re")..    @ERROR
-00013a10: 532e 666f 726d 6174 5f6d 6574 686f 645f  S.format_method_
-00013a20: 646f 6373 7472 696e 670a 2020 2020 6465  docstring.    de
-00013a30: 6620 6765 745f 6174 7472 7328 0a20 2020  f get_attrs(.   
-00013a40: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00013a50: 2020 2063 665f 6e61 6d65 2c0a 2020 2020     cf_name,.    
-00013a60: 2020 2020 7365 6c65 6374 3d4e 6f6e 652c      select=None,
-00013a70: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
-00013a80: 3d4e 6f6e 652c 0a20 2020 2020 2020 2065  =None,.        e
-00013a90: 7272 6f72 733d 2277 6172 6e22 2c0a 2020  rrors="warn",.  
-00013aa0: 2020 2020 2020 6c6f 633d 4e6f 6e65 2c0a        loc=None,.
-00013ab0: 2020 2020 2020 2020 6d75 6c74 693d 4661          multi=Fa
-00013ac0: 6c73 652c 0a20 2020 2020 2020 2073 7461  lse,.        sta
-00013ad0: 6e64 6172 6469 7a65 3d54 7275 652c 0a20  ndardize=True,. 
-00013ae0: 2020 2020 2020 202a 2a65 7874 7261 2c0a         **extra,.
-00013af0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-00013b00: 2222 4765 7420 7468 6520 6465 6661 756c  ""Get the defaul
-00013b10: 7420 6174 7472 6962 7574 6573 2066 726f  t attributes fro
-00013b20: 6d20 6366 2073 7065 6373 0a0a 2020 2020  m cf specs..    
-00013b30: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00013b40: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00013b50: 2d0a 2020 2020 2020 2020 6366 5f6e 616d  -.        cf_nam
-00013b60: 653a 2073 7472 0a20 2020 2020 2020 2020  e: str.         
-00013b70: 2020 2056 616c 6964 2067 656e 6572 6963     Valid generic
-00013b80: 2043 4620 6e61 6d65 0a20 2020 2020 2020   CF name.       
-00013b90: 2073 656c 6563 743a 2073 7472 2c20 6c69   select: str, li
-00013ba0: 7374 0a20 2020 2020 2020 2020 2020 2049  st.            I
-00013bb0: 6e63 6c75 6465 206f 6e6c 7920 7468 6573  nclude only thes
-00013bc0: 6520 6174 7472 6962 7574 6573 0a20 2020  e attributes.   
-00013bd0: 2020 2020 2065 7863 6c75 6465 3a20 7374       exclude: st
-00013be0: 722c 206c 6973 740a 2020 2020 2020 2020  r, list.        
-00013bf0: 2020 2020 4578 636c 7564 6520 7468 6573      Exclude thes
-00013c00: 6520 6174 7472 6962 7574 6573 0a20 2020  e attributes.   
-00013c10: 2020 2020 206d 756c 7469 3a20 626f 6f6c       multi: bool
-00013c20: 0a20 2020 2020 2020 2020 2020 2047 6574  .            Get
-00013c30: 2073 7461 6e64 6172 645f 6e61 6d65 2061   standard_name a
-00013c40: 6e64 206c 6f6e 675f 6e61 6d65 2061 7474  nd long_name att
-00013c50: 7269 6275 7465 2061 7320 6120 6c69 7374  ribute as a list
-00013c60: 206f 6620 706f 7373 6962 6c65 0a20 2020   of possible.   
-00013c70: 2020 2020 2020 2020 2076 616c 7565 730a           values.
-00013c80: 2020 2020 2020 2020 7b65 7272 6f72 737d          {errors}
-00013c90: 0a20 2020 2020 2020 2065 7874 7261 3a20  .        extra: 
-00013ca0: 6469 6374 0a20 2020 2020 2020 2020 2045  dict.          E
-00013cb0: 7874 7261 2070 6172 616d 7320 6172 6520  xtra params are 
-00013cc0: 696e 636c 7564 6564 2061 7320 6578 7472  included as extr
-00013cd0: 6120 6174 7472 6962 7574 6573 0a0a 2020  a attributes..  
-00013ce0: 2020 2020 2020 5265 7475 726e 0a20 2020        Return.   
-00013cf0: 2020 2020 202d 2d2d 2d2d 2d0a 2020 2020       ------.    
-00013d00: 2020 2020 6469 6374 0a20 2020 2020 2020      dict.       
-00013d10: 2022 2222 0a0a 2020 2020 2020 2020 2320   """..        # 
-00013d20: 4765 7420 7370 6563 730a 2020 2020 2020  Get specs.      
-00013d30: 2020 7370 6563 7320 3d20 7365 6c66 2e67    specs = self.g
-00013d40: 6574 5f73 7065 6373 2863 665f 6e61 6d65  et_specs(cf_name
-00013d50: 2c20 6572 726f 7273 3d65 7272 6f72 7329  , errors=errors)
-00013d60: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00013d70: 7370 6563 733a 0a20 2020 2020 2020 2020  specs:.         
-00013d80: 2020 2072 6574 7572 6e20 7b7d 0a0a 2020     return {}..  
-00013d90: 2020 2020 2020 2320 5768 6963 6820 6174        # Which at
-00013da0: 7472 6962 7574 6573 0a20 2020 2020 2020  tributes.       
-00013db0: 2069 6620 6578 636c 7564 6520 6973 204e   if exclude is N
-00013dc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00013dd0: 2065 7863 6c75 6465 203d 205b 5d0a 2020   exclude = [].  
-00013de0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00013df0: 7461 6e63 6528 6578 636c 7564 652c 2073  tance(exclude, s
-00013e00: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00013e10: 2065 7863 6c75 6465 203d 205b 6578 636c   exclude = [excl
-00013e20: 7564 655d 0a20 2020 2020 2020 2023 2065  ude].        # e
-00013e30: 7863 6c75 6465 2e65 7874 656e 6428 7365  xclude.extend(se
-00013e40: 6c66 2e61 7474 7273 5f65 7863 6c75 6465  lf.attrs_exclude
-00013e50: 290a 2020 2020 2020 2020 6578 636c 7564  ).        exclud
-00013e60: 652e 6578 7465 6e64 2865 7874 7261 2e6b  e.extend(extra.k
-00013e70: 6579 7328 2929 0a20 2020 2020 2020 2065  eys()).        e
-00013e80: 7863 6c75 6465 203d 2073 6574 2865 7863  xclude = set(exc
-00013e90: 6c75 6465 290a 2020 2020 2020 2020 6b65  lude).        ke
-00013ea0: 7973 203d 2073 6574 2873 7065 6373 5b22  ys = set(specs["
-00013eb0: 6174 7472 7322 5d2e 6b65 7973 2829 290a  attrs"].keys()).
-00013ec0: 2020 2020 2020 2020 6b65 7973 202d 3d20          keys -= 
-00013ed0: 6578 636c 7564 650a 2020 2020 2020 2020  exclude.        
-00013ee0: 6966 2073 656c 6563 743a 0a20 2020 2020  if select:.     
-00013ef0: 2020 2020 2020 206b 6579 7320 3d20 6b65         keys = ke
-00013f00: 7973 2e69 6e74 6572 7365 6374 696f 6e28  ys.intersection(
-00013f10: 7365 6c65 6374 290a 0a20 2020 2020 2020  select)..       
-00013f20: 2023 204c 6f6f 700a 2020 2020 2020 2020   # Loop.        
-00013f30: 6174 7472 7320 3d20 7b7d 0a20 2020 2020  attrs = {}.     
-00013f40: 2020 2066 6f72 206b 6579 2069 6e20 7370     for key in sp
-00013f50: 6563 735b 2261 7474 7273 225d 2e6b 6579  ecs["attrs"].key
-00013f60: 7328 293a 0a0a 2020 2020 2020 2020 2020  s():..          
-00013f70: 2020 2320 4e6f 206c 6973 7473 206f 7220    # No lists or 
-00013f80: 7475 706c 6573 0a20 2020 2020 2020 2020  tuples.         
-00013f90: 2020 2076 616c 7565 203d 2073 7065 6373     value = specs
-00013fa0: 5b22 6174 7472 7322 5d5b 6b65 795d 0a20  ["attrs"][key]. 
-00013fb0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00013fc0: 696e 7374 616e 6365 2876 616c 7565 2c20  instance(value, 
-00013fd0: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
-00013fe0: 2020 2020 2020 2069 6620 6c65 6e28 7661         if len(va
-00013ff0: 6c75 6529 203d 3d20 303a 0a20 2020 2020  lue) == 0:.     
-00014000: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00014010: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-00014020: 2020 2020 2020 2020 6966 206e 6f74 206d          if not m
-00014030: 756c 7469 206f 7220 6b65 7920 6e6f 7420  ulti or key not 
-00014040: 696e 2028 2273 7461 6e64 6172 645f 6e61  in ("standard_na
-00014050: 6d65 222c 2022 6c6f 6e67 5f6e 616d 6522  me", "long_name"
-00014060: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00014070: 2020 2020 2020 2076 616c 7565 203d 2076         value = v
-00014080: 616c 7565 5b30 5d0a 0a20 2020 2020 2020  alue[0]..       
-00014090: 2020 2020 2023 2053 746f 7265 2069 740a       # Store it.
-000140a0: 2020 2020 2020 2020 2020 2020 6174 7472              attr
-000140b0: 735b 6b65 795d 203d 2076 616c 7565 0a0a  s[key] = value..
-000140c0: 2020 2020 2020 2020 2320 4578 7472 6120          # Extra 
-000140d0: 6174 7472 6962 7574 6573 0a20 2020 2020  attributes.     
-000140e0: 2020 2061 7474 7273 2e75 7064 6174 6528     attrs.update(
-000140f0: 6578 7472 6129 0a0a 2020 2020 2020 2020  extra)..        
-00014100: 2320 4669 6e61 6c69 7a65 2061 6e64 206f  # Finalize and o
-00014110: 7074 696f 6e61 6c6c 7920 6368 616e 6765  ptionally change
-00014120: 206c 6f63 6174 696f 6e0a 2020 2020 2020   location.      
-00014130: 2020 6174 7472 7320 3d20 7365 6c66 2e70    attrs = self.p
-00014140: 6172 656e 742e 7367 6c6f 6361 746f 722e  arent.sglocator.
-00014150: 666f 726d 6174 5f61 7474 7273 2861 7474  format_attrs(att
-00014160: 7273 2c20 6c6f 633d 6c6f 632c 2073 7461  rs, loc=loc, sta
-00014170: 6e64 6172 6469 7a65 3d73 7461 6e64 6172  ndardize=standar
-00014180: 6469 7a65 290a 0a20 2020 2020 2020 2072  dize)..        r
-00014190: 6574 7572 6e20 6174 7472 730a 0a20 2020  eturn attrs..   
-000141a0: 2064 6566 2067 6574 5f6e 616d 6528 7365   def get_name(se
-000141b0: 6c66 2c20 6e61 6d65 2c20 7370 6563 6961  lf, name, specia
-000141c0: 6c69 7a65 3d46 616c 7365 2c20 6c6f 633d  lize=False, loc=
-000141d0: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
-000141e0: 2222 4765 7420 7468 6520 6e61 6d65 206f  ""Get the name o
-000141f0: 6620 7468 6520 6d61 7463 6869 6e67 2043  f the matching C
-00014200: 4620 7370 6563 730a 0a20 2020 2020 2020  F specs..       
-00014210: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00014220: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00014230: 2020 2020 2020 206e 616d 653a 2073 7472         name: str
-00014240: 2c20 7861 7272 6179 2e44 6174 6141 7272  , xarray.DataArr
-00014250: 6179 0a20 2020 2020 2020 2020 2020 2045  ay.            E
-00014260: 6974 6865 7220 6120 6461 7461 2061 7272  ither a data arr
-00014270: 6179 2c20 6120 6b6e 6f77 6e20 6366 206e  ay, a known cf n
-00014280: 616d 6520 6f72 2061 2064 6174 6120 7661  ame or a data va
-00014290: 7220 6e61 6d65 0a20 2020 2020 2020 2073  r name.        s
-000142a0: 7065 6369 616c 697a 653a 2062 6f6f 6c0a  pecialize: bool.
-000142b0: 2020 2020 2020 2020 2020 2020 4765 7420              Get 
-000142c0: 7468 6520 6669 7273 7420 6e61 6d65 0a20  the first name. 
-000142d0: 2020 2020 2020 2020 2020 2061 7320 6c69             as li
-000142e0: 7374 6564 2069 6e20 7370 6563 732c 2077  sted in specs, w
-000142f0: 6869 6368 2069 7320 6765 6e65 7261 6c6c  hich is generall
-00014300: 7920 6120 7370 6563 6961 6c69 7a65 6420  y a specialized 
-00014310: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00014320: 206c 696b 6520 6120 6e61 6d65 2061 646f   like a name ado
-00014330: 7074 6564 2062 7920 7370 6563 6961 6c69  pted by speciali
-00014340: 7a65 6420 6461 7461 7365 742e 0a20 2020  zed dataset..   
-00014350: 2020 2020 206c 6f63 3a20 7374 722c 204e       loc: str, N
-00014360: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00014370: 466f 726d 6174 2069 7420 6174 2074 6869  Format it at thi
-00014380: 7320 6c6f 6361 7469 6f6e 0a0a 2020 2020  s location..    
-00014390: 2020 2020 5265 7475 726e 0a20 2020 2020      Return.     
-000143a0: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
-000143b0: 2020 4e6f 6e65 206f 7220 7374 720a 2020    None or str.  
-000143c0: 2020 2020 2020 2020 2020 4569 7468 6572            Either
-000143d0: 2074 6865 2043 4620 6e61 6d65 206f 7220   the CF name or 
-000143e0: 7468 6520 7370 6563 6961 6c69 7a65 6420  the specialized 
-000143f0: 6e61 6d65 0a20 2020 2020 2020 2022 2222  name.        """
-00014400: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00014410: 6973 696e 7374 616e 6365 286e 616d 652c  isinstance(name,
-00014420: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-00014430: 2020 206e 616d 6520 3d20 6e61 6d65 2e65     name = name.e
-00014440: 6e63 6f64 696e 672e 6765 7428 2263 665f  ncoding.get("cf_
-00014450: 6e61 6d65 222c 2073 656c 662e 6d61 7463  name", self.matc
-00014460: 6828 6e61 6d65 2929 0a20 2020 2020 2020  h(name)).       
-00014470: 2020 2020 2023 2046 4958 4d45 3a20 6361       # FIXME: ca
-00014480: 7465 676f 7279 3f0a 2020 2020 2020 2020  tegory?.        
-00014490: 656c 6966 206e 616d 6520 6e6f 7420 696e  elif name not in
-000144a0: 2073 656c 663a 0a20 2020 2020 2020 2020   self:.         
-000144b0: 2020 206e 616d 6520 3d20 7365 6c66 2e6d     name = self.m
-000144c0: 6174 6368 5f66 726f 6d5f 6e61 6d65 286e  atch_from_name(n
-000144d0: 616d 6529 0a20 2020 2020 2020 2069 6620  ame).        if 
-000144e0: 6e61 6d65 2069 7320 4e6f 6e65 3a0a 2020  name is None:.  
-000144f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00014500: 0a20 2020 2020 2020 2069 6620 7370 6563  .        if spec
-00014510: 6961 6c69 7a65 2061 6e64 2073 656c 665b  ialize and self[
-00014520: 6e61 6d65 5d5b 226e 616d 6522 5d3a 0a20  name]["name"]:. 
-00014530: 2020 2020 2020 2020 2020 206e 616d 6520             name 
-00014540: 3d20 7365 6c66 5b6e 616d 655d 5b22 6e61  = self[name]["na
-00014550: 6d65 225d 0a20 2020 2020 2020 2072 6574  me"].        ret
-00014560: 7572 6e20 7365 6c66 2e73 676c 6f63 6174  urn self.sglocat
-00014570: 6f72 2e66 6f72 6d61 745f 6174 7472 2822  or.format_attr("
-00014580: 6e61 6d65 222c 206e 616d 652c 206c 6f63  name", name, loc
-00014590: 3d6c 6f63 290a 0a20 2020 2064 6566 2067  =loc)..    def g
-000145a0: 6574 5f6c 6f63 5f61 7267 2873 656c 662c  et_loc_arg(self,
-000145b0: 2064 612c 2063 665f 6e61 6d65 3d4e 6f6e   da, cf_name=Non
-000145c0: 652c 206c 6f63 6174 696f 6e73 3d4e 6f6e  e, locations=Non
-000145d0: 6529 3a0a 2020 2020 2020 2020 2222 2247  e):.        """G
-000145e0: 6574 2074 6865 2060 6c6f 6360 2061 7267  et the `loc` arg
-000145f0: 756d 656e 7420 6672 6f6d 2061 206e 616d  ument from a nam
-00014600: 6520 6f72 2064 6174 6120 6172 7261 7920  e or data array 
-00014610: 7769 7468 206e 616d 650a 0a20 2020 2020  with name..     
-00014620: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00014630: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00014640: 0a20 2020 2020 2020 2064 613a 2078 6172  .        da: xar
-00014650: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
-00014660: 2020 2020 2020 6366 5f6e 616d 653a 204e        cf_name: N
-00014670: 6f6e 652c 2073 7472 0a20 2020 2020 2020  one, str.       
-00014680: 2020 2020 2041 2067 656e 6572 6963 2043       A generic C
-00014690: 4620 6e61 6d65 0a20 2020 2020 2020 206c  F name.        l
-000146a0: 6f63 6174 696f 6e73 3a20 4e6f 6e65 2c20  ocations: None, 
-000146b0: 6469 6374 0a0a 2020 2020 2020 2020 5265  dict..        Re
-000146c0: 7475 726e 0a20 2020 2020 2020 202d 2d2d  turn.        ---
-000146d0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-000146e0: 2c20 4661 6c73 652c 2073 7472 0a20 2020  , False, str.   
-000146f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00014700: 2023 204a 7573 7420 6120 6e61 6d65 0a20   # Just a name. 
-00014710: 2020 2020 2020 2023 2046 4958 4d45 3a20         # FIXME: 
-00014720: 7265 616c 6c79 3f0a 2020 2020 2020 2020  really?.        
-00014730: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
-00014740: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-00014750: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00014760: 7367 6c6f 6361 746f 722e 7061 7273 655f  sglocator.parse_
-00014770: 6174 7472 2822 6e61 6d65 222c 2064 6129  attr("name", da)
-00014780: 5b31 5d0a 0a20 2020 2020 2020 2023 2046  [1]..        # F
-00014790: 726f 6d20 636f 6e66 6967 0a20 2020 2020  rom config.     
-000147a0: 2020 2023 2069 6620 2263 665f 6c6f 6322     # if "cf_loc"
-000147b0: 2069 6e20 6461 2e65 6e63 6f64 696e 673a   in da.encoding:
-000147c0: 2020 2320 416c 7265 6164 7920 696e 6665    # Already infe
-000147d0: 7265 6420 616e 6420 7374 6f72 6564 2069  red and stored i
-000147e0: 6e20 656e 636f 6469 6e67 0a20 2020 2020  n encoding.     
-000147f0: 2020 2023 2020 2020 206c 6f63 203d 2064     #     loc = d
-00014800: 612e 656e 636f 6469 6e67 5b22 6366 5f6c  a.encoding["cf_l
-00014810: 6f63 225d 0a20 2020 2020 2020 2023 2065  oc"].        # e
-00014820: 6c73 653a 2020 2320 496e 6665 7220 6672  lse:  # Infer fr
-00014830: 6f6d 2063 6f6e 6669 670a 2020 2020 2020  om config.      
-00014840: 2020 6966 206c 6f63 6174 696f 6e73 2069    if locations i
-00014850: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00014860: 2020 2020 6c6f 6361 7469 6f6e 7320 3d20      locations = 
-00014870: 7365 6c66 2e67 6574 5f6c 6f63 5f6d 6170  self.get_loc_map
-00014880: 7069 6e67 2864 612c 2063 665f 6e61 6d65  ping(da, cf_name
-00014890: 733d 7b64 612e 6e61 6d65 3a20 6366 5f6e  s={da.name: cf_n
-000148a0: 616d 657d 290a 2020 2020 2020 2020 6c6f  ame}).        lo
-000148b0: 6320 3d20 6c6f 6361 7469 6f6e 732e 6765  c = locations.ge
-000148c0: 7428 6461 2e6e 616d 6529 0a20 2020 2020  t(da.name).     
-000148d0: 2020 2069 6620 6c6f 6320 6973 206e 6f74     if loc is not
-000148e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000148f0: 2020 2072 6574 7572 6e20 6c6f 630a 0a20     return loc.. 
-00014900: 2020 2020 2020 2023 2046 726f 6d20 7468         # From th
-00014910: 6520 6172 7261 7920 6174 7472 6962 7574  e array attribut
-00014920: 6573 0a20 2020 2020 2020 2072 6574 7572  es.        retur
-00014930: 6e20 7365 6c66 2e73 676c 6f63 6174 6f72  n self.sglocator
-00014940: 2e67 6574 5f6c 6f63 5f66 726f 6d5f 6461  .get_loc_from_da
-00014950: 2864 6129 0a0a 2020 2020 6465 6620 666f  (da)..    def fo
-00014960: 726d 6174 5f64 6174 6161 7272 6179 280a  rmat_dataarray(.
-00014970: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00014980: 2020 2020 2020 6461 2c0a 2020 2020 2020        da,.      
-00014990: 2020 6366 5f6e 616d 653d 4e6f 6e65 2c0a    cf_name=None,.
-000149a0: 2020 2020 2020 2020 7265 6e61 6d65 3d54          rename=T
-000149b0: 7275 652c 0a20 2020 2020 2020 2073 7065  rue,.        spe
-000149c0: 6369 616c 697a 653d 4661 6c73 652c 0a20  cialize=False,. 
-000149d0: 2020 2020 2020 2023 2072 656e 616d 655f         # rename_
-000149e0: 6469 6d3d 5472 7565 2c0a 2020 2020 2020  dim=True,.      
-000149f0: 2020 6c6f 633d 4e6f 6e65 2c0a 2020 2020    loc=None,.    
-00014a00: 2020 2020 6174 7472 733d 5472 7565 2c0a      attrs=True,.
-00014a10: 2020 2020 2020 2020 7374 616e 6461 7264          standard
-00014a20: 697a 653d 5472 7565 2c0a 2020 2020 2020  ize=True,.      
-00014a30: 2020 7265 706c 6163 655f 6174 7472 733d    replace_attrs=
-00014a40: 4661 6c73 652c 0a20 2020 2020 2020 2063  False,.        c
-00014a50: 6f70 793d 5472 7565 2c0a 2020 2020 2020  opy=True,.      
-00014a60: 2020 2320 6164 645f 6c6f 635f 746f 5f6e    # add_loc_to_n
-00014a70: 616d 653d 4e6f 6e65 2c0a 2020 2020 2020  ame=None,.      
-00014a80: 2020 626f 756e 645f 746f 3d4e 6f6e 652c    bound_to=None,
-00014a90: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00014aa0: 2222 2246 6f72 6d61 7420 6120 4461 7461  """Format a Data
-00014ab0: 4172 7261 7927 7320 6e61 6d65 2061 6e64  Array's name and
-00014ac0: 2061 7474 7269 6275 7465 730a 0a20 2020   attributes..   
-00014ad0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00014ae0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00014af0: 2d2d 0a20 2020 2020 2020 2064 613a 2078  --.        da: x
-00014b00: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
-00014b10: 2020 2020 2020 2020 6366 5f6e 616d 653a          cf_name:
-00014b20: 2073 7472 2c20 4e6f 6e65 0a20 2020 2020   str, None.     
-00014b30: 2020 2020 2020 2041 2067 656e 6572 6963         A generic
-00014b40: 2043 4620 6e61 6d65 2e20 4966 206e 6f74   CF name. If not
-00014b50: 2070 726f 7669 6465 642c 2069 7420 6775   provided, it gu
-00014b60: 6573 7365 6420 7769 7468 203a 6d65 7468  essed with :meth
-00014b70: 3a60 6d61 7463 6860 2e0a 2020 2020 2020  :`match`..      
-00014b80: 2020 6c6f 633a 2073 7472 2c20 7b22 616e    loc: str, {"an
-00014b90: 7922 2c20 4e6f 6e65 7d2c 207b 2222 2c20  y", None}, {"", 
-00014ba0: 4661 6c73 657d 0a20 2020 2020 2020 2020  False}.         
-00014bb0: 2020 202d 2073 7472 3a20 6f6e 6520 6f66     - str: one of
-00014bc0: 2074 6865 7365 206c 6f63 6174 696f 6e73   these locations
-00014bd0: 0a20 2020 2020 2020 2020 2020 202d 204e  .            - N
-00014be0: 6f6e 6520 6f72 2022 616e 7922 3a20 616e  one or "any": an
-00014bf0: 790a 2020 2020 2020 2020 2020 2020 2d20  y.            - 
-00014c00: 4661 6c73 6520 6f72 2027 2222 3a20 6e6f  False or '"": no
-00014c10: 206c 6f63 6174 696f 6e0a 2020 2020 2020   location.      
-00014c20: 2020 7265 6e61 6d65 3a20 626f 6f6c 0a20    rename: bool. 
-00014c30: 2020 2020 2020 2020 2020 2052 656e 616d             Renam
-00014c40: 6520 6172 7261 7973 2077 6865 6e20 7468  e arrays when th
-00014c50: 6569 7220 6e61 6d65 2069 7320 7365 743f  eir name is set?
-00014c60: 0a20 2020 2020 2020 2061 6464 5f6c 6f63  .        add_loc
-00014c70: 5f74 6f5f 6e61 6d65 3a20 4e6f 6e65 2c20  _to_name: None, 
-00014c80: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
-00014c90: 2041 6464 2074 6865 206c 6f63 2074 6f20   Add the loc to 
-00014ca0: 7468 6520 6e61 6d65 2c20 6f76 6572 7269  the name, overri
-00014cb0: 6469 6e67 2074 6865 2073 7065 6373 2e0a  ding the specs..
-00014cc0: 2020 2020 2020 2020 6174 7472 733a 2062          attrs: b
-00014cd0: 6f6f 6c2c 2064 6963 740a 2020 2020 2020  ool, dict.      
-00014ce0: 2020 2020 2020 4966 2046 616c 7365 2c20        If False, 
-00014cf0: 646f 6573 206e 6f74 2063 6861 6e67 6520  does not change 
-00014d00: 6174 7472 6962 7574 6573 2061 7420 616c  attributes at al
-00014d10: 6c2e 0a20 2020 2020 2020 2020 2020 2049  l..            I
-00014d20: 6620 5472 7565 2c20 7573 6520 4366 2061  f True, use Cf a
-00014d30: 7474 7269 6275 7465 732e 0a20 2020 2020  ttributes..     
-00014d40: 2020 2020 2020 2049 6620 6120 6469 6374         If a dict
-00014d50: 2c20 7573 6520 7468 6973 2064 6963 742e  , use this dict.
-00014d60: 0a20 2020 2020 2020 2072 6570 6c61 6365  .        replace
-00014d70: 5f61 7474 7273 3a20 626f 6f6c 0a20 2020  _attrs: bool.   
-00014d80: 2020 2020 2020 2020 2052 6570 6c61 6365           Replace
-00014d90: 2065 7869 7374 696e 6720 6174 7472 6962   existing attrib
-00014da0: 7574 6573 3f0a 2020 2020 2020 2020 7374  utes?.        st
-00014db0: 616e 6461 7264 697a 653a 2062 6f6f 6c0a  andardize: bool.
-00014dc0: 2020 2020 2020 2020 7370 6563 6961 6c69          speciali
-00014dd0: 7a65 3a20 626f 6f6c 0a20 2020 2020 2020  ze: bool.       
-00014de0: 2020 2020 2044 6f20 6e6f 7420 7573 6520       Do not use 
-00014df0: 7468 6520 4346 206e 616d 6520 666f 7220  the CF name for 
-00014e00: 7265 6e61 6d69 6e67 2c20 6275 7420 7468  renaming, but th
-00014e10: 6520 7661 6c75 6520 6f66 2074 6865 2022  e value of the "
-00014e20: 6e61 6d65 2220 656e 7472 792c 0a20 2020  name" entry,.   
-00014e30: 2020 2020 2020 2020 2077 6869 6368 2069           which i
-00014e40: 7320 6765 6e65 7261 6c6c 7920 6120 7370  s generally a sp
-00014e50: 6563 6961 6c69 7a65 6420 6f6e 652c 206c  ecialized one, l
-00014e60: 696b 6520 6120 6e61 6d65 2061 646f 7074  ike a name adopt
-00014e70: 6564 2062 7920 7370 6563 6961 6c69 7a65  ed by specialize
-00014e80: 6420 6461 7461 7365 742e 0a20 2020 2020  d dataset..     
-00014e90: 2020 2072 656e 616d 655f 6469 6d3a 2062     rename_dim: b
-00014ea0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-00014eb0: 466f 7220 6120 3144 2061 7272 6179 2c20  For a 1D array, 
-00014ec0: 7265 6e61 6d65 2074 6865 2064 696d 656e  rename the dimen
-00014ed0: 7369 6f6e 2069 6620 6974 2068 6173 2074  sion if it has t
-00014ee0: 6865 2073 616d 6520 6e61 6d65 0a20 2020  he same name.   
-00014ef0: 2020 2020 2020 2020 2061 7320 7468 6520           as the 
-00014f00: 6172 7261 792e 0a20 2020 2020 2020 2020  array..         
-00014f10: 2020 204e 6f74 6520 7468 6174 2069 7420     Note that it 
-00014f20: 6973 2073 6574 2074 6f20 4661 6c73 652c  is set to False,
-00014f30: 2069 6620 6060 7265 6e61 6d65 6060 2069   if ``rename`` i
-00014f40: 7320 4661 6c73 652e 0a20 2020 2020 2020  s False..       
-00014f50: 2063 6f70 793a 2062 6f6f 6c0a 2020 2020   copy: bool.    
-00014f60: 2020 2020 2020 2020 466f 7263 6520 6120          Force a 
-00014f70: 636f 7079 2028 6e6f 7420 6f66 2074 6865  copy (not of the
-00014f80: 2064 6174 6129 2069 6e20 616e 7920 6361   data) in any ca
-00014f90: 7365 3f0a 0a20 2020 2020 2020 2052 6574  se?..        Ret
-00014fa0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00014fb0: 2d2d 2d2d 0a20 2020 2020 2020 2078 6172  ----.        xar
-00014fc0: 7261 792e 4461 7461 4172 7261 792c 2073  ray.DataArray, s
-00014fd0: 7472 2c20 4e6f 6e65 0a20 2020 2020 2020  tr, None.       
-00014fe0: 2020 2020 2054 6865 2066 6f72 6d61 7474       The formatt
-00014ff0: 6564 2061 7272 6179 206f 7220 636f 7079  ed array or copy
-00015000: 206f 6620 6974 2e0a 2020 2020 2020 2020   of it..        
-00015010: 2020 2020 5468 6520 4346 206e 616d 652c      The CF name,
-00015020: 2067 6976 656e 206f 7220 6d61 7463 6869   given or matchi
-00015030: 6e67 2c20 6966 2072 656e 616d 6520 6966  ng, if rename if
-00015040: 2046 616c 7365 3b20 616e 6420 4e6f 6e65   False; and None
-00015050: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00015060: 6e6f 7420 6d61 7463 6869 6e67 2e0a 0a20  not matching... 
-00015070: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00015080: 2020 2069 6620 7265 6e61 6d65 3a0a 2020     if rename:.  
-00015090: 2020 2020 2020 2020 2020 636f 7079 203d            copy =
-000150a0: 2054 7275 650a 2020 2020 2020 2020 6966   True.        if
-000150b0: 2063 6f70 793a 0a20 2020 2020 2020 2020   copy:.         
-000150c0: 2020 2064 6120 3d20 6461 2e63 6f70 7928     da = da.copy(
-000150d0: 290a 0a20 2020 2020 2020 2023 204e 616d  )..        # Nam
-000150e0: 6573 0a20 2020 2020 2020 2069 6620 6366  es.        if cf
-000150f0: 5f6e 616d 6520 6973 204e 6f6e 653a 0a20  _name is None:. 
-00015100: 2020 2020 2020 2020 2020 2063 665f 6e61             cf_na
-00015110: 6d65 203d 2073 656c 662e 6d61 7463 6828  me = self.match(
-00015120: 6461 290a 2020 2020 2020 2020 6966 2063  da).        if c
-00015130: 665f 6e61 6d65 2069 7320 4e6f 6e65 3a0a  f_name is None:.
-00015140: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00015150: 6f74 2072 656e 616d 653a 0a20 2020 2020  ot rename:.     
-00015160: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00015170: 6e0a 2020 2020 2020 2020 2020 2020 7265  n.            re
-00015180: 7475 726e 2064 612e 636f 7079 2829 2069  turn da.copy() i
-00015190: 6620 636f 7079 2065 6c73 6520 4e6f 6e65  f copy else None
-000151a0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000151b0: 6366 5f6e 616d 6520 696e 2073 656c 662e  cf_name in self.
-000151c0: 6e61 6d65 730a 2020 2020 2020 2020 6f6c  names.        ol
-000151d0: 645f 6e61 6d65 203d 2064 612e 6e61 6d65  d_name = da.name
-000151e0: 0a20 2020 2020 2020 206e 6577 5f6e 616d  .        new_nam
-000151f0: 6520 3d20 7365 6c66 2e67 6574 5f6e 616d  e = self.get_nam
-00015200: 6528 6366 5f6e 616d 652c 2073 7065 6369  e(cf_name, speci
-00015210: 616c 697a 653d 7370 6563 6961 6c69 7a65  alize=specialize
-00015220: 2920 2023 2069 6620 7370 6563 6961 6c69  )  # if speciali
-00015230: 7a65 2065 6c73 6520 6366 5f6e 616d 650a  ze else cf_name.
-00015240: 0a20 2020 2020 2020 2023 204c 6f63 6174  .        # Locat
-00015250: 696f 6e0a 2020 2020 2020 2020 6966 206c  ion.        if l
-00015260: 6f63 2069 7320 4e6f 6e65 3a0a 2020 2020  oc is None:.    
-00015270: 2020 2020 2020 2020 6c6f 6320 3d20 7365          loc = se
-00015280: 6c66 2e67 6574 5f6c 6f63 5f61 7267 2864  lf.get_loc_arg(d
-00015290: 6129 2020 2320 6672 6f6d 2063 6f6e 6669  a)  # from confi
-000152a0: 670a 0a20 2020 2020 2020 2023 2041 7474  g..        # Att
-000152b0: 7269 6275 7465 730a 2020 2020 2020 2020  ributes.        
-000152c0: 6966 2061 7474 7273 2069 7320 5472 7565  if attrs is True
-000152d0: 3a0a 0a20 2020 2020 2020 2020 2020 2023  :..            #
-000152e0: 2047 6574 2061 7474 7269 6275 7465 7320   Get attributes 
-000152f0: 6672 6f6d 2043 6620 7370 6563 730a 2020  from Cf specs.  
-00015300: 2020 2020 2020 2020 2020 6174 7472 7320            attrs 
-00015310: 3d20 7365 6c66 2e67 6574 5f61 7474 7273  = self.get_attrs
-00015320: 2863 665f 6e61 6d65 2c20 6c6f 633d 4e6f  (cf_name, loc=No
-00015330: 6e65 2c20 7374 616e 6461 7264 697a 653d  ne, standardize=
-00015340: 4661 6c73 652c 206d 756c 7469 3d54 7275  False, multi=Tru
-00015350: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
-00015360: 2320 5265 6d6f 7665 2061 7869 7320 6174  # Remove axis at
-00015370: 7472 6962 7574 6520 666f 7220 6175 7869  tribute for auxi
-00015380: 6c61 7279 2063 6f6f 7264 696e 6174 6573  lary coordinates
-00015390: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000153a0: 6461 2e6e 616d 6520 616e 6420 6461 2e6e  da.name and da.n
-000153b0: 616d 6520 6e6f 7420 696e 2064 612e 696e  ame not in da.in
-000153c0: 6465 7865 7320 616e 6420 2261 7869 7322  dexes and "axis"
-000153d0: 2069 6e20 6174 7472 733a 0a20 2020 2020   in attrs:.     
-000153e0: 2020 2020 2020 2020 2020 2064 656c 2061             del a
-000153f0: 7474 7273 5b22 6178 6973 225d 0a0a 2020  ttrs["axis"]..  
-00015400: 2020 2020 2020 656c 6966 206e 6f74 2061        elif not a
-00015410: 7474 7273 3a0a 2020 2020 2020 2020 2020  ttrs:.          
-00015420: 2020 6174 7472 7320 3d20 7b7d 0a0a 2020    attrs = {}..  
-00015430: 2020 2020 2020 2320 466f 726d 6174 2061        # Format a
-00015440: 7272 6179 0a20 2020 2020 2020 206e 6577  rray.        new
-00015450: 5f64 6120 3d20 7365 6c66 2e73 676c 6f63  _da = self.sgloc
-00015460: 6174 6f72 2e66 6f72 6d61 745f 6461 7461  ator.format_data
-00015470: 6172 7261 7928 0a20 2020 2020 2020 2020  array(.         
-00015480: 2020 2064 612c 0a20 2020 2020 2020 2020     da,.         
-00015490: 2020 206c 6f63 3d6c 6f63 2c0a 2020 2020     loc=loc,.    
-000154a0: 2020 2020 2020 2020 6e61 6d65 3d6e 6577          name=new
-000154b0: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
-000154c0: 2020 2061 7474 7273 3d61 7474 7273 2c0a     attrs=attrs,.
-000154d0: 2020 2020 2020 2020 2020 2020 7374 616e              stan
-000154e0: 6461 7264 697a 653d 7374 616e 6461 7264  dardize=standard
-000154f0: 697a 652c 0a20 2020 2020 2020 2020 2020  ize,.           
-00015500: 2072 656e 616d 653d 7265 6e61 6d65 2c0a   rename=rename,.
-00015510: 2020 2020 2020 2020 2020 2020 2320 6164              # ad
-00015520: 645f 6c6f 635f 746f 5f6e 616d 653d 6164  d_loc_to_name=ad
-00015530: 645f 6c6f 635f 746f 5f6e 616d 652c 0a20  d_loc_to_name,. 
-00015540: 2020 2020 2020 2020 2020 2072 6570 6c61             repla
-00015550: 6365 5f61 7474 7273 3d72 6570 6c61 6365  ce_attrs=replace
-00015560: 5f61 7474 7273 2c0a 2020 2020 2020 2020  _attrs,.        
-00015570: 2020 2020 636f 7079 3d46 616c 7365 2c0a      copy=False,.
-00015580: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00015590: 2020 2320 6e65 775f 6461 2e65 6e63 6f64    # new_da.encod
-000155a0: 696e 675b 2263 665f 6e61 6d65 225d 203d  ing["cf_name"] =
-000155b0: 2063 665f 6e61 6d65 0a0a 2020 2020 2020   cf_name..      
-000155c0: 2020 2320 5265 7475 726e 206e 6577 206e    # Return new n
-000155d0: 616d 6520 6275 7420 646f 6e27 7420 7265  ame but don't re
-000155e0: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
-000155f0: 6e6f 7420 7265 6e61 6d65 3a0a 2020 2020  not rename:.    
-00015600: 2020 2020 2020 2020 6966 206f 6c64 5f6e          if old_n
-00015610: 616d 6520 6973 204e 6f6e 653a 0a20 2020  ame is None:.   
-00015620: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00015630: 7572 6e20 7365 6c66 2e73 676c 6f63 6174  urn self.sglocat
-00015640: 6f72 2e66 6f72 6d61 745f 6174 7472 2822  or.format_attr("
-00015650: 6e61 6d65 222c 206e 6577 5f6e 616d 652c  name", new_name,
-00015660: 206c 6f63 290a 2020 2020 2020 2020 2020   loc).          
-00015670: 2020 7265 7475 726e 2073 656c 662e 7367    return self.sg
-00015680: 6c6f 6361 746f 722e 6d65 7267 655f 6174  locator.merge_at
-00015690: 7472 2822 6e61 6d65 222c 206f 6c64 5f6e  tr("name", old_n
-000156a0: 616d 652c 206e 6577 5f6e 616d 652c 206c  ame, new_name, l
-000156b0: 6f63 290a 0a20 2020 2020 2020 2023 2023  oc)..        # #
-000156c0: 2052 656e 616d 6520 6469 6d20 6966 2061   Rename dim if a
-000156d0: 7869 7320 636f 6f72 6469 6e61 7465 0a20  xis coordinate. 
-000156e0: 2020 2020 2020 2023 2072 656e 616d 655f         # rename_
-000156f0: 6469 6d20 3d20 7265 6e61 6d65 2061 6e64  dim = rename and
-00015700: 2072 656e 616d 655f 6469 6d0a 2020 2020   rename_dim.    
-00015710: 2020 2020 2320 6966 2028 7265 6e61 6d65      # if (rename
-00015720: 5f64 696d 2061 6e64 206f 6c64 5f6e 616d  _dim and old_nam
-00015730: 6520 616e 6420 6f6c 645f 6e61 6d65 2069  e and old_name i
-00015740: 6e20 6461 2e69 6e64 6578 6573 293a 0a20  n da.indexes):. 
-00015750: 2020 2020 2020 2023 2020 2020 206e 6577         #     new
-00015760: 5f64 6120 3d20 6e65 775f 6461 2e72 656e  _da = new_da.ren
-00015770: 616d 6528 7b6f 6c64 5f6e 616d 653a 206e  ame({old_name: n
-00015780: 6577 5f64 612e 6e61 6d65 7d29 0a0a 2020  ew_da.name})..  
-00015790: 2020 2020 2020 7265 7475 726e 206e 6577        return new
-000157a0: 5f64 610a 0a20 2020 2064 6566 2072 656e  _da..    def ren
-000157b0: 616d 655f 6461 7461 6172 7261 7928 0a20  ame_dataarray(. 
-000157c0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000157d0: 2020 2020 2064 612c 0a20 2020 2020 2020       da,.       
-000157e0: 206e 616d 653d 4e6f 6e65 2c0a 2020 2020   name=None,.    
-000157f0: 2020 2020 7370 6563 6961 6c69 7a65 3d46      specialize=F
-00015800: 616c 7365 2c0a 2020 2020 2020 2020 6c6f  alse,.        lo
-00015810: 633d 4e6f 6e65 2c0a 2020 2020 2020 2020  c=None,.        
-00015820: 7374 616e 6461 7264 697a 653d 5472 7565  standardize=True
-00015830: 2c0a 2020 2020 2020 2020 7265 6e61 6d65  ,.        rename
-00015840: 5f64 696d 3d54 7275 652c 0a20 2020 2020  _dim=True,.     
-00015850: 2020 2063 6f70 793d 5472 7565 2c0a 2020     copy=True,.  
-00015860: 2020 2020 2020 6164 645f 6c6f 635f 746f        add_loc_to
-00015870: 5f6e 616d 653d 4e6f 6e65 2c0a 2020 2020  _name=None,.    
-00015880: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
-00015890: 6e61 6d65 2061 2044 6174 6141 7272 6179  name a DataArray
-000158a0: 0a0a 2020 2020 2020 2020 4974 2069 7320  ..        It is 
-000158b0: 6120 7370 6563 6961 6c69 7a65 6420 6361  a specialized ca
-000158c0: 6c6c 2074 6f20 3a6d 6574 683a 6066 6f72  ll to :meth:`for
-000158d0: 6d61 745f 6461 7461 6172 7261 7960 2077  mat_dataarray` w
-000158e0: 6865 7265 0a20 2020 2020 2020 2061 7474  here.        att
-000158f0: 7269 6275 7465 7320 6172 6520 6c65 6674  ributes are left
-00015900: 2075 6e63 6861 6e67 6564 2e0a 0a20 2020   unchanged...   
-00015910: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00015920: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00015930: 2d2d 0a20 2020 2020 2020 2064 613a 2078  --.        da: x
-00015940: 6172 7261 792e 4461 7461 4172 7261 790a  array.DataArray.
-00015950: 2020 2020 2020 2020 6e61 6d65 3a20 7374          name: st
-00015960: 722c 204e 6f6e 650a 2020 2020 2020 2020  r, None.        
-00015970: 2020 2020 4120 4346 206e 616d 652e 2049      A CF name. I
-00015980: 6620 6e6f 7420 7072 6f76 6964 6564 2c20  f not provided, 
-00015990: 6974 2067 7565 7373 6564 2077 6974 6820  it guessed with 
-000159a0: 3a6d 6574 683a 606d 6174 6368 602e 0a20  :meth:`match`.. 
-000159b0: 2020 2020 2020 2073 7065 6369 616c 697a         specializ
-000159c0: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
-000159d0: 2020 2020 446f 6573 206e 6f74 2075 7365      Does not use
-000159e0: 2074 6865 2043 4620 6e61 6d65 2066 6f72   the CF name for
-000159f0: 2072 656e 616d 696e 672c 2062 7574 2074   renaming, but t
-00015a00: 6865 2066 6972 7374 206e 616d 650a 2020  he first name.  
-00015a10: 2020 2020 2020 2020 2020 6173 206c 6973            as lis
-00015a20: 7465 6420 696e 2073 7065 6373 2c20 7768  ted in specs, wh
-00015a30: 6963 6820 6973 2067 656e 6572 616c 6c79  ich is generally
-00015a40: 2061 2073 7065 6369 616c 697a 6564 206f   a specialized o
-00015a50: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00015a60: 6c69 6b65 2061 206e 616d 6520 6164 6f70  like a name adop
-00015a70: 7465 6420 6279 2073 7065 6369 616c 697a  ted by specializ
-00015a80: 6564 2064 6174 6173 6574 2e0a 2020 2020  ed dataset..    
-00015a90: 2020 2020 6c6f 633a 2073 7472 2c20 7b22      loc: str, {"
-00015aa0: 616e 7922 2c20 4e6f 6e65 7d2c 207b 2222  any", None}, {""
-00015ab0: 2c20 4661 6c73 657d 0a20 2020 2020 2020  , False}.       
-00015ac0: 2020 2020 202d 2073 7472 3a20 6f6e 6520       - str: one 
-00015ad0: 6f66 2074 6865 7365 206c 6f63 6174 696f  of these locatio
-00015ae0: 6e73 0a20 2020 2020 2020 2020 2020 202d  ns.            -
-00015af0: 204e 6f6e 6520 6f72 2022 616e 7922 3a20   None or "any": 
-00015b00: 616e 790a 2020 2020 2020 2020 2020 2020  any.            
-00015b10: 2d20 4661 6c73 6520 6f72 2027 2222 3a20  - False or '"": 
-00015b20: 6e6f 206c 6f63 6174 696f 6e0a 2020 2020  no location.    
-00015b30: 2020 2020 7374 616e 6461 7264 697a 653a      standardize:
-00015b40: 2062 6f6f 6c0a 2020 2020 2020 2020 7265   bool.        re
-00015b50: 6e61 6d65 5f64 696d 3a20 626f 6f6c 0a20  name_dim: bool. 
-00015b60: 2020 2020 2020 2020 2020 2046 6f72 2061             For a
-00015b70: 2031 4420 6172 7261 792c 2072 656e 616d   1D array, renam
-00015b80: 6520 7468 6520 6469 6d65 6e73 696f 6e20  e the dimension 
-00015b90: 6966 2069 7420 6861 7320 7468 6520 7361  if it has the sa
-00015ba0: 6d65 206e 616d 650a 2020 2020 2020 2020  me name.        
-00015bb0: 2020 2020 6173 2074 6865 2061 7272 6179      as the array
-00015bc0: 2e0a 2020 2020 2020 2020 2020 2020 4e6f  ..            No
-00015bd0: 7465 2074 6861 7420 6974 2069 7320 7365  te that it is se
-00015be0: 7420 746f 2046 616c 7365 2c20 6966 2060  t to False, if `
-00015bf0: 6072 656e 616d 6560 6020 6973 2046 616c  `rename`` is Fal
-00015c00: 7365 2e0a 2020 2020 2020 2020 636f 7079  se..        copy
-00015c10: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
-00015c20: 2020 2046 6f72 6365 2061 2063 6f70 7920     Force a copy 
-00015c30: 286e 6f74 206f 6620 7468 6520 6461 7461  (not of the data
-00015c40: 2920 696e 2061 6e79 2063 6173 653f 0a0a  ) in any case?..
-00015c50: 0a20 2020 2020 2020 2053 6565 2061 6c73  .        See als
-00015c60: 6f0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  o.        ------
-00015c70: 2d2d 0a20 2020 2020 2020 2066 6f72 6d61  --.        forma
-00015c80: 745f 6461 7461 6172 7261 790a 2020 2020  t_dataarray.    
-00015c90: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00015ca0: 7265 7475 726e 2073 656c 662e 666f 726d  return self.form
-00015cb0: 6174 5f64 6174 6161 7272 6179 280a 2020  at_dataarray(.  
-00015cc0: 2020 2020 2020 2020 2020 6461 2c0a 2020            da,.  
-00015cd0: 2020 2020 2020 2020 2020 6e61 6d65 3d6e            name=n
-00015ce0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00015cf0: 2073 7065 6369 616c 697a 653d 7370 6563   specialize=spec
-00015d00: 6961 6c69 7a65 2c0a 2020 2020 2020 2020  ialize,.        
-00015d10: 2020 2020 6c6f 633d 6c6f 632c 0a20 2020      loc=loc,.   
-00015d20: 2020 2020 2020 2020 2061 7474 7273 3d46           attrs=F
-00015d30: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00015d40: 2020 7374 616e 6461 7264 697a 653d 7374    standardize=st
-00015d50: 616e 6461 7264 697a 652c 0a20 2020 2020  andardize,.     
-00015d60: 2020 2020 2020 2072 656e 616d 655f 6469         rename_di
-00015d70: 6d3d 7265 6e61 6d65 5f64 696d 2c0a 2020  m=rename_dim,.  
-00015d80: 2020 2020 2020 2020 2020 636f 7079 3d63            copy=c
-00015d90: 6f70 792c 0a20 2020 2020 2020 2020 2020  opy,.           
-00015da0: 2061 6464 5f6c 6f63 5f74 6f5f 6e61 6d65   add_loc_to_name
-00015db0: 3d61 6464 5f6c 6f63 5f74 6f5f 6e61 6d65  =add_loc_to_name
-00015dc0: 2c0a 2020 2020 2020 2020 290a 0a0a 636c  ,.        )...cl
-00015dd0: 6173 7320 4346 5661 7253 7065 6373 285f  ass CFVarSpecs(_
-00015de0: 4346 4361 7453 7065 6373 5f29 3a0a 2020  CFCatSpecs_):.  
-00015df0: 2020 2222 2243 4620 7370 6563 6966 6963    """CF specific
-00015e00: 6174 696f 6e20 666f 7220 6461 7461 5f76  ation for data_v
-00015e10: 6172 7322 2222 0a0a 2020 2020 6361 7465  ars"""..    cate
-00015e20: 676f 7279 203d 2022 6461 7461 5f76 6172  gory = "data_var
-00015e30: 7322 0a0a 0a63 6c61 7373 2043 4643 6f6f  s"...class CFCoo
-00015e40: 7264 5370 6563 7328 5f43 4643 6174 5370  rdSpecs(_CFCatSp
-00015e50: 6563 735f 293a 0a20 2020 2022 2222 4346  ecs_):.    """CF
-00015e60: 2073 7065 6369 6669 6361 7469 6f6e 2066   specification f
-00015e70: 6f72 2063 6f6f 7264 7322 2222 0a0a 2020  or coords"""..  
-00015e80: 2020 6361 7465 676f 7279 203d 2022 636f    category = "co
-00015e90: 6f72 6473 220a 0a20 2020 2064 6566 2067  ords"..    def g
-00015ea0: 6574 5f6c 6f63 5f6d 6170 7069 6e67 2873  et_loc_mapping(s
-00015eb0: 656c 662c 2064 612c 2063 665f 6e61 6d65  elf, da, cf_name
-00015ec0: 733d 4e6f 6e65 293a 0a20 2020 2020 2020  s=None):.       
-00015ed0: 2072 6574 7572 6e20 7365 6c66 2e70 6172   return self.par
-00015ee0: 656e 742e 6765 745f 6c6f 635f 6d61 7070  ent.get_loc_mapp
-00015ef0: 696e 6728 6461 2c20 6366 5f6e 616d 6573  ing(da, cf_names
-00015f00: 3d63 665f 6e61 6d65 732c 2063 6174 6567  =cf_names, categ
-00015f10: 6f72 6965 733d 5b22 636f 6f72 6473 225d  ories=["coords"]
-00015f20: 290a 0a20 2020 2064 6566 2067 6574 5f61  )..    def get_a
-00015f30: 7869 7328 7365 6c66 2c20 636f 6f72 642c  xis(self, coord,
-00015f40: 206c 6f77 6572 3d46 616c 7365 293a 0a20   lower=False):. 
-00015f50: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
-00015f60: 6520 6469 6d65 6e73 696f 6e20 7479 7065  e dimension type
-00015f70: 2c20 6569 7468 6572 2066 726f 6d20 6178  , either from ax
-00015f80: 6973 2061 7474 7220 6f72 2066 726f 6d20  is attr or from 
-00015f90: 6d61 7463 6820 4366 2063 6f6f 7264 0a0a  match Cf coord..
-00015fa0: 2020 2020 2020 2020 2e2e 206e 6f74 653a          .. note:
-00015fb0: 3a20 5468 6520 6060 6178 6973 6060 2069  : The ``axis`` i
-00015fc0: 7320 7468 6520 7570 7065 7263 6173 6520  s the uppercase 
-00015fd0: 7665 7273 696f 6e20 6f66 2074 6865 2060  version of the `
-00015fe0: 6064 696d 5f74 7970 6560 600a 0a20 2020  `dim_type``..   
-00015ff0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00016000: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00016010: 2d2d 0a20 2020 2020 2020 2063 6f6f 7264  --.        coord
-00016020: 3a20 7861 7272 6179 2e44 6174 6141 7272  : xarray.DataArr
-00016030: 6179 0a20 2020 2020 2020 206c 6f77 6572  ay.        lower
-00016040: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
-00016050: 2020 204c 6f77 6572 2063 6173 653f 0a0a     Lower case?..
-00016060: 2020 2020 2020 2020 5265 7475 726e 0a20          Return. 
-00016070: 2020 2020 2020 202d 2d2d 2d2d 2d0a 2020         ------.  
-00016080: 2020 2020 2020 7b22 7822 2c20 2279 222c        {"x", "y",
-00016090: 2022 7a22 2c20 2274 222c 2022 6622 7d2c   "z", "t", "f"},
-000160a0: 204e 6f6e 650a 0a20 2020 2020 2020 2053   None..        S
-000160b0: 6565 2061 6c73 6f0a 2020 2020 2020 2020  ee also.        
-000160c0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-000160d0: 2067 6574 5f64 696d 5f74 7970 650a 2020   get_dim_type.  
-000160e0: 2020 2020 2020 6765 745f 6469 6d5f 7479        get_dim_ty
-000160f0: 7065 730a 2020 2020 2020 2020 2222 220a  pes.        """.
-00016100: 2020 2020 2020 2020 6178 6973 203d 204e          axis = N
-00016110: 6f6e 650a 2020 2020 2020 2020 6966 2022  one.        if "
-00016120: 6178 6973 2220 696e 2063 6f6f 7264 2e61  axis" in coord.a
-00016130: 7474 7273 3a0a 2020 2020 2020 2020 2020  ttrs:.          
-00016140: 2020 6178 6973 203d 2063 6f6f 7264 2e61    axis = coord.a
-00016150: 7474 7273 5b22 6178 6973 225d 0a20 2020  ttrs["axis"].   
-00016160: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00016170: 2020 2020 2020 2063 666e 616d 6520 3d20         cfname = 
-00016180: 7365 6c66 2e6d 6174 6368 2863 6f6f 7264  self.match(coord
-00016190: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-000161a0: 2063 666e 616d 653a 0a20 2020 2020 2020   cfname:.       
-000161b0: 2020 2020 2020 2020 2061 7869 7320 3d20           axis = 
-000161c0: 7365 6c66 5b63 666e 616d 655d 5b22 6174  self[cfname]["at
-000161d0: 7472 7322 5d5b 2261 7869 7322 5d0a 2020  trs"]["axis"].  
-000161e0: 2020 2020 2020 6966 2061 7869 7320 6973        if axis is
-000161f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00016200: 2020 2020 2020 2069 6620 6c6f 7765 723a         if lower:
-00016210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016220: 2072 6574 7572 6e20 6178 6973 2e6c 6f77   return axis.low
-00016230: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
-00016240: 2072 6574 7572 6e20 6178 6973 2e75 7070   return axis.upp
-00016250: 6572 2829 0a0a 2020 2020 6465 6620 6765  er()..    def ge
-00016260: 745f 6469 6d5f 7479 7065 2873 656c 662c  t_dim_type(self,
-00016270: 2064 696d 2c20 6f62 6a3d 4e6f 6e65 2c20   dim, obj=None, 
-00016280: 6c6f 7765 723d 5472 7565 293a 0a20 2020  lower=True):.   
-00016290: 2020 2020 2022 2222 4765 7420 7468 6520       """Get the 
-000162a0: 7479 7065 206f 6620 6120 6469 6d65 6e73  type of a dimens
-000162b0: 696f 6e0a 0a20 2020 2020 2020 2054 6872  ion..        Thr
-000162c0: 6565 2063 6173 6573 3a0a 0a20 2020 2020  ee cases:..     
-000162d0: 2020 202d 2054 6869 7320 6469 6d65 6e73     - This dimens
-000162e0: 696f 6e20 6973 2072 6567 6973 7465 7265  ion is registere
-000162f0: 6420 696e 2043 4620 6469 6d73 2e0a 2020  d in CF dims..  
-00016300: 2020 2020 2020 2d20 6f62 6a20 6861 7320        - obj has 
-00016310: 6469 6d20 6173 2064 696d 2061 6e64 2068  dim as dim and h
-00016320: 6173 2061 6e20 6178 6973 2061 7474 7269  as an axis attri
-00016330: 6275 7465 2069 6e66 6572 7265 6420 7769  bute inferred wi
-00016340: 7468 203a 6d65 7468 3a60 6765 745f 6178  th :meth:`get_ax
-00016350: 6973 602e 0a20 2020 2020 2020 202d 206f  is`..        - o
-00016360: 626a 2068 6173 2061 2063 6f6f 7264 206e  bj has a coord n
-00016370: 616d 6564 2064 696d 2077 6974 6820 616e  amed dim with an
-00016380: 2061 7869 7320 6174 7472 6962 7574 6520   axis attribute 
-00016390: 696e 6665 7272 6564 2077 6974 6820 3a6d  inferred with :m
-000163a0: 6574 683a 6067 6574 5f61 7869 7360 2e0a  eth:`get_axis`..
-000163b0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-000163c0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-000163d0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2064  ------.        d
-000163e0: 696d 3a20 7374 720a 2020 2020 2020 2020  im: str.        
-000163f0: 2020 2020 4469 6d65 6e73 696f 6e20 6e61      Dimension na
-00016400: 6d65 0a20 2020 2020 2020 206f 626a 3a20  me.        obj: 
-00016410: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-00016420: 2c20 7861 7272 6179 2e44 6174 6173 6574  , xarray.Dataset
-00016430: 0a20 2020 2020 2020 2020 2020 2044 6174  .            Dat
-00016440: 6120 6172 7261 7920 7468 6174 2074 6865  a array that the
-00016450: 2064 696d 656e 7369 6f6e 2062 656c 6f6e   dimension belon
-00016460: 6773 2074 6f2c 2074 6f20 6865 6c70 2069  gs to, to help i
-00016470: 6e66 6572 7269 6e67 0a20 2020 2020 2020  nferring.       
-00016480: 2020 2020 2074 6865 2074 7970 650a 2020       the type.  
-00016490: 2020 2020 2020 6c6f 7765 723a 2062 6f6f        lower: boo
-000164a0: 6c0a 2020 2020 2020 2020 2020 2020 466f  l.            Fo
-000164b0: 7220 6c6f 7765 7220 6361 7365 0a0a 2020  r lower case..  
-000164c0: 2020 2020 2020 5265 7475 726e 0a20 2020        Return.   
-000164d0: 2020 2020 202d 2d2d 2d2d 2d0a 2020 2020       ------.    
-000164e0: 2020 2020 7374 722c 204e 6f6e 650a 2020      str, None.  
-000164f0: 2020 2020 2020 2020 2020 4c65 7474 6572            Letter
-00016500: 2061 7320 6f6e 6520 6f66 2078 2c20 792c   as one of x, y,
-00016510: 207a 2c20 7420 6f72 2066 2c20 6966 2066   z, t or f, if f
-00016520: 6f75 6e64 2c20 656c 7365 204e 6f6e 650a  ound, else None.
-00016530: 0a20 2020 2020 2020 2053 6565 2061 6c73  .        See als
-00016540: 6f0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  o.        ------
-00016550: 2d2d 0a20 2020 2020 2020 2067 6574 5f61  --.        get_a
-00016560: 7869 730a 2020 2020 2020 2020 2222 220a  xis.        """.
-00016570: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
-00016580: 206c 6f63 6174 696f 6e0a 2020 2020 2020   location.      
-00016590: 2020 6469 6d5f 6c6f 6320 3d20 6469 6d0a    dim_loc = dim.
-000165a0: 2020 2020 2020 2020 6469 6d20 3d20 7365          dim = se
-000165b0: 6c66 2e73 676c 6f63 6174 6f72 2e70 6172  lf.sglocator.par
-000165c0: 7365 5f61 7474 7228 276e 616d 6527 2c20  se_attr('name', 
-000165d0: 6469 6d29 5b30 5d0a 0a20 2020 2020 2020  dim)[0]..       
-000165e0: 2023 204c 6f6f 7020 6f6e 2074 7970 6573   # Loop on types
-000165f0: 0a20 2020 2020 2020 2069 6620 6469 6d2e  .        if dim.
-00016600: 6c6f 7765 7228 2920 696e 2073 656c 662e  lower() in self.
-00016610: 6469 6d73 3a0a 2020 2020 2020 2020 2020  dims:.          
-00016620: 2020 7265 7475 726e 2064 696d 2e6c 6f77    return dim.low
-00016630: 6572 2829 0a20 2020 2020 2020 2066 6f72  er().        for
-00016640: 2064 696d 5f74 7970 652c 2064 696d 7320   dim_type, dims 
-00016650: 696e 2073 656c 662e 6469 6d73 2e69 7465  in self.dims.ite
-00016660: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-00016670: 2020 6966 2064 696d 2e6c 6f77 6572 2829    if dim.lower()
-00016680: 2069 6e20 6469 6d73 3a0a 2020 2020 2020   in dims:.      
-00016690: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000166a0: 2064 696d 5f74 7970 650a 0a20 2020 2020   dim_type..     
-000166b0: 2020 2023 2043 6865 636b 2069 6620 6120     # Check if a 
-000166c0: 636f 6f72 6469 6e61 7465 2068 6176 6520  coordinate have 
-000166d0: 7468 6520 7361 6d65 206e 616d 6520 616e  the same name an
-000166e0: 6420 616e 2061 7869 7320 7479 7065 0a20  d an axis type. 
-000166f0: 2020 2020 2020 2069 6620 6f62 6a20 6973         if obj is
-00016700: 206e 6f74 204e 6f6e 653a 0a0a 2020 2020   not None:..    
-00016710: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
-00016720: 6469 6d20 7661 6c69 6469 7479 0a20 2020  dim validity.   
-00016730: 2020 2020 2020 2020 2069 6620 6469 6d5f           if dim_
-00016740: 6c6f 6320 6e6f 7420 696e 206f 626a 2e64  loc not in obj.d
-00016750: 696d 733a 0a20 2020 2020 2020 2020 2020  ims:.           
-00016760: 2020 2020 2072 6169 7365 2058 6f61 4346       raise XoaCF
-00016770: 4572 726f 7228 6622 6469 6d65 6e73 696f  Error(f"dimensio
-00016780: 6e20 277b 6469 6d7d 2720 646f 6573 206e  n '{dim}' does n
-00016790: 6f74 2062 656c 6f6e 6720 746f 206f 626a  ot belong to obj
-000167a0: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
-000167b0: 2320 4368 6563 6b20 6178 6973 2066 726f  # Check axis fro
-000167c0: 6d20 636f 6f72 6473 0a20 2020 2020 2020  m coords.       
-000167d0: 2020 2020 2069 6620 6469 6d20 696e 206f       if dim in o
-000167e0: 626a 2e69 6e64 6578 6573 3a0a 2020 2020  bj.indexes:.    
-000167f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00016800: 726e 2073 656c 662e 6765 745f 6178 6973  rn self.get_axis
-00016810: 286f 626a 2e63 6f6f 7264 735b 6469 6d5d  (obj.coords[dim]
-00016820: 2c20 6c6f 7765 723d 5472 7565 290a 0a20  , lower=True).. 
-00016830: 2020 2020 2020 2020 2020 2023 2043 6865             # Che
-00016840: 636b 206f 626a 2061 7869 7320 6974 7365  ck obj axis itse
-00016850: 6c66 0a20 2020 2020 2020 2020 2020 2069  lf.            i
-00016860: 6620 6e6f 7420 6861 7361 7474 7228 6f62  f not hasattr(ob
-00016870: 6a2c 2022 6461 7461 5f76 6172 7322 293a  j, "data_vars"):
-00016880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016890: 2061 7869 7320 3d20 7365 6c66 2e67 6574   axis = self.get
-000168a0: 5f61 7869 7328 6f62 6a2c 206c 6f77 6572  _axis(obj, lower
-000168b0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-000168c0: 2020 2020 2020 2069 6620 6178 6973 3a0a         if axis:.
-000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168e0: 2020 2020 7265 7475 726e 2061 7869 730a      return axis.
-000168f0: 0a20 2020 2064 6566 2067 6574 5f64 696d  .    def get_dim
-00016900: 5f74 7970 6573 2873 656c 662c 206f 626a  _types(self, obj
-00016910: 2c20 756e 6b6e 6f77 6e3d 4e6f 6e65 2c20  , unknown=None, 
-00016920: 6173 6469 6374 3d46 616c 7365 293a 0a20  asdict=False):. 
-00016930: 2020 2020 2020 2022 2222 4765 7420 6120         """Get a 
-00016940: 7475 706c 6520 6f66 2074 6865 2064 696d  tuple of the dim
-00016950: 656e 7369 6f6e 2074 7970 6573 206f 6620  ension types of 
-00016960: 616e 2061 7272 6179 0a0a 2020 2020 2020  an array..      
-00016970: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00016980: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-00016990: 2020 2020 2020 2020 6f62 6a3a 2078 6172          obj: xar
-000169a0: 7261 792e 4461 7461 4172 7261 792c 2074  ray.DataArray, t
-000169b0: 7570 6c65 2873 7472 292c 2078 6172 7261  uple(str), xarra
-000169c0: 792e 4461 7461 7365 740a 2020 2020 2020  y.Dataset.      
-000169d0: 2020 2020 2020 4461 7461 2061 7272 6179        Data array
-000169e0: 2c20 6461 7461 7365 7420 6f72 2074 7570  , dataset or tup
-000169f0: 6c65 206f 6620 6469 6d65 6e73 696f 6e73  le of dimensions
-00016a00: 0a20 2020 2020 2020 2075 6e6b 6e6f 776e  .        unknown
-00016a10: 3a0a 2020 2020 2020 2020 2020 2020 5661  :.            Va
-00016a20: 6c75 6520 746f 2061 7373 6967 6e20 7768  lue to assign wh
-00016a30: 656e 2074 7970 6520 6973 2075 6e6b 6e6f  en type is unkno
-00016a40: 776e 0a20 2020 2020 2020 2061 7364 6963  wn.        asdic
-00016a50: 743a 2062 6f6f 6c0a 0a20 2020 2020 2020  t: bool..       
-00016a60: 2052 6574 7572 6e0a 2020 2020 2020 2020   Return.        
-00016a70: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2074  ------.        t
-00016a80: 7570 6c65 2c20 6469 6374 0a20 2020 2020  uple, dict.     
-00016a90: 2020 2020 2020 2054 7570 6c65 206f 6620         Tuple of 
-00016aa0: 6469 6d65 6e73 696f 6e20 7479 7065 7320  dimension types 
-00016ab0: 616e 6420 6f66 206c 656e 6774 6820 6060  and of length ``
-00016ac0: 6f62 6a2e 6e64 696d 6060 2e0a 2020 2020  obj.ndim``..    
-00016ad0: 2020 2020 2020 2020 4120 6469 6d65 6e73          A dimens
-00016ae0: 696f 6e20 7479 7065 2069 7320 6569 7468  ion type is eith
-00016af0: 6572 2061 206c 6574 7465 7220 6f72 2074  er a letter or t
-00016b00: 6865 2060 6075 6e6b 6f77 6e60 6020 7661  he ``unkown`` va
-00016b10: 6c75 650a 2020 2020 2020 2020 2020 2020  lue.            
-00016b20: 7768 656e 2074 6865 2069 6e66 6572 656e  when the inferen
-00016b30: 6365 206f 6620 7479 7065 2068 6173 2066  ce of type has f
-00016b40: 6169 6c65 642e 0a20 2020 2020 2020 2020  ailed..         
-00016b50: 2020 2049 6620 6060 6173 6469 6374 6060     If ``asdict``
-00016b60: 2069 7320 5472 7565 2c20 6120 6469 6374   is True, a dict
-00016b70: 2069 7320 7265 7475 726e 6564 2069 6e73   is returned ins
-00016b80: 7465 6164 2c0a 2020 2020 2020 2020 2020  tead,.          
-00016b90: 2020 6060 2864 696d 2c20 6469 6d5f 7479    ``(dim, dim_ty
-00016ba0: 7065 2960 6020 6173 206b 6579 2d76 616c  pe)`` as key-val
-00016bb0: 7565 2070 6169 7273 2e0a 0a20 2020 2020  ue pairs...     
-00016bc0: 2020 2053 6565 2061 6c73 6f0a 2020 2020     See also.    
-00016bd0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-00016be0: 2020 2020 2067 6574 5f64 696d 5f74 7970       get_dim_typ
-00016bf0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
-00016c00: 2020 2020 2020 6469 6d5f 7479 7065 7320        dim_types 
-00016c10: 3d20 7b7d 0a20 2020 2020 2020 2069 6620  = {}.        if 
-00016c20: 6973 696e 7374 616e 6365 286f 626a 2c20  isinstance(obj, 
-00016c30: 7475 706c 6529 3a0a 2020 2020 2020 2020  tuple):.        
-00016c40: 2020 2020 6469 6d73 203d 206f 626a 0a20      dims = obj. 
-00016c50: 2020 2020 2020 2020 2020 206f 626a 203d             obj =
-00016c60: 204e 6f6e 650a 2020 2020 2020 2020 656c   None.        el
-00016c70: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00016c80: 6469 6d73 203d 206f 626a 2e64 696d 730a  dims = obj.dims.
-00016c90: 2020 2020 2020 2020 666f 7220 6469 6d20          for dim 
-00016ca0: 696e 2064 696d 733a 0a20 2020 2020 2020  in dims:.       
-00016cb0: 2020 2020 2064 696d 5f74 7970 6520 3d20       dim_type = 
-00016cc0: 7365 6c66 2e67 6574 5f64 696d 5f74 7970  self.get_dim_typ
-00016cd0: 6528 6469 6d2c 206f 626a 3d6f 626a 290a  e(dim, obj=obj).
-00016ce0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00016cf0: 696d 5f74 7970 6520 6973 204e 6f6e 653a  im_type is None:
-00016d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016d10: 2064 696d 5f74 7970 6520 3d20 756e 6b6e   dim_type = unkn
-00016d20: 6f77 6e0a 2020 2020 2020 2020 2020 2020  own.            
-00016d30: 6469 6d5f 7479 7065 735b 6469 6d5d 203d  dim_types[dim] =
-00016d40: 2064 696d 5f74 7970 650a 2020 2020 2020   dim_type.      
-00016d50: 2020 6966 2061 7364 6963 743a 0a20 2020    if asdict:.   
-00016d60: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00016d70: 6469 6d5f 7479 7065 730a 2020 2020 2020  dim_types.      
-00016d80: 2020 7265 7475 726e 2074 7570 6c65 2864    return tuple(d
-00016d90: 696d 5f74 7970 6573 2e76 616c 7565 7328  im_types.values(
-00016da0: 2929 0a0a 2020 2020 4045 5252 4f52 532e  ))..    @ERRORS.
-00016db0: 666f 726d 6174 5f6d 6574 686f 645f 646f  format_method_do
-00016dc0: 6373 7472 696e 670a 2020 2020 6465 6620  cstring.    def 
-00016dd0: 7365 6172 6368 5f64 696d 2873 656c 662c  search_dim(self,
-00016de0: 206f 626a 2c20 6366 5f61 7267 3d4e 6f6e   obj, cf_arg=Non
-00016df0: 652c 206c 6f63 3d4e 6f6e 652c 2073 696e  e, loc=None, sin
-00016e00: 676c 653d 5472 7565 2c20 6572 726f 7273  gle=True, errors
-00016e10: 3d22 6967 6e6f 7265 2229 3a0a 2020 2020  ="ignore"):.    
-00016e20: 2020 2020 2222 2253 6561 7263 6820 6120      """Search a 
-00016e30: 6461 7461 6172 7261 792f 6461 7461 7365  dataarray/datase
-00016e40: 7420 666f 7220 6120 6469 6d65 6e73 696f  t for a dimensio
-00016e50: 6e20 6e61 6d65 2061 6363 6f72 6469 6e67  n name according
-00016e60: 2074 6f20 6974 7320 6765 6e65 7269 6320   to its generic 
-00016e70: 6e61 6d65 206f 7220 7479 7065 0a0a 2020  name or type..  
-00016e80: 2020 2020 2020 4669 7273 742c 2073 6361        First, sca
-00016e90: 6e20 7468 6520 6469 6d65 6e73 696f 6e20  n the dimension 
-00016ea0: 6e61 6d65 732e 0a20 2020 2020 2020 2054  names..        T
-00016eb0: 6865 6e2c 206c 6f6f 6b20 666f 7220 636f  hen, look for co
-00016ec0: 6f72 6469 6e61 7465 733a 2065 6974 6865  ordinates: eithe
-00016ed0: 7220 6974 2068 6173 2061 6e20 2761 7869  r it has an 'axi
-00016ee0: 7327 2061 7474 7269 6275 7465 2c0a 2020  s' attribute,.  
-00016ef0: 2020 2020 2020 6f72 2069 7420 6120 6b6e        or it a kn
-00016f00: 6f77 6e20 4346 2063 6f6f 7264 696e 6174  own CF coordinat
-00016f10: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
-00016f20: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00016f30: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00016f40: 2020 6f62 6a3a 2078 6172 7261 792e 4461    obj: xarray.Da
-00016f50: 7461 4172 7261 792c 2078 6172 7261 792e  taArray, xarray.
-00016f60: 4461 7461 7365 740a 2020 2020 2020 2020  Dataset.        
-00016f70: 2020 2020 436f 6f72 6469 6e61 7465 206f      Coordinate o
-00016f80: 7220 6461 7461 2061 7272 6179 0a20 2020  r data array.   
-00016f90: 2020 2020 2063 665f 6172 673a 2073 7472       cf_arg: str
-00016fa0: 2c20 7b7b 2278 222c 2022 7922 2c20 227a  , {{"x", "y", "z
-00016fb0: 222c 2022 7422 2c20 2266 227d 7d2c 204e  ", "t", "f"}}, N
-00016fc0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00016fd0: 4f6e 652d 6c65 7474 6572 2064 696d 656e  One-letter dimen
-00016fe0: 7369 6f6e 2074 7970 6520 6f72 2067 656e  sion type or gen
-00016ff0: 6572 6963 2043 4620 6469 6d20 6e61 6d65  eric CF dim name
-00017000: 2e0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-00017010: 656e 2073 6574 2074 6f20 4e6f 6e65 2c20  en set to None, 
-00017020: 646d 656e 7369 6f6e 2074 7970 6520 6973  dmension type is
-00017030: 2069 6e66 6572 7265 6420 7769 7468 203a   inferred with :
-00017040: 6d65 7468 3a60 6765 745f 6178 6973 600a  meth:`get_axis`.
-00017050: 2020 2020 2020 2020 2020 2020 6170 706c              appl
-00017060: 6965 6420 746f 2060 6f62 6a60 0a20 2020  ied to `obj`.   
-00017070: 2020 2020 206c 6f63 3a20 2261 6e79 222c       loc: "any",
-00017080: 206c 6574 7465 720a 2020 2020 2020 2020   letter.        
-00017090: 2020 2020 5374 6167 6765 7265 6420 6772      Staggered gr
-000170a0: 6964 206c 6f63 6174 696f 6e0a 2020 2020  id location.    
-000170b0: 2020 2020 7369 6e67 6c65 3a20 626f 6f6c      single: bool
-000170c0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-000170d0: 5472 7565 2c20 7265 7475 726e 2074 6865  True, return the
-000170e0: 2066 6972 7374 2069 7465 6d20 666f 756e   first item foun
-000170f0: 6420 6f72 204e 6f6e 652e 0a20 2020 2020  d or None..     
-00017100: 2020 2020 2020 2049 6620 4661 6c73 652c         If False,
-00017110: 2072 6574 7572 6e20 6120 706f 7373 6962   return a possib
-00017120: 6c65 2065 6d70 7479 206c 6973 7420 6f66  le empty list of
-00017130: 2066 6f75 6e64 2069 7465 6d73 2e0a 2020   found items..  
-00017140: 2020 2020 2020 7b65 7272 6f72 737d 0a0a        {errors}..
-00017150: 2020 2020 2020 2020 5265 7475 726e 0a20          Return. 
-00017160: 2020 2020 2020 202d 2d2d 2d2d 2d0a 2020         ------.  
-00017170: 2020 2020 2020 7374 722c 2064 6963 742c        str, dict,
-00017180: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00017190: 2020 4469 6d20 6e61 6d65 204f 522c 2064    Dim name OR, d
-000171a0: 6963 7420 7769 7468 2064 696d 2c20 7479  ict with dim, ty
-000171b0: 7065 2061 6e64 2063 665f 6e61 6d65 206b  pe and cf_name k
-000171c0: 6579 7320 6966 2064 696d 5f74 7970 6520  eys if dim_type 
-000171d0: 6973 204e 6f6e 652e 0a20 2020 2020 2020  is None..       
-000171e0: 2020 2020 204e 6f6e 6520 6966 206e 6f74       None if not
-000171f0: 6869 6e67 2066 6f75 6e64 2e0a 2020 2020  hing found..    
-00017200: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00017210: 2320 4578 706c 6963 6974 3f0a 2020 2020  # Explicit?.    
-00017220: 2020 2020 6366 5f6e 616d 6520 3d20 6469      cf_name = di
-00017230: 6d5f 7479 7065 203d 204e 6f6e 650a 2020  m_type = None.  
-00017240: 2020 2020 2020 6966 2063 665f 6172 673a        if cf_arg:
-00017250: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-00017260: 6620 6366 5f61 7267 2069 6e20 6f62 6a2e  f cf_arg in obj.
-00017270: 6469 6d73 3a0a 2020 2020 2020 2020 2020  dims:.          
-00017280: 2020 2320 2020 2020 7265 7475 726e 2063    #     return c
-00017290: 665f 6172 670a 2020 2020 2020 2020 2020  f_arg.          
-000172a0: 2020 6966 206c 656e 2863 665f 6172 6729    if len(cf_arg)
-000172b0: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-000172c0: 2020 2020 2020 2064 696d 5f74 7970 6520         dim_type 
-000172d0: 3d20 6366 5f61 7267 2e6c 6f77 6572 2829  = cf_arg.lower()
-000172e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000172f0: 2069 6620 6366 5f61 7267 2069 6e20 7365   if cf_arg in se
-00017300: 6c66 2e6e 616d 6573 3a0a 2020 2020 2020  lf.names:.      
-00017310: 2020 2020 2020 2020 2020 2020 2020 6366                cf
-00017320: 5f6e 616d 6520 3d20 6366 5f61 7267 0a20  _name = cf_arg. 
-00017330: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00017340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017350: 2069 6620 6e6f 7420 7365 6c66 2e5f 6173   if not self._as
-00017360: 7365 7274 5f6b 6e6f 776e 5f28 6366 5f61  sert_known_(cf_a
-00017370: 7267 2c20 6572 726f 7273 3d65 7272 6f72  rg, errors=error
-00017380: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00017390: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-000173a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000173b0: 665f 6e61 6d65 203d 2063 665f 6172 670a  f_name = cf_arg.
-000173c0: 2020 2020 2020 2020 6973 6473 203d 2068          isds = h
-000173d0: 6173 6174 7472 286f 626a 2c20 2264 6174  asattr(obj, "dat
-000173e0: 615f 7661 7273 2229 0a20 2020 2020 2020  a_vars").       
-000173f0: 2069 6620 6e6f 7420 6973 6473 2061 6e64   if not isds and
-00017400: 2064 696d 5f74 7970 6520 6973 204e 6f6e   dim_type is Non
-00017410: 653a 0a20 2020 2020 2020 2020 2020 2064  e:.            d
-00017420: 696d 5f74 7970 6520 3d20 7365 6c66 2e67  im_type = self.g
-00017430: 6574 5f61 7869 7328 6f62 6a2c 206c 6f77  et_axis(obj, low
-00017440: 6572 3d54 7275 6529 0a20 2020 2020 2020  er=True).       
-00017450: 206c 6f63 203d 2073 656c 662e 7367 6c6f   loc = self.sglo
-00017460: 6361 746f 722e 7061 7273 655f 6c6f 635f  cator.parse_loc_
-00017470: 6172 6728 6c6f 6329 0a0a 2020 2020 2020  arg(loc)..      
-00017480: 2020 2320 4c6f 6f70 206f 6e20 6469 6d73    # Loop on dims
-00017490: 0a20 2020 2020 2020 2066 6f75 6e64 203d  .        found =
-000174a0: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-000174b0: 6469 6d20 696e 206f 626a 2e64 696d 733a  dim in obj.dims:
-000174c0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000174d0: 4669 6c74 6572 2d6f 7574 2062 7920 6c6f  Filter-out by lo
-000174e0: 630a 2020 2020 2020 2020 2020 2020 706e  c.            pn
-000174f0: 616d 652c 2070 6c6f 6320 3d20 7365 6c66  ame, ploc = self
-00017500: 2e73 676c 6f63 6174 6f72 2e70 6172 7365  .sglocator.parse
-00017510: 5f61 7474 7228 276e 616d 6527 2c20 6469  _attr('name', di
-00017520: 6d29 0a20 2020 2020 2020 2020 2020 2070  m).            p
-00017530: 6c6f 6320 3d20 7365 6c66 2e73 676c 6f63  loc = self.sgloc
-00017540: 6174 6f72 2e70 6172 7365 5f6c 6f63 5f61  ator.parse_loc_a
-00017550: 7267 2870 6c6f 6329 0a20 2020 2020 2020  rg(ploc).       
-00017560: 2020 2020 2069 6620 6c6f 6320 6973 206e       if loc is n
-00017570: 6f74 204e 6f6e 6520 616e 6420 6c6f 6320  ot None and loc 
-00017580: 213d 2070 6c6f 633a 0a20 2020 2020 2020  != ploc:.       
-00017590: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-000175a0: 650a 0a20 2020 2020 2020 2020 2020 2023  e..            #
-000175b0: 2046 726f 6d20 6765 6e65 7269 6320 6e61   From generic na
-000175c0: 6d65 0a20 2020 2020 2020 2020 2020 2069  me.            i
-000175d0: 6620 6469 6d20 696e 206f 626a 2e63 6f6f  f dim in obj.coo
-000175e0: 7264 733a 0a20 2020 2020 2020 2020 2020  rds:.           
-000175f0: 2020 2020 2074 6869 735f 6366 5f6e 616d       this_cf_nam
-00017600: 6520 3d20 7365 6c66 2e6d 6174 6368 286f  e = self.match(o
-00017610: 626a 2e63 6f6f 7264 735b 6469 6d5d 290a  bj.coords[dim]).
-00017620: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00017630: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017640: 2020 7468 6973 5f63 665f 6e61 6d65 203d    this_cf_name =
-00017650: 2073 656c 662e 6d61 7463 685f 6672 6f6d   self.match_from
-00017660: 5f6e 616d 6528 6469 6d29 0a20 2020 2020  _name(dim).     
-00017670: 2020 2020 2020 2069 6620 6366 5f6e 616d         if cf_nam
-00017680: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00017690: 2020 2069 6620 7468 6973 5f63 665f 6e61     if this_cf_na
-000176a0: 6d65 203d 3d20 6366 5f6e 616d 653a 0a20  me == cf_name:. 
-000176b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176c0: 2020 2066 6f75 6e64 2e61 7070 656e 6428     found.append(
-000176d0: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
-000176e0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-000176f0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00017700: 2020 6966 2064 696d 5f74 7970 6520 6973    if dim_type is
-00017710: 204e 6f6e 653a 2020 2320 6b65 6570 2073   None:  # keep s
-00017720: 6561 7263 6869 6e67 2069 6620 6469 6d5f  earching if dim_
-00017730: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
-00017740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017750: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-00017760: 2020 2020 2020 2020 2020 2023 2046 726f             # Fro
-00017770: 6d20 6469 6d65 6e73 696f 6e20 7479 7065  m dimension type
-00017780: 0a20 2020 2020 2020 2020 2020 2074 6869  .            thi
-00017790: 735f 6469 6d5f 7479 7065 203d 2073 656c  s_dim_type = sel
-000177a0: 662e 6765 745f 6469 6d5f 7479 7065 2864  f.get_dim_type(d
-000177b0: 696d 2c20 6f62 6a3d 6f62 6a29 0a20 2020  im, obj=obj).   
-000177c0: 2020 2020 2020 2020 206f 7574 203d 207b           out = {
-000177d0: 2264 696d 223a 2064 696d 2c20 2274 7970  "dim": dim, "typ
-000177e0: 6522 3a20 7468 6973 5f64 696d 5f74 7970  e": this_dim_typ
-000177f0: 652c 2022 6366 5f6e 616d 6522 3a20 7468  e, "cf_name": th
-00017800: 6973 5f63 665f 6e61 6d65 7d0a 2020 2020  is_cf_name}.    
-00017810: 2020 2020 2020 2020 6966 2074 6869 735f          if this_
-00017820: 6469 6d5f 7479 7065 2061 6e64 2074 6869  dim_type and thi
-00017830: 735f 6469 6d5f 7479 7065 203d 3d20 6469  s_dim_type == di
-00017840: 6d5f 7479 7065 3a0a 2020 2020 2020 2020  m_type:.        
-00017850: 2020 2020 2020 2020 6966 2063 665f 6172          if cf_ar
-00017860: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-00017870: 2020 2020 2020 2066 6f75 6e64 2e61 7070         found.app
-00017880: 656e 6428 6469 6d29 0a20 2020 2020 2020  end(dim).       
-00017890: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000178a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178b0: 2020 2066 6f75 6e64 2e61 7070 656e 6428     found.append(
-000178c0: 6f75 7429 0a0a 2020 2020 2020 2020 2320  out)..        # 
-000178d0: 4e6f 7420 666f 756e 6420 6275 7420 6f6e  Not found but on
-000178e0: 6c79 2031 6420 616e 6420 6e6f 2064 696d  ly 1d and no dim
-000178f0: 5f74 7970 6520 7370 6563 6966 6965 640a  _type specified.
-00017900: 2020 2020 2020 2020 6966 206e 6f74 2066          if not f
-00017910: 6f75 6e64 2061 6e64 206c 656e 286f 626a  ound and len(obj
-00017920: 2e64 696d 7329 203d 3d20 3120 616e 6420  .dims) == 1 and 
-00017930: 6e6f 7420 6366 5f61 7267 3a0a 2020 2020  not cf_arg:.    
-00017940: 2020 2020 2020 2020 2320 4649 584d 453a          # FIXME:
-00017950: 206c 6f6f 7020 6f6e 2063 6f6f 7264 696e   loop on coordin
-00017960: 6174 6573 3f0a 2020 2020 2020 2020 2020  ates?.          
-00017970: 2020 666f 756e 642e 6170 7065 6e64 286f    found.append(o
-00017980: 7574 290a 0a20 2020 2020 2020 2023 2053  ut)..        # S
-00017990: 696e 676c 653f 0a20 2020 2020 2020 2065  ingle?.        e
-000179a0: 7272 6f72 7320 3d20 4552 524f 5253 5b65  rrors = ERRORS[e
-000179b0: 7272 6f72 735d 0a20 2020 2020 2020 2069  rrors].        i
-000179c0: 6620 7369 6e67 6c65 3a0a 2020 2020 2020  f single:.      
-000179d0: 2020 2020 2020 6966 206c 656e 2866 6f75        if len(fou
-000179e0: 6e64 2920 3d3d 2031 3a0a 2020 2020 2020  nd) == 1:.      
-000179f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00017a00: 2066 6f75 6e64 5b30 5d0a 2020 2020 2020   found[0].      
-00017a10: 2020 2020 2020 6966 206c 656e 2866 6f75        if len(fou
-00017a20: 6e64 2920 3e20 313a 0a20 2020 2020 2020  nd) > 1:.       
-00017a30: 2020 2020 2020 2020 2069 6620 6572 726f           if erro
-00017a40: 7273 2021 3d20 2269 676e 6f72 6522 3a0a  rs != "ignore":.
-00017a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a60: 2020 2020 6d73 6720 3d20 6622 4d75 6c74      msg = f"Mult
-00017a70: 6970 6c65 2063 616e 6469 6461 7465 7320  iple candidates 
-00017a80: 6469 6d65 6e73 696f 6e73 206d 6174 6368  dimensions match
-00017a90: 696e 673a 207b 6366 5f61 7267 7d22 0a20  ing: {cf_arg}". 
-00017aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ab0: 2020 2069 6620 6572 726f 7273 203d 3d20     if errors == 
-00017ac0: 2272 6169 7365 223a 0a20 2020 2020 2020  "raise":.       
-00017ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ae0: 2072 6169 7365 2058 6f61 4346 4572 726f   raise XoaCFErro
-00017af0: 7228 6d73 6729 0a20 2020 2020 2020 2020  r(msg).         
-00017b00: 2020 2020 2020 2020 2020 2078 6f61 5f77             xoa_w
-00017b10: 6172 6e28 6d73 6729 0a20 2020 2020 2020  arn(msg).       
-00017b20: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00017b30: 2020 2072 6574 7572 6e20 666f 756e 640a     return found.
-00017b40: 0a20 2020 2020 2020 2023 2046 6169 6c65  .        # Faile
-00017b50: 640a 2020 2020 2020 2020 6966 2065 7272  d.        if err
-00017b60: 6f72 7320 213d 2022 6967 6e6f 7265 223a  ors != "ignore":
-00017b70: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-00017b80: 203d 2066 224e 6f20 6469 6d65 6e73 696f   = f"No dimensio
-00017b90: 6e20 666f 756e 6420 696e 2064 6174 6161  n found in dataa
-00017ba0: 7272 6179 206d 6174 6368 696e 673a 207b  rray matching: {
-00017bb0: 6366 5f61 7267 7d22 0a20 2020 2020 2020  cf_arg}".       
-00017bc0: 2020 2020 2069 6620 6572 726f 7273 203d       if errors =
-00017bd0: 3d20 2272 6169 7365 223a 0a20 2020 2020  = "raise":.     
-00017be0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00017bf0: 2058 6f61 4346 4572 726f 7228 6d73 6729   XoaCFError(msg)
-00017c00: 0a20 2020 2020 2020 2020 2020 2078 6f61  .            xoa
-00017c10: 5f77 6172 6e28 6d73 6729 0a0a 2020 2020  _warn(msg)..    
-00017c20: 4045 5252 4f52 532e 666f 726d 6174 5f6d  @ERRORS.format_m
-00017c30: 6574 686f 645f 646f 6373 7472 696e 670a  ethod_docstring.
-00017c40: 2020 2020 6465 6620 7365 6172 6368 5f66      def search_f
-00017c50: 726f 6d5f 6469 6d28 7365 6c66 2c20 6f62  rom_dim(self, ob
-00017c60: 6a2c 2064 696d 2c20 6572 726f 7273 3d22  j, dim, errors="
-00017c70: 6967 6e6f 7265 2229 3a0a 2020 2020 2020  ignore"):.      
-00017c80: 2020 2222 2253 6561 7263 6820 6120 6461    """Search a da
-00017c90: 7461 6172 7261 792f 6461 7461 7365 7420  taarray/dataset 
-00017ca0: 666f 7220 6120 636f 6f72 6469 6e61 7465  for a coordinate
-00017cb0: 2066 726f 6d20 6120 6469 6d65 6e73 696f   from a dimensio
-00017cc0: 6e20 6e61 6d65 0a0a 2020 2020 2020 2020  n name..        
-00017cd0: 4974 2066 6972 7374 2073 6561 7263 6865  It first searche
-00017ce0: 7320 666f 7220 6120 636f 6f72 6469 6e61  s for a coordina
-00017cf0: 7465 2077 6974 6820 6120 6469 6666 6572  te with a differ
-00017d00: 656e 7420 6e61 6d65 2061 6e64 2074 6861  ent name and tha
-00017d10: 7420 6973 0a20 2020 2020 2020 2074 6865  t is.        the
-00017d20: 206f 6e6c 7920 6f6e 6520 6861 7669 6e67   only one having
-00017d30: 2074 6869 7320 6469 6d65 6e73 696f 6e2e   this dimension.
-00017d40: 0a20 2020 2020 2020 2054 6865 6e20 6368  .        Then ch
-00017d50: 6563 6b20 6966 2069 7420 6973 2061 6e20  eck if it is an 
-00017d60: 696e 6465 782e 0a20 2020 2020 2020 2054  index..        T
-00017d70: 6865 6e20 6c6f 6f6b 2066 6f72 2063 6f6f  hen look for coo
-00017d80: 7264 696e 6174 6573 2077 6974 6820 7468  rdinates with th
-00017d90: 6520 7361 6d65 2074 7970 6520 6c69 6b65  e same type like
-00017da0: 2078 2c20 792c 2065 7463 2e0a 0a20 2020   x, y, etc...   
-00017db0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00017dc0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00017dd0: 2d2d 0a20 2020 2020 2020 206f 626a 3a20  --.        obj: 
-00017de0: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-00017df0: 2c20 7861 7272 6179 2e44 6174 6173 6574  , xarray.Dataset
-00017e00: 0a20 2020 2020 2020 2064 696d 3a20 7374  .        dim: st
-00017e10: 720a 2020 2020 2020 2020 7b65 7272 6f72  r.        {error
-00017e20: 737d 0a0a 2020 2020 2020 2020 5265 7475  s}..        Retu
-00017e30: 726e 0a20 2020 2020 2020 202d 2d2d 2d2d  rn.        -----
-00017e40: 2d0a 2020 2020 2020 2020 7861 7272 6179  -.        xarray
-00017e50: 2e44 6174 6141 7272 6179 2c20 4e6f 6e65  .DataArray, None
-00017e60: 0a20 2020 2020 2020 2020 2020 2041 6e20  .            An 
-00017e70: 636f 6f72 6469 6e61 7465 2061 7272 6179  coordinate array
-00017e80: 206f 7220 4e6f 6e65 0a0a 2020 2020 2020   or None..      
-00017e90: 2020 5365 6520 616c 736f 0a20 2020 2020    See also.     
-00017ea0: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
-00017eb0: 2020 2020 6765 745f 6178 6973 0a20 2020      get_axis.   
-00017ec0: 2020 2020 2067 6574 5f64 696d 5f74 7970       get_dim_typ
-00017ed0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
-00017ee0: 2020 2020 2020 6966 2064 696d 206e 6f74        if dim not
-00017ef0: 2069 6e20 6f62 6a2e 6469 6d73 3a0a 2020   in obj.dims:.  
-00017f00: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00017f10: 586f 6145 7272 6f72 2866 2249 6e76 616c  XoaError(f"Inval
-00017f20: 6964 2064 696d 656e 7369 6f6e 3a20 7b64  id dimension: {d
-00017f30: 696d 7d22 290a 0a20 2020 2020 2020 2023  im}")..        #
-00017f40: 2041 2063 6f6f 7264 2077 6974 6820 6120   A coord with a 
-00017f50: 6469 6666 6572 656e 7420 6e61 6d65 0a20  different name. 
-00017f60: 2020 2020 2020 2063 6f6f 7264 7320 3d20         coords = 
-00017f70: 5b63 6f6f 7264 2066 6f72 206e 616d 652c  [coord for name,
-00017f80: 2063 6f6f 7264 2069 6e20 6f62 6a2e 636f   coord in obj.co
-00017f90: 6f72 6473 2e69 7465 6d73 2829 2069 6620  ords.items() if 
-00017fa0: 6e61 6d65 2021 3d20 6469 6d20 616e 6420  name != dim and 
-00017fb0: 6469 6d20 696e 2063 6f6f 7264 2e64 696d  dim in coord.dim
-00017fc0: 735d 0a20 2020 2020 2020 2069 6620 6c65  s].        if le
-00017fd0: 6e28 636f 6f72 6473 2920 3d3d 2031 3a0a  n(coords) == 1:.
-00017fe0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00017ff0: 726e 2063 6f6f 7264 735b 305d 0a0a 2020  rn coords[0]..  
-00018000: 2020 2020 2020 2320 4173 2061 6e20 696e        # As an in
-00018010: 6465 780a 2020 2020 2020 2020 6966 2064  dex.        if d
-00018020: 696d 2069 6e20 6f62 6a2e 696e 6465 7865  im in obj.indexe
-00018030: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-00018040: 6574 7572 6e20 6f62 6a2e 636f 6f72 6473  eturn obj.coords
-00018050: 5b64 696d 5d0a 0a20 2020 2020 2020 2023  [dim]..        #
-00018060: 2047 6574 2064 696d 5f74 7970 6520 6672   Get dim_type fr
-00018070: 6f6d 206b 6e6f 776e 2064 696d 206e 616d  om known dim nam
-00018080: 650a 2020 2020 2020 2020 6469 6d5f 7479  e.        dim_ty
-00018090: 7065 203d 2073 656c 662e 6765 745f 6469  pe = self.get_di
-000180a0: 6d5f 7479 7065 2864 696d 2c20 6f62 6a2c  m_type(dim, obj,
-000180b0: 206c 6f77 6572 3d54 7275 6529 0a0a 2020   lower=True)..  
-000180c0: 2020 2020 2020 2320 536f 2077 6520 6361        # So we ca
-000180d0: 6e20 646f 2073 6f6d 6574 6869 6e67 0a20  n do something. 
-000180e0: 2020 2020 2020 2064 6566 2067 6574 5f6e         def get_n
-000180f0: 6469 6d28 6f29 3a0a 2020 2020 2020 2020  dim(o):.        
-00018100: 2020 2020 7265 7475 726e 206c 656e 286f      return len(o
-00018110: 2e64 696d 7329 0a0a 2020 2020 2020 2020  .dims)..        
-00018120: 6966 2064 696d 5f74 7970 6520 6973 206e  if dim_type is n
-00018130: 6f74 204e 6f6e 653a 0a0a 2020 2020 2020  ot None:..      
-00018140: 2020 2020 2020 2320 4c6f 6f6b 2066 6f72        # Look for
-00018150: 2061 2063 6f6f 7264 696e 6174 6520 7769   a coordinate wi
-00018160: 7468 2074 6869 7320 6469 6d5f 7479 7065  th this dim_type
-00018170: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-00018180: 7374 6172 7469 6e67 2066 726f 6d20 636f  starting from co
-00018190: 6f72 6469 6e61 7465 7320 7769 7468 2061  ordinates with a
-000181a0: 2068 6967 6865 7220 6e75 6d62 6572 206f   higher number o
-000181b0: 6620 6469 6d65 6e73 696f 6e73 0a20 2020  f dimensions.   
-000181c0: 2020 2020 2020 2020 2023 2020 6c69 6b65           #  like
-000181d0: 2064 6570 7468 2074 6861 7420 6861 7665   depth that have
-000181e0: 206d 6f72 6520 6469 6d73 2074 6861 6e20   more dims than 
-000181f0: 6c65 7665 6c0a 2020 2020 2020 2020 2020  level.          
-00018200: 2020 666f 7220 636f 6f72 6420 696e 2073    for coord in s
-00018210: 6f72 7465 6428 6f62 6a2e 636f 6f72 6473  orted(obj.coords
-00018220: 2e76 616c 7565 7328 292c 206b 6579 3d67  .values(), key=g
-00018230: 6574 5f6e 6469 6d2c 2072 6576 6572 7365  et_ndim, reverse
-00018240: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
-00018250: 2020 2020 2020 2020 6966 2064 696d 2069          if dim i
-00018260: 6e20 636f 6f72 642e 6469 6d73 3a0a 2020  n coord.dims:.  
-00018270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018280: 2020 636f 6f72 645f 6469 6d5f 7479 7065    coord_dim_type
-00018290: 203d 2073 656c 662e 6765 745f 6178 6973   = self.get_axis
-000182a0: 2863 6f6f 7264 2c20 6c6f 7765 723d 5472  (coord, lower=Tr
-000182b0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-000182c0: 2020 2020 2020 2020 6966 2063 6f6f 7264          if coord
-000182d0: 5f64 696d 5f74 7970 6520 616e 6420 636f  _dim_type and co
-000182e0: 6f72 645f 6469 6d5f 7479 7065 203d 3d20  ord_dim_type == 
-000182f0: 6469 6d5f 7479 7065 3a0a 2020 2020 2020  dim_type:.      
+00013600: 2020 2320 6966 206f 626a 2e6e 616d 6520    # if obj.name 
+00013610: 696e 2066 6f75 6e64 5f6f 626a 733a 0a20  in found_objs:. 
+00013620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013630: 2020 2069 6620 7468 6973 5f6e 616d 6520     if this_name 
+00013640: 696e 2066 6f75 6e64 5f6f 626a 733a 0a20  in found_objs:. 
+00013650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013660: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00013670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013680: 2020 2020 666f 756e 645f 6f62 6a73 2e61      found_objs.a
+00013690: 7070 656e 6428 7468 6973 5f6e 616d 6529  ppend(this_name)
+000136a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000136b0: 2020 2020 2063 665f 6e61 6d65 203d 2063       cf_name = c
+000136c0: 665f 6e61 6d65 2069 6620 6366 5f6e 616d  f_name if cf_nam
+000136d0: 6520 656c 7365 206d 0a20 2020 2020 2020  e else m.       
+000136e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000136f0: 6765 7420 3d3d 2022 626f 7468 223a 0a20  get == "both":. 
+00013700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013710: 2020 2020 2020 2066 6f75 6e64 2e61 7070         found.app
+00013720: 656e 6428 2874 6869 735f 6f62 6a2c 2063  end((this_obj, c
+00013730: 665f 6e61 6d65 2929 0a20 2020 2020 2020  f_name)).       
+00013740: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00013750: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00013760: 2020 2020 2020 2020 2020 2066 6f75 6e64             found
+00013770: 2e61 7070 656e 6428 7468 6973 5f6f 626a  .append(this_obj
+00013780: 2069 6620 6765 7420 3d3d 2022 6f62 6a22   if get == "obj"
+00013790: 2065 6c73 6520 6366 5f6e 616d 6529 0a0a   else cf_name)..
+000137a0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+000137b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000137c0: 7369 6e67 6c65 3a0a 2020 2020 2020 2020  single:.        
+000137d0: 2020 2020 7265 7475 726e 2066 6f75 6e64      return found
+000137e0: 0a20 2020 2020 2020 2065 7272 6f72 7320  .        errors 
+000137f0: 3d20 4552 524f 5253 5b65 7272 6f72 735d  = ERRORS[errors]
+00013800: 0a20 2020 2020 2020 2069 6620 6572 726f  .        if erro
+00013810: 7273 2021 3d20 2269 676e 6f72 6522 2061  rs != "ignore" a
+00013820: 6e64 206c 656e 2866 6f75 6e64 2920 3e20  nd len(found) > 
+00013830: 313a 0a20 2020 2020 2020 2020 2020 206d  1:.            m
+00013840: 7367 203d 2022 4d75 6c74 6970 6c65 2069  sg = "Multiple i
+00013850: 7465 6d73 2066 6f75 6e64 2077 6869 6c65  tems found while
+00013860: 2079 6f75 2072 6571 7565 7374 6564 2061   you requested a
+00013870: 2073 696e 676c 6520 6f6e 6522 0a20 2020   single one".   
+00013880: 2020 2020 2020 2020 2069 6620 6572 726f           if erro
+00013890: 7273 203d 3d20 2272 6169 7365 223a 0a20  rs == "raise":. 
+000138a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000138b0: 6169 7365 2058 6f61 4346 4572 726f 7228  aise XoaCFError(
+000138c0: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
+000138d0: 2078 6f61 5f77 6172 6e28 6d73 6729 0a20   xoa_warn(msg). 
+000138e0: 2020 2020 2020 2069 6620 666f 756e 643a         if found:
+000138f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00013900: 7572 6e20 666f 756e 645b 305d 0a20 2020  urn found[0].   
+00013910: 2020 2020 2069 6620 6572 726f 7273 2021       if errors !
+00013920: 3d20 2269 676e 6f72 6522 3a0a 2020 2020  = "ignore":.    
+00013930: 2020 2020 2020 2020 6d73 6720 3d20 224e          msg = "N
+00013940: 6f20 6d61 7463 6869 6e67 2069 7465 6d20  o matching item 
+00013950: 666f 756e 6422 0a20 2020 2020 2020 2020  found".         
+00013960: 2020 2069 6620 6572 726f 7273 203d 3d20     if errors == 
+00013970: 2272 6169 7365 223a 0a20 2020 2020 2020  "raise":.       
+00013980: 2020 2020 2020 2020 2072 6169 7365 2058           raise X
+00013990: 6f61 4346 4572 726f 7228 6d73 6729 0a20  oaCFError(msg). 
+000139a0: 2020 2020 2020 2020 2020 2078 6f61 5f77             xoa_w
+000139b0: 6172 6e28 6d73 6729 0a0a 2020 2020 6465  arn(msg)..    de
+000139c0: 6620 6765 7428 7365 6c66 2c20 6f62 6a2c  f get(self, obj,
+000139d0: 2063 665f 6e61 6d65 293a 0a20 2020 2020   cf_name):.     
+000139e0: 2020 2022 2222 4361 6c6c 2074 6f20 3a6d     """Call to :m
+000139f0: 6574 683a 6073 6561 7263 6860 2077 6974  eth:`search` wit
+00013a00: 6820 616e 2065 7870 6c69 6369 7420 6e61  h an explicit na
+00013a10: 6d65 2061 6e64 2069 676e 6f72 696e 6720  me and ignoring 
+00013a20: 6572 726f 7273 2222 220a 2020 2020 2020  errors""".      
+00013a30: 2020 7265 7475 726e 2073 656c 662e 7365    return self.se
+00013a40: 6172 6368 286f 626a 2c20 6366 5f6e 616d  arch(obj, cf_nam
+00013a50: 652c 2065 7272 6f72 733d 2269 676e 6f72  e, errors="ignor
+00013a60: 6522 290a 0a20 2020 2040 4552 524f 5253  e")..    @ERRORS
+00013a70: 2e66 6f72 6d61 745f 6d65 7468 6f64 5f64  .format_method_d
+00013a80: 6f63 7374 7269 6e67 0a20 2020 2064 6566  ocstring.    def
+00013a90: 2067 6574 5f61 7474 7273 280a 2020 2020   get_attrs(.    
+00013aa0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00013ab0: 2020 6366 5f6e 616d 652c 0a20 2020 2020    cf_name,.     
+00013ac0: 2020 2073 656c 6563 743d 4e6f 6e65 2c0a     select=None,.
+00013ad0: 2020 2020 2020 2020 6578 636c 7564 653d          exclude=
+00013ae0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6572  None,.        er
+00013af0: 726f 7273 3d22 7761 726e 222c 0a20 2020  rors="warn",.   
+00013b00: 2020 2020 206c 6f63 3d4e 6f6e 652c 0a20       loc=None,. 
+00013b10: 2020 2020 2020 206d 756c 7469 3d46 616c         multi=Fal
+00013b20: 7365 2c0a 2020 2020 2020 2020 7374 616e  se,.        stan
+00013b30: 6461 7264 697a 653d 5472 7565 2c0a 2020  dardize=True,.  
+00013b40: 2020 2020 2020 2a2a 6578 7472 612c 0a20        **extra,. 
+00013b50: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00013b60: 2247 6574 2074 6865 2064 6566 6175 6c74  "Get the default
+00013b70: 2061 7474 7269 6275 7465 7320 6672 6f6d   attributes from
+00013b80: 2063 6620 7370 6563 730a 0a20 2020 2020   cf specs..     
+00013b90: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00013ba0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00013bb0: 0a20 2020 2020 2020 2063 665f 6e61 6d65  .        cf_name
+00013bc0: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+00013bd0: 2020 5661 6c69 6420 6765 6e65 7269 6320    Valid generic 
+00013be0: 4346 206e 616d 650a 2020 2020 2020 2020  CF name.        
+00013bf0: 7365 6c65 6374 3a20 7374 722c 206c 6973  select: str, lis
+00013c00: 740a 2020 2020 2020 2020 2020 2020 496e  t.            In
+00013c10: 636c 7564 6520 6f6e 6c79 2074 6865 7365  clude only these
+00013c20: 2061 7474 7269 6275 7465 730a 2020 2020   attributes.    
+00013c30: 2020 2020 6578 636c 7564 653a 2073 7472      exclude: str
+00013c40: 2c20 6c69 7374 0a20 2020 2020 2020 2020  , list.         
+00013c50: 2020 2045 7863 6c75 6465 2074 6865 7365     Exclude these
+00013c60: 2061 7474 7269 6275 7465 730a 2020 2020   attributes.    
+00013c70: 2020 2020 6d75 6c74 693a 2062 6f6f 6c0a      multi: bool.
+00013c80: 2020 2020 2020 2020 2020 2020 4765 7420              Get 
+00013c90: 7374 616e 6461 7264 5f6e 616d 6520 616e  standard_name an
+00013ca0: 6420 6c6f 6e67 5f6e 616d 6520 6174 7472  d long_name attr
+00013cb0: 6962 7574 6520 6173 2061 206c 6973 7420  ibute as a list 
+00013cc0: 6f66 2070 6f73 7369 626c 650a 2020 2020  of possible.    
+00013cd0: 2020 2020 2020 2020 7661 6c75 6573 0a20          values. 
+00013ce0: 2020 2020 2020 207b 6572 726f 7273 7d0a         {errors}.
+00013cf0: 2020 2020 2020 2020 6578 7472 613a 2064          extra: d
+00013d00: 6963 740a 2020 2020 2020 2020 2020 4578  ict.          Ex
+00013d10: 7472 6120 7061 7261 6d73 2061 7265 2069  tra params are i
+00013d20: 6e63 6c75 6465 6420 6173 2065 7874 7261  ncluded as extra
+00013d30: 2061 7474 7269 6275 7465 730a 0a20 2020   attributes..   
+00013d40: 2020 2020 2052 6574 7572 6e0a 2020 2020       Return.    
+00013d50: 2020 2020 2d2d 2d2d 2d2d 0a20 2020 2020      ------.     
+00013d60: 2020 2064 6963 740a 2020 2020 2020 2020     dict.        
+00013d70: 2222 220a 0a20 2020 2020 2020 2023 2047  """..        # G
+00013d80: 6574 2073 7065 6373 0a20 2020 2020 2020  et specs.       
+00013d90: 2073 7065 6373 203d 2073 656c 662e 6765   specs = self.ge
+00013da0: 745f 7370 6563 7328 6366 5f6e 616d 652c  t_specs(cf_name,
+00013db0: 2065 7272 6f72 733d 6572 726f 7273 290a   errors=errors).
+00013dc0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00013dd0: 7065 6373 3a0a 2020 2020 2020 2020 2020  pecs:.          
+00013de0: 2020 7265 7475 726e 207b 7d0a 0a20 2020    return {}..   
+00013df0: 2020 2020 2023 2057 6869 6368 2061 7474       # Which att
+00013e00: 7269 6275 7465 730a 2020 2020 2020 2020  ributes.        
+00013e10: 6966 2065 7863 6c75 6465 2069 7320 4e6f  if exclude is No
+00013e20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00013e30: 6578 636c 7564 6520 3d20 5b5d 0a20 2020  exclude = [].   
+00013e40: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00013e50: 616e 6365 2865 7863 6c75 6465 2c20 7374  ance(exclude, st
+00013e60: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00013e70: 6578 636c 7564 6520 3d20 5b65 7863 6c75  exclude = [exclu
+00013e80: 6465 5d0a 2020 2020 2020 2020 2320 6578  de].        # ex
+00013e90: 636c 7564 652e 6578 7465 6e64 2873 656c  clude.extend(sel
+00013ea0: 662e 6174 7472 735f 6578 636c 7564 6529  f.attrs_exclude)
+00013eb0: 0a20 2020 2020 2020 2065 7863 6c75 6465  .        exclude
+00013ec0: 2e65 7874 656e 6428 6578 7472 612e 6b65  .extend(extra.ke
+00013ed0: 7973 2829 290a 2020 2020 2020 2020 6578  ys()).        ex
+00013ee0: 636c 7564 6520 3d20 7365 7428 6578 636c  clude = set(excl
+00013ef0: 7564 6529 0a20 2020 2020 2020 206b 6579  ude).        key
+00013f00: 7320 3d20 7365 7428 7370 6563 735b 2261  s = set(specs["a
+00013f10: 7474 7273 225d 2e6b 6579 7328 2929 0a20  ttrs"].keys()). 
+00013f20: 2020 2020 2020 206b 6579 7320 2d3d 2065         keys -= e
+00013f30: 7863 6c75 6465 0a20 2020 2020 2020 2069  xclude.        i
+00013f40: 6620 7365 6c65 6374 3a0a 2020 2020 2020  f select:.      
+00013f50: 2020 2020 2020 6b65 7973 203d 206b 6579        keys = key
+00013f60: 732e 696e 7465 7273 6563 7469 6f6e 2873  s.intersection(s
+00013f70: 656c 6563 7429 0a0a 2020 2020 2020 2020  elect)..        
+00013f80: 2320 4c6f 6f70 0a20 2020 2020 2020 2061  # Loop.        a
+00013f90: 7474 7273 203d 207b 7d0a 2020 2020 2020  ttrs = {}.      
+00013fa0: 2020 666f 7220 6b65 7920 696e 2073 7065    for key in spe
+00013fb0: 6373 5b22 6174 7472 7322 5d2e 6b65 7973  cs["attrs"].keys
+00013fc0: 2829 3a0a 0a20 2020 2020 2020 2020 2020  ():..           
+00013fd0: 2023 204e 6f20 6c69 7374 7320 6f72 2074   # No lists or t
+00013fe0: 7570 6c65 730a 2020 2020 2020 2020 2020  uples.          
+00013ff0: 2020 7661 6c75 6520 3d20 7370 6563 735b    value = specs[
+00014000: 2261 7474 7273 225d 5b6b 6579 5d0a 2020  "attrs"][key].  
+00014010: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00014020: 6e73 7461 6e63 6528 7661 6c75 652c 206c  nstance(value, l
+00014030: 6973 7429 3a0a 2020 2020 2020 2020 2020  ist):.          
+00014040: 2020 2020 2020 6966 206c 656e 2876 616c        if len(val
+00014050: 7565 2920 3d3d 2030 3a0a 2020 2020 2020  ue) == 0:.      
+00014060: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00014070: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+00014080: 2020 2020 2020 2069 6620 6e6f 7420 6d75         if not mu
+00014090: 6c74 6920 6f72 206b 6579 206e 6f74 2069  lti or key not i
+000140a0: 6e20 2822 7374 616e 6461 7264 5f6e 616d  n ("standard_nam
+000140b0: 6522 2c20 226c 6f6e 675f 6e61 6d65 2229  e", "long_name")
+000140c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000140d0: 2020 2020 2020 7661 6c75 6520 3d20 7661        value = va
+000140e0: 6c75 655b 305d 0a0a 2020 2020 2020 2020  lue[0]..        
+000140f0: 2020 2020 2320 5374 6f72 6520 6974 0a20      # Store it. 
+00014100: 2020 2020 2020 2020 2020 2061 7474 7273             attrs
+00014110: 5b6b 6579 5d20 3d20 7661 6c75 650a 0a20  [key] = value.. 
+00014120: 2020 2020 2020 2023 2045 7874 7261 2061         # Extra a
+00014130: 7474 7269 6275 7465 730a 2020 2020 2020  ttributes.      
+00014140: 2020 6174 7472 732e 7570 6461 7465 2865    attrs.update(e
+00014150: 7874 7261 290a 0a20 2020 2020 2020 2023  xtra)..        #
+00014160: 2046 696e 616c 697a 6520 616e 6420 6f70   Finalize and op
+00014170: 7469 6f6e 616c 6c79 2063 6861 6e67 6520  tionally change 
+00014180: 6c6f 6361 7469 6f6e 0a20 2020 2020 2020  location.       
+00014190: 2061 7474 7273 203d 2073 656c 662e 7061   attrs = self.pa
+000141a0: 7265 6e74 2e73 676c 6f63 6174 6f72 2e66  rent.sglocator.f
+000141b0: 6f72 6d61 745f 6174 7472 7328 6174 7472  ormat_attrs(attr
+000141c0: 732c 206c 6f63 3d6c 6f63 2c20 7374 616e  s, loc=loc, stan
+000141d0: 6461 7264 697a 653d 7374 616e 6461 7264  dardize=standard
+000141e0: 697a 6529 0a0a 2020 2020 2020 2020 7265  ize)..        re
+000141f0: 7475 726e 2061 7474 7273 0a0a 2020 2020  turn attrs..    
+00014200: 6465 6620 6765 745f 6e61 6d65 2873 656c  def get_name(sel
+00014210: 662c 206e 616d 652c 2073 7065 6369 616c  f, name, special
+00014220: 697a 653d 4661 6c73 652c 206c 6f63 3d4e  ize=False, loc=N
+00014230: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
+00014240: 2247 6574 2074 6865 206e 616d 6520 6f66  "Get the name of
+00014250: 2074 6865 206d 6174 6368 696e 6720 4346   the matching CF
+00014260: 2073 7065 6373 0a0a 2020 2020 2020 2020   specs..        
+00014270: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00014280: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00014290: 2020 2020 2020 6e61 6d65 3a20 7374 722c        name: str,
+000142a0: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
+000142b0: 790a 2020 2020 2020 2020 2020 2020 4569  y.            Ei
+000142c0: 7468 6572 2061 2064 6174 6120 6172 7261  ther a data arra
+000142d0: 792c 2061 206b 6e6f 776e 2063 6620 6e61  y, a known cf na
+000142e0: 6d65 206f 7220 6120 6461 7461 2076 6172  me or a data var
+000142f0: 206e 616d 650a 2020 2020 2020 2020 7370   name.        sp
+00014300: 6563 6961 6c69 7a65 3a20 626f 6f6c 0a20  ecialize: bool. 
+00014310: 2020 2020 2020 2020 2020 2047 6574 2074             Get t
+00014320: 6865 2066 6972 7374 206e 616d 650a 2020  he first name.  
+00014330: 2020 2020 2020 2020 2020 6173 206c 6973            as lis
+00014340: 7465 6420 696e 2073 7065 6373 2c20 7768  ted in specs, wh
+00014350: 6963 6820 6973 2067 656e 6572 616c 6c79  ich is generally
+00014360: 2061 2073 7065 6369 616c 697a 6564 206f   a specialized o
+00014370: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00014380: 6c69 6b65 2061 206e 616d 6520 6164 6f70  like a name adop
+00014390: 7465 6420 6279 2073 7065 6369 616c 697a  ted by specializ
+000143a0: 6564 2064 6174 6173 6574 2e0a 2020 2020  ed dataset..    
+000143b0: 2020 2020 6c6f 633a 2073 7472 2c20 4e6f      loc: str, No
+000143c0: 6e65 0a20 2020 2020 2020 2020 2020 2046  ne.            F
+000143d0: 6f72 6d61 7420 6974 2061 7420 7468 6973  ormat it at this
+000143e0: 206c 6f63 6174 696f 6e0a 0a20 2020 2020   location..     
+000143f0: 2020 2052 6574 7572 6e0a 2020 2020 2020     Return.      
+00014400: 2020 2d2d 2d2d 2d2d 0a20 2020 2020 2020    ------.       
+00014410: 204e 6f6e 6520 6f72 2073 7472 0a20 2020   None or str.   
+00014420: 2020 2020 2020 2020 2045 6974 6865 7220           Either 
+00014430: 7468 6520 4346 206e 616d 6520 6f72 2074  the CF name or t
+00014440: 6865 2073 7065 6369 616c 697a 6564 206e  he specialized n
+00014450: 616d 650a 2020 2020 2020 2020 2222 220a  ame.        """.
+00014460: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00014470: 7369 6e73 7461 6e63 6528 6e61 6d65 2c20  sinstance(name, 
+00014480: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00014490: 2020 6e61 6d65 203d 206e 616d 652e 656e    name = name.en
+000144a0: 636f 6469 6e67 2e67 6574 2822 6366 5f6e  coding.get("cf_n
+000144b0: 616d 6522 2c20 7365 6c66 2e6d 6174 6368  ame", self.match
+000144c0: 286e 616d 6529 290a 2020 2020 2020 2020  (name)).        
+000144d0: 2020 2020 2320 4649 584d 453a 2063 6174      # FIXME: cat
+000144e0: 6567 6f72 793f 0a20 2020 2020 2020 2065  egory?.        e
+000144f0: 6c69 6620 6e61 6d65 206e 6f74 2069 6e20  lif name not in 
+00014500: 7365 6c66 3a0a 2020 2020 2020 2020 2020  self:.          
+00014510: 2020 6e61 6d65 203d 2073 656c 662e 6d61    name = self.ma
+00014520: 7463 685f 6672 6f6d 5f6e 616d 6528 6e61  tch_from_name(na
+00014530: 6d65 290a 2020 2020 2020 2020 6966 206e  me).        if n
+00014540: 616d 6520 6973 204e 6f6e 653a 0a20 2020  ame is None:.   
+00014550: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00014560: 2020 2020 2020 2020 6966 2073 7065 6369          if speci
+00014570: 616c 697a 6520 616e 6420 7365 6c66 5b6e  alize and self[n
+00014580: 616d 655d 5b22 6e61 6d65 225d 3a0a 2020  ame]["name"]:.  
+00014590: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
+000145a0: 2073 656c 665b 6e61 6d65 5d5b 226e 616d   self[name]["nam
+000145b0: 6522 5d0a 2020 2020 2020 2020 7265 7475  e"].        retu
+000145c0: 726e 2073 656c 662e 7367 6c6f 6361 746f  rn self.sglocato
+000145d0: 722e 666f 726d 6174 5f61 7474 7228 226e  r.format_attr("n
+000145e0: 616d 6522 2c20 6e61 6d65 2c20 6c6f 633d  ame", name, loc=
+000145f0: 6c6f 6329 0a0a 2020 2020 6465 6620 6765  loc)..    def ge
+00014600: 745f 6c6f 635f 6172 6728 7365 6c66 2c20  t_loc_arg(self, 
+00014610: 6461 2c20 6366 5f6e 616d 653d 4e6f 6e65  da, cf_name=None
+00014620: 2c20 6c6f 6361 7469 6f6e 733d 4e6f 6e65  , locations=None
+00014630: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+00014640: 7420 7468 6520 606c 6f63 6020 6172 6775  t the `loc` argu
+00014650: 6d65 6e74 2066 726f 6d20 6120 6e61 6d65  ment from a name
+00014660: 206f 7220 6461 7461 2061 7272 6179 2077   or data array w
+00014670: 6974 6820 6e61 6d65 0a0a 2020 2020 2020  ith name..      
+00014680: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00014690: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+000146a0: 2020 2020 2020 2020 6461 3a20 7861 7272          da: xarr
+000146b0: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
+000146c0: 2020 2020 2063 665f 6e61 6d65 3a20 4e6f       cf_name: No
+000146d0: 6e65 2c20 7374 720a 2020 2020 2020 2020  ne, str.        
+000146e0: 2020 2020 4120 6765 6e65 7269 6320 4346      A generic CF
+000146f0: 206e 616d 650a 2020 2020 2020 2020 6c6f   name.        lo
+00014700: 6361 7469 6f6e 733a 204e 6f6e 652c 2064  cations: None, d
+00014710: 6963 740a 0a20 2020 2020 2020 2052 6574  ict..        Ret
+00014720: 7572 6e0a 2020 2020 2020 2020 2d2d 2d2d  urn.        ----
+00014730: 2d2d 0a20 2020 2020 2020 204e 6f6e 652c  --.        None,
+00014740: 2046 616c 7365 2c20 7374 720a 2020 2020   False, str.    
+00014750: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014760: 2320 4a75 7374 2061 206e 616d 650a 2020  # Just a name.  
+00014770: 2020 2020 2020 2320 4649 584d 453a 2072        # FIXME: r
+00014780: 6561 6c6c 793f 0a20 2020 2020 2020 2069  eally?.        i
+00014790: 6620 6973 696e 7374 616e 6365 2864 612c  f isinstance(da,
+000147a0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+000147b0: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
+000147c0: 676c 6f63 6174 6f72 2e70 6172 7365 5f61  glocator.parse_a
+000147d0: 7474 7228 226e 616d 6522 2c20 6461 295b  ttr("name", da)[
+000147e0: 315d 0a0a 2020 2020 2020 2020 2320 4672  1]..        # Fr
+000147f0: 6f6d 2063 6f6e 6669 670a 2020 2020 2020  om config.      
+00014800: 2020 2320 6966 2022 6366 5f6c 6f63 2220    # if "cf_loc" 
+00014810: 696e 2064 612e 656e 636f 6469 6e67 3a20  in da.encoding: 
+00014820: 2023 2041 6c72 6561 6479 2069 6e66 6572   # Already infer
+00014830: 6564 2061 6e64 2073 746f 7265 6420 696e  ed and stored in
+00014840: 2065 6e63 6f64 696e 670a 2020 2020 2020   encoding.      
+00014850: 2020 2320 2020 2020 6c6f 6320 3d20 6461    #     loc = da
+00014860: 2e65 6e63 6f64 696e 675b 2263 665f 6c6f  .encoding["cf_lo
+00014870: 6322 5d0a 2020 2020 2020 2020 2320 656c  c"].        # el
+00014880: 7365 3a20 2023 2049 6e66 6572 2066 726f  se:  # Infer fro
+00014890: 6d20 636f 6e66 6967 0a20 2020 2020 2020  m config.       
+000148a0: 2069 6620 6c6f 6361 7469 6f6e 7320 6973   if locations is
+000148b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000148c0: 2020 206c 6f63 6174 696f 6e73 203d 2073     locations = s
+000148d0: 656c 662e 6765 745f 6c6f 635f 6d61 7070  elf.get_loc_mapp
+000148e0: 696e 6728 6461 2c20 6366 5f6e 616d 6573  ing(da, cf_names
+000148f0: 3d7b 6461 2e6e 616d 653a 2063 665f 6e61  ={da.name: cf_na
+00014900: 6d65 7d29 0a20 2020 2020 2020 206c 6f63  me}).        loc
+00014910: 203d 206c 6f63 6174 696f 6e73 2e67 6574   = locations.get
+00014920: 2864 612e 6e61 6d65 290a 2020 2020 2020  (da.name).      
+00014930: 2020 6966 206c 6f63 2069 7320 6e6f 7420    if loc is not 
+00014940: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00014950: 2020 7265 7475 726e 206c 6f63 0a0a 2020    return loc..  
+00014960: 2020 2020 2020 2320 4672 6f6d 2074 6865        # From the
+00014970: 2061 7272 6179 2061 7474 7269 6275 7465   array attribute
+00014980: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
+00014990: 2073 656c 662e 7367 6c6f 6361 746f 722e   self.sglocator.
+000149a0: 6765 745f 6c6f 635f 6672 6f6d 5f64 6128  get_loc_from_da(
+000149b0: 6461 290a 0a20 2020 2064 6566 2066 6f72  da)..    def for
+000149c0: 6d61 745f 6461 7461 6172 7261 7928 0a20  mat_dataarray(. 
+000149d0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000149e0: 2020 2020 2064 612c 0a20 2020 2020 2020       da,.       
+000149f0: 2063 665f 6e61 6d65 3d4e 6f6e 652c 0a20   cf_name=None,. 
+00014a00: 2020 2020 2020 2072 656e 616d 653d 5472         rename=Tr
+00014a10: 7565 2c0a 2020 2020 2020 2020 7370 6563  ue,.        spec
+00014a20: 6961 6c69 7a65 3d46 616c 7365 2c0a 2020  ialize=False,.  
+00014a30: 2020 2020 2020 2320 7265 6e61 6d65 5f64        # rename_d
+00014a40: 696d 3d54 7275 652c 0a20 2020 2020 2020  im=True,.       
+00014a50: 206c 6f63 3d4e 6f6e 652c 0a20 2020 2020   loc=None,.     
+00014a60: 2020 2061 7474 7273 3d54 7275 652c 0a20     attrs=True,. 
+00014a70: 2020 2020 2020 2073 7461 6e64 6172 6469         standardi
+00014a80: 7a65 3d54 7275 652c 0a20 2020 2020 2020  ze=True,.       
+00014a90: 2072 6570 6c61 6365 5f61 7474 7273 3d46   replace_attrs=F
+00014aa0: 616c 7365 2c0a 2020 2020 2020 2020 636f  alse,.        co
+00014ab0: 7079 3d54 7275 652c 0a20 2020 2020 2020  py=True,.       
+00014ac0: 2023 2061 6464 5f6c 6f63 5f74 6f5f 6e61   # add_loc_to_na
+00014ad0: 6d65 3d4e 6f6e 652c 0a20 2020 2029 3a0a  me=None,.    ):.
+00014ae0: 2020 2020 2020 2020 2222 2246 6f72 6d61          """Forma
+00014af0: 7420 6120 4461 7461 4172 7261 7927 7320  t a DataArray's 
+00014b00: 6e61 6d65 2061 6e64 2061 7474 7269 6275  name and attribu
+00014b10: 7465 730a 0a20 2020 2020 2020 2050 6172  tes..        Par
+00014b20: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00014b30: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00014b40: 2020 2064 613a 2078 6172 7261 792e 4461     da: xarray.Da
+00014b50: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
+00014b60: 6366 5f6e 616d 653a 2073 7472 2c20 4e6f  cf_name: str, No
+00014b70: 6e65 0a20 2020 2020 2020 2020 2020 2041  ne.            A
+00014b80: 2067 656e 6572 6963 2043 4620 6e61 6d65   generic CF name
+00014b90: 2e20 4966 206e 6f74 2070 726f 7669 6465  . If not provide
+00014ba0: 642c 2069 7420 6775 6573 7365 6420 7769  d, it guessed wi
+00014bb0: 7468 203a 6d65 7468 3a60 6d61 7463 6860  th :meth:`match`
+00014bc0: 2e0a 2020 2020 2020 2020 6c6f 633a 2073  ..        loc: s
+00014bd0: 7472 2c20 7b22 616e 7922 2c20 4e6f 6e65  tr, {"any", None
+00014be0: 7d2c 207b 2222 2c20 4661 6c73 657d 0a20  }, {"", False}. 
+00014bf0: 2020 2020 2020 2020 2020 202d 2073 7472             - str
+00014c00: 3a20 6f6e 6520 6f66 2074 6865 7365 206c  : one of these l
+00014c10: 6f63 6174 696f 6e73 0a20 2020 2020 2020  ocations.       
+00014c20: 2020 2020 202d 204e 6f6e 6520 6f72 2022       - None or "
+00014c30: 616e 7922 3a20 616e 790a 2020 2020 2020  any": any.      
+00014c40: 2020 2020 2020 2d20 4661 6c73 6520 6f72        - False or
+00014c50: 2027 2222 3a20 6e6f 206c 6f63 6174 696f   '"": no locatio
+00014c60: 6e0a 2020 2020 2020 2020 7265 6e61 6d65  n.        rename
+00014c70: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
+00014c80: 2020 2052 656e 616d 6520 6172 7261 7973     Rename arrays
+00014c90: 2077 6865 6e20 7468 6569 7220 6e61 6d65   when their name
+00014ca0: 2069 7320 7365 743f 0a20 2020 2020 2020   is set?.       
+00014cb0: 2061 6464 5f6c 6f63 5f74 6f5f 6e61 6d65   add_loc_to_name
+00014cc0: 3a20 4e6f 6e65 2c20 626f 6f6c 0a20 2020  : None, bool.   
+00014cd0: 2020 2020 2020 2020 2041 6464 2074 6865           Add the
+00014ce0: 206c 6f63 2074 6f20 7468 6520 6e61 6d65   loc to the name
+00014cf0: 2c20 6f76 6572 7269 6469 6e67 2074 6865  , overriding the
+00014d00: 2073 7065 6373 2e0a 2020 2020 2020 2020   specs..        
+00014d10: 6174 7472 733a 2062 6f6f 6c2c 2064 6963  attrs: bool, dic
+00014d20: 740a 2020 2020 2020 2020 2020 2020 4966  t.            If
+00014d30: 2046 616c 7365 2c20 646f 6573 206e 6f74   False, does not
+00014d40: 2063 6861 6e67 6520 6174 7472 6962 7574   change attribut
+00014d50: 6573 2061 7420 616c 6c2e 0a20 2020 2020  es at all..     
+00014d60: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+00014d70: 7573 6520 4366 2061 7474 7269 6275 7465  use Cf attribute
+00014d80: 732e 0a20 2020 2020 2020 2020 2020 2049  s..            I
+00014d90: 6620 6120 6469 6374 2c20 7573 6520 7468  f a dict, use th
+00014da0: 6973 2064 6963 742e 0a20 2020 2020 2020  is dict..       
+00014db0: 2072 6570 6c61 6365 5f61 7474 7273 3a20   replace_attrs: 
+00014dc0: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
+00014dd0: 2052 6570 6c61 6365 2065 7869 7374 696e   Replace existin
+00014de0: 6720 6174 7472 6962 7574 6573 3f0a 2020  g attributes?.  
+00014df0: 2020 2020 2020 7374 616e 6461 7264 697a        standardiz
+00014e00: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00014e10: 7370 6563 6961 6c69 7a65 3a20 626f 6f6c  specialize: bool
+00014e20: 0a20 2020 2020 2020 2020 2020 2044 6f20  .            Do 
+00014e30: 6e6f 7420 7573 6520 7468 6520 4346 206e  not use the CF n
+00014e40: 616d 6520 666f 7220 7265 6e61 6d69 6e67  ame for renaming
+00014e50: 2c20 6275 7420 7468 6520 7661 6c75 6520  , but the value 
+00014e60: 6f66 2074 6865 2022 6e61 6d65 2220 656e  of the "name" en
+00014e70: 7472 792c 0a20 2020 2020 2020 2020 2020  try,.           
+00014e80: 2077 6869 6368 2069 7320 6765 6e65 7261   which is genera
+00014e90: 6c6c 7920 6120 7370 6563 6961 6c69 7a65  lly a specialize
+00014ea0: 6420 6f6e 652c 206c 696b 6520 6120 6e61  d one, like a na
+00014eb0: 6d65 2061 646f 7074 6564 2062 7920 7370  me adopted by sp
+00014ec0: 6563 6961 6c69 7a65 6420 6461 7461 7365  ecialized datase
+00014ed0: 742e 0a20 2020 2020 2020 2072 656e 616d  t..        renam
+00014ee0: 655f 6469 6d3a 2062 6f6f 6c0a 2020 2020  e_dim: bool.    
+00014ef0: 2020 2020 2020 2020 466f 7220 6120 3144          For a 1D
+00014f00: 2061 7272 6179 2c20 7265 6e61 6d65 2074   array, rename t
+00014f10: 6865 2064 696d 656e 7369 6f6e 2069 6620  he dimension if 
+00014f20: 6974 2068 6173 2074 6865 2073 616d 6520  it has the same 
+00014f30: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+00014f40: 2061 7320 7468 6520 6172 7261 792e 0a20   as the array.. 
+00014f50: 2020 2020 2020 2020 2020 204e 6f74 6520             Note 
+00014f60: 7468 6174 2069 7420 6973 2073 6574 2074  that it is set t
+00014f70: 6f20 4661 6c73 652c 2069 6620 6060 7265  o False, if ``re
+00014f80: 6e61 6d65 6060 2069 7320 4661 6c73 652e  name`` is False.
+00014f90: 0a20 2020 2020 2020 2063 6f70 793a 2062  .        copy: b
+00014fa0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+00014fb0: 466f 7263 6520 6120 636f 7079 2028 6e6f  Force a copy (no
+00014fc0: 7420 6f66 2074 6865 2064 6174 6129 2069  t of the data) i
+00014fd0: 6e20 616e 7920 6361 7365 3f0a 0a20 2020  n any case?..   
+00014fe0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00014ff0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00015000: 2020 2020 2078 6172 7261 792e 4461 7461       xarray.Data
+00015010: 4172 7261 792c 2073 7472 2c20 4e6f 6e65  Array, str, None
+00015020: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00015030: 2066 6f72 6d61 7474 6564 2061 7272 6179   formatted array
+00015040: 206f 7220 636f 7079 206f 6620 6974 2e0a   or copy of it..
+00015050: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00015060: 4346 206e 616d 652c 2067 6976 656e 206f  CF name, given o
+00015070: 7220 6d61 7463 6869 6e67 2c20 6966 2072  r matching, if r
+00015080: 656e 616d 6520 6966 2046 616c 7365 3b20  ename if False; 
+00015090: 616e 6420 4e6f 6e65 0a20 2020 2020 2020  and None.       
+000150a0: 2020 2020 2069 6620 6e6f 7420 6d61 7463       if not matc
+000150b0: 6869 6e67 2e0a 0a20 2020 2020 2020 2022  hing...        "
+000150c0: 2222 0a20 2020 2020 2020 2069 6620 7265  "".        if re
+000150d0: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
+000150e0: 2020 636f 7079 203d 2054 7275 650a 2020    copy = True.  
+000150f0: 2020 2020 2020 6966 2063 6f70 793a 0a20        if copy:. 
+00015100: 2020 2020 2020 2020 2020 2064 6120 3d20             da = 
+00015110: 6461 2e63 6f70 7928 290a 0a20 2020 2020  da.copy()..     
+00015120: 2020 2023 204e 616d 6573 0a20 2020 2020     # Names.     
+00015130: 2020 2069 6620 6366 5f6e 616d 6520 6973     if cf_name is
+00015140: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00015150: 2020 2063 665f 6e61 6d65 203d 2073 656c     cf_name = sel
+00015160: 662e 6d61 7463 6828 6461 290a 2020 2020  f.match(da).    
+00015170: 2020 2020 6966 2063 665f 6e61 6d65 2069      if cf_name i
+00015180: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00015190: 2020 2020 6966 206e 6f74 2072 656e 616d      if not renam
+000151a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000151b0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+000151c0: 2020 2020 2020 7265 7475 726e 2064 612e        return da.
+000151d0: 636f 7079 2829 2069 6620 636f 7079 2065  copy() if copy e
+000151e0: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
+000151f0: 2061 7373 6572 7420 6366 5f6e 616d 6520   assert cf_name 
+00015200: 696e 2073 656c 662e 6e61 6d65 730a 2020  in self.names.  
+00015210: 2020 2020 2020 6f6c 645f 6e61 6d65 203d        old_name =
+00015220: 2064 612e 6e61 6d65 0a20 2020 2020 2020   da.name.       
+00015230: 206e 6577 5f6e 616d 6520 3d20 7365 6c66   new_name = self
+00015240: 2e67 6574 5f6e 616d 6528 6366 5f6e 616d  .get_name(cf_nam
+00015250: 652c 2073 7065 6369 616c 697a 653d 7370  e, specialize=sp
+00015260: 6563 6961 6c69 7a65 2920 2023 2069 6620  ecialize)  # if 
+00015270: 7370 6563 6961 6c69 7a65 2065 6c73 6520  specialize else 
+00015280: 6366 5f6e 616d 650a 0a20 2020 2020 2020  cf_name..       
+00015290: 2023 204c 6f63 6174 696f 6e0a 2020 2020   # Location.    
+000152a0: 2020 2020 6966 206c 6f63 2069 7320 4e6f      if loc is No
+000152b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000152c0: 6c6f 6320 3d20 7365 6c66 2e67 6574 5f6c  loc = self.get_l
+000152d0: 6f63 5f61 7267 2864 6129 2020 2320 6672  oc_arg(da)  # fr
+000152e0: 6f6d 2063 6f6e 6669 670a 0a20 2020 2020  om config..     
+000152f0: 2020 2023 2041 7474 7269 6275 7465 730a     # Attributes.
+00015300: 2020 2020 2020 2020 6966 2061 7474 7273          if attrs
+00015310: 2069 7320 5472 7565 3a0a 0a20 2020 2020   is True:..     
+00015320: 2020 2020 2020 2023 2047 6574 2061 7474         # Get att
+00015330: 7269 6275 7465 7320 6672 6f6d 2043 6620  ributes from Cf 
+00015340: 7370 6563 730a 2020 2020 2020 2020 2020  specs.          
+00015350: 2020 6174 7472 7320 3d20 7365 6c66 2e67    attrs = self.g
+00015360: 6574 5f61 7474 7273 2863 665f 6e61 6d65  et_attrs(cf_name
+00015370: 2c20 6c6f 633d 4e6f 6e65 2c20 7374 616e  , loc=None, stan
+00015380: 6461 7264 697a 653d 4661 6c73 652c 206d  dardize=False, m
+00015390: 756c 7469 3d54 7275 6529 0a0a 2020 2020  ulti=True)..    
+000153a0: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
+000153b0: 2061 7869 7320 6174 7472 6962 7574 6520   axis attribute 
+000153c0: 666f 7220 6175 7869 6c61 7279 2063 6f6f  for auxilary coo
+000153d0: 7264 696e 6174 6573 0a20 2020 2020 2020  rdinates.       
+000153e0: 2020 2020 2069 6620 6461 2e6e 616d 6520       if da.name 
+000153f0: 616e 6420 6461 2e6e 616d 6520 6e6f 7420  and da.name not 
+00015400: 696e 2064 612e 696e 6465 7865 7320 616e  in da.indexes an
+00015410: 6420 2261 7869 7322 2069 6e20 6174 7472  d "axis" in attr
+00015420: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00015430: 2020 2064 656c 2061 7474 7273 5b22 6178     del attrs["ax
+00015440: 6973 225d 0a0a 2020 2020 2020 2020 656c  is"]..        el
+00015450: 6966 206e 6f74 2061 7474 7273 3a0a 2020  if not attrs:.  
+00015460: 2020 2020 2020 2020 2020 6174 7472 7320            attrs 
+00015470: 3d20 7b7d 0a0a 2020 2020 2020 2020 2320  = {}..        # 
+00015480: 466f 726d 6174 2061 7272 6179 0a20 2020  Format array.   
+00015490: 2020 2020 206e 6577 5f64 6120 3d20 7365       new_da = se
+000154a0: 6c66 2e73 676c 6f63 6174 6f72 2e66 6f72  lf.sglocator.for
+000154b0: 6d61 745f 6461 7461 6172 7261 7928 0a20  mat_dataarray(. 
+000154c0: 2020 2020 2020 2020 2020 2064 612c 0a20             da,. 
+000154d0: 2020 2020 2020 2020 2020 206c 6f63 3d6c             loc=l
+000154e0: 6f63 2c0a 2020 2020 2020 2020 2020 2020  oc,.            
+000154f0: 6e61 6d65 3d6e 6577 5f6e 616d 652c 0a20  name=new_name,. 
+00015500: 2020 2020 2020 2020 2020 2061 7474 7273             attrs
+00015510: 3d61 7474 7273 2c0a 2020 2020 2020 2020  =attrs,.        
+00015520: 2020 2020 7374 616e 6461 7264 697a 653d      standardize=
+00015530: 7374 616e 6461 7264 697a 652c 0a20 2020  standardize,.   
+00015540: 2020 2020 2020 2020 2072 656e 616d 653d           rename=
+00015550: 7265 6e61 6d65 2c0a 2020 2020 2020 2020  rename,.        
+00015560: 2020 2020 2320 6164 645f 6c6f 635f 746f      # add_loc_to
+00015570: 5f6e 616d 653d 6164 645f 6c6f 635f 746f  _name=add_loc_to
+00015580: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
+00015590: 2020 2072 6570 6c61 6365 5f61 7474 7273     replace_attrs
+000155a0: 3d72 6570 6c61 6365 5f61 7474 7273 2c0a  =replace_attrs,.
+000155b0: 2020 2020 2020 2020 2020 2020 636f 7079              copy
+000155c0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+000155d0: 290a 2020 2020 2020 2020 2320 6e65 775f  ).        # new_
+000155e0: 6461 2e65 6e63 6f64 696e 675b 2263 665f  da.encoding["cf_
+000155f0: 6e61 6d65 225d 203d 2063 665f 6e61 6d65  name"] = cf_name
+00015600: 0a0a 2020 2020 2020 2020 2320 5265 7475  ..        # Retu
+00015610: 726e 206e 6577 206e 616d 6520 6275 7420  rn new name but 
+00015620: 646f 6e27 7420 7265 6e61 6d65 0a20 2020  don't rename.   
+00015630: 2020 2020 2069 6620 6e6f 7420 7265 6e61       if not rena
+00015640: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
+00015650: 6966 206f 6c64 5f6e 616d 6520 6973 204e  if old_name is N
+00015660: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00015670: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00015680: 2e73 676c 6f63 6174 6f72 2e66 6f72 6d61  .sglocator.forma
+00015690: 745f 6174 7472 2822 6e61 6d65 222c 206e  t_attr("name", n
+000156a0: 6577 5f6e 616d 652c 206c 6f63 290a 2020  ew_name, loc).  
+000156b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000156c0: 2073 656c 662e 7367 6c6f 6361 746f 722e   self.sglocator.
+000156d0: 6d65 7267 655f 6174 7472 2822 6e61 6d65  merge_attr("name
+000156e0: 222c 206f 6c64 5f6e 616d 652c 206e 6577  ", old_name, new
+000156f0: 5f6e 616d 652c 206c 6f63 290a 0a20 2020  _name, loc)..   
+00015700: 2020 2020 2023 2023 2052 656e 616d 6520       # # Rename 
+00015710: 6469 6d20 6966 2061 7869 7320 636f 6f72  dim if axis coor
+00015720: 6469 6e61 7465 0a20 2020 2020 2020 2023  dinate.        #
+00015730: 2072 656e 616d 655f 6469 6d20 3d20 7265   rename_dim = re
+00015740: 6e61 6d65 2061 6e64 2072 656e 616d 655f  name and rename_
+00015750: 6469 6d0a 2020 2020 2020 2020 2320 6966  dim.        # if
+00015760: 2028 7265 6e61 6d65 5f64 696d 2061 6e64   (rename_dim and
+00015770: 206f 6c64 5f6e 616d 6520 616e 6420 6f6c   old_name and ol
+00015780: 645f 6e61 6d65 2069 6e20 6461 2e69 6e64  d_name in da.ind
+00015790: 6578 6573 293a 0a20 2020 2020 2020 2023  exes):.        #
+000157a0: 2020 2020 206e 6577 5f64 6120 3d20 6e65       new_da = ne
+000157b0: 775f 6461 2e72 656e 616d 6528 7b6f 6c64  w_da.rename({old
+000157c0: 5f6e 616d 653a 206e 6577 5f64 612e 6e61  _name: new_da.na
+000157d0: 6d65 7d29 0a0a 2020 2020 2020 2020 7265  me})..        re
+000157e0: 7475 726e 206e 6577 5f64 610a 0a20 2020  turn new_da..   
+000157f0: 2064 6566 2072 656e 616d 655f 6461 7461   def rename_data
+00015800: 6172 7261 7928 0a20 2020 2020 2020 2073  array(.        s
+00015810: 656c 662c 0a20 2020 2020 2020 2064 612c  elf,.        da,
+00015820: 0a20 2020 2020 2020 206e 616d 653d 4e6f  .        name=No
+00015830: 6e65 2c0a 2020 2020 2020 2020 7370 6563  ne,.        spec
+00015840: 6961 6c69 7a65 3d46 616c 7365 2c0a 2020  ialize=False,.  
+00015850: 2020 2020 2020 6c6f 633d 4e6f 6e65 2c0a        loc=None,.
+00015860: 2020 2020 2020 2020 7374 616e 6461 7264          standard
+00015870: 697a 653d 5472 7565 2c0a 2020 2020 2020  ize=True,.      
+00015880: 2020 7265 6e61 6d65 5f64 696d 3d54 7275    rename_dim=Tru
+00015890: 652c 0a20 2020 2020 2020 2063 6f70 793d  e,.        copy=
+000158a0: 5472 7565 2c0a 2020 2020 2020 2020 6164  True,.        ad
+000158b0: 645f 6c6f 635f 746f 5f6e 616d 653d 4e6f  d_loc_to_name=No
+000158c0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+000158d0: 2020 2022 2222 5265 6e61 6d65 2061 2044     """Rename a D
+000158e0: 6174 6141 7272 6179 0a0a 2020 2020 2020  ataArray..      
+000158f0: 2020 4974 2069 7320 6120 7370 6563 6961    It is a specia
+00015900: 6c69 7a65 6420 6361 6c6c 2074 6f20 3a6d  lized call to :m
+00015910: 6574 683a 6066 6f72 6d61 745f 6461 7461  eth:`format_data
+00015920: 6172 7261 7960 2077 6865 7265 0a20 2020  array` where.   
+00015930: 2020 2020 2061 7474 7269 6275 7465 7320       attributes 
+00015940: 6172 6520 6c65 6674 2075 6e63 6861 6e67  are left unchang
+00015950: 6564 2e0a 0a20 2020 2020 2020 2050 6172  ed...        Par
+00015960: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00015970: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00015980: 2020 2064 613a 2078 6172 7261 792e 4461     da: xarray.Da
+00015990: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
+000159a0: 6e61 6d65 3a20 7374 722c 204e 6f6e 650a  name: str, None.
+000159b0: 2020 2020 2020 2020 2020 2020 4120 4346              A CF
+000159c0: 206e 616d 652e 2049 6620 6e6f 7420 7072   name. If not pr
+000159d0: 6f76 6964 6564 2c20 6974 2067 7565 7373  ovided, it guess
+000159e0: 6564 2077 6974 6820 3a6d 6574 683a 606d  ed with :meth:`m
+000159f0: 6174 6368 602e 0a20 2020 2020 2020 2073  atch`..        s
+00015a00: 7065 6369 616c 697a 653a 2062 6f6f 6c0a  pecialize: bool.
+00015a10: 2020 2020 2020 2020 2020 2020 446f 6573              Does
+00015a20: 206e 6f74 2075 7365 2074 6865 2043 4620   not use the CF 
+00015a30: 6e61 6d65 2066 6f72 2072 656e 616d 696e  name for renamin
+00015a40: 672c 2062 7574 2074 6865 2066 6972 7374  g, but the first
+00015a50: 206e 616d 650a 2020 2020 2020 2020 2020   name.          
+00015a60: 2020 6173 206c 6973 7465 6420 696e 2073    as listed in s
+00015a70: 7065 6373 2c20 7768 6963 6820 6973 2067  pecs, which is g
+00015a80: 656e 6572 616c 6c79 2061 2073 7065 6369  enerally a speci
+00015a90: 616c 697a 6564 206f 6e65 2c0a 2020 2020  alized one,.    
+00015aa0: 2020 2020 2020 2020 6c69 6b65 2061 206e          like a n
+00015ab0: 616d 6520 6164 6f70 7465 6420 6279 2073  ame adopted by s
+00015ac0: 7065 6369 616c 697a 6564 2064 6174 6173  pecialized datas
+00015ad0: 6574 2e0a 2020 2020 2020 2020 6c6f 633a  et..        loc:
+00015ae0: 2073 7472 2c20 7b22 616e 7922 2c20 4e6f   str, {"any", No
+00015af0: 6e65 7d2c 207b 2222 2c20 4661 6c73 657d  ne}, {"", False}
+00015b00: 0a20 2020 2020 2020 2020 2020 202d 2073  .            - s
+00015b10: 7472 3a20 6f6e 6520 6f66 2074 6865 7365  tr: one of these
+00015b20: 206c 6f63 6174 696f 6e73 0a20 2020 2020   locations.     
+00015b30: 2020 2020 2020 202d 204e 6f6e 6520 6f72         - None or
+00015b40: 2022 616e 7922 3a20 616e 790a 2020 2020   "any": any.    
+00015b50: 2020 2020 2020 2020 2d20 4661 6c73 6520          - False 
+00015b60: 6f72 2027 2222 3a20 6e6f 206c 6f63 6174  or '"": no locat
+00015b70: 696f 6e0a 2020 2020 2020 2020 7374 616e  ion.        stan
+00015b80: 6461 7264 697a 653a 2062 6f6f 6c0a 2020  dardize: bool.  
+00015b90: 2020 2020 2020 7265 6e61 6d65 5f64 696d        rename_dim
+00015ba0: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
+00015bb0: 2020 2046 6f72 2061 2031 4420 6172 7261     For a 1D arra
+00015bc0: 792c 2072 656e 616d 6520 7468 6520 6469  y, rename the di
+00015bd0: 6d65 6e73 696f 6e20 6966 2069 7420 6861  mension if it ha
+00015be0: 7320 7468 6520 7361 6d65 206e 616d 650a  s the same name.
+00015bf0: 2020 2020 2020 2020 2020 2020 6173 2074              as t
+00015c00: 6865 2061 7272 6179 2e0a 2020 2020 2020  he array..      
+00015c10: 2020 2020 2020 4e6f 7465 2074 6861 7420        Note that 
+00015c20: 6974 2069 7320 7365 7420 746f 2046 616c  it is set to Fal
+00015c30: 7365 2c20 6966 2060 6072 656e 616d 6560  se, if ``rename`
+00015c40: 6020 6973 2046 616c 7365 2e0a 2020 2020  ` is False..    
+00015c50: 2020 2020 636f 7079 3a20 626f 6f6c 0a20      copy: bool. 
+00015c60: 2020 2020 2020 2020 2020 2046 6f72 6365             Force
+00015c70: 2061 2063 6f70 7920 286e 6f74 206f 6620   a copy (not of 
+00015c80: 7468 6520 6461 7461 2920 696e 2061 6e79  the data) in any
+00015c90: 2063 6173 653f 0a0a 0a20 2020 2020 2020   case?...       
+00015ca0: 2053 6565 2061 6c73 6f0a 2020 2020 2020   See also.      
+00015cb0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020    --------.     
+00015cc0: 2020 2066 6f72 6d61 745f 6461 7461 6172     format_dataar
+00015cd0: 7261 790a 2020 2020 2020 2020 2222 220a  ray.        """.
+00015ce0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00015cf0: 656c 662e 666f 726d 6174 5f64 6174 6161  elf.format_dataa
+00015d00: 7272 6179 280a 2020 2020 2020 2020 2020  rray(.          
+00015d10: 2020 6461 2c0a 2020 2020 2020 2020 2020    da,.          
+00015d20: 2020 6e61 6d65 3d6e 616d 652c 0a20 2020    name=name,.   
+00015d30: 2020 2020 2020 2020 2073 7065 6369 616c           special
+00015d40: 697a 653d 7370 6563 6961 6c69 7a65 2c0a  ize=specialize,.
+00015d50: 2020 2020 2020 2020 2020 2020 6c6f 633d              loc=
+00015d60: 6c6f 632c 0a20 2020 2020 2020 2020 2020  loc,.           
+00015d70: 2061 7474 7273 3d46 616c 7365 2c0a 2020   attrs=False,.  
+00015d80: 2020 2020 2020 2020 2020 7374 616e 6461            standa
+00015d90: 7264 697a 653d 7374 616e 6461 7264 697a  rdize=standardiz
+00015da0: 652c 0a20 2020 2020 2020 2020 2020 2072  e,.            r
+00015db0: 656e 616d 655f 6469 6d3d 7265 6e61 6d65  ename_dim=rename
+00015dc0: 5f64 696d 2c0a 2020 2020 2020 2020 2020  _dim,.          
+00015dd0: 2020 636f 7079 3d63 6f70 792c 0a20 2020    copy=copy,.   
+00015de0: 2020 2020 2020 2020 2061 6464 5f6c 6f63           add_loc
+00015df0: 5f74 6f5f 6e61 6d65 3d61 6464 5f6c 6f63  _to_name=add_loc
+00015e00: 5f74 6f5f 6e61 6d65 2c0a 2020 2020 2020  _to_name,.      
+00015e10: 2020 290a 0a0a 636c 6173 7320 4346 5661    )...class CFVa
+00015e20: 7253 7065 6373 285f 4346 4361 7453 7065  rSpecs(_CFCatSpe
+00015e30: 6373 5f29 3a0a 2020 2020 2222 2243 4620  cs_):.    """CF 
+00015e40: 7370 6563 6966 6963 6174 696f 6e20 666f  specification fo
+00015e50: 7220 6461 7461 5f76 6172 7322 2222 0a0a  r data_vars"""..
+00015e60: 2020 2020 6361 7465 676f 7279 203d 2022      category = "
+00015e70: 6461 7461 5f76 6172 7322 0a0a 0a63 6c61  data_vars"...cla
+00015e80: 7373 2043 4643 6f6f 7264 5370 6563 7328  ss CFCoordSpecs(
+00015e90: 5f43 4643 6174 5370 6563 735f 293a 0a20  _CFCatSpecs_):. 
+00015ea0: 2020 2022 2222 4346 2073 7065 6369 6669     """CF specifi
+00015eb0: 6361 7469 6f6e 2066 6f72 2063 6f6f 7264  cation for coord
+00015ec0: 7322 2222 0a0a 2020 2020 6361 7465 676f  s"""..    catego
+00015ed0: 7279 203d 2022 636f 6f72 6473 220a 0a20  ry = "coords".. 
+00015ee0: 2020 2064 6566 2067 6574 5f6c 6f63 5f6d     def get_loc_m
+00015ef0: 6170 7069 6e67 2873 656c 662c 2064 612c  apping(self, da,
+00015f00: 2063 665f 6e61 6d65 733d 4e6f 6e65 293a   cf_names=None):
+00015f10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00015f20: 7365 6c66 2e70 6172 656e 742e 6765 745f  self.parent.get_
+00015f30: 6c6f 635f 6d61 7070 696e 6728 6461 2c20  loc_mapping(da, 
+00015f40: 6366 5f6e 616d 6573 3d63 665f 6e61 6d65  cf_names=cf_name
+00015f50: 732c 2063 6174 6567 6f72 6965 733d 5b22  s, categories=["
+00015f60: 636f 6f72 6473 225d 290a 0a20 2020 2064  coords"])..    d
+00015f70: 6566 2067 6574 5f61 7869 7328 7365 6c66  ef get_axis(self
+00015f80: 2c20 636f 6f72 642c 206c 6f77 6572 3d46  , coord, lower=F
+00015f90: 616c 7365 293a 0a20 2020 2020 2020 2022  alse):.        "
+00015fa0: 2222 4765 7420 7468 6520 6469 6d65 6e73  ""Get the dimens
+00015fb0: 696f 6e20 7479 7065 2c20 6569 7468 6572  ion type, either
+00015fc0: 2066 726f 6d20 6178 6973 2061 7474 7220   from axis attr 
+00015fd0: 6f72 2066 726f 6d20 6d61 7463 6820 4366  or from match Cf
+00015fe0: 2063 6f6f 7264 0a0a 2020 2020 2020 2020   coord..        
+00015ff0: 2e2e 206e 6f74 653a 3a20 5468 6520 6060  .. note:: The ``
+00016000: 6178 6973 6060 2069 7320 7468 6520 7570  axis`` is the up
+00016010: 7065 7263 6173 6520 7665 7273 696f 6e20  percase version 
+00016020: 6f66 2074 6865 2060 6064 696d 5f74 7970  of the ``dim_typ
+00016030: 6560 600a 0a20 2020 2020 2020 2050 6172  e``..        Par
+00016040: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00016050: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00016060: 2020 2063 6f6f 7264 3a20 7861 7272 6179     coord: xarray
+00016070: 2e44 6174 6141 7272 6179 0a20 2020 2020  .DataArray.     
+00016080: 2020 206c 6f77 6572 3a20 626f 6f6c 0a20     lower: bool. 
+00016090: 2020 2020 2020 2020 2020 204c 6f77 6572             Lower
+000160a0: 2063 6173 653f 0a0a 2020 2020 2020 2020   case?..        
+000160b0: 5265 7475 726e 0a20 2020 2020 2020 202d  Return.        -
+000160c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7b22  -----.        {"
+000160d0: 7822 2c20 2279 222c 2022 7a22 2c20 2274  x", "y", "z", "t
+000160e0: 222c 2022 6622 7d2c 204e 6f6e 650a 0a20  ", "f"}, None.. 
+000160f0: 2020 2020 2020 2053 6565 2061 6c73 6f0a         See also.
+00016100: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00016110: 0a20 2020 2020 2020 2067 6574 5f64 696d  .        get_dim
+00016120: 5f74 7970 650a 2020 2020 2020 2020 6765  _type.        ge
+00016130: 745f 6469 6d5f 7479 7065 730a 2020 2020  t_dim_types.    
+00016140: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00016150: 6178 6973 203d 204e 6f6e 650a 2020 2020  axis = None.    
+00016160: 2020 2020 6966 2022 6178 6973 2220 696e      if "axis" in
+00016170: 2063 6f6f 7264 2e61 7474 7273 3a0a 2020   coord.attrs:.  
+00016180: 2020 2020 2020 2020 2020 6178 6973 203d            axis =
+00016190: 2063 6f6f 7264 2e61 7474 7273 5b22 6178   coord.attrs["ax
+000161a0: 6973 225d 0a20 2020 2020 2020 2065 6c73  is"].        els
+000161b0: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
+000161c0: 666e 616d 6520 3d20 7365 6c66 2e6d 6174  fname = self.mat
+000161d0: 6368 2863 6f6f 7264 290a 2020 2020 2020  ch(coord).      
+000161e0: 2020 2020 2020 6966 2063 666e 616d 653a        if cfname:
+000161f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016200: 2061 7869 7320 3d20 7365 6c66 5b63 666e   axis = self[cfn
+00016210: 616d 655d 5b22 6174 7472 7322 5d5b 2261  ame]["attrs"]["a
+00016220: 7869 7322 5d0a 2020 2020 2020 2020 6966  xis"].        if
+00016230: 2061 7869 7320 6973 206e 6f74 204e 6f6e   axis is not Non
+00016240: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00016250: 6620 6c6f 7765 723a 0a20 2020 2020 2020  f lower:.       
+00016260: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00016270: 6178 6973 2e6c 6f77 6572 2829 0a20 2020  axis.lower().   
+00016280: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00016290: 6178 6973 2e75 7070 6572 2829 0a0a 2020  axis.upper()..  
+000162a0: 2020 6465 6620 6765 745f 6469 6d5f 7479    def get_dim_ty
+000162b0: 7065 2873 656c 662c 2064 696d 2c20 6f62  pe(self, dim, ob
+000162c0: 6a3d 4e6f 6e65 2c20 6c6f 7765 723d 5472  j=None, lower=Tr
+000162d0: 7565 293a 0a20 2020 2020 2020 2022 2222  ue):.        """
+000162e0: 4765 7420 7468 6520 7479 7065 206f 6620  Get the type of 
+000162f0: 6120 6469 6d65 6e73 696f 6e0a 0a20 2020  a dimension..   
+00016300: 2020 2020 2054 6872 6565 2063 6173 6573       Three cases
+00016310: 3a0a 0a20 2020 2020 2020 202d 2054 6869  :..        - Thi
+00016320: 7320 6469 6d65 6e73 696f 6e20 6973 2072  s dimension is r
+00016330: 6567 6973 7465 7265 6420 696e 2043 4620  egistered in CF 
+00016340: 6469 6d73 2e0a 2020 2020 2020 2020 2d20  dims..        - 
+00016350: 6f62 6a20 6861 7320 6469 6d20 6173 2064  obj has dim as d
+00016360: 696d 2061 6e64 2068 6173 2061 6e20 6178  im and has an ax
+00016370: 6973 2061 7474 7269 6275 7465 2069 6e66  is attribute inf
+00016380: 6572 7265 6420 7769 7468 203a 6d65 7468  erred with :meth
+00016390: 3a60 6765 745f 6178 6973 602e 0a20 2020  :`get_axis`..   
+000163a0: 2020 2020 202d 206f 626a 2068 6173 2061       - obj has a
+000163b0: 2063 6f6f 7264 206e 616d 6564 2064 696d   coord named dim
+000163c0: 2077 6974 6820 616e 2061 7869 7320 6174   with an axis at
+000163d0: 7472 6962 7574 6520 696e 6665 7272 6564  tribute inferred
+000163e0: 2077 6974 6820 3a6d 6574 683a 6067 6574   with :meth:`get
+000163f0: 5f61 7869 7360 2e0a 0a20 2020 2020 2020  _axis`...       
+00016400: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00016410: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00016420: 2020 2020 2020 2064 696d 3a20 7374 720a         dim: str.
+00016430: 2020 2020 2020 2020 2020 2020 4469 6d65              Dime
+00016440: 6e73 696f 6e20 6e61 6d65 0a20 2020 2020  nsion name.     
+00016450: 2020 206f 626a 3a20 7861 7272 6179 2e44     obj: xarray.D
+00016460: 6174 6141 7272 6179 2c20 7861 7272 6179  ataArray, xarray
+00016470: 2e44 6174 6173 6574 0a20 2020 2020 2020  .Dataset.       
+00016480: 2020 2020 2044 6174 6120 6172 7261 7920       Data array 
+00016490: 7468 6174 2074 6865 2064 696d 656e 7369  that the dimensi
+000164a0: 6f6e 2062 656c 6f6e 6773 2074 6f2c 2074  on belongs to, t
+000164b0: 6f20 6865 6c70 2069 6e66 6572 7269 6e67  o help inferring
+000164c0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+000164d0: 2074 7970 650a 2020 2020 2020 2020 6c6f   type.        lo
+000164e0: 7765 723a 2062 6f6f 6c0a 2020 2020 2020  wer: bool.      
+000164f0: 2020 2020 2020 466f 7220 6c6f 7765 7220        For lower 
+00016500: 6361 7365 0a0a 2020 2020 2020 2020 5265  case..        Re
+00016510: 7475 726e 0a20 2020 2020 2020 202d 2d2d  turn.        ---
+00016520: 2d2d 2d0a 2020 2020 2020 2020 7374 722c  ---.        str,
+00016530: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00016540: 2020 4c65 7474 6572 2061 7320 6f6e 6520    Letter as one 
+00016550: 6f66 2078 2c20 792c 207a 2c20 7420 6f72  of x, y, z, t or
+00016560: 2066 2c20 6966 2066 6f75 6e64 2c20 656c   f, if found, el
+00016570: 7365 204e 6f6e 650a 0a20 2020 2020 2020  se None..       
+00016580: 2053 6565 2061 6c73 6f0a 2020 2020 2020   See also.      
+00016590: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020    --------.     
+000165a0: 2020 2067 6574 5f61 7869 730a 2020 2020     get_axis.    
+000165b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000165c0: 2320 5265 6d6f 7665 206c 6f63 6174 696f  # Remove locatio
+000165d0: 6e0a 2020 2020 2020 2020 6469 6d5f 6c6f  n.        dim_lo
+000165e0: 6320 3d20 6469 6d0a 2020 2020 2020 2020  c = dim.        
+000165f0: 6469 6d20 3d20 7365 6c66 2e73 676c 6f63  dim = self.sgloc
+00016600: 6174 6f72 2e70 6172 7365 5f61 7474 7228  ator.parse_attr(
+00016610: 276e 616d 6527 2c20 6469 6d29 5b30 5d0a  'name', dim)[0].
+00016620: 0a20 2020 2020 2020 2023 204c 6f6f 7020  .        # Loop 
+00016630: 6f6e 2074 7970 6573 0a20 2020 2020 2020  on types.       
+00016640: 2069 6620 6469 6d2e 6c6f 7765 7228 2920   if dim.lower() 
+00016650: 696e 2073 656c 662e 6469 6d73 3a0a 2020  in self.dims:.  
+00016660: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00016670: 2064 696d 2e6c 6f77 6572 2829 0a20 2020   dim.lower().   
+00016680: 2020 2020 2066 6f72 2064 696d 5f74 7970       for dim_typ
+00016690: 652c 2064 696d 7320 696e 2073 656c 662e  e, dims in self.
+000166a0: 6469 6d73 2e69 7465 6d73 2829 3a0a 2020  dims.items():.  
+000166b0: 2020 2020 2020 2020 2020 6966 2064 696d            if dim
+000166c0: 2e6c 6f77 6572 2829 2069 6e20 6469 6d73  .lower() in dims
+000166d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000166e0: 2020 7265 7475 726e 2064 696d 5f74 7970    return dim_typ
+000166f0: 650a 0a20 2020 2020 2020 2023 2043 6865  e..        # Che
+00016700: 636b 2069 6620 6120 636f 6f72 6469 6e61  ck if a coordina
+00016710: 7465 2068 6176 6520 7468 6520 7361 6d65  te have the same
+00016720: 206e 616d 6520 616e 6420 616e 2061 7869   name and an axi
+00016730: 7320 7479 7065 0a20 2020 2020 2020 2069  s type.        i
+00016740: 6620 6f62 6a20 6973 206e 6f74 204e 6f6e  f obj is not Non
+00016750: 653a 0a0a 2020 2020 2020 2020 2020 2020  e:..            
+00016760: 2320 4368 6563 6b20 6469 6d20 7661 6c69  # Check dim vali
+00016770: 6469 7479 0a20 2020 2020 2020 2020 2020  dity.           
+00016780: 2069 6620 6469 6d5f 6c6f 6320 6e6f 7420   if dim_loc not 
+00016790: 696e 206f 626a 2e64 696d 733a 0a20 2020  in obj.dims:.   
+000167a0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+000167b0: 7365 2058 6f61 4346 4572 726f 7228 6622  se XoaCFError(f"
+000167c0: 6469 6d65 6e73 696f 6e20 277b 6469 6d7d  dimension '{dim}
+000167d0: 2720 646f 6573 206e 6f74 2062 656c 6f6e  ' does not belon
+000167e0: 6720 746f 206f 626a 2229 0a0a 2020 2020  g to obj")..    
+000167f0: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
+00016800: 6178 6973 2066 726f 6d20 636f 6f72 6473  axis from coords
+00016810: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00016820: 6469 6d20 696e 206f 626a 2e69 6e64 6578  dim in obj.index
+00016830: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00016840: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00016850: 6765 745f 6178 6973 286f 626a 2e63 6f6f  get_axis(obj.coo
+00016860: 7264 735b 6469 6d5d 2c20 6c6f 7765 723d  rds[dim], lower=
+00016870: 5472 7565 290a 0a20 2020 2020 2020 2020  True)..         
+00016880: 2020 2023 2043 6865 636b 206f 626a 2061     # Check obj a
+00016890: 7869 7320 6974 7365 6c66 0a20 2020 2020  xis itself.     
+000168a0: 2020 2020 2020 2069 6620 6e6f 7420 6861         if not ha
+000168b0: 7361 7474 7228 6f62 6a2c 2022 6461 7461  sattr(obj, "data
+000168c0: 5f76 6172 7322 293a 0a20 2020 2020 2020  _vars"):.       
+000168d0: 2020 2020 2020 2020 2061 7869 7320 3d20           axis = 
+000168e0: 7365 6c66 2e67 6574 5f61 7869 7328 6f62  self.get_axis(ob
+000168f0: 6a2c 206c 6f77 6572 3d54 7275 6529 0a20  j, lower=True). 
+00016900: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00016910: 6620 6178 6973 3a0a 2020 2020 2020 2020  f axis:.        
+00016920: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00016930: 726e 2061 7869 730a 0a20 2020 2064 6566  rn axis..    def
+00016940: 2067 6574 5f64 696d 5f74 7970 6573 2873   get_dim_types(s
+00016950: 656c 662c 206f 626a 2c20 756e 6b6e 6f77  elf, obj, unknow
+00016960: 6e3d 4e6f 6e65 2c20 6173 6469 6374 3d46  n=None, asdict=F
+00016970: 616c 7365 293a 0a20 2020 2020 2020 2022  alse):.        "
+00016980: 2222 4765 7420 6120 7475 706c 6520 6f66  ""Get a tuple of
+00016990: 2074 6865 2064 696d 656e 7369 6f6e 2074   the dimension t
+000169a0: 7970 6573 206f 6620 616e 2061 7272 6179  ypes of an array
+000169b0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+000169c0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+000169d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000169e0: 6f62 6a3a 2078 6172 7261 792e 4461 7461  obj: xarray.Data
+000169f0: 4172 7261 792c 2074 7570 6c65 2873 7472  Array, tuple(str
+00016a00: 292c 2078 6172 7261 792e 4461 7461 7365  ), xarray.Datase
+00016a10: 740a 2020 2020 2020 2020 2020 2020 4461  t.            Da
+00016a20: 7461 2061 7272 6179 2c20 6461 7461 7365  ta array, datase
+00016a30: 7420 6f72 2074 7570 6c65 206f 6620 6469  t or tuple of di
+00016a40: 6d65 6e73 696f 6e73 0a20 2020 2020 2020  mensions.       
+00016a50: 2075 6e6b 6e6f 776e 3a0a 2020 2020 2020   unknown:.      
+00016a60: 2020 2020 2020 5661 6c75 6520 746f 2061        Value to a
+00016a70: 7373 6967 6e20 7768 656e 2074 7970 6520  ssign when type 
+00016a80: 6973 2075 6e6b 6e6f 776e 0a20 2020 2020  is unknown.     
+00016a90: 2020 2061 7364 6963 743a 2062 6f6f 6c0a     asdict: bool.
+00016aa0: 0a20 2020 2020 2020 2052 6574 7572 6e0a  .        Return.
+00016ab0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0a20          ------. 
+00016ac0: 2020 2020 2020 2074 7570 6c65 2c20 6469         tuple, di
+00016ad0: 6374 0a20 2020 2020 2020 2020 2020 2054  ct.            T
+00016ae0: 7570 6c65 206f 6620 6469 6d65 6e73 696f  uple of dimensio
+00016af0: 6e20 7479 7065 7320 616e 6420 6f66 206c  n types and of l
+00016b00: 656e 6774 6820 6060 6f62 6a2e 6e64 696d  ength ``obj.ndim
+00016b10: 6060 2e0a 2020 2020 2020 2020 2020 2020  ``..            
+00016b20: 4120 6469 6d65 6e73 696f 6e20 7479 7065  A dimension type
+00016b30: 2069 7320 6569 7468 6572 2061 206c 6574   is either a let
+00016b40: 7465 7220 6f72 2074 6865 2060 6075 6e6b  ter or the ``unk
+00016b50: 6f77 6e60 6020 7661 6c75 650a 2020 2020  own`` value.    
+00016b60: 2020 2020 2020 2020 7768 656e 2074 6865          when the
+00016b70: 2069 6e66 6572 656e 6365 206f 6620 7479   inference of ty
+00016b80: 7065 2068 6173 2066 6169 6c65 642e 0a20  pe has failed.. 
+00016b90: 2020 2020 2020 2020 2020 2049 6620 6060             If ``
+00016ba0: 6173 6469 6374 6060 2069 7320 5472 7565  asdict`` is True
+00016bb0: 2c20 6120 6469 6374 2069 7320 7265 7475  , a dict is retu
+00016bc0: 726e 6564 2069 6e73 7465 6164 2c0a 2020  rned instead,.  
+00016bd0: 2020 2020 2020 2020 2020 6060 2864 696d            ``(dim
+00016be0: 2c20 6469 6d5f 7479 7065 2960 6020 6173  , dim_type)`` as
+00016bf0: 206b 6579 2d76 616c 7565 2070 6169 7273   key-value pairs
+00016c00: 2e0a 0a20 2020 2020 2020 2053 6565 2061  ...        See a
+00016c10: 6c73 6f0a 2020 2020 2020 2020 2d2d 2d2d  lso.        ----
+00016c20: 2d2d 2d2d 0a20 2020 2020 2020 2067 6574  ----.        get
+00016c30: 5f64 696d 5f74 7970 650a 2020 2020 2020  _dim_type.      
+00016c40: 2020 2222 220a 2020 2020 2020 2020 6469    """.        di
+00016c50: 6d5f 7479 7065 7320 3d20 7b7d 0a20 2020  m_types = {}.   
+00016c60: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00016c70: 6365 286f 626a 2c20 7475 706c 6529 3a0a  ce(obj, tuple):.
+00016c80: 2020 2020 2020 2020 2020 2020 6469 6d73              dims
+00016c90: 203d 206f 626a 0a20 2020 2020 2020 2020   = obj.         
+00016ca0: 2020 206f 626a 203d 204e 6f6e 650a 2020     obj = None.  
+00016cb0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00016cc0: 2020 2020 2020 2020 6469 6d73 203d 206f          dims = o
+00016cd0: 626a 2e64 696d 730a 2020 2020 2020 2020  bj.dims.        
+00016ce0: 666f 7220 6469 6d20 696e 2064 696d 733a  for dim in dims:
+00016cf0: 0a20 2020 2020 2020 2020 2020 2064 696d  .            dim
+00016d00: 5f74 7970 6520 3d20 7365 6c66 2e67 6574  _type = self.get
+00016d10: 5f64 696d 5f74 7970 6528 6469 6d2c 206f  _dim_type(dim, o
+00016d20: 626a 3d6f 626a 290a 2020 2020 2020 2020  bj=obj).        
+00016d30: 2020 2020 6966 2064 696d 5f74 7970 6520      if dim_type 
+00016d40: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00016d50: 2020 2020 2020 2020 2064 696d 5f74 7970           dim_typ
+00016d60: 6520 3d20 756e 6b6e 6f77 6e0a 2020 2020  e = unknown.    
+00016d70: 2020 2020 2020 2020 6469 6d5f 7479 7065          dim_type
+00016d80: 735b 6469 6d5d 203d 2064 696d 5f74 7970  s[dim] = dim_typ
+00016d90: 650a 2020 2020 2020 2020 6966 2061 7364  e.        if asd
+00016da0: 6963 743a 0a20 2020 2020 2020 2020 2020  ict:.           
+00016db0: 2072 6574 7572 6e20 6469 6d5f 7479 7065   return dim_type
+00016dc0: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
+00016dd0: 2074 7570 6c65 2864 696d 5f74 7970 6573   tuple(dim_types
+00016de0: 2e76 616c 7565 7328 2929 0a0a 2020 2020  .values())..    
+00016df0: 4045 5252 4f52 532e 666f 726d 6174 5f6d  @ERRORS.format_m
+00016e00: 6574 686f 645f 646f 6373 7472 696e 670a  ethod_docstring.
+00016e10: 2020 2020 6465 6620 7365 6172 6368 5f64      def search_d
+00016e20: 696d 2873 656c 662c 206f 626a 2c20 6366  im(self, obj, cf
+00016e30: 5f61 7267 3d4e 6f6e 652c 206c 6f63 3d4e  _arg=None, loc=N
+00016e40: 6f6e 652c 2073 696e 676c 653d 5472 7565  one, single=True
+00016e50: 2c20 6572 726f 7273 3d22 6967 6e6f 7265  , errors="ignore
+00016e60: 2229 3a0a 2020 2020 2020 2020 2222 2253  "):.        """S
+00016e70: 6561 7263 6820 6120 6461 7461 6172 7261  earch a dataarra
+00016e80: 792f 6461 7461 7365 7420 666f 7220 6120  y/dataset for a 
+00016e90: 6469 6d65 6e73 696f 6e20 6e61 6d65 2061  dimension name a
+00016ea0: 6363 6f72 6469 6e67 2074 6f20 6974 7320  ccording to its 
+00016eb0: 6765 6e65 7269 6320 6e61 6d65 206f 7220  generic name or 
+00016ec0: 7479 7065 0a0a 2020 2020 2020 2020 4669  type..        Fi
+00016ed0: 7273 742c 2073 6361 6e20 7468 6520 6469  rst, scan the di
+00016ee0: 6d65 6e73 696f 6e20 6e61 6d65 732e 0a20  mension names.. 
+00016ef0: 2020 2020 2020 2054 6865 6e2c 206c 6f6f         Then, loo
+00016f00: 6b20 666f 7220 636f 6f72 6469 6e61 7465  k for coordinate
+00016f10: 733a 2065 6974 6865 7220 6974 2068 6173  s: either it has
+00016f20: 2061 6e20 2761 7869 7327 2061 7474 7269   an 'axis' attri
+00016f30: 6275 7465 2c0a 2020 2020 2020 2020 6f72  bute,.        or
+00016f40: 2069 7420 6120 6b6e 6f77 6e20 4346 2063   it a known CF c
+00016f50: 6f6f 7264 696e 6174 652e 0a0a 2020 2020  oordinate...    
+00016f60: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00016f70: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00016f80: 2d0a 2020 2020 2020 2020 6f62 6a3a 2078  -.        obj: x
+00016f90: 6172 7261 792e 4461 7461 4172 7261 792c  array.DataArray,
+00016fa0: 2078 6172 7261 792e 4461 7461 7365 740a   xarray.Dataset.
+00016fb0: 2020 2020 2020 2020 2020 2020 436f 6f72              Coor
+00016fc0: 6469 6e61 7465 206f 7220 6461 7461 2061  dinate or data a
+00016fd0: 7272 6179 0a20 2020 2020 2020 2063 665f  rray.        cf_
+00016fe0: 6172 673a 2073 7472 2c20 7b7b 2278 222c  arg: str, {{"x",
+00016ff0: 2022 7922 2c20 227a 222c 2022 7422 2c20   "y", "z", "t", 
+00017000: 2266 227d 7d2c 204e 6f6e 650a 2020 2020  "f"}}, None.    
+00017010: 2020 2020 2020 2020 4f6e 652d 6c65 7474          One-lett
+00017020: 6572 2064 696d 656e 7369 6f6e 2074 7970  er dimension typ
+00017030: 6520 6f72 2067 656e 6572 6963 2043 4620  e or generic CF 
+00017040: 6469 6d20 6e61 6d65 2e0a 2020 2020 2020  dim name..      
+00017050: 2020 2020 2020 5768 656e 2073 6574 2074        When set t
+00017060: 6f20 4e6f 6e65 2c20 646d 656e 7369 6f6e  o None, dmension
+00017070: 2074 7970 6520 6973 2069 6e66 6572 7265   type is inferre
+00017080: 6420 7769 7468 203a 6d65 7468 3a60 6765  d with :meth:`ge
+00017090: 745f 6178 6973 600a 2020 2020 2020 2020  t_axis`.        
+000170a0: 2020 2020 6170 706c 6965 6420 746f 2060      applied to `
+000170b0: 6f62 6a60 0a20 2020 2020 2020 206c 6f63  obj`.        loc
+000170c0: 3a20 2261 6e79 222c 206c 6574 7465 720a  : "any", letter.
+000170d0: 2020 2020 2020 2020 2020 2020 5374 6167              Stag
+000170e0: 6765 7265 6420 6772 6964 206c 6f63 6174  gered grid locat
+000170f0: 696f 6e0a 2020 2020 2020 2020 7369 6e67  ion.        sing
+00017100: 6c65 3a20 626f 6f6c 0a20 2020 2020 2020  le: bool.       
+00017110: 2020 2020 2049 6620 5472 7565 2c20 7265       If True, re
+00017120: 7475 726e 2074 6865 2066 6972 7374 2069  turn the first i
+00017130: 7465 6d20 666f 756e 6420 6f72 204e 6f6e  tem found or Non
+00017140: 652e 0a20 2020 2020 2020 2020 2020 2049  e..            I
+00017150: 6620 4661 6c73 652c 2072 6574 7572 6e20  f False, return 
+00017160: 6120 706f 7373 6962 6c65 2065 6d70 7479  a possible empty
+00017170: 206c 6973 7420 6f66 2066 6f75 6e64 2069   list of found i
+00017180: 7465 6d73 2e0a 2020 2020 2020 2020 7b65  tems..        {e
+00017190: 7272 6f72 737d 0a0a 2020 2020 2020 2020  rrors}..        
+000171a0: 5265 7475 726e 0a20 2020 2020 2020 202d  Return.        -
+000171b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7374  -----.        st
+000171c0: 722c 2064 6963 742c 204e 6f6e 650a 2020  r, dict, None.  
+000171d0: 2020 2020 2020 2020 2020 4469 6d20 6e61            Dim na
+000171e0: 6d65 204f 522c 2064 6963 7420 7769 7468  me OR, dict with
+000171f0: 2064 696d 2c20 7479 7065 2061 6e64 2063   dim, type and c
+00017200: 665f 6e61 6d65 206b 6579 7320 6966 2064  f_name keys if d
+00017210: 696d 5f74 7970 6520 6973 204e 6f6e 652e  im_type is None.
+00017220: 0a20 2020 2020 2020 2020 2020 204e 6f6e  .            Non
+00017230: 6520 6966 206e 6f74 6869 6e67 2066 6f75  e if nothing fou
+00017240: 6e64 2e0a 2020 2020 2020 2020 2222 220a  nd..        """.
+00017250: 2020 2020 2020 2020 2320 4578 706c 6963          # Explic
+00017260: 6974 3f0a 2020 2020 2020 2020 6366 5f6e  it?.        cf_n
+00017270: 616d 6520 3d20 6469 6d5f 7479 7065 203d  ame = dim_type =
+00017280: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
+00017290: 2063 665f 6172 673a 0a20 2020 2020 2020   cf_arg:.       
+000172a0: 2020 2020 2023 2069 6620 6366 5f61 7267       # if cf_arg
+000172b0: 2069 6e20 6f62 6a2e 6469 6d73 3a0a 2020   in obj.dims:.  
+000172c0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+000172d0: 7265 7475 726e 2063 665f 6172 670a 2020  return cf_arg.  
+000172e0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+000172f0: 2863 665f 6172 6729 203d 3d20 313a 0a20  (cf_arg) == 1:. 
+00017300: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00017310: 696d 5f74 7970 6520 3d20 6366 5f61 7267  im_type = cf_arg
+00017320: 2e6c 6f77 6572 2829 0a20 2020 2020 2020  .lower().       
+00017330: 2020 2020 2020 2020 2069 6620 6366 5f61           if cf_a
+00017340: 7267 2069 6e20 7365 6c66 2e6e 616d 6573  rg in self.names
+00017350: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017360: 2020 2020 2020 6366 5f6e 616d 6520 3d20        cf_name = 
+00017370: 6366 5f61 7267 0a20 2020 2020 2020 2020  cf_arg.         
+00017380: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00017390: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000173a0: 7365 6c66 2e5f 6173 7365 7274 5f6b 6e6f  self._assert_kno
+000173b0: 776e 5f28 6366 5f61 7267 2c20 6572 726f  wn_(cf_arg, erro
+000173c0: 7273 3d65 7272 6f72 7329 3a0a 2020 2020  rs=errors):.    
+000173d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173e0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+000173f0: 2020 2020 2020 2063 665f 6e61 6d65 203d         cf_name =
+00017400: 2063 665f 6172 670a 2020 2020 2020 2020   cf_arg.        
+00017410: 6973 6473 203d 2068 6173 6174 7472 286f  isds = hasattr(o
+00017420: 626a 2c20 2264 6174 615f 7661 7273 2229  bj, "data_vars")
+00017430: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00017440: 6973 6473 2061 6e64 2064 696d 5f74 7970  isds and dim_typ
+00017450: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+00017460: 2020 2020 2020 2064 696d 5f74 7970 6520         dim_type 
+00017470: 3d20 7365 6c66 2e67 6574 5f61 7869 7328  = self.get_axis(
+00017480: 6f62 6a2c 206c 6f77 6572 3d54 7275 6529  obj, lower=True)
+00017490: 0a20 2020 2020 2020 206c 6f63 203d 2073  .        loc = s
+000174a0: 656c 662e 7367 6c6f 6361 746f 722e 7061  elf.sglocator.pa
+000174b0: 7273 655f 6c6f 635f 6172 6728 6c6f 6329  rse_loc_arg(loc)
+000174c0: 0a0a 2020 2020 2020 2020 2320 4c6f 6f70  ..        # Loop
+000174d0: 206f 6e20 6469 6d73 0a20 2020 2020 2020   on dims.       
+000174e0: 2066 6f75 6e64 203d 205b 5d0a 2020 2020   found = [].    
+000174f0: 2020 2020 666f 7220 6469 6d20 696e 206f      for dim in o
+00017500: 626a 2e64 696d 733a 0a0a 2020 2020 2020  bj.dims:..      
+00017510: 2020 2020 2020 2320 4669 6c74 6572 2d6f        # Filter-o
+00017520: 7574 2062 7920 6c6f 630a 2020 2020 2020  ut by loc.      
+00017530: 2020 2020 2020 706e 616d 652c 2070 6c6f        pname, plo
+00017540: 6320 3d20 7365 6c66 2e73 676c 6f63 6174  c = self.sglocat
+00017550: 6f72 2e70 6172 7365 5f61 7474 7228 276e  or.parse_attr('n
+00017560: 616d 6527 2c20 6469 6d29 0a20 2020 2020  ame', dim).     
+00017570: 2020 2020 2020 2070 6c6f 6320 3d20 7365         ploc = se
+00017580: 6c66 2e73 676c 6f63 6174 6f72 2e70 6172  lf.sglocator.par
+00017590: 7365 5f6c 6f63 5f61 7267 2870 6c6f 6329  se_loc_arg(ploc)
+000175a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000175b0: 6c6f 6320 6973 206e 6f74 204e 6f6e 6520  loc is not None 
+000175c0: 616e 6420 6c6f 6320 213d 2070 6c6f 633a  and loc != ploc:
+000175d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000175e0: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
+000175f0: 2020 2020 2020 2023 2046 726f 6d20 6765         # From ge
+00017600: 6e65 7269 6320 6e61 6d65 0a20 2020 2020  neric name.     
+00017610: 2020 2020 2020 2069 6620 6469 6d20 696e         if dim in
+00017620: 206f 626a 2e63 6f6f 7264 733a 0a20 2020   obj.coords:.   
+00017630: 2020 2020 2020 2020 2020 2020 2074 6869               thi
+00017640: 735f 6366 5f6e 616d 6520 3d20 7365 6c66  s_cf_name = self
+00017650: 2e6d 6174 6368 286f 626a 2e63 6f6f 7264  .match(obj.coord
+00017660: 735b 6469 6d5d 290a 2020 2020 2020 2020  s[dim]).        
+00017670: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00017680: 2020 2020 2020 2020 2020 7468 6973 5f63            this_c
+00017690: 665f 6e61 6d65 203d 2073 656c 662e 6d61  f_name = self.ma
+000176a0: 7463 685f 6672 6f6d 5f6e 616d 6528 6469  tch_from_name(di
+000176b0: 6d29 0a20 2020 2020 2020 2020 2020 2069  m).            i
+000176c0: 6620 6366 5f6e 616d 653a 0a20 2020 2020  f cf_name:.     
+000176d0: 2020 2020 2020 2020 2020 2069 6620 7468             if th
+000176e0: 6973 5f63 665f 6e61 6d65 203d 3d20 6366  is_cf_name == cf
+000176f0: 5f6e 616d 653a 0a20 2020 2020 2020 2020  _name:.         
+00017700: 2020 2020 2020 2020 2020 2066 6f75 6e64             found
+00017710: 2e61 7070 656e 6428 6469 6d29 0a20 2020  .append(dim).   
+00017720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017730: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+00017740: 2020 2020 2020 2020 2020 6966 2064 696d            if dim
+00017750: 5f74 7970 6520 6973 204e 6f6e 653a 2020  _type is None:  
+00017760: 2320 6b65 6570 2073 6561 7263 6869 6e67  # keep searching
+00017770: 2069 6620 6469 6d5f 7479 7065 2069 7320   if dim_type is 
+00017780: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+00017790: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000177a0: 7469 6e75 650a 0a20 2020 2020 2020 2020  tinue..         
+000177b0: 2020 2023 2046 726f 6d20 6469 6d65 6e73     # From dimens
+000177c0: 696f 6e20 7479 7065 0a20 2020 2020 2020  ion type.       
+000177d0: 2020 2020 2074 6869 735f 6469 6d5f 7479       this_dim_ty
+000177e0: 7065 203d 2073 656c 662e 6765 745f 6469  pe = self.get_di
+000177f0: 6d5f 7479 7065 2864 696d 2c20 6f62 6a3d  m_type(dim, obj=
+00017800: 6f62 6a29 0a20 2020 2020 2020 2020 2020  obj).           
+00017810: 206f 7574 203d 207b 2264 696d 223a 2064   out = {"dim": d
+00017820: 696d 2c20 2274 7970 6522 3a20 7468 6973  im, "type": this
+00017830: 5f64 696d 5f74 7970 652c 2022 6366 5f6e  _dim_type, "cf_n
+00017840: 616d 6522 3a20 7468 6973 5f63 665f 6e61  ame": this_cf_na
+00017850: 6d65 7d0a 2020 2020 2020 2020 2020 2020  me}.            
+00017860: 6966 2074 6869 735f 6469 6d5f 7479 7065  if this_dim_type
+00017870: 2061 6e64 2074 6869 735f 6469 6d5f 7479   and this_dim_ty
+00017880: 7065 203d 3d20 6469 6d5f 7479 7065 3a0a  pe == dim_type:.
+00017890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178a0: 6966 2063 665f 6172 673a 0a20 2020 2020  if cf_arg:.     
+000178b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000178c0: 6f75 6e64 2e61 7070 656e 6428 6469 6d29  ound.append(dim)
+000178d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000178e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000178f0: 2020 2020 2020 2020 2020 2066 6f75 6e64             found
+00017900: 2e61 7070 656e 6428 6f75 7429 0a0a 2020  .append(out)..  
+00017910: 2020 2020 2020 2320 4e6f 7420 666f 756e        # Not foun
+00017920: 6420 6275 7420 6f6e 6c79 2031 6420 616e  d but only 1d an
+00017930: 6420 6e6f 2064 696d 5f74 7970 6520 7370  d no dim_type sp
+00017940: 6563 6966 6965 640a 2020 2020 2020 2020  ecified.        
+00017950: 6966 206e 6f74 2066 6f75 6e64 2061 6e64  if not found and
+00017960: 206c 656e 286f 626a 2e64 696d 7329 203d   len(obj.dims) =
+00017970: 3d20 3120 616e 6420 6e6f 7420 6366 5f61  = 1 and not cf_a
+00017980: 7267 3a0a 2020 2020 2020 2020 2020 2020  rg:.            
+00017990: 2320 4649 584d 453a 206c 6f6f 7020 6f6e  # FIXME: loop on
+000179a0: 2063 6f6f 7264 696e 6174 6573 3f0a 2020   coordinates?.  
+000179b0: 2020 2020 2020 2020 2020 666f 756e 642e            found.
+000179c0: 6170 7065 6e64 286f 7574 290a 0a20 2020  append(out)..   
+000179d0: 2020 2020 2023 2053 696e 676c 653f 0a20       # Single?. 
+000179e0: 2020 2020 2020 2065 7272 6f72 7320 3d20         errors = 
+000179f0: 4552 524f 5253 5b65 7272 6f72 735d 0a20  ERRORS[errors]. 
+00017a00: 2020 2020 2020 2069 6620 7369 6e67 6c65         if single
+00017a10: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00017a20: 206c 656e 2866 6f75 6e64 2920 3d3d 2031   len(found) == 1
+00017a30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017a40: 2020 7265 7475 726e 2066 6f75 6e64 5b30    return found[0
+00017a50: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
+00017a60: 206c 656e 2866 6f75 6e64 2920 3e20 313a   len(found) > 1:
+00017a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017a80: 2069 6620 6572 726f 7273 2021 3d20 2269   if errors != "i
+00017a90: 676e 6f72 6522 3a0a 2020 2020 2020 2020  gnore":.        
+00017aa0: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
+00017ab0: 3d20 6622 4d75 6c74 6970 6c65 2063 616e  = f"Multiple can
+00017ac0: 6469 6461 7465 7320 6469 6d65 6e73 696f  didates dimensio
+00017ad0: 6e73 206d 6174 6368 696e 673a 207b 6366  ns matching: {cf
+00017ae0: 5f61 7267 7d22 0a20 2020 2020 2020 2020  _arg}".         
+00017af0: 2020 2020 2020 2020 2020 2069 6620 6572             if er
+00017b00: 726f 7273 203d 3d20 2272 6169 7365 223a  rors == "raise":
+00017b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017b20: 2020 2020 2020 2020 2072 6169 7365 2058           raise X
+00017b30: 6f61 4346 4572 726f 7228 6d73 6729 0a20  oaCFError(msg). 
+00017b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b50: 2020 2078 6f61 5f77 6172 6e28 6d73 6729     xoa_warn(msg)
+00017b60: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00017b70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00017b80: 6e20 666f 756e 640a 0a20 2020 2020 2020  n found..       
+00017b90: 2023 2046 6169 6c65 640a 2020 2020 2020   # Failed.      
+00017ba0: 2020 6966 2065 7272 6f72 7320 213d 2022    if errors != "
+00017bb0: 6967 6e6f 7265 223a 0a20 2020 2020 2020  ignore":.       
+00017bc0: 2020 2020 206d 7367 203d 2066 224e 6f20       msg = f"No 
+00017bd0: 6469 6d65 6e73 696f 6e20 666f 756e 6420  dimension found 
+00017be0: 696e 2064 6174 6161 7272 6179 206d 6174  in dataarray mat
+00017bf0: 6368 696e 673a 207b 6366 5f61 7267 7d22  ching: {cf_arg}"
+00017c00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017c10: 6572 726f 7273 203d 3d20 2272 6169 7365  errors == "raise
+00017c20: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00017c30: 2020 2072 6169 7365 2058 6f61 4346 4572     raise XoaCFEr
+00017c40: 726f 7228 6d73 6729 0a20 2020 2020 2020  ror(msg).       
+00017c50: 2020 2020 2078 6f61 5f77 6172 6e28 6d73       xoa_warn(ms
+00017c60: 6729 0a0a 2020 2020 4045 5252 4f52 532e  g)..    @ERRORS.
+00017c70: 666f 726d 6174 5f6d 6574 686f 645f 646f  format_method_do
+00017c80: 6373 7472 696e 670a 2020 2020 6465 6620  cstring.    def 
+00017c90: 7365 6172 6368 5f66 726f 6d5f 6469 6d28  search_from_dim(
+00017ca0: 7365 6c66 2c20 6f62 6a2c 2064 696d 2c20  self, obj, dim, 
+00017cb0: 6572 726f 7273 3d22 6967 6e6f 7265 2229  errors="ignore")
+00017cc0: 3a0a 2020 2020 2020 2020 2222 2253 6561  :.        """Sea
+00017cd0: 7263 6820 6120 6461 7461 6172 7261 792f  rch a dataarray/
+00017ce0: 6461 7461 7365 7420 666f 7220 6120 636f  dataset for a co
+00017cf0: 6f72 6469 6e61 7465 2066 726f 6d20 6120  ordinate from a 
+00017d00: 6469 6d65 6e73 696f 6e20 6e61 6d65 0a0a  dimension name..
+00017d10: 2020 2020 2020 2020 4974 2066 6972 7374          It first
+00017d20: 2073 6561 7263 6865 7320 666f 7220 6120   searches for a 
+00017d30: 636f 6f72 6469 6e61 7465 2077 6974 6820  coordinate with 
+00017d40: 6120 6469 6666 6572 656e 7420 6e61 6d65  a different name
+00017d50: 2061 6e64 2074 6861 7420 6973 0a20 2020   and that is.   
+00017d60: 2020 2020 2074 6865 206f 6e6c 7920 6f6e       the only on
+00017d70: 6520 6861 7669 6e67 2074 6869 7320 6469  e having this di
+00017d80: 6d65 6e73 696f 6e2e 0a20 2020 2020 2020  mension..       
+00017d90: 2054 6865 6e20 6368 6563 6b20 6966 2069   Then check if i
+00017da0: 7420 6973 2061 6e20 696e 6465 782e 0a20  t is an index.. 
+00017db0: 2020 2020 2020 2054 6865 6e20 6c6f 6f6b         Then look
+00017dc0: 2066 6f72 2063 6f6f 7264 696e 6174 6573   for coordinates
+00017dd0: 2077 6974 6820 7468 6520 7361 6d65 2074   with the same t
+00017de0: 7970 6520 6c69 6b65 2078 2c20 792c 2065  ype like x, y, e
+00017df0: 7463 2e0a 0a20 2020 2020 2020 2050 6172  tc...        Par
+00017e00: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00017e10: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00017e20: 2020 206f 626a 3a20 7861 7272 6179 2e44     obj: xarray.D
+00017e30: 6174 6141 7272 6179 2c20 7861 7272 6179  ataArray, xarray
+00017e40: 2e44 6174 6173 6574 0a20 2020 2020 2020  .Dataset.       
+00017e50: 2064 696d 3a20 7374 720a 2020 2020 2020   dim: str.      
+00017e60: 2020 7b65 7272 6f72 737d 0a0a 2020 2020    {errors}..    
+00017e70: 2020 2020 5265 7475 726e 0a20 2020 2020      Return.     
+00017e80: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
+00017e90: 2020 7861 7272 6179 2e44 6174 6141 7272    xarray.DataArr
+00017ea0: 6179 2c20 4e6f 6e65 0a20 2020 2020 2020  ay, None.       
+00017eb0: 2020 2020 2041 6e20 636f 6f72 6469 6e61       An coordina
+00017ec0: 7465 2061 7272 6179 206f 7220 4e6f 6e65  te array or None
+00017ed0: 0a0a 2020 2020 2020 2020 5365 6520 616c  ..        See al
+00017ee0: 736f 0a20 2020 2020 2020 202d 2d2d 2d2d  so.        -----
+00017ef0: 2d2d 2d0a 2020 2020 2020 2020 6765 745f  ---.        get_
+00017f00: 6178 6973 0a20 2020 2020 2020 2067 6574  axis.        get
+00017f10: 5f64 696d 5f74 7970 650a 2020 2020 2020  _dim_type.      
+00017f20: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00017f30: 2064 696d 206e 6f74 2069 6e20 6f62 6a2e   dim not in obj.
+00017f40: 6469 6d73 3a0a 2020 2020 2020 2020 2020  dims:.          
+00017f50: 2020 7261 6973 6520 586f 6145 7272 6f72    raise XoaError
+00017f60: 2866 2249 6e76 616c 6964 2064 696d 656e  (f"Invalid dimen
+00017f70: 7369 6f6e 3a20 7b64 696d 7d22 290a 0a20  sion: {dim}").. 
+00017f80: 2020 2020 2020 2023 2041 2063 6f6f 7264         # A coord
+00017f90: 2077 6974 6820 6120 6469 6666 6572 656e   with a differen
+00017fa0: 7420 6e61 6d65 0a20 2020 2020 2020 2063  t name.        c
+00017fb0: 6f6f 7264 7320 3d20 5b63 6f6f 7264 2066  oords = [coord f
+00017fc0: 6f72 206e 616d 652c 2063 6f6f 7264 2069  or name, coord i
+00017fd0: 6e20 6f62 6a2e 636f 6f72 6473 2e69 7465  n obj.coords.ite
+00017fe0: 6d73 2829 2069 6620 6e61 6d65 2021 3d20  ms() if name != 
+00017ff0: 6469 6d20 616e 6420 6469 6d20 696e 2063  dim and dim in c
+00018000: 6f6f 7264 2e64 696d 735d 0a20 2020 2020  oord.dims].     
+00018010: 2020 2069 6620 6c65 6e28 636f 6f72 6473     if len(coords
+00018020: 2920 3d3d 2031 3a0a 2020 2020 2020 2020  ) == 1:.        
+00018030: 2020 2020 7265 7475 726e 2063 6f6f 7264      return coord
+00018040: 735b 305d 0a0a 2020 2020 2020 2020 2320  s[0]..        # 
+00018050: 4173 2061 6e20 696e 6465 780a 2020 2020  As an index.    
+00018060: 2020 2020 6966 2064 696d 2069 6e20 6f62      if dim in ob
+00018070: 6a2e 696e 6465 7865 733a 0a20 2020 2020  j.indexes:.     
+00018080: 2020 2020 2020 2072 6574 7572 6e20 6f62         return ob
+00018090: 6a2e 636f 6f72 6473 5b64 696d 5d0a 0a20  j.coords[dim].. 
+000180a0: 2020 2020 2020 2023 2047 6574 2064 696d         # Get dim
+000180b0: 5f74 7970 6520 6672 6f6d 206b 6e6f 776e  _type from known
+000180c0: 2064 696d 206e 616d 650a 2020 2020 2020   dim name.      
+000180d0: 2020 6469 6d5f 7479 7065 203d 2073 656c    dim_type = sel
+000180e0: 662e 6765 745f 6469 6d5f 7479 7065 2864  f.get_dim_type(d
+000180f0: 696d 2c20 6f62 6a2c 206c 6f77 6572 3d54  im, obj, lower=T
+00018100: 7275 6529 0a0a 2020 2020 2020 2020 2320  rue)..        # 
+00018110: 536f 2077 6520 6361 6e20 646f 2073 6f6d  So we can do som
+00018120: 6574 6869 6e67 0a20 2020 2020 2020 2064  ething.        d
+00018130: 6566 2067 6574 5f6e 6469 6d28 6f29 3a0a  ef get_ndim(o):.
+00018140: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00018150: 726e 206c 656e 286f 2e64 696d 7329 0a0a  rn len(o.dims)..
+00018160: 2020 2020 2020 2020 6966 2064 696d 5f74          if dim_t
+00018170: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
+00018180: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00018190: 4c6f 6f6b 2066 6f72 2061 2063 6f6f 7264  Look for a coord
+000181a0: 696e 6174 6520 7769 7468 2074 6869 7320  inate with this 
+000181b0: 6469 6d5f 7479 7065 0a20 2020 2020 2020  dim_type.       
+000181c0: 2020 2020 2023 2020 7374 6172 7469 6e67       #  starting
+000181d0: 2066 726f 6d20 636f 6f72 6469 6e61 7465   from coordinate
+000181e0: 7320 7769 7468 2061 2068 6967 6865 7220  s with a higher 
+000181f0: 6e75 6d62 6572 206f 6620 6469 6d65 6e73  number of dimens
+00018200: 696f 6e73 0a20 2020 2020 2020 2020 2020  ions.           
+00018210: 2023 2020 6c69 6b65 2064 6570 7468 2074   #  like depth t
+00018220: 6861 7420 6861 7665 206d 6f72 6520 6469  hat have more di
+00018230: 6d73 2074 6861 6e20 6c65 7665 6c0a 2020  ms than level.  
+00018240: 2020 2020 2020 2020 2020 666f 7220 636f            for co
+00018250: 6f72 6420 696e 2073 6f72 7465 6428 6f62  ord in sorted(ob
+00018260: 6a2e 636f 6f72 6473 2e76 616c 7565 7328  j.coords.values(
+00018270: 292c 206b 6579 3d67 6574 5f6e 6469 6d2c  ), key=get_ndim,
+00018280: 2072 6576 6572 7365 3d54 7275 6529 3a0a   reverse=True):.
+00018290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182a0: 6966 2064 696d 2069 6e20 636f 6f72 642e  if dim in coord.
+000182b0: 6469 6d73 3a0a 2020 2020 2020 2020 2020  dims:.          
+000182c0: 2020 2020 2020 2020 2020 636f 6f72 645f            coord_
+000182d0: 6469 6d5f 7479 7065 203d 2073 656c 662e  dim_type = self.
+000182e0: 6765 745f 6178 6973 2863 6f6f 7264 2c20  get_axis(coord, 
+000182f0: 6c6f 7765 723d 5472 7565 290a 2020 2020  lower=True).    
 00018300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018310: 2020 7265 7475 726e 2063 6f6f 7264 0a0a    return coord..
-00018320: 2020 2020 2020 2020 2320 4e6f 7468 696e          # Nothin
-00018330: 6720 666f 756e 640a 2020 2020 2020 2020  g found.        
-00018340: 6572 726f 7273 203d 2045 5252 4f52 535b  errors = ERRORS[
-00018350: 6572 726f 7273 5d0a 2020 2020 2020 2020  errors].        
-00018360: 6966 2065 7272 6f72 7320 213d 2022 6967  if errors != "ig
-00018370: 6e6f 7265 223a 0a20 2020 2020 2020 2020  nore":.         
-00018380: 2020 206d 7367 203d 2066 224e 6f20 6461     msg = f"No da
-00018390: 7461 6172 7261 7920 636f 6f72 6420 666f  taarray coord fo
-000183a0: 756e 6420 6672 6f6d 2064 696d 3a20 7b64  und from dim: {d
-000183b0: 696d 7d22 0a20 2020 2020 2020 2020 2020  im}".           
-000183c0: 2069 6620 6572 726f 7273 203d 3d20 2272   if errors == "r
-000183d0: 6169 7365 223a 0a20 2020 2020 2020 2020  aise":.         
-000183e0: 2020 2020 2020 2072 6169 7365 2058 6f61         raise Xoa
-000183f0: 4346 4572 726f 7228 6d73 6729 0a20 2020  CFError(msg).   
-00018400: 2020 2020 2020 2020 2078 6f61 5f77 6172           xoa_war
-00018410: 6e28 6d73 6729 0a0a 2020 2020 4045 5252  n(msg)..    @ERR
-00018420: 4f52 532e 666f 726d 6174 5f6d 6574 686f  ORS.format_metho
-00018430: 645f 646f 6373 7472 696e 670a 2020 2020  d_docstring.    
-00018440: 6465 6620 6765 745f 6469 6d73 280a 2020  def get_dims(.  
-00018450: 2020 2020 2020 7365 6c66 2c20 6f62 6a2c        self, obj,
-00018460: 2063 665f 6172 6773 2c20 616c 6c6f 775f   cf_args, allow_
-00018470: 706f 7369 7469 6f6e 616c 3d46 616c 7365  positional=False
-00018480: 2c20 706f 7369 7469 6f6e 733d 2774 7a79  , positions='tzy
-00018490: 7827 2c20 7369 6e67 6c65 3d54 7275 652c  x', single=True,
-000184a0: 2065 7272 6f72 733d 2277 6172 6e22 0a20   errors="warn". 
-000184b0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-000184c0: 2247 6574 2074 6865 2064 6174 6120 6172  "Get the data ar
-000184d0: 7261 7920 6469 6d65 6e73 696f 6e73 206e  ray dimensions n
-000184e0: 616d 6573 2066 726f 6d20 7468 6569 7220  ames from their 
-000184f0: 7479 7065 206f 7220 6765 6e65 7269 6320  type or generic 
-00018500: 4346 206e 616d 650a 0a20 2020 2020 2020  CF name..       
-00018510: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00018520: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00018530: 2020 2020 2020 206f 626a 3a20 7861 7272         obj: xarr
-00018540: 6179 2e44 6174 6141 7272 6179 2c20 7861  ay.DataArray, xa
-00018550: 7272 6179 2e44 6174 6173 6574 0a20 2020  rray.Dataset.   
-00018560: 2020 2020 2020 2020 2041 7272 6179 2f64           Array/d
-00018570: 6174 6173 6574 2074 6f20 7363 616e 0a20  ataset to scan. 
-00018580: 2020 2020 2020 2063 665f 6172 6773 3a20         cf_args: 
-00018590: 6c69 7374 0a20 2020 2020 2020 2020 2020  list.           
-000185a0: 204c 6973 7420 6f66 206c 6574 7465 7273   List of letters
-000185b0: 2061 6d6f 6e67 2022 7822 2c20 2279 222c   among "x", "y",
-000185c0: 2022 7a22 2c20 2274 2220 616e 6420 2266   "z", "t" and "f
-000185d0: 222c 0a20 2020 2020 2020 2020 2020 206f  ",.            o
-000185e0: 7220 6765 6e65 7269 6320 6e61 6d65 732e  r generic names.
-000185f0: 0a20 2020 2020 2020 2061 6c6c 6f77 5f70  .        allow_p
-00018600: 6f73 6974 696f 6e61 6c3a 2062 6f6f 6c0a  ositional: bool.
-00018610: 2020 2020 2020 2020 2020 2020 4661 6c6c              Fall
-00018620: 2062 6163 6b20 746f 2070 6f73 6974 696f   back to positio
-00018630: 6e61 6c20 6469 6d65 6e73 696f 6e20 6f66  nal dimension of
-00018640: 2074 7970 6573 2069 7320 756e 6b6f 776e   types is unkown
-00018650: 2e0a 2020 2020 2020 2020 706f 7369 7469  ..        positi
-00018660: 6f6e 733a 2073 7472 0a20 2020 2020 2020  ons: str.       
-00018670: 2020 2020 2044 6566 6175 6c74 2065 7870       Default exp
-00018680: 6563 7465 6420 706f 7369 7469 6f6e 206f  ected position o
-00018690: 6620 6469 6d20 7065 7220 7479 7065 2069  f dim per type i
-000186a0: 6e20 606f 626a 600a 2020 2020 2020 2020  n `obj`.        
-000186b0: 2020 2020 7374 6172 7469 6e67 2066 726f      starting fro
-000186c0: 6d20 7468 6520 656e 642e 0a20 2020 2020  m the end..     
-000186d0: 2020 2073 696e 676c 653a 2062 6f6f 6c0a     single: bool.
-000186e0: 2020 2020 2020 2020 2020 2020 4966 2054              If T
-000186f0: 7275 652c 2072 6574 7572 6e20 7468 6520  rue, return the 
-00018700: 6669 7273 7420 6974 656d 2066 6f75 6e64  first item found
-00018710: 206f 7220 4e6f 6e65 2e0a 2020 2020 2020   or None..      
-00018720: 2020 2020 2020 4966 2046 616c 7365 2c20        If False, 
-00018730: 7265 7475 726e 2061 2070 6f73 7369 626c  return a possibl
-00018740: 6520 656d 7074 7920 6c69 7374 206f 6620  e empty list of 
-00018750: 666f 756e 6420 6974 656d 732e 0a20 2020  found items..   
-00018760: 2020 2020 207b 6572 726f 7273 7d0a 0a20       {errors}.. 
-00018770: 2020 2020 2020 2052 6574 7572 6e0a 2020         Return.  
-00018780: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
-00018790: 2020 2020 2074 7570 6c65 2c20 7475 706c       tuple, tupl
-000187a0: 6528 6c69 7374 290a 2020 2020 2020 2020  e(list).        
-000187b0: 2020 2020 5475 706c 6520 6f66 2064 696d      Tuple of dim
-000187c0: 656e 7369 6f6e 206e 616d 6573 206f 7220  ension names or 
-000187d0: 4e6f 6e65 2077 6865 6e20 7468 6520 6469  None when the di
-000187e0: 6d65 6e73 696f 6e20 6973 206e 6f74 2066  mension is not f
-000187f0: 6f75 6e64 0a0a 2020 2020 2020 2020 5365  ound..        Se
-00018800: 6520 616c 736f 0a20 2020 2020 2020 202d  e also.        -
-00018810: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00018820: 7365 6172 6368 5f64 696d 0a20 2020 2020  search_dim.     
-00018830: 2020 2067 6574 5f64 696d 5f74 7970 650a     get_dim_type.
-00018840: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00018850: 2020 2020 2320 4368 6563 6b20 7368 6170      # Check shap
-00018860: 650a 2020 2020 2020 2020 6572 726f 7273  e.        errors
-00018870: 203d 2045 5252 4f52 535b 6572 726f 7273   = ERRORS[errors
-00018880: 5d0a 2020 2020 2020 2020 6469 6d73 203d  ].        dims =
-00018890: 206c 6973 7428 6f62 6a2e 6469 6d73 290a   list(obj.dims).
-000188a0: 2020 2020 2020 2020 6e64 696d 203d 206c          ndim = l
-000188b0: 656e 2864 696d 7329 0a20 2020 2020 2020  en(dims).       
-000188c0: 2069 6620 6c65 6e28 6366 5f61 7267 7329   if len(cf_args)
-000188d0: 203e 206c 656e 2864 696d 7329 3a0a 2020   > len(dims):.  
-000188e0: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
-000188f0: 6622 5468 6973 2064 6174 6120 6172 7261  f"This data arra
-00018900: 7920 6861 7320 6c65 7373 2064 696d 656e  y has less dimen
-00018910: 7369 6f6e 7320 287b 6e64 696d 7d29 2220  sions ({ndim})" 
-00018920: 2220 7468 616e 2072 6571 7565 7374 6564  " than requested
-00018930: 2028 7b7d 2922 2e66 6f72 6d61 7428 0a20   ({})".format(. 
-00018940: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00018950: 656e 2863 665f 6172 6773 290a 2020 2020  en(cf_args).    
-00018960: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00018970: 2020 2020 2020 6966 2065 7272 6f72 7320        if errors 
-00018980: 3d3d 2022 7261 6973 6522 3a0a 2020 2020  == "raise":.    
-00018990: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000189a0: 6520 586f 6145 7272 6f72 286d 7367 290a  e XoaError(msg).
-000189b0: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-000189c0: 7272 6f72 7320 3d3d 2022 7761 726e 223a  rrors == "warn":
-000189d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000189e0: 2078 6f61 5f77 6172 6e28 6d73 6729 0a0a   xoa_warn(msg)..
-000189f0: 2020 2020 2020 2020 2320 4c6f 6f70 206f          # Loop o
-00018a00: 6e20 6172 6773 0a20 2020 2020 2020 2073  n args.        s
-00018a10: 6361 6e6e 6564 203d 207b 7d0a 2020 2020  canned = {}.    
-00018a20: 2020 2020 666f 7220 6366 5f61 7267 2069      for cf_arg i
-00018a30: 6e20 6366 5f61 7267 733a 0a20 2020 2020  n cf_args:.     
-00018a40: 2020 2020 2020 2073 6361 6e6e 6564 5b63         scanned[c
-00018a50: 665f 6172 675d 203d 2073 656c 662e 7365  f_arg] = self.se
-00018a60: 6172 6368 5f64 696d 286f 626a 2c20 6366  arch_dim(obj, cf
-00018a70: 5f61 7267 2c20 7369 6e67 6c65 3d46 616c  _arg, single=Fal
-00018a80: 7365 2c20 6572 726f 7273 3d22 6967 6e6f  se, errors="igno
-00018a90: 7265 2229 0a0a 2020 2020 2020 2020 2320  re")..        # 
-00018aa0: 4775 6573 7320 6672 6f6d 2070 6f73 6974  Guess from posit
-00018ab0: 696f 6e0a 2020 2020 2020 2020 6966 2061  ion.        if a
-00018ac0: 6c6c 6f77 5f70 6f73 6974 696f 6e61 6c3a  llow_positional:
-00018ad0: 0a20 2020 2020 2020 2020 2020 206e 6f74  .            not
-00018ae0: 5f66 6f75 6e64 203d 205b 6974 656d 5b30  _found = [item[0
-00018af0: 5d20 666f 7220 6974 656d 2069 6e20 7363  ] for item in sc
-00018b00: 616e 6e65 642e 6974 656d 7328 2920 6966  anned.items() if
-00018b10: 206e 6f74 2069 7465 6d5b 315d 5d0a 2020   not item[1]].  
-00018b20: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
-00018b30: 2063 665f 6172 6720 696e 2065 6e75 6d65   cf_arg in enume
-00018b40: 7261 7465 2870 6f73 6974 696f 6e73 5b3a  rate(positions[:
-00018b50: 3a2d 315d 293a 0a20 2020 2020 2020 2020  :-1]):.         
-00018b60: 2020 2020 2020 2069 6620 6366 5f61 7267         if cf_arg
-00018b70: 2069 6e20 6e6f 745f 666f 756e 643a 0a20   in not_found:. 
-00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b90: 2020 2073 6361 6e6e 6564 5b63 665f 6172     scanned[cf_ar
-00018ba0: 675d 203d 205b 6469 6d73 5b2d 6920 2d20  g] = [dims[-i - 
-00018bb0: 315d 5d0a 0a20 2020 2020 2020 2023 2046  1]]..        # F
-00018bc0: 696e 616c 2063 6865 636b 0a20 2020 2020  inal check.     
-00018bd0: 2020 2069 6620 7369 6e67 6c65 3a0a 2020     if single:.  
-00018be0: 2020 2020 2020 2020 2020 666f 7220 6366            for cf
-00018bf0: 5f61 7267 2c20 6469 6d20 696e 2073 6361  _arg, dim in sca
-00018c00: 6e6e 6564 2e69 7465 6d73 2829 3a0a 2020  nned.items():.  
-00018c10: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00018c20: 206e 6f74 2064 696d 3a0a 2020 2020 2020   not dim:.      
-00018c30: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00018c40: 2065 7272 6f72 7320 213d 2027 6967 6e6f   errors != 'igno
-00018c50: 7265 273a 0a20 2020 2020 2020 2020 2020  re':.           
-00018c60: 2020 2020 2020 2020 2020 2020 206d 7367               msg
-00018c70: 203d 2066 224e 6f20 6469 6d65 6e73 696f   = f"No dimensio
-00018c80: 6e20 666f 756e 6420 6d61 7463 6869 6e67  n found matching
-00018c90: 3a20 7b63 665f 6172 677d 220a 2020 2020  : {cf_arg}".    
-00018ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cb0: 2020 2020 6966 2065 7272 6f72 7320 3d3d      if errors ==
-00018cc0: 2027 7261 6973 6527 3a0a 2020 2020 2020   'raise':.      
-00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ce0: 2020 2020 2020 7261 6973 6520 586f 6145        raise XoaE
-00018cf0: 7272 6f72 286d 7367 290a 2020 2020 2020  rror(msg).      
-00018d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d10: 2020 786f 615f 7761 726e 286d 7367 290a    xoa_warn(msg).
-00018d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d30: 2020 2020 7363 616e 6e65 645b 6366 5f61      scanned[cf_a
-00018d40: 7267 5d20 3d20 4e6f 6e65 0a20 2020 2020  rg] = None.     
-00018d50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00018d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018d70: 2020 2020 2069 6620 6c65 6e28 6469 6d29       if len(dim)
-00018d80: 203e 2031 2061 6e64 2065 7272 6f72 7320   > 1 and errors 
-00018d90: 213d 2022 6967 6e6f 7265 223a 0a20 2020  != "ignore":.   
-00018da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018db0: 2020 2020 206d 7367 203d 2066 224d 756c       msg = f"Mul
-00018dc0: 7469 706c 6520 6361 6e64 6964 6174 6573  tiple candidates
-00018dd0: 2064 696d 656e 7369 6f6e 7320 6d61 7463   dimensions matc
-00018de0: 6869 6e67 3a20 7b63 665f 6172 677d 220a  hing: {cf_arg}".
-00018df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e00: 2020 2020 2020 2020 6966 2065 7272 6f72          if error
-00018e10: 7320 3d3d 2022 7261 6973 6522 3a0a 2020  s == "raise":.  
-00018e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00018e40: 586f 6143 4645 7272 6f72 286d 7367 290a  XoaCFError(msg).
+00018310: 6966 2063 6f6f 7264 5f64 696d 5f74 7970  if coord_dim_typ
+00018320: 6520 616e 6420 636f 6f72 645f 6469 6d5f  e and coord_dim_
+00018330: 7479 7065 203d 3d20 6469 6d5f 7479 7065  type == dim_type
+00018340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018350: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00018360: 2063 6f6f 7264 0a0a 2020 2020 2020 2020   coord..        
+00018370: 2320 4e6f 7468 696e 6720 666f 756e 640a  # Nothing found.
+00018380: 2020 2020 2020 2020 6572 726f 7273 203d          errors =
+00018390: 2045 5252 4f52 535b 6572 726f 7273 5d0a   ERRORS[errors].
+000183a0: 2020 2020 2020 2020 6966 2065 7272 6f72          if error
+000183b0: 7320 213d 2022 6967 6e6f 7265 223a 0a20  s != "ignore":. 
+000183c0: 2020 2020 2020 2020 2020 206d 7367 203d             msg =
+000183d0: 2066 224e 6f20 6461 7461 6172 7261 7920   f"No dataarray 
+000183e0: 636f 6f72 6420 666f 756e 6420 6672 6f6d  coord found from
+000183f0: 2064 696d 3a20 7b64 696d 7d22 0a20 2020   dim: {dim}".   
+00018400: 2020 2020 2020 2020 2069 6620 6572 726f           if erro
+00018410: 7273 203d 3d20 2272 6169 7365 223a 0a20  rs == "raise":. 
+00018420: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00018430: 6169 7365 2058 6f61 4346 4572 726f 7228  aise XoaCFError(
+00018440: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
+00018450: 2078 6f61 5f77 6172 6e28 6d73 6729 0a0a   xoa_warn(msg)..
+00018460: 2020 2020 4045 5252 4f52 532e 666f 726d      @ERRORS.form
+00018470: 6174 5f6d 6574 686f 645f 646f 6373 7472  at_method_docstr
+00018480: 696e 670a 2020 2020 6465 6620 6765 745f  ing.    def get_
+00018490: 6469 6d73 280a 2020 2020 2020 2020 7365  dims(.        se
+000184a0: 6c66 2c20 6f62 6a2c 2063 665f 6172 6773  lf, obj, cf_args
+000184b0: 2c20 616c 6c6f 775f 706f 7369 7469 6f6e  , allow_position
+000184c0: 616c 3d46 616c 7365 2c20 706f 7369 7469  al=False, positi
+000184d0: 6f6e 733d 2774 7a79 7827 2c20 7369 6e67  ons='tzyx', sing
+000184e0: 6c65 3d54 7275 652c 2065 7272 6f72 733d  le=True, errors=
+000184f0: 2277 6172 6e22 0a20 2020 2029 3a0a 2020  "warn".    ):.  
+00018500: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
+00018510: 2064 6174 6120 6172 7261 7920 6469 6d65   data array dime
+00018520: 6e73 696f 6e73 206e 616d 6573 2066 726f  nsions names fro
+00018530: 6d20 7468 6569 7220 7479 7065 206f 7220  m their type or 
+00018540: 6765 6e65 7269 6320 4346 206e 616d 650a  generic CF name.
+00018550: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00018560: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00018570: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 206f  ------.        o
+00018580: 626a 3a20 7861 7272 6179 2e44 6174 6141  bj: xarray.DataA
+00018590: 7272 6179 2c20 7861 7272 6179 2e44 6174  rray, xarray.Dat
+000185a0: 6173 6574 0a20 2020 2020 2020 2020 2020  aset.           
+000185b0: 2041 7272 6179 2f64 6174 6173 6574 2074   Array/dataset t
+000185c0: 6f20 7363 616e 0a20 2020 2020 2020 2063  o scan.        c
+000185d0: 665f 6172 6773 3a20 6c69 7374 0a20 2020  f_args: list.   
+000185e0: 2020 2020 2020 2020 204c 6973 7420 6f66           List of
+000185f0: 206c 6574 7465 7273 2061 6d6f 6e67 2022   letters among "
+00018600: 7822 2c20 2279 222c 2022 7a22 2c20 2274  x", "y", "z", "t
+00018610: 2220 616e 6420 2266 222c 0a20 2020 2020  " and "f",.     
+00018620: 2020 2020 2020 206f 7220 6765 6e65 7269         or generi
+00018630: 6320 6e61 6d65 732e 0a20 2020 2020 2020  c names..       
+00018640: 2061 6c6c 6f77 5f70 6f73 6974 696f 6e61   allow_positiona
+00018650: 6c3a 2062 6f6f 6c0a 2020 2020 2020 2020  l: bool.        
+00018660: 2020 2020 4661 6c6c 2062 6163 6b20 746f      Fall back to
+00018670: 2070 6f73 6974 696f 6e61 6c20 6469 6d65   positional dime
+00018680: 6e73 696f 6e20 6f66 2074 7970 6573 2069  nsion of types i
+00018690: 7320 756e 6b6f 776e 2e0a 2020 2020 2020  s unkown..      
+000186a0: 2020 706f 7369 7469 6f6e 733a 2073 7472    positions: str
+000186b0: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
+000186c0: 6175 6c74 2065 7870 6563 7465 6420 706f  ault expected po
+000186d0: 7369 7469 6f6e 206f 6620 6469 6d20 7065  sition of dim pe
+000186e0: 7220 7479 7065 2069 6e20 606f 626a 600a  r type in `obj`.
+000186f0: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00018700: 7469 6e67 2066 726f 6d20 7468 6520 656e  ting from the en
+00018710: 642e 0a20 2020 2020 2020 2073 696e 676c  d..        singl
+00018720: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00018730: 2020 2020 4966 2054 7275 652c 2072 6574      If True, ret
+00018740: 7572 6e20 7468 6520 6669 7273 7420 6974  urn the first it
+00018750: 656d 2066 6f75 6e64 206f 7220 4e6f 6e65  em found or None
+00018760: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+00018770: 2046 616c 7365 2c20 7265 7475 726e 2061   False, return a
+00018780: 2070 6f73 7369 626c 6520 656d 7074 7920   possible empty 
+00018790: 6c69 7374 206f 6620 666f 756e 6420 6974  list of found it
+000187a0: 656d 732e 0a20 2020 2020 2020 207b 6572  ems..        {er
+000187b0: 726f 7273 7d0a 0a20 2020 2020 2020 2052  rors}..        R
+000187c0: 6574 7572 6e0a 2020 2020 2020 2020 2d2d  eturn.        --
+000187d0: 2d2d 2d2d 0a20 2020 2020 2020 2074 7570  ----.        tup
+000187e0: 6c65 2c20 7475 706c 6528 6c69 7374 290a  le, tuple(list).
+000187f0: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
+00018800: 6520 6f66 2064 696d 656e 7369 6f6e 206e  e of dimension n
+00018810: 616d 6573 206f 7220 4e6f 6e65 2077 6865  ames or None whe
+00018820: 6e20 7468 6520 6469 6d65 6e73 696f 6e20  n the dimension 
+00018830: 6973 206e 6f74 2066 6f75 6e64 0a0a 2020  is not found..  
+00018840: 2020 2020 2020 5365 6520 616c 736f 0a20        See also. 
+00018850: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0a         --------.
+00018860: 2020 2020 2020 2020 7365 6172 6368 5f64          search_d
+00018870: 696d 0a20 2020 2020 2020 2067 6574 5f64  im.        get_d
+00018880: 696d 5f74 7970 650a 2020 2020 2020 2020  im_type.        
+00018890: 2222 220a 2020 2020 2020 2020 2320 4368  """.        # Ch
+000188a0: 6563 6b20 7368 6170 650a 2020 2020 2020  eck shape.      
+000188b0: 2020 6572 726f 7273 203d 2045 5252 4f52    errors = ERROR
+000188c0: 535b 6572 726f 7273 5d0a 2020 2020 2020  S[errors].      
+000188d0: 2020 6469 6d73 203d 206c 6973 7428 6f62    dims = list(ob
+000188e0: 6a2e 6469 6d73 290a 2020 2020 2020 2020  j.dims).        
+000188f0: 6e64 696d 203d 206c 656e 2864 696d 7329  ndim = len(dims)
+00018900: 0a20 2020 2020 2020 2073 696e 676c 655f  .        single_
+00018910: 6172 6720 3d20 6973 696e 7374 616e 6365  arg = isinstance
+00018920: 2863 665f 6172 6773 2c20 7374 7229 0a20  (cf_args, str). 
+00018930: 2020 2020 2020 2069 6620 7369 6e67 6c65         if single
+00018940: 5f61 7267 3a0a 2020 2020 2020 2020 2020  _arg:.          
+00018950: 2020 6366 5f61 7267 7320 3d20 5b63 665f    cf_args = [cf_
+00018960: 6172 6773 5d0a 2020 2020 2020 2020 6966  args].        if
+00018970: 206c 656e 2863 665f 6172 6773 2920 3e20   len(cf_args) > 
+00018980: 6c65 6e28 6469 6d73 293a 0a20 2020 2020  len(dims):.     
+00018990: 2020 2020 2020 206d 7367 203d 2066 2254         msg = f"T
+000189a0: 6869 7320 6461 7461 2061 7272 6179 2068  his data array h
+000189b0: 6173 206c 6573 7320 6469 6d65 6e73 696f  as less dimensio
+000189c0: 6e73 2028 7b6e 6469 6d7d 2922 2022 2074  ns ({ndim})" " t
+000189d0: 6861 6e20 7265 7175 6573 7465 6420 287b  han requested ({
+000189e0: 7d29 222e 666f 726d 6174 280a 2020 2020  })".format(.    
+000189f0: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+00018a00: 6366 5f61 7267 7329 0a20 2020 2020 2020  cf_args).       
+00018a10: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00018a20: 2020 2069 6620 6572 726f 7273 203d 3d20     if errors == 
+00018a30: 2272 6169 7365 223a 0a20 2020 2020 2020  "raise":.       
+00018a40: 2020 2020 2020 2020 2072 6169 7365 2058           raise X
+00018a50: 6f61 4572 726f 7228 6d73 6729 0a20 2020  oaError(msg).   
+00018a60: 2020 2020 2020 2020 2069 6620 6572 726f           if erro
+00018a70: 7273 203d 3d20 2277 6172 6e22 3a0a 2020  rs == "warn":.  
+00018a80: 2020 2020 2020 2020 2020 2020 2020 786f                xo
+00018a90: 615f 7761 726e 286d 7367 290a 0a20 2020  a_warn(msg)..   
+00018aa0: 2020 2020 2023 204c 6f6f 7020 6f6e 2061       # Loop on a
+00018ab0: 7267 730a 2020 2020 2020 2020 7363 616e  rgs.        scan
+00018ac0: 6e65 6420 3d20 7b7d 0a20 2020 2020 2020  ned = {}.       
+00018ad0: 2066 6f72 2063 665f 6172 6720 696e 2063   for cf_arg in c
+00018ae0: 665f 6172 6773 3a0a 2020 2020 2020 2020  f_args:.        
+00018af0: 2020 2020 7363 616e 6e65 645b 6366 5f61      scanned[cf_a
+00018b00: 7267 5d20 3d20 7365 6c66 2e73 6561 7263  rg] = self.searc
+00018b10: 685f 6469 6d28 6f62 6a2c 2063 665f 6172  h_dim(obj, cf_ar
+00018b20: 672c 2073 696e 676c 653d 4661 6c73 652c  g, single=False,
+00018b30: 2065 7272 6f72 733d 2269 676e 6f72 6522   errors="ignore"
+00018b40: 290a 0a20 2020 2020 2020 2023 2047 7565  )..        # Gue
+00018b50: 7373 2066 726f 6d20 706f 7369 7469 6f6e  ss from position
+00018b60: 0a20 2020 2020 2020 2069 6620 616c 6c6f  .        if allo
+00018b70: 775f 706f 7369 7469 6f6e 616c 3a0a 2020  w_positional:.  
+00018b80: 2020 2020 2020 2020 2020 6e6f 745f 666f            not_fo
+00018b90: 756e 6420 3d20 5b69 7465 6d5b 305d 2066  und = [item[0] f
+00018ba0: 6f72 2069 7465 6d20 696e 2073 6361 6e6e  or item in scann
+00018bb0: 6564 2e69 7465 6d73 2829 2069 6620 6e6f  ed.items() if no
+00018bc0: 7420 6974 656d 5b31 5d5d 0a20 2020 2020  t item[1]].     
+00018bd0: 2020 2020 2020 2066 6f72 2069 2c20 6366         for i, cf
+00018be0: 5f61 7267 2069 6e20 656e 756d 6572 6174  _arg in enumerat
+00018bf0: 6528 706f 7369 7469 6f6e 735b 3a3a 2d31  e(positions[::-1
+00018c00: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+00018c10: 2020 2020 6966 2063 665f 6172 6720 696e      if cf_arg in
+00018c20: 206e 6f74 5f66 6f75 6e64 3a0a 2020 2020   not_found:.    
+00018c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c40: 7363 616e 6e65 645b 6366 5f61 7267 5d20  scanned[cf_arg] 
+00018c50: 3d20 5b64 696d 735b 2d69 202d 2031 5d5d  = [dims[-i - 1]]
+00018c60: 0a0a 2020 2020 2020 2020 2320 4669 6e61  ..        # Fina
+00018c70: 6c20 6368 6563 6b0a 2020 2020 2020 2020  l check.        
+00018c80: 6966 2073 696e 676c 653a 0a20 2020 2020  if single:.     
+00018c90: 2020 2020 2020 2066 6f72 2063 665f 6172         for cf_ar
+00018ca0: 672c 2064 696d 2069 6e20 7363 616e 6e65  g, dim in scanne
+00018cb0: 642e 6974 656d 7328 293a 0a20 2020 2020  d.items():.     
+00018cc0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00018cd0: 7420 6469 6d3a 0a20 2020 2020 2020 2020  t dim:.         
+00018ce0: 2020 2020 2020 2020 2020 2069 6620 6572             if er
+00018cf0: 726f 7273 2021 3d20 2769 676e 6f72 6527  rors != 'ignore'
+00018d00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018d10: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
+00018d20: 6622 4e6f 2064 696d 656e 7369 6f6e 2066  f"No dimension f
+00018d30: 6f75 6e64 206d 6174 6368 696e 673a 207b  ound matching: {
+00018d40: 6366 5f61 7267 7d22 0a20 2020 2020 2020  cf_arg}".       
+00018d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d60: 2069 6620 6572 726f 7273 203d 3d20 2772   if errors == 'r
+00018d70: 6169 7365 273a 0a20 2020 2020 2020 2020  aise':.         
+00018d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d90: 2020 2072 6169 7365 2058 6f61 4572 726f     raise XoaErro
+00018da0: 7228 6d73 6729 0a20 2020 2020 2020 2020  r(msg).         
+00018db0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00018dc0: 6f61 5f77 6172 6e28 6d73 6729 0a20 2020  oa_warn(msg).   
+00018dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018de0: 2073 6361 6e6e 6564 5b63 665f 6172 675d   scanned[cf_arg]
+00018df0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00018e00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00018e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e20: 2020 6966 206c 656e 2864 696d 2920 3e20    if len(dim) > 
+00018e30: 3120 616e 6420 6572 726f 7273 2021 3d20  1 and errors != 
+00018e40: 2269 676e 6f72 6522 3a0a 2020 2020 2020  "ignore":.      
 00018e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e60: 2020 2020 2020 2020 786f 615f 7761 726e          xoa_warn
-00018e70: 286d 7367 290a 2020 2020 2020 2020 2020  (msg).          
-00018e80: 2020 2020 2020 2020 2020 7363 616e 6e65            scanne
-00018e90: 645b 6366 5f61 7267 5d20 3d20 6469 6d5b  d[cf_arg] = dim[
-00018ea0: 305d 0a0a 2020 2020 2020 2020 7265 7475  0]..        retu
-00018eb0: 726e 2074 7570 6c65 2873 6361 6e6e 6564  rn tuple(scanned
-00018ec0: 2e76 616c 7565 7328 2929 0a0a 2020 2020  .values())..    
-00018ed0: 6465 6620 6765 745f 7265 6e61 6d65 5f64  def get_rename_d
-00018ee0: 696d 735f 6172 6773 2873 656c 662c 206f  ims_args(self, o
-00018ef0: 626a 2c20 6c6f 6361 7469 6f6e 733d 4e6f  bj, locations=No
-00018f00: 6e65 2c20 7370 6563 6961 6c69 7a65 3d46  ne, specialize=F
-00018f10: 616c 7365 293a 0a20 2020 2020 2020 2022  alse):.        "
-00018f20: 2222 4765 7420 6172 6773 2066 6f72 2072  ""Get args for r
-00018f30: 656e 616d 696e 6720 6469 6d65 6e73 696f  enaming dimensio
-00018f40: 6e73 2074 6861 7420 6172 6520 6e6f 7420  ns that are not 
-00018f50: 636f 6f72 6469 6e61 7465 730a 0a20 2020  coordinates..   
-00018f60: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00018f70: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00018f80: 2d2d 0a20 2020 2020 2020 206f 626a 3a20  --.        obj: 
-00018f90: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-00018fa0: 2c20 7861 7272 6179 2e44 6174 6173 6574  , xarray.Dataset
-00018fb0: 0a20 2020 2020 2020 2020 2020 2041 7272  .            Arr
-00018fc0: 6179 206f 7220 6461 7461 7365 740a 2020  ay or dataset.  
-00018fd0: 2020 2020 2020 6c6f 6361 7469 6f6e 733a        locations:
-00018fe0: 2064 6963 742c 204e 6f6e 650a 2020 2020   dict, None.    
-00018ff0: 2020 2020 2020 2020 4469 6374 206f 6620          Dict of 
-00019000: 7374 6167 6765 7264 2067 7269 6420 6c6f  staggerd grid lo
-00019010: 6361 7469 6f6e 7320 7769 7468 206e 616d  cations with nam
-00019020: 6573 2061 7320 6b65 7973 0a20 2020 2020  es as keys.     
-00019030: 2020 2073 7065 6369 616c 697a 653a 2062     specialize: b
-00019040: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-00019050: 446f 206e 6f74 2075 7365 2074 6865 2043  Do not use the C
-00019060: 4620 6e61 6d65 2066 6f72 2072 656e 616d  F name for renam
-00019070: 696e 672c 2062 7574 2074 6865 2066 6972  ing, but the fir
-00019080: 7374 206e 616d 650a 2020 2020 2020 2020  st name.        
-00019090: 2020 2020 6173 206c 6973 7465 6420 696e      as listed in
-000190a0: 2073 7065 6373 2c20 7768 6963 6820 6973   specs, which is
-000190b0: 2067 656e 6572 616c 6c79 2061 2073 7065   generally a spe
-000190c0: 6369 616c 697a 6564 206f 6e65 2c0a 2020  cialized one,.  
-000190d0: 2020 2020 2020 2020 2020 6c69 6b65 2061            like a
-000190e0: 206e 616d 6520 6164 6f70 7465 6420 6279   name adopted by
-000190f0: 2073 7065 6369 616c 697a 6564 2064 6174   specialized dat
-00019100: 6173 6574 2e0a 0a20 2020 2020 2020 2052  aset...        R
-00019110: 6574 7572 6e0a 2020 2020 2020 2020 2d2d  eturn.        --
-00019120: 2d2d 2d2d 0a20 2020 2020 2020 2064 6963  ----.        dic
-00019130: 743a 0a20 2020 2020 2020 2020 2020 2041  t:.            A
-00019140: 7267 756d 656e 7420 636f 6d70 6174 6962  rgument compatib
-00019150: 6c65 2077 6974 6820 3a6d 6574 683a 6078  le with :meth:`x
-00019160: 6172 7261 792e 4461 7461 7365 742e 7265  array.Dataset.re
-00019170: 6e61 6d65 600a 2020 2020 2020 2020 2222  name`.        ""
-00019180: 220a 0a20 2020 2020 2020 2023 2047 6574  "..        # Get
-00019190: 206c 6f63 6174 696f 6e20 7370 6563 730a   location specs.
-000191a0: 2020 2020 2020 2020 6966 206c 6f63 6174          if locat
-000191b0: 696f 6e73 2069 7320 4e6f 6e65 3a0a 2020  ions is None:.  
-000191c0: 2020 2020 2020 2020 2020 6c6f 6361 7469            locati
-000191d0: 6f6e 7320 3d20 7365 6c66 2e67 6574 5f6c  ons = self.get_l
-000191e0: 6f63 5f6d 6170 7069 6e67 286f 626a 290a  oc_mapping(obj).
-000191f0: 0a20 2020 2020 2020 2023 204c 6f6f 7020  .        # Loop 
-00019200: 6f6e 2064 696d 730a 2020 2020 2020 2020  on dims.        
-00019210: 7265 6e61 6d65 5f61 7267 7320 3d20 7b7d  rename_args = {}
-00019220: 0a20 2020 2020 2020 2066 6f72 2064 696d  .        for dim
-00019230: 2069 6e20 6f62 6a2e 6469 6d73 3a0a 0a20   in obj.dims:.. 
-00019240: 2020 2020 2020 2020 2020 2023 2053 6b69             # Ski
-00019250: 7020 6566 6665 6374 6976 6520 636f 6f72  p effective coor
-00019260: 6469 6e61 7465 2064 696d 730a 2020 2020  dinate dims.    
-00019270: 2020 2020 2020 2020 6966 2064 696d 2069          if dim i
-00019280: 6e20 6f62 6a2e 636f 6f72 6473 3a0a 2020  n obj.coords:.  
-00019290: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000192a0: 6e74 696e 7565 0a0a 2020 2020 2020 2020  ntinue..        
-000192b0: 2020 2020 2320 4973 2069 7420 6b6e 6f77      # Is it know
-000192c0: 6e3f 0a20 2020 2020 2020 2020 2020 2063  n?.            c
-000192d0: 665f 6469 6d5f 6e61 6d65 203d 2073 656c  f_dim_name = sel
-000192e0: 662e 6d61 7463 685f 6672 6f6d 5f6e 616d  f.match_from_nam
-000192f0: 6528 6469 6d29 2020 2320 6b6e 6f77 6e20  e(dim)  # known 
-00019300: 636f 6f72 6469 6e61 7465 206e 616d 650a  coordinate name.
-00019310: 2020 2020 2020 2020 2020 2020 6469 6d5f              dim_
-00019320: 7479 7065 203d 2073 656c 662e 6765 745f  type = self.get_
-00019330: 6469 6d5f 7479 7065 2864 696d 2c20 6f62  dim_type(dim, ob
-00019340: 6a29 2020 2320 6b6e 6f77 6e20 6469 6d65  j)  # known dime
-00019350: 6e73 696f 6e20 7479 7065 0a20 2020 2020  nsion type.     
-00019360: 2020 2020 2020 2064 696d 5f6c 6f63 203d         dim_loc =
-00019370: 206c 6f63 6174 696f 6e73 2e67 6574 2864   locations.get(d
-00019380: 696d 290a 0a20 2020 2020 2020 2020 2020  im)..           
-00019390: 2023 2052 6f6f 7420 6e61 6d65 0a20 2020   # Root name.   
-000193a0: 2020 2020 2020 2020 2069 6620 6366 5f64           if cf_d
-000193b0: 696d 5f6e 616d 653a 0a20 2020 2020 2020  im_name:.       
-000193c0: 2020 2020 2020 2020 206e 6577 5f6e 616d           new_nam
-000193d0: 6520 3d20 7365 6c66 2e67 6574 5f6e 616d  e = self.get_nam
-000193e0: 6528 6366 5f64 696d 5f6e 616d 652c 2073  e(cf_dim_name, s
-000193f0: 7065 6369 616c 697a 653d 7370 6563 6961  pecialize=specia
-00019400: 6c69 7a65 290a 2020 2020 2020 2020 2020  lize).          
-00019410: 2020 656c 6966 2064 696d 5f74 7970 653a    elif dim_type:
-00019420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019430: 206e 6577 5f6e 616d 6520 3d20 6469 6d5f   new_name = dim_
-00019440: 7479 7065 0a20 2020 2020 2020 2020 2020  type.           
-00019450: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00019460: 2020 2020 2020 206e 6577 5f6e 616d 6520         new_name 
-00019470: 3d20 6469 6d0a 0a20 2020 2020 2020 2020  = dim..         
-00019480: 2020 2023 2041 6464 206c 6f63 0a20 2020     # Add loc.   
-00019490: 2020 2020 2020 2020 2069 6620 6469 6d5f           if dim_
-000194a0: 6c6f 6320 6973 206e 6f74 2046 616c 7365  loc is not False
-000194b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000194c0: 2020 6e65 775f 6e61 6d65 203d 2073 656c    new_name = sel
-000194d0: 662e 7367 6c6f 6361 746f 722e 6d65 7267  f.sglocator.merg
-000194e0: 655f 6174 7472 2827 6e61 6d65 272c 2064  e_attr('name', d
-000194f0: 696d 2c20 6e65 775f 6e61 6d65 2c20 6c6f  im, new_name, lo
-00019500: 633d 6469 6d5f 6c6f 6329 0a0a 2020 2020  c=dim_loc)..    
-00019510: 2020 2020 2020 2020 2320 5265 6769 7374          # Regist
-00019520: 6572 2061 7267 0a20 2020 2020 2020 2020  er arg.         
-00019530: 2020 2069 6620 6e65 775f 6e61 6d65 2021     if new_name !
-00019540: 3d20 6469 6d3a 0a20 2020 2020 2020 2020  = dim:.         
-00019550: 2020 2020 2020 2072 656e 616d 655f 6172         rename_ar
-00019560: 6773 5b64 696d 5d20 3d20 6e65 775f 6e61  gs[dim] = new_na
-00019570: 6d65 0a0a 2020 2020 2020 2020 7265 7475  me..        retu
-00019580: 726e 2072 656e 616d 655f 6172 6773 0a0a  rn rename_args..
-00019590: 2020 2020 6465 6620 7061 7273 655f 6469      def parse_di
-000195a0: 6d73 2873 656c 662c 2064 696d 732c 206f  ms(self, dims, o
-000195b0: 626a 293a 0a20 2020 2020 2020 2022 2222  bj):.        """
-000195c0: 436f 6e76 6572 7420 6672 6f6d 2067 656e  Convert from gen
-000195d0: 6572 6963 2064 696d 206e 616d 6573 2074  eric dim names t
-000195e0: 6f20 7370 6563 6961 6c69 7a65 6420 6e61  o specialized na
-000195f0: 6d65 730a 0a20 2020 2020 2020 2050 6172  mes..        Par
-00019600: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00019610: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00019620: 2020 2064 696d 733a 2073 7472 2c20 7475     dims: str, tu
-00019630: 706c 652c 206c 6973 742c 2064 6963 740a  ple, list, dict.
-00019640: 2020 2020 2020 2020 6f62 6a3a 2078 6172          obj: xar
-00019650: 7261 792e 4461 7461 7365 742c 2078 6172  ray.Dataset, xar
-00019660: 7261 792e 4461 7461 4172 7261 790a 0a20  ray.DataArray.. 
-00019670: 2020 2020 2020 2052 6574 7572 6e0a 2020         Return.  
-00019680: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
-00019690: 2020 2020 2053 616d 6520 7479 7065 2061       Same type a
-000196a0: 7320 6469 6d73 0a20 2020 2020 2020 2022  s dims.        "
-000196b0: 2222 0a20 2020 2020 2020 2023 2064 696d  "".        # dim
-000196c0: 5f74 7970 6573 203d 2073 656c 662e 6765  _types = self.ge
-000196d0: 745f 6469 6d5f 7479 7065 7328 6f62 6a2c  t_dim_types(obj,
-000196e0: 2061 7364 6963 743d 5472 7565 290a 0a20   asdict=True).. 
-000196f0: 2020 2020 2020 2064 6566 205f 7061 7273         def _pars
-00019700: 655f 6469 6d5f 2863 665f 6172 6729 3a0a  e_dim_(cf_arg):.
-00019710: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00019720: 665f 6172 6720 696e 206f 626a 2e64 696d  f_arg in obj.dim
-00019730: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00019740: 2020 2072 6574 7572 6e20 6366 5f61 7267     return cf_arg
-00019750: 0a20 2020 2020 2020 2020 2020 2064 696d  .            dim
-00019760: 203d 2073 656c 662e 7365 6172 6368 5f64   = self.search_d
-00019770: 696d 286f 626a 2c20 6366 5f61 7267 290a  im(obj, cf_arg).
-00019780: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00019790: 6f74 2064 696d 3a0a 2020 2020 2020 2020  ot dim:.        
-000197a0: 2020 2020 2020 2020 7261 6973 6520 586f          raise Xo
-000197b0: 6143 4645 7272 6f72 2866 2249 6e76 616c  aCFError(f"Inval
-000197c0: 6964 2061 7267 756d 656e 7420 666f 7220  id argument for 
-000197d0: 6469 6d65 6e73 696f 6e3a 207b 6366 5f61  dimension: {cf_a
-000197e0: 7267 7d22 290a 2020 2020 2020 2020 2020  rg}").          
-000197f0: 2020 7265 7475 726e 2064 696d 0a0a 2020    return dim..  
-00019800: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00019810: 6e63 6528 6469 6d73 2c20 7374 7229 3a0a  nce(dims, str):.
-00019820: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00019830: 726e 205f 7061 7273 655f 6469 6d5f 2864  rn _parse_dim_(d
-00019840: 696d 7329 0a20 2020 2020 2020 2069 6620  ims).        if 
-00019850: 6973 696e 7374 616e 6365 2864 696d 732c  isinstance(dims,
-00019860: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
-00019870: 2020 2020 7265 7475 726e 2064 6963 7428      return dict(
-00019880: 285f 7061 7273 655f 6469 6d5f 2864 696d  (_parse_dim_(dim
-00019890: 292c 2076 616c 7565 2920 666f 7220 6469  ), value) for di
-000198a0: 6d2c 2076 616c 7565 2069 6e20 6469 6d73  m, value in dims
-000198b0: 2e69 7465 6d73 2829 290a 2020 2020 2020  .items()).      
-000198c0: 2020 7265 7475 726e 2074 7970 6528 6469    return type(di
-000198d0: 6d73 2928 5f70 6172 7365 5f64 696d 5f28  ms)(_parse_dim_(
-000198e0: 6469 6d29 2066 6f72 2064 696d 2069 6e20  dim) for dim in 
-000198f0: 6469 6d73 290a 0a0a 666f 7220 6d65 7468  dims)...for meth
-00019900: 2069 6e20 2827 6765 745f 6178 6973 272c   in ('get_axis',
-00019910: 2027 6765 745f 6469 6d5f 7479 7065 272c   'get_dim_type',
-00019920: 2027 6765 745f 6469 6d5f 7479 7065 7327   'get_dim_types'
-00019930: 2c20 2773 6561 7263 685f 6469 6d27 2c20  , 'search_dim', 
-00019940: 2767 6574 5f64 696d 7327 293a 0a20 2020  'get_dims'):.   
-00019950: 2064 6f63 203d 2067 6574 6174 7472 2843   doc = getattr(C
-00019960: 4643 6f6f 7264 5370 6563 732c 206d 6574  FCoordSpecs, met
-00019970: 6829 2e5f 5f64 6f63 5f5f 0a20 2020 2067  h).__doc__.    g
-00019980: 6574 6174 7472 2843 4653 7065 6373 2c20  etattr(CFSpecs, 
-00019990: 6d65 7468 292e 5f5f 646f 635f 5f20 3d20  meth).__doc__ = 
-000199a0: 646f 630a 0a0a 6465 6620 5f67 6574 5f63  doc...def _get_c
-000199b0: 6667 6d5f 2829 3a0a 2020 2020 2222 2247  fgm_():.    """G
-000199c0: 6574 2061 203a 636c 6173 733a 607e 786f  et a :class:`~xo
-000199d0: 612e 6366 676d 2e43 6f6e 6669 674d 616e  a.cfgm.ConfigMan
-000199e0: 6167 6572 6020 696e 7374 616e 6365 2074  ager` instance t
-000199f0: 6f20 6d61 6e61 6765 0a20 2020 2063 6f6f  o manage.    coo
-00019a00: 7264 7320 616e 6420 6461 7461 5f76 6172  rds and data_var
-00019a10: 7320 7370 c3a9 6369 6669 6361 7469 6f6e  s sp..cification
-00019a20: 7322 2222 0a20 2020 2063 665f 6361 6368  s""".    cf_cach
-00019a30: 6520 3d20 5f67 6574 5f63 6163 6865 5f28  e = _get_cache_(
-00019a40: 290a 2020 2020 6966 2022 6366 676d 2220  ).    if "cfgm" 
-00019a50: 6e6f 7420 696e 2063 665f 6361 6368 653a  not in cf_cache:
-00019a60: 0a20 2020 2020 2020 2066 726f 6d20 2e63  .        from .c
-00019a70: 6667 6d20 696d 706f 7274 2043 6f6e 6669  fgm import Confi
-00019a80: 674d 616e 6167 6572 0a0a 2020 2020 2020  gManager..      
-00019a90: 2020 6366 5f63 6163 6865 5b22 6366 676d    cf_cache["cfgm
-00019aa0: 225d 203d 2043 6f6e 6669 674d 616e 6167  "] = ConfigManag
-00019ab0: 6572 285f 494e 4946 494c 4529 0a20 2020  er(_INIFILE).   
-00019ac0: 2072 6574 7572 6e20 6366 5f63 6163 6865   return cf_cache
-00019ad0: 5b22 6366 676d 225d 0a0a 0a64 6566 2067  ["cfgm"]...def g
-00019ae0: 6574 5f6d 6174 6368 696e 675f 6974 656d  et_matching_item
-00019af0: 5f73 7065 6373 2864 612c 206c 6f63 3d22  _specs(da, loc="
-00019b00: 616e 7922 293a 0a20 2020 2022 2222 4765  any"):.    """Ge
-00019b10: 7420 7468 6520 6974 656d 2043 4620 7370  t the item CF sp
-00019b20: 6563 7320 7468 6174 206d 6174 6368 2074  ecs that match t
-00019b30: 6869 7320 6461 7461 2061 7272 6179 0a0a  his data array..
-00019b40: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00019b50: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00019b60: 2020 6461 3a20 7861 7272 6179 2e44 6174    da: xarray.Dat
-00019b70: 6141 7272 6179 0a0a 2020 2020 5265 7475  aArray..    Retu
-00019b80: 726e 0a20 2020 202d 2d2d 2d2d 2d0a 2020  rn.    ------.  
-00019b90: 2020 6469 6374 206f 7220 4e6f 6e65 0a0a    dict or None..
-00019ba0: 2020 2020 5365 6520 616c 736f 0a20 2020      See also.   
-00019bb0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 4346   --------.    CF
-00019bc0: 5370 6563 732e 6d61 7463 680a 2020 2020  Specs.match.    
-00019bd0: 2222 220a 2020 2020 6366 7370 6563 7320  """.    cfspecs 
-00019be0: 3d20 6765 745f 6366 5f73 7065 6373 2864  = get_cf_specs(d
-00019bf0: 6129 0a20 2020 2063 6174 2c20 6e61 6d65  a).    cat, name
-00019c00: 203d 2063 6673 7065 6373 2e6d 6174 6368   = cfspecs.match
-00019c10: 2864 612c 206c 6f63 3d6c 6f63 290a 2020  (da, loc=loc).  
-00019c20: 2020 6966 2063 6174 3a0a 2020 2020 2020    if cat:.      
-00019c30: 2020 7265 7475 726e 2063 6673 7065 6373    return cfspecs
-00019c40: 5b63 6174 5d5b 6e61 6d65 5d0a 0a0a 6465  [cat][name]...de
-00019c50: 6620 5f73 616d 655f 6174 7472 5f28 6461  f _same_attr_(da
-00019c60: 302c 2064 6131 2c20 6174 7472 293a 0a20  0, da1, attr):. 
-00019c70: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
-00019c80: 2020 2020 6174 7472 2069 6e20 6461 302e      attr in da0.
-00019c90: 6174 7472 730a 2020 2020 2020 2020 616e  attrs.        an
-00019ca0: 6420 6174 7472 2069 6e20 6461 312e 6174  d attr in da1.at
-00019cb0: 7472 730a 2020 2020 2020 2020 616e 6420  trs.        and 
-00019cc0: 6461 302e 6174 7472 735b 6174 7472 5d2e  da0.attrs[attr].
-00019cd0: 6c6f 7765 7228 2920 3d3d 2064 6131 2e61  lower() == da1.a
-00019ce0: 7474 7273 5b61 7474 725d 2e6c 6f77 6572  ttrs[attr].lower
-00019cf0: 2829 0a20 2020 2029 0a0a 0a64 6566 2061  ().    )...def a
-00019d00: 7265 5f73 696d 696c 6172 2864 6130 2c20  re_similar(da0, 
-00019d10: 6461 3129 3a0a 2020 2020 2222 2243 6865  da1):.    """Che
-00019d20: 636b 2069 6620 7477 6f20 4461 7461 4172  ck if two DataAr
-00019d30: 7261 7973 2061 7265 2073 696d 696c 6172  rays are similar
-00019d40: 0a0a 2020 2020 5665 7269 6669 6361 7469  ..    Verificati
-00019d50: 6f6e 7320 6172 6520 7065 7266 6f72 6d65  ons are performe
-00019d60: 6420 696e 2074 6865 2066 6f6c 6c6f 7769  d in the followi
-00019d70: 6e67 206f 7264 6572 3a0a 0a20 2020 202d  ng order:..    -
-00019d80: 2060 6073 7461 6e64 6172 645f 6e61 6d65   ``standard_name
-00019d90: 6060 2061 7474 7269 6275 7465 2c0a 2020  `` attribute,.  
-00019da0: 2020 2d20 4d61 7463 6869 6e67 2043 4653    - Matching CFS
-00019db0: 7065 6373 2069 7465 6d20 6e61 6d65 2e0a  pecs item name..
-00019dc0: 2020 2020 2d20 6060 6e61 6d65 6060 2061      - ``name`` a
-00019dd0: 7474 7269 6275 7465 2e0a 2020 2020 2d20  ttribute..    - 
-00019de0: 6060 6c6f 6e67 5f6e 616d 6560 6020 6174  ``long_name`` at
-00019df0: 7472 6962 7574 652e 0a0a 2020 2020 5061  tribute...    Pa
-00019e00: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00019e10: 2d2d 2d2d 2d2d 2d0a 2020 2020 6461 303a  -------.    da0:
-00019e20: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
-00019e30: 790a 2020 2020 6461 313a 2078 6172 7261  y.    da1: xarra
-00019e40: 792e 4461 7461 4172 7261 790a 0a20 2020  y.DataArray..   
-00019e50: 2052 6574 7572 6e0a 2020 2020 2d2d 2d2d   Return.    ----
-00019e60: 2d2d 0a20 2020 2062 6f6f 6c0a 2020 2020  --.    bool.    
-00019e70: 2222 220a 2020 2020 2320 5374 616e 6461  """.    # Standa
-00019e80: 7264 206e 616d 650a 2020 2020 6966 205f  rd name.    if _
-00019e90: 7361 6d65 5f61 7474 725f 2864 6130 2c20  same_attr_(da0, 
-00019ea0: 6461 312c 2022 7374 616e 6461 7264 5f6e  da1, "standard_n
-00019eb0: 616d 6522 293a 0a20 2020 2020 2020 2072  ame"):.        r
-00019ec0: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
-00019ed0: 2320 4366 206e 616d 650a 2020 2020 6366  # Cf name.    cf
-00019ee0: 3020 3d20 6765 745f 6d61 7463 6869 6e67  0 = get_matching
-00019ef0: 5f69 7465 6d5f 7370 6563 7328 6461 3029  _item_specs(da0)
-00019f00: 0a20 2020 2063 6631 203d 2067 6574 5f6d  .    cf1 = get_m
-00019f10: 6174 6368 696e 675f 6974 656d 5f73 7065  atching_item_spe
-00019f20: 6373 2864 6131 290a 2020 2020 6966 2063  cs(da1).    if c
-00019f30: 6630 2061 6e64 2063 6631 2061 6e64 2063  f0 and cf1 and c
-00019f40: 6630 2e6e 616d 6520 3d3d 2063 6631 2e6e  f0.name == cf1.n
-00019f50: 616d 653a 0a20 2020 2020 2020 2072 6574  ame:.        ret
-00019f60: 7572 6e20 5472 7565 0a0a 2020 2020 2320  urn True..    # 
-00019f70: 4e61 6d65 0a20 2020 2069 6620 6461 302e  Name.    if da0.
-00019f80: 6e61 6d65 2061 6e64 2064 6130 2e6e 616d  name and da0.nam
-00019f90: 6520 616e 6420 6461 302e 6e61 6d65 203d  e and da0.name =
-00019fa0: 3d20 6461 312e 6e61 6d65 3a0a 2020 2020  = da1.name:.    
-00019fb0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-00019fc0: 0a20 2020 2023 204c 6f6e 6720 6e61 6d65  .    # Long name
-00019fd0: 0a20 2020 2072 6574 7572 6e20 5f73 616d  .    return _sam
-00019fe0: 655f 6174 7472 5f28 6461 302c 2064 6131  e_attr_(da0, da1
-00019ff0: 2c20 226c 6f6e 675f 6e61 6d65 2229 0a0a  , "long_name")..
-0001a000: 0a64 6566 2073 6561 7263 685f 7369 6d69  .def search_simi
-0001a010: 6c61 7228 6f62 6a2c 2064 6129 3a0a 2020  lar(obj, da):.  
-0001a020: 2020 2222 2253 6561 7263 6820 696e 2064    """Search in d
-0001a030: 7320 666f 7220 6120 7369 6d69 6c61 7220  s for a similar 
-0001a040: 4461 7461 4172 7261 790a 0a20 2020 2053  DataArray..    S
-0001a050: 6565 203a 6675 6e63 3a60 6973 5f73 696d  ee :func:`is_sim
-0001a060: 696c 6172 6020 666f 7220 7768 6174 206d  ilar` for what m
-0001a070: 6561 6e73 2022 7369 6d69 6c61 7222 2e0a  eans "similar"..
-0001a080: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-0001a090: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0001a0a0: 2020 206f 626a 3a20 7861 7272 6179 2e44     obj: xarray.D
-0001a0b0: 6174 6173 6574 2c20 7861 7272 6179 2e44  ataset, xarray.D
-0001a0c0: 6174 6141 7272 6179 0a20 2020 2020 2020  ataArray.       
-0001a0d0: 2044 6174 6173 6574 2074 6861 7420 6d75   Dataset that mu
-0001a0e0: 7374 2062 6520 7363 616e 6e65 642e 0a20  st be scanned.. 
-0001a0f0: 2020 2064 613a 2078 6172 7261 792e 4461     da: xarray.Da
-0001a100: 7461 4172 7261 790a 2020 2020 2020 2020  taArray.        
-0001a110: 4172 7261 7920 7468 6174 206d 7573 7420  Array that must 
-0001a120: 6265 2063 6f6d 7061 7265 6420 746f 2074  be compared to t
-0001a130: 6865 2063 6f6e 7465 6e74 206f 6620 6060  he content of ``
-0001a140: 6473 6060 0a0a 2020 2020 5265 7475 726e  ds``..    Return
-0001a150: 0a20 2020 202d 2d2d 2d2d 2d0a 2020 2020  .    ------.    
-0001a160: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-0001a170: 206f 7220 4e6f 6e65 0a0a 2020 2020 5365   or None..    Se
-0001a180: 6520 616c 736f 0a20 2020 202d 2d2d 2d2d  e also.    -----
-0001a190: 2d2d 2d0a 2020 2020 6973 5f73 696d 696c  ---.    is_simil
-0001a1a0: 6172 0a20 2020 2067 6574 5f6d 6174 6368  ar.    get_match
-0001a1b0: 696e 675f 6974 656d 5f73 7065 6373 0a20  ing_item_specs. 
-0001a1c0: 2020 2022 2222 0a20 2020 2074 6172 6765     """.    targe
-0001a1d0: 7473 203d 205f 6c69 7374 5f78 725f 6e61  ts = _list_xr_na
-0001a1e0: 6d65 735f 2864 612c 2064 6174 615f 7661  mes_(da, data_va
-0001a1f0: 7273 3d46 616c 7365 290a 2020 2020 666f  rs=False).    fo
-0001a200: 7220 6473 5f64 6120 696e 2074 6172 6765  r ds_da in targe
-0001a210: 7473 3a0a 2020 2020 2020 2020 6966 2061  ts:.        if a
-0001a220: 7265 5f73 696d 696c 6172 2864 735f 6461  re_similar(ds_da
-0001a230: 2c20 6461 293a 0a20 2020 2020 2020 2020  , da):.         
-0001a240: 2020 2072 6574 7572 6e20 6473 5f64 610a     return ds_da.
-0001a250: 0a0a 636c 6173 7320 7365 745f 6366 5f73  ..class set_cf_s
-0001a260: 7065 6373 286f 626a 6563 7429 3a0a 2020  pecs(object):.  
-0001a270: 2020 2222 2253 6574 2074 6865 2063 7572    """Set the cur
-0001a280: 7265 6e74 2043 4620 7370 6563 730a 0a20  rent CF specs.. 
-0001a290: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0001a2a0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0001a2b0: 2063 665f 736f 7572 6365 3a20 4346 5370   cf_source: CFSp
-0001a2c0: 6563 732c 2073 7472 2c20 6c69 7374 2c20  ecs, str, list, 
-0001a2d0: 6469 6374 0a20 2020 2020 2020 2045 6974  dict.        Eit
-0001a2e0: 6865 7220 6120 3a63 6c61 7373 3a60 4346  her a :class:`CF
-0001a2f0: 5370 6563 7360 2069 6e73 7461 6e63 6520  Specs` instance 
-0001a300: 6f72 2074 6865 206e 616d 6520 6f66 2061  or the name of a
-0001a310: 2072 6567 6973 7465 7265 6420 6f6e 652c   registered one,
-0001a320: 0a20 2020 2020 2020 206f 7220 616e 2061  .        or an a
-0001a330: 7267 756d 656e 7420 746f 2069 6e73 7461  rgument to insta
-0001a340: 6e74 6961 6e74 6520 6f6e 652e 0a0a 2020  ntiante one...  
-0001a350: 2020 5365 6520 616c 736f 0a20 2020 202d    See also.    -
-0001a360: 2d2d 2d2d 2d2d 2d0a 2020 2020 6765 745f  -------.    get_
-0001a370: 6366 5f73 7065 6373 0a20 2020 2072 6567  cf_specs.    reg
-0001a380: 6973 7465 725f 6366 5f73 7065 6373 0a20  ister_cf_specs. 
-0001a390: 2020 2067 6574 5f72 6567 6973 7465 7265     get_registere
-0001a3a0: 645f 6366 5f73 7065 6373 0a20 2020 2022  d_cf_specs.    "
-0001a3b0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
-0001a3c0: 6974 5f5f 2873 656c 662c 2063 665f 736f  it__(self, cf_so
-0001a3d0: 7572 6365 293a 0a20 2020 2020 2020 2069  urce):.        i
-0001a3e0: 6620 6973 696e 7374 616e 6365 2863 665f  f isinstance(cf_
-0001a3f0: 736f 7572 6365 2c20 7374 7229 3a0a 2020  source, str):.  
-0001a400: 2020 2020 2020 2020 2020 6366 7370 6563            cfspec
-0001a410: 7320 3d20 6765 745f 6366 5f73 7065 6373  s = get_cf_specs
-0001a420: 5f66 726f 6d5f 6e61 6d65 2863 665f 736f  _from_name(cf_so
-0001a430: 7572 6365 2c20 6572 726f 7273 3d22 6967  urce, errors="ig
-0001a440: 6e6f 7265 2229 0a20 2020 2020 2020 2020  nore").         
-0001a450: 2020 2069 6620 6366 7370 6563 733a 0a20     if cfspecs:. 
-0001a460: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001a470: 665f 736f 7572 6365 203d 2063 6673 7065  f_source = cfspe
-0001a480: 6373 0a20 2020 2020 2020 2069 6620 6e6f  cs.        if no
-0001a490: 7420 6973 696e 7374 616e 6365 2863 665f  t isinstance(cf_
-0001a4a0: 736f 7572 6365 2c20 4346 5370 6563 7329  source, CFSpecs)
-0001a4b0: 3a0a 2020 2020 2020 2020 2020 2020 6366  :.            cf
-0001a4c0: 5f73 6f75 7263 6520 3d20 4346 5370 6563  _source = CFSpec
-0001a4d0: 7328 6366 5f73 6f75 7263 6529 0a20 2020  s(cf_source).   
-0001a4e0: 2020 2020 2073 656c 662e 6366 5f63 6163       self.cf_cac
-0001a4f0: 6865 203d 205f 6765 745f 6361 6368 655f  he = _get_cache_
-0001a500: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0001a510: 6f6c 645f 7370 6563 7320 3d20 7365 6c66  old_specs = self
-0001a520: 2e63 665f 6361 6368 655b 2263 7572 7265  .cf_cache["curre
-0001a530: 6e74 225d 0a20 2020 2020 2020 2073 656c  nt"].        sel
-0001a540: 662e 6366 5f63 6163 6865 5b22 6375 7272  f.cf_cache["curr
-0001a550: 656e 7422 5d20 3d20 7365 6c66 2e73 7065  ent"] = self.spe
-0001a560: 6373 203d 2063 665f 736f 7572 6365 0a0a  cs = cf_source..
-0001a570: 2020 2020 6465 6620 5f5f 656e 7465 725f      def __enter_
-0001a580: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-0001a590: 2072 6574 7572 6e20 7365 6c66 2e73 7065   return self.spe
-0001a5a0: 6373 0a0a 2020 2020 6465 6620 5f5f 6578  cs..    def __ex
-0001a5b0: 6974 5f5f 2873 656c 662c 2065 7863 5f74  it__(self, exc_t
-0001a5c0: 7970 652c 2065 7863 5f76 616c 7565 2c20  ype, exc_value, 
-0001a5d0: 7472 6163 6562 6163 6b29 3a0a 2020 2020  traceback):.    
-0001a5e0: 2020 2020 6966 2073 656c 662e 6f6c 645f      if self.old_
-0001a5f0: 7370 6563 7320 6973 204e 6f6e 653a 0a20  specs is None:. 
-0001a600: 2020 2020 2020 2020 2020 2064 656c 2073             del s
-0001a610: 656c 662e 6366 5f63 6163 6865 5b22 6375  elf.cf_cache["cu
-0001a620: 7272 656e 7422 5d0a 2020 2020 2020 2020  rrent"].        
-0001a630: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00018e60: 2020 6d73 6720 3d20 6622 4d75 6c74 6970    msg = f"Multip
+00018e70: 6c65 2063 616e 6469 6461 7465 7320 6469  le candidates di
+00018e80: 6d65 6e73 696f 6e73 206d 6174 6368 696e  mensions matchin
+00018e90: 673a 207b 6366 5f61 7267 7d22 0a20 2020  g: {cf_arg}".   
+00018ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018eb0: 2020 2020 2069 6620 6572 726f 7273 203d       if errors =
+00018ec0: 3d20 2272 6169 7365 223a 0a20 2020 2020  = "raise":.     
+00018ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ee0: 2020 2020 2020 2072 6169 7365 2058 6f61         raise Xoa
+00018ef0: 4346 4572 726f 7228 6d73 6729 0a20 2020  CFError(msg).   
+00018f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f10: 2020 2020 2078 6f61 5f77 6172 6e28 6d73       xoa_warn(ms
+00018f20: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
+00018f30: 2020 2020 2020 2073 6361 6e6e 6564 5b63         scanned[c
+00018f40: 665f 6172 675d 203d 2064 696d 5b30 5d0a  f_arg] = dim[0].
+00018f50: 0a20 2020 2020 2020 2076 616c 7565 7320  .        values 
+00018f60: 3d20 7475 706c 6528 7363 616e 6e65 642e  = tuple(scanned.
+00018f70: 7661 6c75 6573 2829 290a 2020 2020 2020  values()).      
+00018f80: 2020 6966 2073 696e 676c 655f 6172 6720    if single_arg 
+00018f90: 616e 6420 7363 616e 6e65 643a 0a20 2020  and scanned:.   
+00018fa0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00018fb0: 7661 6c75 6573 5b30 5d0a 2020 2020 2020  values[0].      
+00018fc0: 2020 7265 7475 726e 2076 616c 7565 730a    return values.
+00018fd0: 0a20 2020 2064 6566 2067 6574 5f72 656e  .    def get_ren
+00018fe0: 616d 655f 6469 6d73 5f61 7267 7328 7365  ame_dims_args(se
+00018ff0: 6c66 2c20 6f62 6a2c 206c 6f63 6174 696f  lf, obj, locatio
+00019000: 6e73 3d4e 6f6e 652c 2073 7065 6369 616c  ns=None, special
+00019010: 697a 653d 4661 6c73 6529 3a0a 2020 2020  ize=False):.    
+00019020: 2020 2020 2222 2247 6574 2061 7267 7320      """Get args 
+00019030: 666f 7220 7265 6e61 6d69 6e67 2064 696d  for renaming dim
+00019040: 656e 7369 6f6e 7320 7468 6174 2061 7265  ensions that are
+00019050: 206e 6f74 2063 6f6f 7264 696e 6174 6573   not coordinates
+00019060: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00019070: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00019080: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00019090: 6f62 6a3a 2078 6172 7261 792e 4461 7461  obj: xarray.Data
+000190a0: 4172 7261 792c 2078 6172 7261 792e 4461  Array, xarray.Da
+000190b0: 7461 7365 740a 2020 2020 2020 2020 2020  taset.          
+000190c0: 2020 4172 7261 7920 6f72 2064 6174 6173    Array or datas
+000190d0: 6574 0a20 2020 2020 2020 206c 6f63 6174  et.        locat
+000190e0: 696f 6e73 3a20 6469 6374 2c20 4e6f 6e65  ions: dict, None
+000190f0: 0a20 2020 2020 2020 2020 2020 2044 6963  .            Dic
+00019100: 7420 6f66 2073 7461 6767 6572 6420 6772  t of staggerd gr
+00019110: 6964 206c 6f63 6174 696f 6e73 2077 6974  id locations wit
+00019120: 6820 6e61 6d65 7320 6173 206b 6579 730a  h names as keys.
+00019130: 2020 2020 2020 2020 7370 6563 6961 6c69          speciali
+00019140: 7a65 3a20 626f 6f6c 0a20 2020 2020 2020  ze: bool.       
+00019150: 2020 2020 2044 6f20 6e6f 7420 7573 6520       Do not use 
+00019160: 7468 6520 4346 206e 616d 6520 666f 7220  the CF name for 
+00019170: 7265 6e61 6d69 6e67 2c20 6275 7420 7468  renaming, but th
+00019180: 6520 6669 7273 7420 6e61 6d65 0a20 2020  e first name.   
+00019190: 2020 2020 2020 2020 2061 7320 6c69 7374           as list
+000191a0: 6564 2069 6e20 7370 6563 732c 2077 6869  ed in specs, whi
+000191b0: 6368 2069 7320 6765 6e65 7261 6c6c 7920  ch is generally 
+000191c0: 6120 7370 6563 6961 6c69 7a65 6420 6f6e  a specialized on
+000191d0: 652c 0a20 2020 2020 2020 2020 2020 206c  e,.            l
+000191e0: 696b 6520 6120 6e61 6d65 2061 646f 7074  ike a name adopt
+000191f0: 6564 2062 7920 7370 6563 6961 6c69 7a65  ed by specialize
+00019200: 6420 6461 7461 7365 742e 0a0a 2020 2020  d dataset...    
+00019210: 2020 2020 5265 7475 726e 0a20 2020 2020      Return.     
+00019220: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
+00019230: 2020 6469 6374 3a0a 2020 2020 2020 2020    dict:.        
+00019240: 2020 2020 4172 6775 6d65 6e74 2063 6f6d      Argument com
+00019250: 7061 7469 626c 6520 7769 7468 203a 6d65  patible with :me
+00019260: 7468 3a60 7861 7272 6179 2e44 6174 6173  th:`xarray.Datas
+00019270: 6574 2e72 656e 616d 6560 0a20 2020 2020  et.rename`.     
+00019280: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00019290: 2320 4765 7420 6c6f 6361 7469 6f6e 2073  # Get location s
+000192a0: 7065 6373 0a20 2020 2020 2020 2069 6620  pecs.        if 
+000192b0: 6c6f 6361 7469 6f6e 7320 6973 204e 6f6e  locations is Non
+000192c0: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
+000192d0: 6f63 6174 696f 6e73 203d 2073 656c 662e  ocations = self.
+000192e0: 6765 745f 6c6f 635f 6d61 7070 696e 6728  get_loc_mapping(
+000192f0: 6f62 6a29 0a0a 2020 2020 2020 2020 2320  obj)..        # 
+00019300: 4c6f 6f70 206f 6e20 6469 6d73 0a20 2020  Loop on dims.   
+00019310: 2020 2020 2072 656e 616d 655f 6172 6773       rename_args
+00019320: 203d 207b 7d0a 2020 2020 2020 2020 666f   = {}.        fo
+00019330: 7220 6469 6d20 696e 206f 626a 2e64 696d  r dim in obj.dim
+00019340: 733a 0a0a 2020 2020 2020 2020 2020 2020  s:..            
+00019350: 2320 536b 6970 2065 6666 6563 7469 7665  # Skip effective
+00019360: 2063 6f6f 7264 696e 6174 6520 6469 6d73   coordinate dims
+00019370: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00019380: 6469 6d20 696e 206f 626a 2e63 6f6f 7264  dim in obj.coord
+00019390: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000193a0: 2020 2063 6f6e 7469 6e75 650a 0a20 2020     continue..   
+000193b0: 2020 2020 2020 2020 2023 2049 7320 6974           # Is it
+000193c0: 206b 6e6f 776e 3f0a 2020 2020 2020 2020   known?.        
+000193d0: 2020 2020 6366 5f64 696d 5f6e 616d 6520      cf_dim_name 
+000193e0: 3d20 7365 6c66 2e6d 6174 6368 5f66 726f  = self.match_fro
+000193f0: 6d5f 6e61 6d65 2864 696d 2920 2023 206b  m_name(dim)  # k
+00019400: 6e6f 776e 2063 6f6f 7264 696e 6174 6520  nown coordinate 
+00019410: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+00019420: 2064 696d 5f74 7970 6520 3d20 7365 6c66   dim_type = self
+00019430: 2e67 6574 5f64 696d 5f74 7970 6528 6469  .get_dim_type(di
+00019440: 6d2c 206f 626a 2920 2023 206b 6e6f 776e  m, obj)  # known
+00019450: 2064 696d 656e 7369 6f6e 2074 7970 650a   dimension type.
+00019460: 2020 2020 2020 2020 2020 2020 6469 6d5f              dim_
+00019470: 6c6f 6320 3d20 6c6f 6361 7469 6f6e 732e  loc = locations.
+00019480: 6765 7428 6469 6d29 0a0a 2020 2020 2020  get(dim)..      
+00019490: 2020 2020 2020 2320 526f 6f74 206e 616d        # Root nam
+000194a0: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+000194b0: 2063 665f 6469 6d5f 6e61 6d65 3a0a 2020   cf_dim_name:.  
+000194c0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+000194d0: 775f 6e61 6d65 203d 2073 656c 662e 6765  w_name = self.ge
+000194e0: 745f 6e61 6d65 2863 665f 6469 6d5f 6e61  t_name(cf_dim_na
+000194f0: 6d65 2c20 7370 6563 6961 6c69 7a65 3d73  me, specialize=s
+00019500: 7065 6369 616c 697a 6529 0a20 2020 2020  pecialize).     
+00019510: 2020 2020 2020 2065 6c69 6620 6469 6d5f         elif dim_
+00019520: 7479 7065 3a0a 2020 2020 2020 2020 2020  type:.          
+00019530: 2020 2020 2020 6e65 775f 6e61 6d65 203d        new_name =
+00019540: 2064 696d 5f74 7970 650a 2020 2020 2020   dim_type.      
+00019550: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00019560: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00019570: 6e61 6d65 203d 2064 696d 0a0a 2020 2020  name = dim..    
+00019580: 2020 2020 2020 2020 2320 4164 6420 6c6f          # Add lo
+00019590: 630a 2020 2020 2020 2020 2020 2020 6966  c.            if
+000195a0: 2064 696d 5f6c 6f63 2069 7320 6e6f 7420   dim_loc is not 
+000195b0: 4661 6c73 653a 0a20 2020 2020 2020 2020  False:.         
+000195c0: 2020 2020 2020 206e 6577 5f6e 616d 6520         new_name 
+000195d0: 3d20 7365 6c66 2e73 676c 6f63 6174 6f72  = self.sglocator
+000195e0: 2e6d 6572 6765 5f61 7474 7228 276e 616d  .merge_attr('nam
+000195f0: 6527 2c20 6469 6d2c 206e 6577 5f6e 616d  e', dim, new_nam
+00019600: 652c 206c 6f63 3d64 696d 5f6c 6f63 290a  e, loc=dim_loc).
+00019610: 0a20 2020 2020 2020 2020 2020 2023 2052  .            # R
+00019620: 6567 6973 7465 7220 6172 670a 2020 2020  egister arg.    
+00019630: 2020 2020 2020 2020 6966 206e 6577 5f6e          if new_n
+00019640: 616d 6520 213d 2064 696d 3a0a 2020 2020  ame != dim:.    
+00019650: 2020 2020 2020 2020 2020 2020 7265 6e61              rena
+00019660: 6d65 5f61 7267 735b 6469 6d5d 203d 206e  me_args[dim] = n
+00019670: 6577 5f6e 616d 650a 0a20 2020 2020 2020  ew_name..       
+00019680: 2072 6574 7572 6e20 7265 6e61 6d65 5f61   return rename_a
+00019690: 7267 730a 0a20 2020 2064 6566 2070 6172  rgs..    def par
+000196a0: 7365 5f64 696d 7328 7365 6c66 2c20 6469  se_dims(self, di
+000196b0: 6d73 2c20 6f62 6a29 3a0a 2020 2020 2020  ms, obj):.      
+000196c0: 2020 2222 2243 6f6e 7665 7274 2066 726f    """Convert fro
+000196d0: 6d20 6765 6e65 7269 6320 6469 6d20 6e61  m generic dim na
+000196e0: 6d65 7320 746f 2073 7065 6369 616c 697a  mes to specializ
+000196f0: 6564 206e 616d 6573 0a0a 2020 2020 2020  ed names..      
+00019700: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00019710: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00019720: 2020 2020 2020 2020 6469 6d73 3a20 7374          dims: st
+00019730: 722c 2074 7570 6c65 2c20 6c69 7374 2c20  r, tuple, list, 
+00019740: 6469 6374 0a20 2020 2020 2020 206f 626a  dict.        obj
+00019750: 3a20 7861 7272 6179 2e44 6174 6173 6574  : xarray.Dataset
+00019760: 2c20 7861 7272 6179 2e44 6174 6141 7272  , xarray.DataArr
+00019770: 6179 0a0a 2020 2020 2020 2020 5265 7475  ay..        Retu
+00019780: 726e 0a20 2020 2020 2020 202d 2d2d 2d2d  rn.        -----
+00019790: 2d0a 2020 2020 2020 2020 5361 6d65 2074  -.        Same t
+000197a0: 7970 6520 6173 2064 696d 730a 2020 2020  ype as dims.    
+000197b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000197c0: 2320 6469 6d5f 7479 7065 7320 3d20 7365  # dim_types = se
+000197d0: 6c66 2e67 6574 5f64 696d 5f74 7970 6573  lf.get_dim_types
+000197e0: 286f 626a 2c20 6173 6469 6374 3d54 7275  (obj, asdict=Tru
+000197f0: 6529 0a0a 2020 2020 2020 2020 6465 6620  e)..        def 
+00019800: 5f70 6172 7365 5f64 696d 5f28 6366 5f61  _parse_dim_(cf_a
+00019810: 7267 293a 0a20 2020 2020 2020 2020 2020  rg):.           
+00019820: 2069 6620 6366 5f61 7267 2069 6e20 6f62   if cf_arg in ob
+00019830: 6a2e 6469 6d73 3a0a 2020 2020 2020 2020  j.dims:.        
+00019840: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00019850: 665f 6172 670a 2020 2020 2020 2020 2020  f_arg.          
+00019860: 2020 6469 6d20 3d20 7365 6c66 2e73 6561    dim = self.sea
+00019870: 7263 685f 6469 6d28 6f62 6a2c 2063 665f  rch_dim(obj, cf_
+00019880: 6172 6729 0a20 2020 2020 2020 2020 2020  arg).           
+00019890: 2069 6620 6e6f 7420 6469 6d3a 0a20 2020   if not dim:.   
+000198a0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+000198b0: 7365 2058 6f61 4346 4572 726f 7228 6622  se XoaCFError(f"
+000198c0: 496e 7661 6c69 6420 6172 6775 6d65 6e74  Invalid argument
+000198d0: 2066 6f72 2064 696d 656e 7369 6f6e 3a20   for dimension: 
+000198e0: 7b63 665f 6172 677d 2229 0a20 2020 2020  {cf_arg}").     
+000198f0: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
+00019900: 6d0a 0a20 2020 2020 2020 2069 6620 6973  m..        if is
+00019910: 696e 7374 616e 6365 2864 696d 732c 2073  instance(dims, s
+00019920: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00019930: 2072 6574 7572 6e20 5f70 6172 7365 5f64   return _parse_d
+00019940: 696d 5f28 6469 6d73 290a 2020 2020 2020  im_(dims).      
+00019950: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00019960: 6469 6d73 2c20 6469 6374 293a 0a20 2020  dims, dict):.   
+00019970: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00019980: 6469 6374 2828 5f70 6172 7365 5f64 696d  dict((_parse_dim
+00019990: 5f28 6469 6d29 2c20 7661 6c75 6529 2066  _(dim), value) f
+000199a0: 6f72 2064 696d 2c20 7661 6c75 6520 696e  or dim, value in
+000199b0: 2064 696d 732e 6974 656d 7328 2929 0a20   dims.items()). 
+000199c0: 2020 2020 2020 2072 6574 7572 6e20 7479         return ty
+000199d0: 7065 2864 696d 7329 285f 7061 7273 655f  pe(dims)(_parse_
+000199e0: 6469 6d5f 2864 696d 2920 666f 7220 6469  dim_(dim) for di
+000199f0: 6d20 696e 2064 696d 7329 0a0a 0a66 6f72  m in dims)...for
+00019a00: 206d 6574 6820 696e 2028 2767 6574 5f61   meth in ('get_a
+00019a10: 7869 7327 2c20 2767 6574 5f64 696d 5f74  xis', 'get_dim_t
+00019a20: 7970 6527 2c20 2767 6574 5f64 696d 5f74  ype', 'get_dim_t
+00019a30: 7970 6573 272c 2027 7365 6172 6368 5f64  ypes', 'search_d
+00019a40: 696d 272c 2027 6765 745f 6469 6d73 2729  im', 'get_dims')
+00019a50: 3a0a 2020 2020 646f 6320 3d20 6765 7461  :.    doc = geta
+00019a60: 7474 7228 4346 436f 6f72 6453 7065 6373  ttr(CFCoordSpecs
+00019a70: 2c20 6d65 7468 292e 5f5f 646f 635f 5f0a  , meth).__doc__.
+00019a80: 2020 2020 6765 7461 7474 7228 4346 5370      getattr(CFSp
+00019a90: 6563 732c 206d 6574 6829 2e5f 5f64 6f63  ecs, meth).__doc
+00019aa0: 5f5f 203d 2064 6f63 0a0a 0a64 6566 205f  __ = doc...def _
+00019ab0: 6765 745f 6366 676d 5f28 293a 0a20 2020  get_cfgm_():.   
+00019ac0: 2022 2222 4765 7420 6120 3a63 6c61 7373   """Get a :class
+00019ad0: 3a60 7e78 6f61 2e63 6667 6d2e 436f 6e66  :`~xoa.cfgm.Conf
+00019ae0: 6967 4d61 6e61 6765 7260 2069 6e73 7461  igManager` insta
+00019af0: 6e63 6520 746f 206d 616e 6167 650a 2020  nce to manage.  
+00019b00: 2020 636f 6f72 6473 2061 6e64 2064 6174    coords and dat
+00019b10: 615f 7661 7273 2073 70c3 a963 6966 6963  a_vars sp..cific
+00019b20: 6174 696f 6e73 2222 220a 2020 2020 6366  ations""".    cf
+00019b30: 5f63 6163 6865 203d 205f 6765 745f 6361  _cache = _get_ca
+00019b40: 6368 655f 2829 0a20 2020 2069 6620 2263  che_().    if "c
+00019b50: 6667 6d22 206e 6f74 2069 6e20 6366 5f63  fgm" not in cf_c
+00019b60: 6163 6865 3a0a 2020 2020 2020 2020 6672  ache:.        fr
+00019b70: 6f6d 202e 6366 676d 2069 6d70 6f72 7420  om .cfgm import 
+00019b80: 436f 6e66 6967 4d61 6e61 6765 720a 0a20  ConfigManager.. 
+00019b90: 2020 2020 2020 2063 665f 6361 6368 655b         cf_cache[
+00019ba0: 2263 6667 6d22 5d20 3d20 436f 6e66 6967  "cfgm"] = Config
+00019bb0: 4d61 6e61 6765 7228 5f49 4e49 4649 4c45  Manager(_INIFILE
+00019bc0: 290a 2020 2020 7265 7475 726e 2063 665f  ).    return cf_
+00019bd0: 6361 6368 655b 2263 6667 6d22 5d0a 0a0a  cache["cfgm"]...
+00019be0: 6465 6620 6765 745f 6d61 7463 6869 6e67  def get_matching
+00019bf0: 5f69 7465 6d5f 7370 6563 7328 6461 2c20  _item_specs(da, 
+00019c00: 6c6f 633d 2261 6e79 2229 3a0a 2020 2020  loc="any"):.    
+00019c10: 2222 2247 6574 2074 6865 2069 7465 6d20  """Get the item 
+00019c20: 4346 2073 7065 6373 2074 6861 7420 6d61  CF specs that ma
+00019c30: 7463 6820 7468 6973 2064 6174 6120 6172  tch this data ar
+00019c40: 7261 790a 0a20 2020 2050 6172 616d 6574  ray..    Paramet
+00019c50: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00019c60: 2d2d 0a20 2020 2064 613a 2078 6172 7261  --.    da: xarra
+00019c70: 792e 4461 7461 4172 7261 790a 0a20 2020  y.DataArray..   
+00019c80: 2052 6574 7572 6e0a 2020 2020 2d2d 2d2d   Return.    ----
+00019c90: 2d2d 0a20 2020 2064 6963 7420 6f72 204e  --.    dict or N
+00019ca0: 6f6e 650a 0a20 2020 2053 6565 2061 6c73  one..    See als
+00019cb0: 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  o.    --------. 
+00019cc0: 2020 2043 4653 7065 6373 2e6d 6174 6368     CFSpecs.match
+00019cd0: 0a20 2020 2022 2222 0a20 2020 2063 6673  .    """.    cfs
+00019ce0: 7065 6373 203d 2067 6574 5f63 665f 7370  pecs = get_cf_sp
+00019cf0: 6563 7328 6461 290a 2020 2020 6361 742c  ecs(da).    cat,
+00019d00: 206e 616d 6520 3d20 6366 7370 6563 732e   name = cfspecs.
+00019d10: 6d61 7463 6828 6461 2c20 6c6f 633d 6c6f  match(da, loc=lo
+00019d20: 6329 0a20 2020 2069 6620 6361 743a 0a20  c).    if cat:. 
+00019d30: 2020 2020 2020 2072 6574 7572 6e20 6366         return cf
+00019d40: 7370 6563 735b 6361 745d 5b6e 616d 655d  specs[cat][name]
+00019d50: 0a0a 0a64 6566 205f 7361 6d65 5f61 7474  ...def _same_att
+00019d60: 725f 2864 6130 2c20 6461 312c 2061 7474  r_(da0, da1, att
+00019d70: 7229 3a0a 2020 2020 7265 7475 726e 2028  r):.    return (
+00019d80: 0a20 2020 2020 2020 2061 7474 7220 696e  .        attr in
+00019d90: 2064 6130 2e61 7474 7273 0a20 2020 2020   da0.attrs.     
+00019da0: 2020 2061 6e64 2061 7474 7220 696e 2064     and attr in d
+00019db0: 6131 2e61 7474 7273 0a20 2020 2020 2020  a1.attrs.       
+00019dc0: 2061 6e64 2064 6130 2e61 7474 7273 5b61   and da0.attrs[a
+00019dd0: 7474 725d 2e6c 6f77 6572 2829 203d 3d20  ttr].lower() == 
+00019de0: 6461 312e 6174 7472 735b 6174 7472 5d2e  da1.attrs[attr].
+00019df0: 6c6f 7765 7228 290a 2020 2020 290a 0a0a  lower().    )...
+00019e00: 6465 6620 6172 655f 7369 6d69 6c61 7228  def are_similar(
+00019e10: 6461 302c 2064 6131 293a 0a20 2020 2022  da0, da1):.    "
+00019e20: 2222 4368 6563 6b20 6966 2074 776f 2044  ""Check if two D
+00019e30: 6174 6141 7272 6179 7320 6172 6520 7369  ataArrays are si
+00019e40: 6d69 6c61 720a 0a20 2020 2056 6572 6966  milar..    Verif
+00019e50: 6963 6174 696f 6e73 2061 7265 2070 6572  ications are per
+00019e60: 666f 726d 6564 2069 6e20 7468 6520 666f  formed in the fo
+00019e70: 6c6c 6f77 696e 6720 6f72 6465 723a 0a0a  llowing order:..
+00019e80: 2020 2020 2d20 6060 7374 616e 6461 7264      - ``standard
+00019e90: 5f6e 616d 6560 6020 6174 7472 6962 7574  _name`` attribut
+00019ea0: 652c 0a20 2020 202d 204d 6174 6368 696e  e,.    - Matchin
+00019eb0: 6720 4346 5370 6563 7320 6974 656d 206e  g CFSpecs item n
+00019ec0: 616d 652e 0a20 2020 202d 2060 606e 616d  ame..    - ``nam
+00019ed0: 6560 6020 6174 7472 6962 7574 652e 0a20  e`` attribute.. 
+00019ee0: 2020 202d 2060 606c 6f6e 675f 6e61 6d65     - ``long_name
+00019ef0: 6060 2061 7474 7269 6275 7465 2e0a 0a20  `` attribute... 
+00019f00: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00019f10: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00019f20: 2064 6130 3a20 7861 7272 6179 2e44 6174   da0: xarray.Dat
+00019f30: 6141 7272 6179 0a20 2020 2064 6131 3a20  aArray.    da1: 
+00019f40: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
+00019f50: 0a0a 2020 2020 5265 7475 726e 0a20 2020  ..    Return.   
+00019f60: 202d 2d2d 2d2d 2d0a 2020 2020 626f 6f6c   ------.    bool
+00019f70: 0a20 2020 2022 2222 0a20 2020 2023 2053  .    """.    # S
+00019f80: 7461 6e64 6172 6420 6e61 6d65 0a20 2020  tandard name.   
+00019f90: 2069 6620 5f73 616d 655f 6174 7472 5f28   if _same_attr_(
+00019fa0: 6461 302c 2064 6131 2c20 2273 7461 6e64  da0, da1, "stand
+00019fb0: 6172 645f 6e61 6d65 2229 3a0a 2020 2020  ard_name"):.    
+00019fc0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00019fd0: 0a20 2020 2023 2043 6620 6e61 6d65 0a20  .    # Cf name. 
+00019fe0: 2020 2063 6630 203d 2067 6574 5f6d 6174     cf0 = get_mat
+00019ff0: 6368 696e 675f 6974 656d 5f73 7065 6373  ching_item_specs
+0001a000: 2864 6130 290a 2020 2020 6366 3120 3d20  (da0).    cf1 = 
+0001a010: 6765 745f 6d61 7463 6869 6e67 5f69 7465  get_matching_ite
+0001a020: 6d5f 7370 6563 7328 6461 3129 0a20 2020  m_specs(da1).   
+0001a030: 2069 6620 6366 3020 616e 6420 6366 3120   if cf0 and cf1 
+0001a040: 616e 6420 6366 302e 6e61 6d65 203d 3d20  and cf0.name == 
+0001a050: 6366 312e 6e61 6d65 3a0a 2020 2020 2020  cf1.name:.      
+0001a060: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
+0001a070: 2020 2023 204e 616d 650a 2020 2020 6966     # Name.    if
+0001a080: 2064 6130 2e6e 616d 6520 616e 6420 6461   da0.name and da
+0001a090: 302e 6e61 6d65 2061 6e64 2064 6130 2e6e  0.name and da0.n
+0001a0a0: 616d 6520 3d3d 2064 6131 2e6e 616d 653a  ame == da1.name:
+0001a0b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001a0c0: 5472 7565 0a0a 2020 2020 2320 4c6f 6e67  True..    # Long
+0001a0d0: 206e 616d 650a 2020 2020 7265 7475 726e   name.    return
+0001a0e0: 205f 7361 6d65 5f61 7474 725f 2864 6130   _same_attr_(da0
+0001a0f0: 2c20 6461 312c 2022 6c6f 6e67 5f6e 616d  , da1, "long_nam
+0001a100: 6522 290a 0a0a 6465 6620 7365 6172 6368  e")...def search
+0001a110: 5f73 696d 696c 6172 286f 626a 2c20 6461  _similar(obj, da
+0001a120: 293a 0a20 2020 2022 2222 5365 6172 6368  ):.    """Search
+0001a130: 2069 6e20 6473 2066 6f72 2061 2073 696d   in ds for a sim
+0001a140: 696c 6172 2044 6174 6141 7272 6179 0a0a  ilar DataArray..
+0001a150: 2020 2020 5365 6520 3a66 756e 633a 6069      See :func:`i
+0001a160: 735f 7369 6d69 6c61 7260 2066 6f72 2077  s_similar` for w
+0001a170: 6861 7420 6d65 616e 7320 2273 696d 696c  hat means "simil
+0001a180: 6172 222e 0a0a 2020 2020 5061 7261 6d65  ar"...    Parame
+0001a190: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0001a1a0: 2d2d 2d0a 2020 2020 6f62 6a3a 2078 6172  ---.    obj: xar
+0001a1b0: 7261 792e 4461 7461 7365 742c 2078 6172  ray.Dataset, xar
+0001a1c0: 7261 792e 4461 7461 4172 7261 790a 2020  ray.DataArray.  
+0001a1d0: 2020 2020 2020 4461 7461 7365 7420 7468        Dataset th
+0001a1e0: 6174 206d 7573 7420 6265 2073 6361 6e6e  at must be scann
+0001a1f0: 6564 2e0a 2020 2020 6461 3a20 7861 7272  ed..    da: xarr
+0001a200: 6179 2e44 6174 6141 7272 6179 0a20 2020  ay.DataArray.   
+0001a210: 2020 2020 2041 7272 6179 2074 6861 7420       Array that 
+0001a220: 6d75 7374 2062 6520 636f 6d70 6172 6564  must be compared
+0001a230: 2074 6f20 7468 6520 636f 6e74 656e 7420   to the content 
+0001a240: 6f66 2060 6064 7360 600a 0a20 2020 2052  of ``ds``..    R
+0001a250: 6574 7572 6e0a 2020 2020 2d2d 2d2d 2d2d  eturn.    ------
+0001a260: 0a20 2020 2078 6172 7261 792e 4461 7461  .    xarray.Data
+0001a270: 4172 7261 7920 6f72 204e 6f6e 650a 0a20  Array or None.. 
+0001a280: 2020 2053 6565 2061 6c73 6f0a 2020 2020     See also.    
+0001a290: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069 735f  --------.    is_
+0001a2a0: 7369 6d69 6c61 720a 2020 2020 6765 745f  similar.    get_
+0001a2b0: 6d61 7463 6869 6e67 5f69 7465 6d5f 7370  matching_item_sp
+0001a2c0: 6563 730a 2020 2020 2222 220a 2020 2020  ecs.    """.    
+0001a2d0: 7461 7267 6574 7320 3d20 5f6c 6973 745f  targets = _list_
+0001a2e0: 7872 5f6e 616d 6573 5f28 6461 2c20 6461  xr_names_(da, da
+0001a2f0: 7461 5f76 6172 733d 4661 6c73 6529 0a20  ta_vars=False). 
+0001a300: 2020 2066 6f72 2064 735f 6461 2069 6e20     for ds_da in 
+0001a310: 7461 7267 6574 733a 0a20 2020 2020 2020  targets:.       
+0001a320: 2069 6620 6172 655f 7369 6d69 6c61 7228   if are_similar(
+0001a330: 6473 5f64 612c 2064 6129 3a0a 2020 2020  ds_da, da):.    
+0001a340: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+0001a350: 735f 6461 0a0a 0a63 6c61 7373 2073 6574  s_da...class set
+0001a360: 5f63 665f 7370 6563 7328 6f62 6a65 6374  _cf_specs(object
+0001a370: 293a 0a20 2020 2022 2222 5365 7420 7468  ):.    """Set th
+0001a380: 6520 6375 7272 656e 7420 4346 2073 7065  e current CF spe
+0001a390: 6373 0a0a 2020 2020 5061 7261 6d65 7465  cs..    Paramete
+0001a3a0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+0001a3b0: 2d0a 2020 2020 6366 5f73 6f75 7263 653a  -.    cf_source:
+0001a3c0: 2043 4653 7065 6373 2c20 7374 722c 206c   CFSpecs, str, l
+0001a3d0: 6973 742c 2064 6963 740a 2020 2020 2020  ist, dict.      
+0001a3e0: 2020 4569 7468 6572 2061 203a 636c 6173    Either a :clas
+0001a3f0: 733a 6043 4653 7065 6373 6020 696e 7374  s:`CFSpecs` inst
+0001a400: 616e 6365 206f 7220 7468 6520 6e61 6d65  ance or the name
+0001a410: 206f 6620 6120 7265 6769 7374 6572 6564   of a registered
+0001a420: 206f 6e65 2c0a 2020 2020 2020 2020 6f72   one,.        or
+0001a430: 2061 6e20 6172 6775 6d65 6e74 2074 6f20   an argument to 
+0001a440: 696e 7374 616e 7469 616e 7465 206f 6e65  instantiante one
+0001a450: 2e0a 0a20 2020 2053 6565 2061 6c73 6f0a  ...    See also.
+0001a460: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0001a470: 2067 6574 5f63 665f 7370 6563 730a 2020   get_cf_specs.  
+0001a480: 2020 7265 6769 7374 6572 5f63 665f 7370    register_cf_sp
+0001a490: 6563 730a 2020 2020 6765 745f 7265 6769  ecs.    get_regi
+0001a4a0: 7374 6572 6564 5f63 665f 7370 6563 730a  stered_cf_specs.
+0001a4b0: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
+0001a4c0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0001a4d0: 6366 5f73 6f75 7263 6529 3a0a 2020 2020  cf_source):.    
+0001a4e0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0001a4f0: 6528 6366 5f73 6f75 7263 652c 2073 7472  e(cf_source, str
+0001a500: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+0001a510: 6673 7065 6373 203d 2067 6574 5f63 665f  fspecs = get_cf_
+0001a520: 7370 6563 735f 6672 6f6d 5f6e 616d 6528  specs_from_name(
+0001a530: 6366 5f73 6f75 7263 652c 2065 7272 6f72  cf_source, error
+0001a540: 733d 2269 676e 6f72 6522 290a 2020 2020  s="ignore").    
+0001a550: 2020 2020 2020 2020 6966 2063 6673 7065          if cfspe
+0001a560: 6373 3a0a 2020 2020 2020 2020 2020 2020  cs:.            
+0001a570: 2020 2020 6366 5f73 6f75 7263 6520 3d20      cf_source = 
+0001a580: 6366 7370 6563 730a 2020 2020 2020 2020  cfspecs.        
+0001a590: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+0001a5a0: 6528 6366 5f73 6f75 7263 652c 2043 4653  e(cf_source, CFS
+0001a5b0: 7065 6373 293a 0a20 2020 2020 2020 2020  pecs):.         
+0001a5c0: 2020 2063 665f 736f 7572 6365 203d 2043     cf_source = C
+0001a5d0: 4653 7065 6373 2863 665f 736f 7572 6365  FSpecs(cf_source
+0001a5e0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0001a5f0: 665f 6361 6368 6520 3d20 5f67 6574 5f63  f_cache = _get_c
+0001a600: 6163 6865 5f28 290a 2020 2020 2020 2020  ache_().        
+0001a610: 7365 6c66 2e6f 6c64 5f73 7065 6373 203d  self.old_specs =
+0001a620: 2073 656c 662e 6366 5f63 6163 6865 5b22   self.cf_cache["
+0001a630: 6375 7272 656e 7422 5d0a 2020 2020 2020  current"].      
 0001a640: 2020 7365 6c66 2e63 665f 6361 6368 655b    self.cf_cache[
 0001a650: 2263 7572 7265 6e74 225d 203d 2073 656c  "current"] = sel
-0001a660: 662e 6f6c 645f 7370 6563 730a 0a0a 6465  f.old_specs...de
-0001a670: 6620 7265 7365 745f 6361 6368 6528 6469  f reset_cache(di
-0001a680: 736b 3d54 7275 652c 206d 656d 6f72 793d  sk=True, memory=
-0001a690: 4661 6c73 6529 3a0a 2020 2020 2222 2252  False):.    """R
-0001a6a0: 6573 6574 2074 6865 206f 6e20 6469 736b  eset the on disk
-0001a6b0: 2061 6e64 2f6f 7220 696e 206d 656d 6f72   and/or in memor
-0001a6c0: 7920 6366 2073 7065 6373 2063 6163 6865  y cf specs cache
-0001a6d0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-0001a6e0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-0001a6f0: 2020 2020 6469 736b 3a20 626f 6f6c 0a20      disk: bool. 
-0001a700: 2020 2020 2020 2052 656d 6f76 6520 7468         Remove th
-0001a710: 6520 6366 2073 7065 6373 2063 6168 6365  e cf specs cahce
-0001a720: 2066 696c 6520 283a 6461 7461 3a60 5553   file (:data:`US
-0001a730: 4552 5f43 465f 4341 4348 455f 4649 4c45  ER_CF_CACHE_FILE
-0001a740: 6029 0a20 2020 206d 656d 6f72 793a 2062  `).    memory: b
-0001a750: 6f6f 6c0a 2020 2020 2020 2020 5265 6d6f  ool.        Remo
-0001a760: 7665 2074 6865 2069 6e2d 6d65 6d6f 7279  ve the in-memory
-0001a770: 2063 6163 6865 2e0a 0a20 2020 2020 2020   cache...       
-0001a780: 202e 2e20 7761 726e 696e 673a 3a20 5468   .. warning:: Th
-0001a790: 6973 206d 6179 206c 6561 6420 746f 2075  is may lead to u
-0001a7a0: 6e70 7265 6469 6374 6564 2062 6568 6176  npredicted behav
-0001a7b0: 696f 7273 2e0a 0a20 2020 2022 2222 0a20  iors...    """. 
-0001a7c0: 2020 2069 6620 6469 736b 2061 6e64 206f     if disk and o
-0001a7d0: 732e 7061 7468 2e65 7869 7374 7328 5553  s.path.exists(US
-0001a7e0: 4552 5f43 465f 4341 4348 455f 4649 4c45  ER_CF_CACHE_FILE
-0001a7f0: 293a 0a20 2020 2020 2020 206f 732e 7265  ):.        os.re
-0001a800: 6d6f 7665 2855 5345 525f 4346 5f43 4143  move(USER_CF_CAC
-0001a810: 4845 5f46 494c 4529 0a0a 2020 2020 6966  HE_FILE)..    if
-0001a820: 206d 656d 6f72 793a 0a20 2020 2020 2020   memory:.       
-0001a830: 2063 665f 6361 6368 6520 3d20 5f67 6574   cf_cache = _get
-0001a840: 5f63 6667 6d5f 2829 0a20 2020 2020 2020  _cfgm_().       
-0001a850: 2063 665f 6361 6368 655b 226c 6f61 6465   cf_cache["loade
-0001a860: 645f 6469 6374 7322 5d2e 636c 6561 7228  d_dicts"].clear(
-0001a870: 290a 2020 2020 2020 2020 6366 5f63 6163  ).        cf_cac
-0001a880: 6865 5b22 6375 7272 656e 7422 5d20 3d20  he["current"] = 
-0001a890: 4e6f 6e65 0a20 2020 2020 2020 2063 665f  None.        cf_
-0001a8a0: 6361 6368 655b 2264 6566 6175 6c74 225d  cache["default"]
-0001a8b0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0001a8c0: 6366 5f63 6163 6865 5b22 7265 6769 7374  cf_cache["regist
-0001a8d0: 6572 6564 225d 2e63 6c65 6172 2829 0a0a  ered"].clear()..
-0001a8e0: 0a64 6566 2073 686f 775f 6361 6368 6528  .def show_cache(
-0001a8f0: 293a 0a20 2020 2022 2222 5368 6f77 2074  ):.    """Show t
-0001a900: 6865 2063 6620 7370 6563 7320 6361 6368  he cf specs cach
-0001a910: 6520 6669 6c65 2222 220a 2020 2020 7072  e file""".    pr
-0001a920: 696e 7428 5553 4552 5f43 465f 4341 4348  int(USER_CF_CACH
-0001a930: 455f 4649 4c45 290a 0a0a 4045 5252 4f52  E_FILE)...@ERROR
-0001a940: 532e 666f 726d 6174 5f66 756e 6374 696f  S.format_functio
-0001a950: 6e5f 646f 6373 7472 696e 670a 6465 6620  n_docstring.def 
-0001a960: 6765 745f 6366 5f73 7065 6373 5f66 726f  get_cf_specs_fro
-0001a970: 6d5f 6e61 6d65 286e 616d 652c 2065 7272  m_name(name, err
-0001a980: 6f72 733d 2277 6172 6e22 293a 0a20 2020  ors="warn"):.   
-0001a990: 2022 2222 4765 7420 6120 7265 6769 7374   """Get a regist
-0001a9a0: 6572 6564 2043 4620 7370 6563 7320 696e  ered CF specs in
-0001a9b0: 7374 616e 6365 2066 726f 6d20 6974 7320  stance from its 
-0001a9c0: 6e61 6d65 0a0a 2020 2020 5061 7261 6d65  name..    Parame
-0001a9d0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0001a9e0: 2d2d 2d0a 2020 2020 6e61 6d65 3a20 7374  ---.    name: st
-0001a9f0: 720a 2020 2020 7b65 7272 6f72 737d 0a0a  r.    {errors}..
-0001aa00: 2020 2020 5265 7475 726e 0a20 2020 202d      Return.    -
-0001aa10: 2d2d 2d2d 2d0a 2020 2020 4346 5370 6563  -----.    CFSpec
-0001aa20: 7320 6f72 204e 6f6e 650a 2020 2020 2020  s or None.      
-0001aa30: 2020 4973 7375 6520 6120 7761 726e 696e    Issue a warnin
-0001aa40: 6720 6966 206e 6f74 2066 6f75 6e64 0a20  g if not found. 
-0001aa50: 2020 2022 2222 0a20 2020 2063 665f 6361     """.    cf_ca
-0001aa60: 6368 6520 3d20 5f67 6574 5f63 6163 6865  che = _get_cache
-0001aa70: 5f28 290a 2020 2020 666f 7220 6366 7370  _().    for cfsp
-0001aa80: 6563 7320 696e 2063 665f 6361 6368 655b  ecs in cf_cache[
-0001aa90: 2272 6567 6973 7465 7265 6422 5d5b 3a3a  "registered"][::
-0001aaa0: 2d31 5d3a 0a20 2020 2020 2020 2069 6620  -1]:.        if 
-0001aab0: 6366 7370 6563 735b 2272 6567 6973 7465  cfspecs["registe
-0001aac0: 7222 5d5b 226e 616d 6522 5d20 616e 6420  r"]["name"] and 
-0001aad0: 6366 7370 6563 735b 2272 6567 6973 7465  cfspecs["registe
-0001aae0: 7222 5d5b 226e 616d 6522 5d20 3d3d 206e  r"]["name"] == n
-0001aaf0: 616d 652e 6c6f 7765 7228 293a 0a20 2020  ame.lower():.   
-0001ab00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001ab10: 6366 7370 6563 730a 2020 2020 6572 726f  cfspecs.    erro
-0001ab20: 7273 203d 2045 5252 4f52 535b 6572 726f  rs = ERRORS[erro
-0001ab30: 7273 5d0a 2020 2020 6d73 6720 3d20 6622  rs].    msg = f"
-0001ab40: 496e 7661 6c69 6420 7265 6769 7374 7261  Invalid registra
-0001ab50: 7469 6f6e 206e 616d 6520 666f 7220 4346  tion name for CF
-0001ab60: 2073 7065 6373 3a20 7b6e 616d 657d 220a   specs: {name}".
-0001ab70: 2020 2020 6966 2065 7272 6f72 7320 3d3d      if errors ==
-0001ab80: 2022 7261 6973 6522 3a0a 2020 2020 2020   "raise":.      
-0001ab90: 2020 7261 6973 6520 586f 6143 4645 7272    raise XoaCFErr
-0001aba0: 6f72 286d 7367 290a 2020 2020 656c 6966  or(msg).    elif
-0001abb0: 2065 7272 6f72 7320 3d3d 2022 7761 726e   errors == "warn
-0001abc0: 223a 0a20 2020 2020 2020 2078 6f61 5f77  ":.        xoa_w
-0001abd0: 6172 6e28 6d73 6729 0a0a 0a64 6566 2067  arn(msg)...def g
-0001abe0: 6574 5f63 665f 7370 6563 735f 656e 636f  et_cf_specs_enco
-0001abf0: 6469 6e67 2864 7329 3a0a 2020 2020 2222  ding(ds):.    ""
-0001ac00: 2247 6574 2074 6865 2060 6063 665f 7370  "Get the ``cf_sp
-0001ac10: 6563 7360 6020 656e 636f 6469 6e67 2076  ecs`` encoding v
-0001ac20: 616c 7565 0a0a 2020 2020 5061 7261 6d65  alue..    Parame
-0001ac30: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0001ac40: 2d2d 2d0a 2020 2020 6473 3a20 7861 7272  ---.    ds: xarr
-0001ac50: 6179 2e44 6174 6141 7272 6179 2c20 7861  ay.DataArray, xa
-0001ac60: 7272 6179 2e44 6174 6173 6574 0a0a 2020  rray.Dataset..  
-0001ac70: 2020 5265 7475 726e 0a20 2020 202d 2d2d    Return.    ---
-0001ac80: 2d2d 2d0a 2020 2020 7374 7220 6f72 204e  ---.    str or N
-0001ac90: 6f6e 650a 0a20 2020 2053 6565 2061 6c73  one..    See als
-0001aca0: 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  o.    --------. 
-0001acb0: 2020 2067 6574 5f63 665f 7370 6563 735f     get_cf_specs_
-0001acc0: 6672 6f6d 5f65 6e63 6f64 696e 670a 2020  from_encoding.  
-0001acd0: 2020 2222 220a 2020 2020 6966 2064 7320    """.    if ds 
-0001ace0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-0001acf0: 6e6f 7420 6973 696e 7374 616e 6365 2864  not isinstance(d
-0001ad00: 732c 2073 7472 293a 0a20 2020 2020 2020  s, str):.       
-0001ad10: 2066 6f72 2073 6f75 7263 6520 696e 2064   for source in d
-0001ad20: 732e 656e 636f 6469 6e67 2c20 6473 2e61  s.encoding, ds.a
-0001ad30: 7474 7273 3a0a 2020 2020 2020 2020 2020  ttrs:.          
-0001ad40: 2020 666f 7220 6174 7472 2c20 7661 6c75    for attr, valu
-0001ad50: 6520 696e 2073 6f75 7263 652e 6974 656d  e in source.item
-0001ad60: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-0001ad70: 2020 2020 2069 6620 6174 7472 2e6c 6f77       if attr.low
-0001ad80: 6572 2829 203d 3d20 2263 665f 7370 6563  er() == "cf_spec
-0001ad90: 7322 3a0a 2020 2020 2020 2020 2020 2020  s":.            
-0001ada0: 2020 2020 2020 2020 7265 7475 726e 2076          return v
-0001adb0: 616c 7565 0a0a 0a64 6566 2067 6574 5f63  alue...def get_c
-0001adc0: 665f 7370 6563 735f 6672 6f6d 5f65 6e63  f_specs_from_enc
-0001add0: 6f64 696e 6728 6473 293a 0a20 2020 2022  oding(ds):.    "
-0001ade0: 2222 4765 7420 6120 7265 6769 7374 6572  ""Get a register
-0001adf0: 6564 2043 4620 7370 6563 7320 696e 7374  ed CF specs inst
-0001ae00: 616e 6365 2066 726f 6d20 7468 6520 6060  ance from the ``
-0001ae10: 6366 5f73 7065 6373 6060 2065 6e63 6f64  cf_specs`` encod
-0001ae20: 696e 6720 7661 6c75 650a 0a20 2020 2050  ing value..    P
-0001ae30: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-0001ae40: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 733a  --------.    ds:
-0001ae50: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
-0001ae60: 792c 2078 6172 7261 792e 4461 7461 7365  y, xarray.Datase
-0001ae70: 740a 0a20 2020 2052 6574 7572 6e0a 2020  t..    Return.  
-0001ae80: 2020 2d2d 2d2d 2d2d 0a20 2020 2043 4653    ------.    CFS
-0001ae90: 7065 6373 206f 7220 4e6f 6e65 0a0a 2020  pecs or None..  
-0001aea0: 2020 5365 6520 616c 736f 0a20 2020 202d    See also.    -
-0001aeb0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6765 745f  -------.    get_
-0001aec0: 6366 5f73 7065 6373 5f65 6e63 6f64 696e  cf_specs_encodin
-0001aed0: 670a 2020 2020 2222 220a 2020 2020 6966  g.    """.    if
-0001aee0: 2064 7320 6973 206e 6f74 204e 6f6e 6520   ds is not None 
-0001aef0: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
-0001af00: 6365 2864 732c 2073 7472 293a 0a20 2020  ce(ds, str):.   
-0001af10: 2020 2020 206e 616d 6520 3d20 6765 745f       name = get_
-0001af20: 6366 5f73 7065 6373 5f65 6e63 6f64 696e  cf_specs_encodin
-0001af30: 6728 6473 290a 2020 2020 2020 2020 6966  g(ds).        if
-0001af40: 206e 616d 6520 6973 206e 6f74 204e 6f6e   name is not Non
-0001af50: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0001af60: 6574 7572 6e20 6765 745f 6366 5f73 7065  eturn get_cf_spe
-0001af70: 6373 5f66 726f 6d5f 6e61 6d65 286e 616d  cs_from_name(nam
-0001af80: 652c 2065 7272 6f72 733d 2277 6172 6e22  e, errors="warn"
-0001af90: 290a 0a0a 6465 6620 6765 745f 6465 6661  )...def get_defa
-0001afa0: 756c 745f 6366 5f73 7065 6373 2863 6163  ult_cf_specs(cac
-0001afb0: 6865 3d22 7277 2229 3a0a 2020 2020 2222  he="rw"):.    ""
-0001afc0: 2247 6574 2074 6865 2064 6566 6175 6c74  "Get the default
-0001afd0: 2043 4620 7370 6563 6966 6963 6174 696f   CF specificatio
-0001afe0: 6e73 0a0a 2020 2020 5061 7261 6d65 7465  ns..    Paramete
-0001aff0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-0001b000: 2d0a 2020 2020 6361 6368 653a 2073 7472  -.    cache: str
-0001b010: 2c20 626f 6f6c 2c20 4e6f 6e65 0a20 2020  , bool, None.   
-0001b020: 2020 2020 2043 6163 6865 2064 6566 6175       Cache defau
-0001b030: 6c74 2073 7065 6373 206f 6e20 6469 736b  lt specs on disk
-0001b040: 2077 6974 6820 7069 636b 6c69 6e67 2066   with pickling f
-0001b050: 6f72 2066 6173 7420 6c6f 6164 696e 672e  or fast loading.
-0001b060: 0a20 2020 2020 2020 2049 6620 6060 4e6f  .        If ``No
-0001b070: 6e65 6060 2c20 6974 2064 6566 6175 6c74  ne``, it default
-0001b080: 7320 746f 2062 6f6f 6c65 616e 206f 7074  s to boolean opt
-0001b090: 696f 6e20 3a78 6f61 6f70 7469 6f6e 3a60  ion :xoaoption:`
-0001b0a0: 6366 2e63 6163 6865 602e 0a20 2020 2020  cf.cache`..     
-0001b0b0: 2020 2050 6f73 7369 626c 6520 7374 7269     Possible stri
-0001b0c0: 6e67 2076 616c 7565 733a 2060 6022 6967  ng values: ``"ig
-0001b0d0: 6e6f 7265 2260 602c 2060 6022 7277 2260  nore"``, ``"rw"`
-0001b0e0: 602c 2060 6022 7265 6164 2260 602c 0a20  `, ``"read"``,. 
-0001b0f0: 2020 2020 2020 2060 6022 7772 6974 6522         ``"write"
-0001b100: 6060 2c20 6060 2263 6c65 616e 2260 602e  ``, ``"clean"``.
-0001b110: 0a20 2020 2020 2020 2049 6620 6060 5472  .        If ``Tr
-0001b120: 7565 6060 2c20 6974 2069 7320 7365 7420  ue``, it is set 
-0001b130: 746f 2060 6022 7277 2260 602e 0a20 2020  to ``"rw"``..   
-0001b140: 2020 2020 2049 6620 6060 4661 6c73 6560       If ``False`
-0001b150: 602c 2069 7420 6973 2073 6574 2074 6f20  `, it is set to 
-0001b160: 6060 2269 676e 6f72 6522 6060 2e0a 2020  ``"ignore"``..  
-0001b170: 2020 2222 220a 2020 2020 6966 2063 6163    """.    if cac
-0001b180: 6865 2069 7320 4e6f 6e65 3a0a 2020 2020  he is None:.    
-0001b190: 2020 2020 6361 6368 6520 3d20 6765 745f      cache = get_
-0001b1a0: 6f70 7469 6f6e 2827 6366 2e63 6163 6865  option('cf.cache
-0001b1b0: 2729 0a20 2020 2069 6620 6361 6368 6520  ').    if cache 
-0001b1c0: 6973 2054 7275 653a 0a20 2020 2020 2020  is True:.       
-0001b1d0: 2063 6163 6865 203d 2022 7277 220a 2020   cache = "rw".  
-0001b1e0: 2020 656c 6966 2063 6163 6865 2069 7320    elif cache is 
-0001b1f0: 4661 6c73 653a 0a20 2020 2020 2020 2063  False:.        c
-0001b200: 6163 6865 203d 2022 6967 6e6f 7265 220a  ache = "ignore".
-0001b210: 2020 2020 6173 7365 7274 2063 6163 6865      assert cache
-0001b220: 2069 6e20 2822 6967 6e6f 7265 222c 2022   in ("ignore", "
-0001b230: 7277 222c 2022 7265 6164 222c 2022 7772  rw", "read", "wr
-0001b240: 6974 6522 2c20 2263 6c65 616e 2229 0a20  ite", "clean"). 
-0001b250: 2020 2063 665f 6361 6368 6520 3d20 5f67     cf_cache = _g
-0001b260: 6574 5f63 6163 6865 5f28 290a 2020 2020  et_cache_().    
-0001b270: 6966 2063 665f 6361 6368 655b 2264 6566  if cf_cache["def
-0001b280: 6175 6c74 225d 2069 7320 6e6f 7420 4e6f  ault"] is not No
-0001b290: 6e65 3a0a 2020 2020 2020 2020 7265 7475  ne:.        retu
-0001b2a0: 726e 2063 665f 6361 6368 655b 2264 6566  rn cf_cache["def
-0001b2b0: 6175 6c74 225d 0a20 2020 2063 6673 7065  ault"].    cfspe
-0001b2c0: 6373 203d 204e 6f6e 650a 0a20 2020 2023  cs = None..    #
-0001b2d0: 2054 7279 2066 726f 6d20 6469 736b 2063   Try from disk c
-0001b2e0: 6163 6865 0a20 2020 2069 6620 6361 6368  ache.    if cach
-0001b2f0: 6520 696e 2028 2272 6561 6422 2c20 2272  e in ("read", "r
-0001b300: 7722 293a 0a20 2020 2020 2020 2069 6620  w"):.        if 
-0001b310: 6f73 2e70 6174 682e 6578 6973 7473 2855  os.path.exists(U
-0001b320: 5345 525f 4346 5f43 4143 4845 5f46 494c  SER_CF_CACHE_FIL
-0001b330: 4529 2061 6e64 2028 0a20 2020 2020 2020  E) and (.       
-0001b340: 2020 2020 206f 732e 7374 6174 285f 4346       os.stat(_CF
-0001b350: 4746 494c 4529 2e73 745f 6d74 696d 6520  GFILE).st_mtime 
-0001b360: 3c20 6f73 2e73 7461 7428 5553 4552 5f43  < os.stat(USER_C
-0001b370: 465f 4341 4348 455f 4649 4c45 292e 7374  F_CACHE_FILE).st
-0001b380: 5f6d 7469 6d65 0a20 2020 2020 2020 2029  _mtime.        )
-0001b390: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-0001b3a0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0001b3b0: 2020 2077 6974 6820 6f70 656e 2855 5345     with open(USE
-0001b3c0: 525f 4346 5f43 4143 4845 5f46 494c 452c  R_CF_CACHE_FILE,
-0001b3d0: 2022 7262 2229 2061 7320 663a 0a20 2020   "rb") as f:.   
-0001b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3f0: 2063 6673 7065 6373 203d 2070 6963 6b6c   cfspecs = pickl
-0001b400: 652e 6c6f 6164 2866 290a 2020 2020 2020  e.load(f).      
-0001b410: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-0001b420: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
-0001b430: 2020 2020 2020 2020 2020 2020 2078 6f61               xoa
-0001b440: 5f77 6172 6e28 2245 7272 6f72 2077 6869  _warn("Error whi
-0001b450: 6c65 206c 6f61 6469 6e67 2063 6163 6865  le loading cache
-0001b460: 6420 6366 2073 7065 6373 3a20 2220 2b20  d cf specs: " + 
-0001b470: 7374 7228 652e 6172 6773 2929 0a0a 2020  str(e.args))..  
-0001b480: 2020 2320 436f 6d70 7574 6520 6974 2066    # Compute it f
-0001b490: 726f 6d20 7363 7261 7463 680a 2020 2020  rom scratch.    
-0001b4a0: 6966 2063 6673 7065 6373 2069 7320 4e6f  if cfspecs is No
-0001b4b0: 6e65 3a0a 0a20 2020 2020 2020 2023 2053  ne:..        # S
-0001b4c0: 6574 7570 0a20 2020 2020 2020 2063 6673  etup.        cfs
-0001b4d0: 7065 6373 203d 2043 4653 7065 6373 2829  pecs = CFSpecs()
-0001b4e0: 0a0a 2020 2020 2020 2020 2320 4361 6368  ..        # Cach
-0001b4f0: 6520 6974 206f 6e20 6469 736b 0a20 2020  e it on disk.   
-0001b500: 2020 2020 2069 6620 6361 6368 6520 696e       if cache in
-0001b510: 2028 2277 7269 7465 222c 2022 7277 2229   ("write", "rw")
-0001b520: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-0001b530: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0001b540: 2020 2063 6163 6865 6469 7220 3d20 6f73     cachedir = os
-0001b550: 2e70 6174 682e 6469 726e 616d 6528 5553  .path.dirname(US
-0001b560: 4552 5f43 465f 4341 4348 455f 4649 4c45  ER_CF_CACHE_FILE
-0001b570: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001b580: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
-0001b590: 2e65 7869 7374 7328 6361 6368 6564 6972  .exists(cachedir
-0001b5a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001b5b0: 2020 2020 2020 206f 732e 6d61 6b65 6469         os.makedi
-0001b5c0: 7273 2863 6163 6865 6469 7229 0a20 2020  rs(cachedir).   
-0001b5d0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-0001b5e0: 6820 6f70 656e 2855 5345 525f 4346 5f43  h open(USER_CF_C
-0001b5f0: 4143 4845 5f46 494c 452c 2022 7762 2229  ACHE_FILE, "wb")
-0001b600: 2061 7320 663a 0a20 2020 2020 2020 2020   as f:.         
-0001b610: 2020 2020 2020 2020 2020 2070 6963 6b6c             pickl
-0001b620: 652e 6475 6d70 2863 6673 7065 6373 2c20  e.dump(cfspecs, 
-0001b630: 6629 0a20 2020 2020 2020 2020 2020 2065  f).            e
-0001b640: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-0001b650: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-0001b660: 2020 2020 2020 786f 615f 7761 726e 2822        xoa_warn("
-0001b670: 4572 726f 7220 7768 696c 6520 6361 6368  Error while cach
-0001b680: 696e 6720 6366 2073 7065 6373 3a20 2220  ing cf specs: " 
-0001b690: 2b20 7374 7228 652e 6172 6773 2929 0a0a  + str(e.args))..
-0001b6a0: 2020 2020 6366 5f63 6163 6865 5b22 6465      cf_cache["de
-0001b6b0: 6661 756c 7422 5d20 3d20 6366 7370 6563  fault"] = cfspec
-0001b6c0: 730a 2020 2020 6966 206e 6f74 2069 735f  s.    if not is_
-0001b6d0: 7265 6769 7374 6572 6564 5f63 665f 7370  registered_cf_sp
-0001b6e0: 6563 7328 6366 7370 6563 7329 3a0a 2020  ecs(cfspecs):.  
-0001b6f0: 2020 2020 2020 7265 6769 7374 6572 5f63        register_c
-0001b700: 665f 7370 6563 7328 6366 7370 6563 7329  f_specs(cfspecs)
-0001b710: 0a20 2020 2072 6574 7572 6e20 6366 7370  .    return cfsp
-0001b720: 6563 730a 0a0a 6465 6620 6765 745f 6366  ecs...def get_cf
-0001b730: 5f73 7065 6373 286e 616d 653d 4e6f 6e65  _specs(name=None
-0001b740: 2c20 6361 6368 653d 2272 7722 293a 0a20  , cache="rw"):. 
-0001b750: 2020 2022 2222 4765 7420 7468 6520 6375     """Get the cu
-0001b760: 7272 656e 7420 6f72 2061 2072 6567 6973  rrent or a regis
-0001b770: 7465 7265 6420 4346 2073 7065 6369 6669  tered CF specifi
-0001b780: 6361 7469 6f6e 7320 696e 7374 616e 6365  cations instance
-0001b790: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-0001b7a0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-0001b7b0: 2020 2020 6e61 6d65 3a20 7374 722c 2022      name: str, "
-0001b7c0: 6375 7272 656e 7422 2c20 2264 6566 6175  current", "defau
-0001b7d0: 6c74 222c 204e 6f6e 652c 2078 6172 7261  lt", None, xarra
-0001b7e0: 792e 4461 7461 7365 742c 2078 6172 7261  y.Dataset, xarra
-0001b7f0: 792e 4461 7461 4172 7261 790a 2020 2020  y.DataArray.    
-0001b800: 2020 2020 2264 6566 6175 6c74 2220 6d65      "default" me
-0001b810: 616e 7320 7468 6520 6465 6661 756c 7420  ans the default 
-0001b820: 786f 6120 7370 6563 732e 0a20 2020 2020  xoa specs..     
-0001b830: 2020 2022 6375 7272 656e 7422 2069 7320     "current" is 
-0001b840: 6571 7569 7661 6c65 6e74 2074 6f20 4e6f  equivalent to No
-0001b850: 6e65 2061 6e64 206d 6561 6e73 2074 6865  ne and means the
-0001b860: 2063 7572 7265 6e74 7320 7370 6563 732c   currents specs,
-0001b870: 0a20 2020 2020 2020 2077 6869 6368 2064  .        which d
-0001b880: 6566 6175 6c74 7320 746f 2074 6865 2078  efaults to the x
-0001b890: 6f61 2064 6566 6175 6c74 7321 0a20 2020  oa defaults!.   
-0001b8a0: 2020 2020 2045 6c73 6520 7265 6769 7374       Else regist
-0001b8b0: 7261 7469 6f6e 206e 616d 6520 666f 7220  ration name for 
-0001b8c0: 7468 6573 6520 7370 6563 7320 6f72 2061  these specs or a
-0001b8d0: 2064 6174 6120 6172 7261 7920 6f72 2064   data array or d
-0001b8e0: 6174 6173 6574 0a20 2020 2020 2020 2074  ataset.        t
-0001b8f0: 6861 7420 6361 6e20 6265 2075 7365 6420  hat can be used 
-0001b900: 746f 2067 6574 2074 6865 2072 6567 6973  to get the regis
-0001b910: 7472 6174 696f 6e20 6e61 6d65 2069 6620  tration name if 
-0001b920: 6974 2073 6574 2069 6e20 7468 650a 2020  it set in the.  
-0001b930: 2020 2020 2020 3a61 7474 723a 6063 665f        :attr:`cf_
-0001b940: 7370 6563 7360 2061 7474 7269 6275 7465  specs` attribute
-0001b950: 206f 7220 656e 636f 6469 6e67 2e0a 2020   or encoding..  
-0001b960: 2020 2020 2020 5768 656e 2073 6574 2c20        When set, 
-0001b970: 6060 6361 6368 6560 6020 6973 2069 676e  ``cache`` is ign
-0001b980: 6f72 6564 2e0a 2020 2020 2020 2020 5261  ored..        Ra
-0001b990: 6973 6573 2061 203a 636c 6173 733a 6058  ises a :class:`X
-0001b9a0: 6f61 4346 4572 726f 7260 2069 7320 6361  oaCFError` is ca
-0001b9b0: 7365 206f 6620 696e 7661 6c69 6420 6e61  se of invalid na
-0001b9c0: 6d65 2e0a 2020 2020 6361 6368 653a 2073  me..    cache: s
-0001b9d0: 7472 2c20 626f 6f6c 2c20 4e6f 6e65 0a20  tr, bool, None. 
-0001b9e0: 2020 2020 2020 2043 6163 6865 2064 6566         Cache def
-0001b9f0: 6175 6c74 2073 7065 6373 206f 6e20 6469  ault specs on di
-0001ba00: 736b 2077 6974 6820 7069 636b 6c69 6e67  sk with pickling
-0001ba10: 2066 6f72 2066 6173 7420 6c6f 6164 696e   for fast loadin
-0001ba20: 672e 0a20 2020 2020 2020 2049 6620 6060  g..        If ``
-0001ba30: 4e6f 6e65 6060 2c20 6974 2064 6566 6175  None``, it defau
-0001ba40: 6c74 7320 746f 2062 6f6f 6c65 616e 206f  lts to boolean o
-0001ba50: 7074 696f 6e20 3a78 6f61 6f70 7469 6f6e  ption :xoaoption
-0001ba60: 3a60 6366 2e63 6163 6865 602e 0a20 2020  :`cf.cache`..   
-0001ba70: 2020 2020 2050 6f73 7369 626c 6520 7374       Possible st
-0001ba80: 7269 6e67 2076 616c 7565 733a 2060 6022  ring values: ``"
-0001ba90: 6967 6e6f 7265 2260 602c 2060 6022 7277  ignore"``, ``"rw
-0001baa0: 2260 602c 2060 6022 7265 6164 2260 602c  "``, ``"read"``,
-0001bab0: 2060 6022 7772 6974 6522 6060 2e0a 2020   ``"write"``..  
-0001bac0: 2020 2020 2020 4966 2060 6054 7275 6560        If ``True`
-0001bad0: 602c 2069 7420 6973 2073 6574 2074 6f20  `, it is set to 
-0001bae0: 6060 2272 7722 6060 2e0a 2020 2020 2020  ``"rw"``..      
-0001baf0: 2020 4966 2060 6046 616c 7365 6060 2c20    If ``False``, 
-0001bb00: 6974 2069 7320 7365 7420 746f 2060 6022  it is set to ``"
-0001bb10: 6967 6e6f 7265 2260 602e 0a0a 2020 2020  ignore"``...    
-0001bb20: 5265 7475 726e 0a20 2020 202d 2d2d 2d2d  Return.    -----
-0001bb30: 2d0a 2020 2020 4346 5370 6563 730a 2020  -.    CFSpecs.  
-0001bb40: 2020 2020 2020 4e6f 6e65 2069 7320 7265        None is re
-0001bb50: 7475 726e 2069 6620 6e6f 2073 7065 6373  turn if no specs
-0001bb60: 2061 7265 2066 6f75 6e64 0a0a 2020 2020   are found..    
-0001bb70: 5261 6973 650a 2020 2020 2d2d 2d2d 2d0a  Raise.    -----.
-0001bb80: 2020 2020 586f 6143 4645 7272 6f72 0a20      XoaCFError. 
-0001bb90: 2020 2020 2020 2057 6865 6e20 6060 6e61         When ``na
-0001bba0: 6d65 6060 2069 7320 7072 6f76 6964 6564  me`` is provided
-0001bbb0: 2061 7320 6120 7374 7269 6e67 2061 6e64   as a string and
-0001bbc0: 2069 7320 696e 7661 6c69 642e 0a20 2020   is invalid..   
-0001bbd0: 2022 2222 0a20 2020 2023 2045 7870 6c69   """.    # Expli
-0001bbe0: 6369 7420 7265 7175 6573 740a 2020 2020  cit request.    
-0001bbf0: 6966 206e 616d 6520 6973 204e 6f6e 653a  if name is None:
-0001bc00: 0a20 2020 2020 2020 206e 616d 6520 3d20  .        name = 
-0001bc10: 2263 7572 7265 6e74 220a 2020 2020 6966  "current".    if
-0001bc20: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-0001bc30: 6e61 6d65 2c20 7374 7229 206f 7220 6e61  name, str) or na
-0001bc40: 6d65 206e 6f74 2069 6e20 2822 6375 7272  me not in ("curr
-0001bc50: 656e 7422 2c20 2264 6566 6175 6c74 2229  ent", "default")
-0001bc60: 3a0a 0a20 2020 2020 2020 2023 2052 6567  :..        # Reg
-0001bc70: 6973 7465 7265 6420 6e61 6d65 0a20 2020  istered name.   
-0001bc80: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0001bc90: 6365 286e 616d 652c 2073 7472 293a 0a20  ce(name, str):. 
-0001bca0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001bcb0: 6e20 6765 745f 6366 5f73 7065 6373 5f66  n get_cf_specs_f
-0001bcc0: 726f 6d5f 6e61 6d65 286e 616d 652c 2065  rom_name(name, e
-0001bcd0: 7272 6f72 733d 2272 6169 7365 2229 0a0a  rrors="raise")..
-0001bce0: 2020 2020 2020 2020 2320 4e61 6d65 2061          # Name a
-0001bcf0: 7320 6461 7461 7365 7420 6f72 2064 6174  s dataset or dat
-0001bd00: 6120 6172 7261 7920 736f 2077 6520 6775  a array so we gu
-0001bd10: 6573 7320 7468 6520 6e61 6d65 0a20 2020  ess the name.   
-0001bd20: 2020 2020 2063 6673 7065 6373 203d 2067       cfspecs = g
-0001bd30: 6574 5f63 665f 7370 6563 735f 6672 6f6d  et_cf_specs_from
-0001bd40: 5f65 6e63 6f64 696e 6728 6e61 6d65 290a  _encoding(name).
-0001bd50: 2020 2020 2020 2020 6966 2063 6673 7065          if cfspe
-0001bd60: 6373 3a0a 2020 2020 2020 2020 2020 2020  cs:.            
-0001bd70: 7265 7475 726e 2063 6673 7065 6373 0a20  return cfspecs. 
-0001bd80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001bd90: 2020 2020 2020 2020 206e 616d 6520 3d20           name = 
-0001bda0: 2263 7572 7265 6e74 220a 0a20 2020 2023  "current"..    #
-0001bdb0: 204e 6f74 206e 616d 6564 203d 3e20 6375   Not named => cu
-0001bdc0: 7272 656e 7420 6f72 2064 6566 6175 6c74  rrent or default
-0001bdd0: 2073 7065 6373 0a20 2020 2069 6620 6e61   specs.    if na
-0001bde0: 6d65 203d 3d20 2263 7572 7265 6e74 223a  me == "current":
-0001bdf0: 0a20 2020 2020 2020 2063 665f 6361 6368  .        cf_cach
-0001be00: 6520 3d20 5f67 6574 5f63 6163 6865 5f28  e = _get_cache_(
-0001be10: 290a 2020 2020 2020 2020 6966 2063 665f  ).        if cf_
-0001be20: 6361 6368 655b 2263 7572 7265 6e74 225d  cache["current"]
-0001be30: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0001be40: 2020 2020 2020 6366 5f63 6163 6865 5b22        cf_cache["
-0001be50: 6375 7272 656e 7422 5d20 3d20 6765 745f  current"] = get_
-0001be60: 6465 6661 756c 745f 6366 5f73 7065 6373  default_cf_specs
-0001be70: 2829 0a20 2020 2020 2020 2063 6673 7065  ().        cfspe
-0001be80: 6373 203d 2063 665f 6361 6368 655b 2263  cs = cf_cache["c
-0001be90: 7572 7265 6e74 225d 0a20 2020 2065 6c73  urrent"].    els
-0001bea0: 653a 0a20 2020 2020 2020 2063 6673 7065  e:.        cfspe
-0001beb0: 6373 203d 2067 6574 5f64 6566 6175 6c74  cs = get_default
-0001bec0: 5f63 665f 7370 6563 7328 290a 0a20 2020  _cf_specs()..   
-0001bed0: 2072 6574 7572 6e20 6366 7370 6563 730a   return cfspecs.
-0001bee0: 0a0a 6465 6620 7265 6769 7374 6572 5f63  ..def register_c
-0001bef0: 665f 7370 6563 7328 2a61 7267 732c 202a  f_specs(*args, *
-0001bf00: 2a6b 7761 7267 7329 3a0a 2020 2020 2222  *kwargs):.    ""
-0001bf10: 2252 6567 6973 7465 7220 3a63 6c61 7373  "Register :class
-0001bf20: 3a60 4346 5370 6563 7360 2069 6e20 6120  :`CFSpecs` in a 
-0001bf30: 6261 6e6b 206f 7074 696f 6e61 6c6c 7920  bank optionally 
-0001bf40: 7769 7468 2061 206e 616d 6522 2222 0a20  with a name""". 
-0001bf50: 2020 2061 7267 7320 3d20 6c69 7374 2861     args = list(a
-0001bf60: 7267 7329 0a20 2020 2066 6f72 206e 616d  rgs).    for nam
-0001bf70: 652c 2063 6673 7065 6373 2069 6e20 6b77  e, cfspecs in kw
-0001bf80: 6172 6773 2e69 7465 6d73 2829 3a0a 2020  args.items():.  
-0001bf90: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-0001bfa0: 6e73 7461 6e63 6528 6366 7370 6563 732c  nstance(cfspecs,
-0001bfb0: 2043 4653 7065 6373 293a 0a20 2020 2020   CFSpecs):.     
-0001bfc0: 2020 2020 2020 2063 6673 7065 6373 203d         cfspecs =
-0001bfd0: 2043 4653 7065 6373 2863 6673 7065 6373   CFSpecs(cfspecs
-0001bfe0: 290a 2020 2020 2020 2020 6366 7370 6563  ).        cfspec
-0001bff0: 732e 6e61 6d65 203d 206e 616d 650a 2020  s.name = name.  
-0001c000: 2020 2020 2020 6172 6773 2e61 7070 656e        args.appen
-0001c010: 6428 6366 7370 6563 7329 0a20 2020 2066  d(cfspecs).    f
-0001c020: 6f72 2063 6673 7065 6373 2069 6e20 6172  or cfspecs in ar
-0001c030: 6773 3a0a 2020 2020 2020 2020 6966 206e  gs:.        if n
-0001c040: 6f74 2069 7369 6e73 7461 6e63 6528 6366  ot isinstance(cf
-0001c050: 7370 6563 732c 2043 4653 7065 6373 293a  specs, CFSpecs):
-0001c060: 0a20 2020 2020 2020 2020 2020 2063 6673  .            cfs
-0001c070: 7065 6373 203d 2043 4653 7065 6373 2863  pecs = CFSpecs(c
-0001c080: 6673 7065 6373 290a 2020 2020 2020 2020  fspecs).        
-0001c090: 6366 5f63 6163 6865 203d 205f 6765 745f  cf_cache = _get_
-0001c0a0: 6361 6368 655f 2829 0a20 2020 2020 2020  cache_().       
-0001c0b0: 2069 6620 6366 7370 6563 7320 6e6f 7420   if cfspecs not 
-0001c0c0: 696e 2063 665f 6361 6368 655b 2272 6567  in cf_cache["reg
-0001c0d0: 6973 7465 7265 6422 5d3a 0a20 2020 2020  istered"]:.     
-0001c0e0: 2020 2020 2020 2063 665f 6361 6368 655b         cf_cache[
-0001c0f0: 2272 6567 6973 7465 7265 6422 5d2e 6170  "registered"].ap
-0001c100: 7065 6e64 2863 6673 7065 6373 290a 0a0a  pend(cfspecs)...
-0001c110: 6465 6620 6765 745f 7265 6769 7374 6572  def get_register
-0001c120: 6564 5f63 665f 7370 6563 7328 6375 7272  ed_cf_specs(curr
-0001c130: 656e 743d 5472 7565 2c20 7265 7665 7273  ent=True, revers
-0001c140: 653d 5472 7565 2c20 6e61 6d65 643d 4661  e=True, named=Fa
-0001c150: 6c73 6529 3a0a 2020 2020 2222 2247 6574  lse):.    """Get
-0001c160: 2074 6865 206c 6973 7420 6f66 2072 6567   the list of reg
-0001c170: 6973 7465 7265 6420 4346 5370 6563 730a  istered CFSpecs.
-0001c180: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-0001c190: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0001c1a0: 2020 2063 7572 7265 6e74 3a20 626f 6f6c     current: bool
-0001c1b0: 0a20 2020 2020 2020 2041 6c73 6f20 696e  .        Also in
-0001c1c0: 636c 7564 6520 7468 6520 6375 7272 656e  clude the curren
-0001c1d0: 7420 7370 6563 7320 6966 2061 6e79 2c20  t specs if any, 
-0001c1e0: 616c 7761 7973 2061 7420 7468 6520 6c61  always at the la
-0001c1f0: 7374 2070 6f73 6974 696f 6e0a 2020 2020  st position.    
-0001c200: 7265 7665 7273 653a 2062 6f6f 6c0a 2020  reverse: bool.  
-0001c210: 2020 2020 2020 5265 7665 7273 6520 7468        Reverse th
-0001c220: 6520 6c69 7374 0a20 2020 206e 616d 6564  e list.    named
-0001c230: 3a20 626f 6f6c 0a20 2020 2020 2020 204d  : bool.        M
-0001c240: 616b 6520 7375 7265 2074 6865 2072 6574  ake sure the ret
-0001c250: 7572 6e65 6420 4346 5370 6563 7320 6861  urned CFSpecs ha
-0001c260: 7665 2061 2076 616c 6964 2072 6567 6973  ve a valid regis
-0001c270: 7472 6174 696f 6e20 6e61 6d65 0a0a 2020  tration name..  
-0001c280: 2020 5265 7475 726e 0a20 2020 202d 2d2d    Return.    ---
-0001c290: 2d2d 2d0a 2020 2020 6c69 7374 0a0a 2020  ---.    list..  
-0001c2a0: 2020 5365 6520 616c 736f 0a20 2020 202d    See also.    -
-0001c2b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7265 6769  -------.    regi
-0001c2c0: 7374 6572 5f63 665f 7370 6563 730a 2020  ster_cf_specs.  
-0001c2d0: 2020 2222 220a 2020 2020 6366 5f63 6163    """.    cf_cac
-0001c2e0: 6865 203d 205f 6765 745f 6361 6368 655f  he = _get_cache_
-0001c2f0: 2829 0a20 2020 2063 666c 203d 2063 665f  ().    cfl = cf_
-0001c300: 6361 6368 655b 2272 6567 6973 7465 7265  cache["registere
-0001c310: 6422 5d0a 2020 2020 6966 2072 6576 6572  d"].    if rever
-0001c320: 7365 3a0a 2020 2020 2020 2020 6366 6c20  se:.        cfl 
-0001c330: 3d20 6366 6c5b 3a3a 2d31 5d0a 2020 2020  = cfl[::-1].    
-0001c340: 6966 2063 7572 7265 6e74 2061 6e64 2063  if current and c
-0001c350: 665f 6361 6368 655b 2263 7572 7265 6e74  f_cache["current
-0001c360: 225d 2069 7320 6e6f 7420 4e6f 6e65 3a0a  "] is not None:.
-0001c370: 2020 2020 2020 2020 6366 6c2e 6170 7065          cfl.appe
-0001c380: 6e64 2863 665f 6361 6368 655b 2263 7572  nd(cf_cache["cur
-0001c390: 7265 6e74 225d 290a 2020 2020 6966 206e  rent"]).    if n
-0001c3a0: 616d 6564 2069 7320 4661 6c73 653a 0a20  amed is False:. 
-0001c3b0: 2020 2020 2020 2063 6664 6566 203d 2067         cfdef = g
-0001c3c0: 6574 5f64 6566 6175 6c74 5f63 665f 7370  et_default_cf_sp
-0001c3d0: 6563 7328 290a 2020 2020 2020 2020 6966  ecs().        if
-0001c3e0: 2063 6664 6566 206e 6f74 2069 6e20 6366   cfdef not in cf
-0001c3f0: 6c3a 0a20 2020 2020 2020 2020 2020 2063  l:.            c
-0001c400: 666c 2e61 7070 656e 6428 6366 6465 6629  fl.append(cfdef)
-0001c410: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0001c420: 2020 2063 666c 203d 205b 6320 666f 7220     cfl = [c for 
-0001c430: 6320 696e 2063 666c 2069 6620 632e 6e61  c in cfl if c.na
-0001c440: 6d65 5d0a 2020 2020 7265 7475 726e 2063  me].    return c
-0001c450: 666c 0a0a 0a64 6566 2069 735f 7265 6769  fl...def is_regi
-0001c460: 7374 6572 6564 5f63 665f 7370 6563 7328  stered_cf_specs(
-0001c470: 6e61 6d65 293a 0a20 2020 2022 2222 4368  name):.    """Ch
-0001c480: 6563 6b20 6966 2067 6976 656e 2063 6620  eck if given cf 
-0001c490: 7370 6563 7320 7365 7420 6973 2072 6567  specs set is reg
-0001c4a0: 6973 7465 7265 640a 0a20 2020 2050 6172  istered..    Par
-0001c4b0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-0001c4c0: 2d2d 2d2d 2d2d 0a20 2020 206e 616d 653a  ------.    name:
-0001c4d0: 2073 7472 2c20 4346 5370 6563 730a 0a20   str, CFSpecs.. 
-0001c4e0: 2020 2052 6574 7572 6e0a 2020 2020 2d2d     Return.    --
-0001c4f0: 2d2d 2d2d 0a20 2020 2062 6f6f 6c0a 2020  ----.    bool.  
-0001c500: 2020 2222 220a 2020 2020 666f 7220 6366    """.    for cf
-0001c510: 7370 6563 7320 696e 2067 6574 5f72 6567  specs in get_reg
-0001c520: 6973 7465 7265 645f 6366 5f73 7065 6373  istered_cf_specs
-0001c530: 2829 3a0a 2020 2020 2020 2020 6966 2028  ():.        if (
-0001c540: 0a20 2020 2020 2020 2020 2020 2069 7369  .            isi
-0001c550: 6e73 7461 6e63 6528 6e61 6d65 2c20 7374  nstance(name, st
-0001c560: 7229 0a20 2020 2020 2020 2020 2020 2061  r).            a
-0001c570: 6e64 2063 6673 7065 6373 5b22 7265 6769  nd cfspecs["regi
-0001c580: 7374 6572 225d 5b22 6e61 6d65 225d 0a20  ster"]["name"]. 
-0001c590: 2020 2020 2020 2020 2020 2061 6e64 2063             and c
-0001c5a0: 6673 7065 6373 5b22 7265 6769 7374 6572  fspecs["register
-0001c5b0: 225d 5b22 6e61 6d65 225d 203d 3d20 6e61  "]["name"] == na
-0001c5c0: 6d65 0a20 2020 2020 2020 2029 3a0a 2020  me.        ):.  
-0001c5d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001c5e0: 2054 7275 650a 2020 2020 2020 2020 6966   True.        if
-0001c5f0: 2069 7369 6e73 7461 6e63 6528 6e61 6d65   isinstance(name
-0001c600: 2c20 4346 5370 6563 7329 2061 6e64 206e  , CFSpecs) and n
-0001c610: 616d 6520 6973 2063 6673 7065 6373 3a0a  ame is cfspecs:.
-0001c620: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001c630: 726e 2054 7275 650a 2020 2020 7265 7475  rn True.    retu
-0001c640: 726e 2046 616c 7365 0a0a 0a64 6566 2067  rn False...def g
-0001c650: 6574 5f63 665f 7370 6563 735f 6d61 7463  et_cf_specs_matc
-0001c660: 6869 6e67 5f73 636f 7265 2864 732c 2063  hing_score(ds, c
-0001c670: 6673 7065 6373 293a 0a20 2020 2022 2222  fspecs):.    """
-0001c680: 4765 7420 7468 6520 6d61 7463 6869 6e67  Get the matching
-0001c690: 2073 636f 7265 2062 6574 7765 656e 2064   score between d
-0001c6a0: 7320 6461 7461 5f76 6172 7320 616e 6420  s data_vars and 
-0001c6b0: 636f 6f72 6420 6e61 6d65 7320 616e 6420  coord names and 
-0001c6c0: 6120 4346 5370 6563 7320 696e 7374 616e  a CFSpecs instan
-0001c6d0: 6365 206e 616d 6573 0a0a 2020 2020 5061  ce names..    Pa
-0001c6e0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-0001c6f0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6473 3a20  -------.    ds: 
-0001c700: 7861 7272 6179 2e44 6174 6173 6574 2c20  xarray.Dataset, 
-0001c710: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-0001c720: 0a20 2020 2063 665f 7370 6563 733a 2043  .    cf_specs: C
-0001c730: 4653 7065 6373 0a0a 2020 2020 5265 7475  FSpecs..    Retu
-0001c740: 726e 0a20 2020 202d 2d2d 2d2d 2d0a 2020  rn.    ------.  
-0001c750: 2020 666c 6f61 740a 2020 2020 2020 2020    float.        
-0001c760: 4120 7065 7263 656e 7461 6765 206f 6620  A percentage of 
-0001c770: 7468 6520 6e75 6d62 6572 206f 6620 6964  the number of id
-0001c780: 656e 7469 6669 6564 2064 6174 6120 6172  entified data ar
-0001c790: 7261 7973 2076 730a 2020 2020 2020 2020  rays vs.        
-0001c7a0: 7468 6520 746f 7461 6c20 6e75 6d62 6572  the total number
-0001c7b0: 206f 6620 6461 7461 2061 7272 6179 730a   of data arrays.
-0001c7c0: 2020 2020 2222 220a 2020 2020 6869 7420      """.    hit 
-0001c7d0: 3d20 300a 2020 2020 746f 7461 6c20 3d20  = 0.    total = 
-0001c7e0: 300a 2020 2020 666f 7220 6361 7420 696e  0.    for cat in
-0001c7f0: 2022 6461 7461 5f76 6172 7322 2c20 2263   "data_vars", "c
-0001c800: 6f6f 7264 7322 3a0a 2020 2020 2020 2020  oords":.        
-0001c810: 6366 6e61 6d65 7320 3d20 5b63 6673 7065  cfnames = [cfspe
-0001c820: 6373 5b63 6174 5d2e 6765 745f 6e61 6d65  cs[cat].get_name
-0001c830: 286e 616d 652c 2073 7065 6369 616c 697a  (name, specializ
-0001c840: 653d 5472 7565 2920 666f 7220 6e61 6d65  e=True) for name
-0001c850: 2069 6e20 6366 7370 6563 735b 6361 745d   in cfspecs[cat]
-0001c860: 2e6e 616d 6573 5d0a 2020 2020 2020 2020  .names].        
-0001c870: 6966 206e 6f74 2068 6173 6174 7472 2864  if not hasattr(d
-0001c880: 732c 2022 6461 7461 5f76 6172 7322 293a  s, "data_vars"):
-0001c890: 2020 2320 4461 7461 4172 7261 790a 2020    # DataArray.  
-0001c8a0: 2020 2020 2020 2020 2020 6473 6e61 6d65            dsname
-0001c8b0: 7320 3d20 5b64 732e 6e61 6d65 5d20 6966  s = [ds.name] if
-0001c8c0: 2064 732e 6e61 6d65 2065 6c73 6520 5b5d   ds.name else []
-0001c8d0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0001c8e0: 2020 2020 2020 2020 2020 2064 736e 616d             dsnam
-0001c8f0: 6573 203d 206c 6973 7428 6765 7461 7474  es = list(getatt
-0001c900: 7228 6473 2c20 6361 7429 2e6b 6579 7328  r(ds, cat).keys(
-0001c910: 2929 0a20 2020 2020 2020 2064 736e 616d  )).        dsnam
-0001c920: 6573 203d 205b 6366 7370 6563 732e 7367  es = [cfspecs.sg
-0001c930: 6c6f 6361 746f 722e 7061 7273 655f 6174  locator.parse_at
-0001c940: 7472 2822 6e61 6d65 222c 2064 736e 616d  tr("name", dsnam
-0001c950: 6529 5b30 5d20 666f 7220 6473 6e61 6d65  e)[0] for dsname
-0001c960: 2069 6e20 6473 6e61 6d65 735d 0a20 2020   in dsnames].   
-0001c970: 2020 2020 2074 6f74 616c 202b 3d20 6c65       total += le
-0001c980: 6e28 6473 6e61 6d65 7329 0a20 2020 2020  n(dsnames).     
-0001c990: 2020 2068 6974 202b 3d20 6c65 6e28 7365     hit += len(se
-0001c9a0: 7428 6473 6e61 6d65 7329 2e69 6e74 6572  t(dsnames).inter
-0001c9b0: 7365 6374 696f 6e28 6366 6e61 6d65 7329  section(cfnames)
-0001c9c0: 290a 2020 2020 6966 2074 6f74 616c 203d  ).    if total =
-0001c9d0: 3d20 303a 0a20 2020 2020 2020 2072 6574  = 0:.        ret
-0001c9e0: 7572 6e20 300a 2020 2020 7265 7475 726e  urn 0.    return
-0001c9f0: 2031 3030 202a 2068 6974 202f 2074 6f74   100 * hit / tot
-0001ca00: 616c 0a0a 0a64 6566 2069 6e66 6572 5f63  al...def infer_c
-0001ca10: 665f 7370 6563 7328 6473 2c20 6e61 6d65  f_specs(ds, name
-0001ca20: 643d 4661 6c73 6529 3a0a 2020 2020 2222  d=False):.    ""
-0001ca30: 2247 6574 2074 6865 2072 6567 6973 7465  "Get the registe
-0001ca40: 7265 6420 4346 5370 6563 7320 7468 6174  red CFSpecs that
-0001ca50: 2061 7265 2062 6573 7420 6d61 7463 6869   are best matchi
-0001ca60: 6e67 2074 6869 7320 6461 7461 7365 740a  ng this dataset.
-0001ca70: 0a20 2020 2054 6869 7320 6163 636f 6d70  .    This accomp
-0001ca80: 6c69 7368 6564 2077 6974 6820 736f 6d65  lished with some
-0001ca90: 2068 6575 7265 7374 6963 732e 0a20 2020   heurestics..   
-0001caa0: 2046 6972 7374 2c20 7468 6520 3a61 7474   First, the :att
-0001cab0: 723a 6063 665f 7370 6563 7360 2067 6c6f  r:`cf_specs` glo
-0001cac0: 6261 6c20 6174 7472 6962 7574 6520 6f72  bal attribute or
-0001cad0: 2065 6e63 6f64 696e 6720 6f66 2074 6865   encoding of the
-0001cae0: 2064 6174 6173 6574 2069 7320 636f 6d70   dataset is comp
-0001caf0: 6172 6564 0a20 2020 2077 6974 6820 7468  ared.    with th
-0001cb00: 6520 6e61 6d65 206f 6620 616c 6c20 7265  e name of all re
-0001cb10: 6769 7374 6572 6564 2064 6174 6173 6574  gistered dataset
-0001cb20: 732e 0a20 2020 2053 6563 6f6e 642c 2061  s..    Second, a
-0001cb30: 2073 636f 7265 2062 6173 6564 206f 6e20   score based on 
-0001cb40: 7468 6520 6e75 6d62 6572 206f 6620 6461  the number of da
-0001cb50: 7461 5f76 6172 7320 616e 6420 636f 6f72  ta_vars and coor
-0001cb60: 6420 6e61 6d65 730a 2020 2020 7468 6174  d names.    that
-0001cb70: 2061 7265 2062 6f74 6820 696e 2074 6865   are both in the
-0001cb80: 2063 6673 7065 6373 2061 6e64 2074 6865   cfspecs and the
-0001cb90: 2064 6174 6173 6574 2069 7320 636f 6d70   dataset is comp
-0001cba0: 7574 6564 2062 7920 3a66 756e 633a 6067  uted by :func:`g
-0001cbb0: 6574 5f63 665f 7370 6563 735f 6d61 7463  et_cf_specs_matc
-0001cbc0: 6869 6e67 5f73 636f 7265 600a 2020 2020  hing_score`.    
-0001cbd0: 666f 7220 7468 6520 7265 6769 7374 6572  for the register
-0001cbe0: 6564 2069 6e73 7461 6e63 6573 2e0a 2020  ed instances..  
-0001cbf0: 2020 4669 6e61 6c6c 792c 2069 6620 6e6f    Finally, if no
-0001cc00: 206d 6174 6368 696e 6720 6461 7461 7365   matching datase
-0001cc10: 7420 6973 2066 6f75 6e64 2c20 7468 6520  t is found, the 
-0001cc20: 6375 7272 656e 7420 6f6e 6520 6973 2072  current one is r
-0001cc30: 6574 7572 6e65 642e 0a0a 0a20 2020 2050  eturned....    P
-0001cc40: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-0001cc50: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 733a  --------.    ds:
-0001cc60: 2078 6172 7261 792e 4461 7461 7365 742c   xarray.Dataset,
-0001cc70: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
-0001cc80: 790a 2020 2020 6e61 6d65 643a 2062 6f6f  y.    named: boo
-0001cc90: 6c0a 2020 2020 2020 2020 4d61 6b65 2073  l.        Make s
-0001cca0: 7572 6520 7468 6520 6361 6e64 6964 6174  ure the candidat
-0001ccb0: 6520 4346 5370 6563 7320 6861 7665 2061  e CFSpecs have a
-0001ccc0: 206e 616d 650a 0a20 2020 2052 6574 7572   name..    Retur
-0001ccd0: 6e0a 2020 2020 2d2d 2d2d 2d2d 0a20 2020  n.    ------.   
-0001cce0: 2043 4653 7065 6373 0a20 2020 2020 2020   CFSpecs.       
-0001ccf0: 2054 6865 206d 6174 6368 696e 6720 6366   The matching cf
-0001cd00: 2073 7065 6373 206f 7220 7468 6520 6375   specs or the cu
-0001cd10: 7272 656e 7420 6f6e 6573 0a0a 2020 2020  rrent ones..    
-0001cd20: 5365 6520 616c 736f 0a20 2020 202d 2d2d  See also.    ---
-0001cd30: 2d2d 2d2d 2d0a 2020 2020 7265 6769 7374  -----.    regist
-0001cd40: 6572 5f63 665f 7370 6563 730a 2020 2020  er_cf_specs.    
-0001cd50: 6765 745f 7265 6769 7374 6572 6564 5f63  get_registered_c
-0001cd60: 665f 7370 6563 730a 2020 2020 6765 745f  f_specs.    get_
-0001cd70: 6366 5f73 7065 6373 5f6d 6174 6368 696e  cf_specs_matchin
-0001cd80: 675f 7363 6f72 650a 2020 2020 6765 745f  g_score.    get_
-0001cd90: 6366 5f73 7065 6373 0a20 2020 2067 6574  cf_specs.    get
-0001cda0: 5f63 665f 7370 6563 730a 2020 2020 6765  _cf_specs.    ge
-0001cdb0: 745f 6366 5f73 7065 6373 5f66 726f 6d5f  t_cf_specs_from_
-0001cdc0: 6e61 6d65 0a20 2020 2067 6574 5f63 665f  name.    get_cf_
-0001cdd0: 7370 6563 735f 6672 6f6d 5f65 6e63 6f64  specs_from_encod
-0001cde0: 696e 670a 2020 2020 2222 220a 2020 2020  ing.    """.    
-0001cdf0: 2320 4279 2072 6567 6973 7472 6174 696f  # By registratio
-0001ce00: 6e20 6e61 6d65 2066 6972 7374 0a20 2020  n name first.   
-0001ce10: 2063 6673 7065 6373 203d 2067 6574 5f63   cfspecs = get_c
-0001ce20: 665f 7370 6563 735f 6672 6f6d 5f65 6e63  f_specs_from_enc
-0001ce30: 6f64 696e 6728 6473 290a 2020 2020 6966  oding(ds).    if
-0001ce40: 2063 6673 7065 6373 3a0a 2020 2020 2020   cfspecs:.      
-0001ce50: 2020 7265 7475 726e 2063 6673 7065 6373    return cfspecs
-0001ce60: 0a0a 2020 2020 2320 4361 6e64 6964 6174  ..    # Candidat
-0001ce70: 6573 0a20 2020 2063 616e 6469 6461 7465  es.    candidate
-0001ce80: 7320 3d20 6765 745f 7265 6769 7374 6572  s = get_register
-0001ce90: 6564 5f63 665f 7370 6563 7328 6e61 6d65  ed_cf_specs(name
-0001cea0: 643d 6e61 6d65 6429 0a0a 2020 2020 2320  d=named)..    # 
-0001ceb0: 4279 2061 7474 7269 6275 7465 730a 2020  By attributes.  
-0001cec0: 2020 6174 7472 7320 3d20 6469 6374 2864    attrs = dict(d
-0001ced0: 732e 6174 7472 7329 0a20 2020 2061 7474  s.attrs).    att
-0001cee0: 7273 2e75 7064 6174 6528 6473 2e65 6e63  rs.update(ds.enc
-0001cef0: 6f64 696e 6729 0a20 2020 2069 6620 6174  oding).    if at
-0001cf00: 7472 733a 0a20 2020 2020 2020 2066 6f72  trs:.        for
-0001cf10: 2063 6673 7065 6373 2069 6e20 6361 6e64   cfspecs in cand
-0001cf20: 6964 6174 6573 3a0a 2020 2020 2020 2020  idates:.        
-0001cf30: 2020 2020 666f 7220 6174 7472 2c20 7061      for attr, pa
-0001cf40: 7474 6572 6e20 696e 2063 6673 7065 6373  ttern in cfspecs
-0001cf50: 5b22 7265 6769 7374 6572 225d 5b22 6174  ["register"]["at
-0001cf60: 7472 7322 5d2e 6974 656d 7328 293a 0a20  trs"].items():. 
-0001cf70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001cf80: 6620 6174 7472 2069 6e20 6174 7472 733a  f attr in attrs:
-0001cf90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001cfa0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0001cfb0: 6365 2870 6174 7465 726e 2c20 7374 7229  ce(pattern, str)
-0001cfc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001cfd0: 2020 2020 2020 2020 2020 7061 7474 6572            patter
-0001cfe0: 6e20 3d20 5b70 6174 7465 726e 5d0a 2020  n = [pattern].  
-0001cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d000: 2020 666f 7220 7061 7420 696e 2070 6174    for pat in pat
-0001d010: 7465 726e 3a0a 2020 2020 2020 2020 2020  tern:.          
-0001d020: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001d030: 2066 6e6d 6174 6368 2e66 6e6d 6174 6368   fnmatch.fnmatch
-0001d040: 2873 7472 2861 7474 7273 5b61 7474 725d  (str(attrs[attr]
-0001d050: 292e 6c6f 7765 7228 292c 2070 6174 2e6c  ).lower(), pat.l
-0001d060: 6f77 6572 2829 293a 0a20 2020 2020 2020  ower()):.       
-0001d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d080: 2020 2020 2072 6574 7572 6e20 6366 7370       return cfsp
-0001d090: 6563 730a 0a20 2020 2023 2042 7920 6d61  ecs..    # By ma
-0001d0a0: 7463 6869 6e67 2073 636f 7265 0a20 2020  tching score.   
-0001d0b0: 2062 6573 745f 7363 6f72 6520 3d20 2d31   best_score = -1
-0001d0c0: 0a20 2020 2066 6f72 2063 6673 7065 6373  .    for cfspecs
-0001d0d0: 2069 6e20 6361 6e64 6964 6174 6573 3a0a   in candidates:.
-0001d0e0: 2020 2020 2020 2020 7363 6f72 6520 3d20          score = 
-0001d0f0: 6765 745f 6366 5f73 7065 6373 5f6d 6174  get_cf_specs_mat
-0001d100: 6368 696e 675f 7363 6f72 6528 6473 2c20  ching_score(ds, 
-0001d110: 6366 7370 6563 7329 0a20 2020 2020 2020  cfspecs).       
-0001d120: 2069 6620 7363 6f72 6520 213d 2030 2061   if score != 0 a
-0001d130: 6e64 2073 636f 7265 203e 2062 6573 745f  nd score > best_
-0001d140: 7363 6f72 653a 0a20 2020 2020 2020 2020  score:.         
-0001d150: 2020 2062 6573 745f 6366 7370 6563 7320     best_cfspecs 
-0001d160: 3d20 6366 7370 6563 730a 2020 2020 2020  = cfspecs.      
-0001d170: 2020 2020 2020 6265 7374 5f73 636f 7265        best_score
-0001d180: 203d 2073 636f 7265 0a20 2020 2069 6620   = score.    if 
-0001d190: 6265 7374 5f73 636f 7265 2021 3d20 2d31  best_score != -1
-0001d1a0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0001d1b0: 2062 6573 745f 6366 7370 6563 730a 0a20   best_cfspecs.. 
-0001d1c0: 2020 2023 2046 616c 6c62 6163 6b20 746f     # Fallback to
-0001d1d0: 2064 6566 6175 6c74 2073 7065 6373 0a20   default specs. 
-0001d1e0: 2020 2063 6673 7065 6373 203d 2067 6574     cfspecs = get
-0001d1f0: 5f63 665f 7370 6563 7328 290a 2020 2020  _cf_specs().    
-0001d200: 6966 206e 616d 6564 2061 6e64 206e 6f74  if named and not
-0001d210: 2063 6673 7065 6373 2e6e 616d 653a 0a20   cfspecs.name:. 
-0001d220: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0001d230: 2020 7265 7475 726e 2063 6673 7065 6373    return cfspecs
-0001d240: 0a0a 0a64 6566 2061 7373 6967 6e5f 6366  ...def assign_cf
-0001d250: 5f73 7065 6373 2864 732c 206e 616d 653d  _specs(ds, name=
-0001d260: 4e6f 6e65 2c20 7265 6769 7374 6572 3d46  None, register=F
-0001d270: 616c 7365 293a 0a20 2020 2022 2222 5365  alse):.    """Se
-0001d280: 7420 7468 6520 6060 6366 5f73 7065 6373  t the ``cf_specs
-0001d290: 6060 2065 6e63 6f64 696e 6720 746f 2060  `` encoding to `
-0001d2a0: 606e 616d 6560 6020 696e 2061 6c6c 2064  `name`` in all d
-0001d2b0: 6174 6120 7661 7273 2061 6e64 2063 6f6f  ata vars and coo
-0001d2c0: 7264 730a 0a20 2020 2050 6172 616d 6574  rds..    Paramet
-0001d2d0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-0001d2e0: 2d2d 0a20 2020 2064 733a 2078 6172 7261  --.    ds: xarra
-0001d2f0: 792e 4461 7461 4172 7261 792c 2078 6172  y.DataArray, xar
-0001d300: 7261 792e 4461 7461 7365 740a 2020 2020  ray.Dataset.    
-0001d310: 6e61 6d65 3a20 4e6f 6e65 2c20 7374 722c  name: None, str,
-0001d320: 2043 4653 7065 6373 2c20 7861 7272 6179   CFSpecs, xarray
-0001d330: 2e44 6174 6141 7272 6179 2c20 7861 7272  .DataArray, xarr
-0001d340: 6179 2e44 6174 6173 6574 0a20 2020 2020  ay.Dataset.     
-0001d350: 2020 2049 6620 6120 3a63 6c61 7373 3a60     If a :class:`
-0001d360: 4346 5370 6563 7360 2c20 6974 206d 7573  CFSpecs`, it mus
-0001d370: 7420 6861 7665 2061 2072 6567 6973 7472  t have a registr
-0001d380: 6174 696f 6e20 6e61 6d65 203a 0a0a 2020  ation name :..  
-0001d390: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
-0001d3a0: 6f63 6b3a 3a20 696e 690a 0a20 2020 2020  ock:: ini..     
-0001d3b0: 2020 2020 2020 205b 7265 6769 7374 6572         [register
-0001d3c0: 5d0a 2020 2020 2020 2020 2020 2020 6e61  ].            na
-0001d3d0: 6d65 3d72 6567 6973 7472 6174 696f 6e5f  me=registration_
-0001d3e0: 6e61 6d65 0a0a 2020 2020 2020 2020 4966  name..        If
-0001d3f0: 206e 6f74 2070 726f 7669 6465 642c 203a   not provided, :
-0001d400: 6675 6e63 3a60 696e 6665 725f 6366 5f73  func:`infer_cf_s
-0001d410: 7065 6373 6020 6973 2063 616c 6c65 6420  pecs` is called 
-0001d420: 746f 2069 6e66 6572 0a20 2020 2020 2020  to infer.       
-0001d430: 2074 6865 2062 6573 7420 6e61 6d65 6420   the best named 
-0001d440: 7265 6769 7374 6572 6564 2073 7065 6373  registered specs
-0001d450: 2e0a 0a20 2020 2072 6567 6973 7465 723a  ...    register:
-0001d460: 2062 6f6f 6c0a 2020 2020 2020 2020 5265   bool.        Re
-0001d470: 6769 7374 6572 2074 6865 2073 7065 6373  gister the specs
-0001d480: 2069 6620 6e61 6d65 2069 7320 6120 6e61   if name is a na
-0001d490: 6d65 642c 2075 6e72 6567 6973 7465 7265  med, unregistere
-0001d4a0: 6420 3a63 6c61 7373 3a60 4346 5370 6563  d :class:`CFSpec
-0001d4b0: 7360 2069 6e73 7461 6e63 652e 0a0a 2020  s` instance...  
-0001d4c0: 2020 5265 7475 726e 0a20 2020 202d 2d2d    Return.    ---
-0001d4d0: 2d2d 2d0a 2020 2020 7861 7272 6179 2e44  ---.    xarray.D
-0001d4e0: 6174 6173 6574 2c20 7861 7272 6179 2e44  ataset, xarray.D
-0001d4f0: 6174 6141 7272 6179 0a0a 2020 2020 4578  ataArray..    Ex
-0001d500: 616d 706c 650a 2020 2020 2d2d 2d2d 2d2d  ample.    ------
-0001d510: 2d0a 2020 2020 2e2e 2069 7079 7468 6f6e  -.    .. ipython
-0001d520: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
-0001d530: 2020 2040 7375 7070 7265 7373 0a20 2020     @suppress.   
-0001d540: 2020 2020 2066 726f 6d20 786f 612e 6366       from xoa.cf
-0001d550: 2069 6d70 6f72 7420 6173 7369 676e 5f63   import assign_c
-0001d560: 665f 7370 6563 730a 2020 2020 2020 2020  f_specs.        
-0001d570: 4073 7570 7072 6573 730a 2020 2020 2020  @suppress.      
-0001d580: 2020 696d 706f 7274 2078 6172 7261 7920    import xarray 
-0001d590: 6173 2078 720a 2020 2020 2020 2020 6473  as xr.        ds
-0001d5a0: 203d 2078 722e 4461 7461 7365 7428 7b27   = xr.Dataset({'
-0001d5b0: 7465 6d70 273a 2028 276c 6f6e 272c 205b  temp': ('lon', [
-0001d5c0: 355d 297d 2c20 636f 6f72 6473 3d7b 276c  5])}, coords={'l
-0001d5d0: 6f6e 273a 205b 365d 7d29 0a20 2020 2020  on': [6]}).     
-0001d5e0: 2020 2061 7373 6967 6e5f 6366 5f73 7065     assign_cf_spe
-0001d5f0: 6373 2864 732c 2022 6d79 6372 6f63 6f22  cs(ds, "mycroco"
-0001d600: 293b 0a20 2020 2020 2020 2064 732e 656e  );.        ds.en
-0001d610: 636f 6469 6e67 0a20 2020 2020 2020 2064  coding.        d
-0001d620: 732e 7465 6d70 2e65 6e63 6f64 696e 670a  s.temp.encoding.
-0001d630: 2020 2020 2020 2020 6473 2e6c 6f6e 2e65          ds.lon.e
-0001d640: 6e63 6f64 696e 670a 0a20 2020 2022 2222  ncoding..    """
-0001d650: 0a20 2020 2023 204e 616d 6520 6173 2061  .    # Name as a
-0001d660: 2043 4653 7065 6373 2069 6e73 7461 6e63   CFSpecs instanc
-0001d670: 650a 2020 2020 6966 206e 616d 6520 6973  e.    if name is
-0001d680: 204e 6f6e 653a 0a20 2020 2020 2020 2063   None:.        c
-0001d690: 6673 7065 6373 203d 2069 6e66 6572 5f63  fspecs = infer_c
-0001d6a0: 665f 7370 6563 7328 6473 2c20 6e61 6d65  f_specs(ds, name
-0001d6b0: 643d 5472 7565 290a 2020 2020 2020 2020  d=True).        
-0001d6c0: 6966 2063 6673 7065 6373 2e6e 616d 653a  if cfspecs.name:
-0001d6d0: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-0001d6e0: 6520 3d20 6366 7370 6563 732e 6e61 6d65  e = cfspecs.name
-0001d6f0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0001d700: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001d710: 6e20 6473 0a20 2020 2065 6c69 6620 6861  n ds.    elif ha
-0001d720: 7361 7474 7228 6e61 6d65 2c20 2263 6f6f  sattr(name, "coo
-0001d730: 7264 7322 293a 2020 2320 6672 6f6d 2061  rds"):  # from a
-0001d740: 2064 6174 6173 6574 2f64 6174 6161 7272   dataset/dataarr
-0001d750: 6179 0a20 2020 2020 2020 206e 616d 6520  ay.        name 
-0001d760: 3d20 6765 745f 6366 5f73 7065 6373 5f65  = get_cf_specs_e
-0001d770: 6e63 6f64 696e 6728 6473 290a 2020 2020  ncoding(ds).    
-0001d780: 2020 2020 6966 206e 616d 6520 6973 204e      if name is N
-0001d790: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0001d7a0: 2072 6574 7572 6e20 6473 0a20 2020 2069   return ds.    i
-0001d7b0: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-0001d7c0: 286e 616d 652c 2073 7472 293a 0a20 2020  (name, str):.   
-0001d7d0: 2020 2020 2069 6620 6e6f 7420 6e61 6d65       if not name
-0001d7e0: 2e6e 616d 653a 0a20 2020 2020 2020 2020  .name:.         
-0001d7f0: 2020 2078 6f61 5f77 6172 6e28 2243 4653     xoa_warn("CFS
-0001d800: 7065 6373 2069 6e73 7461 6e63 6520 6861  pecs instance ha
-0001d810: 7320 6e6f 2072 6567 6973 7472 6174 696f  s no registratio
-0001d820: 6e20 6e61 6d65 2229 0a20 2020 2020 2020  n name").       
-0001d830: 2020 2020 2072 6574 7572 6e20 6473 0a20       return ds. 
-0001d840: 2020 2020 2020 2069 6620 7265 6769 7374         if regist
-0001d850: 6572 2061 6e64 206e 6f74 2069 735f 7265  er and not is_re
-0001d860: 6769 7374 6572 6564 5f63 665f 7370 6563  gistered_cf_spec
-0001d870: 7328 6e61 6d65 293a 0a20 2020 2020 2020  s(name):.       
-0001d880: 2020 2020 2072 6567 6973 7465 725f 6366       register_cf
-0001d890: 5f73 7065 6373 286e 616d 6529 0a20 2020  _specs(name).   
-0001d8a0: 2020 2020 206e 616d 6520 3d20 6e61 6d65       name = name
-0001d8b0: 2e6e 616d 650a 0a20 2020 2023 2053 6574  .name..    # Set
-0001d8c0: 2061 7320 656e 636f 6469 6e67 0a20 2020   as encoding.   
-0001d8d0: 2074 6172 6765 7473 203d 205b 6473 5d20   targets = [ds] 
-0001d8e0: 2b20 5b64 735b 6e61 6d65 5d20 666f 7220  + [ds[name] for 
-0001d8f0: 6e61 6d65 2069 6e20 5f6c 6973 745f 7872  name in _list_xr
-0001d900: 5f6e 616d 6573 5f28 6473 2c20 6469 6d73  _names_(ds, dims
-0001d910: 3d46 616c 7365 295d 0a20 2020 2066 6f72  =False)].    for
-0001d920: 2074 6172 6765 7420 696e 2074 6172 6765   target in targe
-0001d930: 7473 3a0a 2020 2020 2020 2020 7461 7267  ts:.        targ
-0001d940: 6574 2e65 6e63 6f64 696e 672e 7570 6461  et.encoding.upda
-0001d950: 7465 2863 665f 7370 6563 733d 6e61 6d65  te(cf_specs=name
-0001d960: 290a 2020 2020 7265 7475 726e 2064 730a  ).    return ds.
-0001d970: 0a0a 6465 6620 696e 6665 725f 636f 6f72  ..def infer_coor
-0001d980: 6473 2864 7329 3a0a 2020 2020 2222 2249  ds(ds):.    """I
-0001d990: 6e66 6572 2077 6869 6368 206f 6620 7468  nfer which of th
-0001d9a0: 6520 6461 7461 2061 7272 6179 7320 6f66  e data arrays of
-0001d9b0: 2061 2064 6174 6173 6574 2061 7265 2063   a dataset are c
-0001d9c0: 6f6f 7264 696e 6174 6573 0a0a 2020 2020  oordinates..    
-0001d9d0: 5768 656e 2063 6f6f 7264 696e 6174 6573  When coordinates
-0001d9e0: 2061 7265 2066 6f75 6e64 2c20 6974 206d   are found, it m
-0001d9f0: 616b 6573 2073 7572 6520 7468 6579 2061  akes sure they a
-0001da00: 7265 2072 6567 6973 7465 7265 6420 696e  re registered in
-0001da10: 2074 6865 2064 6174 6173 6574 0a20 2020   the dataset.   
-0001da20: 2061 7320 636f 6f72 6469 6e64 6174 6573   as coordindates
-0001da30: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-0001da40: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-0001da50: 0a20 2020 2064 733a 2078 6172 7261 792e  .    ds: xarray.
-0001da60: 4461 7461 7365 740a 0a20 2020 2053 6565  Dataset..    See
-0001da70: 2061 6c73 6f0a 2020 2020 2d2d 2d2d 2d2d   also.    ------
-0001da80: 2d2d 0a20 2020 2043 4653 7065 6373 2e69  --.    CFSpecs.i
-0001da90: 6e66 6572 5f63 6f6f 7264 730a 2020 2020  nfer_coords.    
-0001daa0: 2222 220a 2020 2020 7265 7475 726e 2067  """.    return g
-0001dab0: 6574 5f63 665f 7370 6563 7328 6473 292e  et_cf_specs(ds).
-0001dac0: 696e 6665 725f 636f 6f72 6473 2864 7329  infer_coords(ds)
-0001dad0: 0a0a 0a69 6e66 6572 5f63 6f6f 7264 732e  ...infer_coords.
-0001dae0: 5f5f 646f 635f 5f20 3d20 4346 5370 6563  __doc__ = CFSpec
-0001daf0: 732e 696e 6665 725f 636f 6f72 6473 2e5f  s.infer_coords._
-0001db00: 5f64 6f63 5f5f 0a                        _doc__.
+0001a660: 662e 7370 6563 7320 3d20 6366 5f73 6f75  f.specs = cf_sou
+0001a670: 7263 650a 0a20 2020 2064 6566 205f 5f65  rce..    def __e
+0001a680: 6e74 6572 5f5f 2873 656c 6629 3a0a 2020  nter__(self):.  
+0001a690: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001a6a0: 662e 7370 6563 730a 0a20 2020 2064 6566  f.specs..    def
+0001a6b0: 205f 5f65 7869 745f 5f28 7365 6c66 2c20   __exit__(self, 
+0001a6c0: 6578 635f 7479 7065 2c20 6578 635f 7661  exc_type, exc_va
+0001a6d0: 6c75 652c 2074 7261 6365 6261 636b 293a  lue, traceback):
+0001a6e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0001a6f0: 2e6f 6c64 5f73 7065 6373 2069 7320 4e6f  .old_specs is No
+0001a700: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001a710: 6465 6c20 7365 6c66 2e63 665f 6361 6368  del self.cf_cach
+0001a720: 655b 2263 7572 7265 6e74 225d 0a20 2020  e["current"].   
+0001a730: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001a740: 2020 2020 2020 2073 656c 662e 6366 5f63         self.cf_c
+0001a750: 6163 6865 5b22 6375 7272 656e 7422 5d20  ache["current"] 
+0001a760: 3d20 7365 6c66 2e6f 6c64 5f73 7065 6373  = self.old_specs
+0001a770: 0a0a 0a64 6566 2072 6573 6574 5f63 6163  ...def reset_cac
+0001a780: 6865 2864 6973 6b3d 5472 7565 2c20 6d65  he(disk=True, me
+0001a790: 6d6f 7279 3d46 616c 7365 293a 0a20 2020  mory=False):.   
+0001a7a0: 2022 2222 5265 7365 7420 7468 6520 6f6e   """Reset the on
+0001a7b0: 2064 6973 6b20 616e 642f 6f72 2069 6e20   disk and/or in 
+0001a7c0: 6d65 6d6f 7279 2063 6620 7370 6563 7320  memory cf specs 
+0001a7d0: 6361 6368 650a 0a20 2020 2050 6172 616d  cache..    Param
+0001a7e0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+0001a7f0: 2d2d 2d2d 0a20 2020 2064 6973 6b3a 2062  ----.    disk: b
+0001a800: 6f6f 6c0a 2020 2020 2020 2020 5265 6d6f  ool.        Remo
+0001a810: 7665 2074 6865 2063 6620 7370 6563 7320  ve the cf specs 
+0001a820: 6361 6863 6520 6669 6c65 2028 3a64 6174  cahce file (:dat
+0001a830: 613a 6055 5345 525f 4346 5f43 4143 4845  a:`USER_CF_CACHE
+0001a840: 5f46 494c 4560 290a 2020 2020 6d65 6d6f  _FILE`).    memo
+0001a850: 7279 3a20 626f 6f6c 0a20 2020 2020 2020  ry: bool.       
+0001a860: 2052 656d 6f76 6520 7468 6520 696e 2d6d   Remove the in-m
+0001a870: 656d 6f72 7920 6361 6368 652e 0a0a 2020  emory cache...  
+0001a880: 2020 2020 2020 2e2e 2077 6172 6e69 6e67        .. warning
+0001a890: 3a3a 2054 6869 7320 6d61 7920 6c65 6164  :: This may lead
+0001a8a0: 2074 6f20 756e 7072 6564 6963 7465 6420   to unpredicted 
+0001a8b0: 6265 6861 7669 6f72 732e 0a0a 2020 2020  behaviors...    
+0001a8c0: 2222 220a 2020 2020 6966 2064 6973 6b20  """.    if disk 
+0001a8d0: 616e 6420 6f73 2e70 6174 682e 6578 6973  and os.path.exis
+0001a8e0: 7473 2855 5345 525f 4346 5f43 4143 4845  ts(USER_CF_CACHE
+0001a8f0: 5f46 494c 4529 3a0a 2020 2020 2020 2020  _FILE):.        
+0001a900: 6f73 2e72 656d 6f76 6528 5553 4552 5f43  os.remove(USER_C
+0001a910: 465f 4341 4348 455f 4649 4c45 290a 0a20  F_CACHE_FILE).. 
+0001a920: 2020 2069 6620 6d65 6d6f 7279 3a0a 2020     if memory:.  
+0001a930: 2020 2020 2020 6366 5f63 6163 6865 203d        cf_cache =
+0001a940: 205f 6765 745f 6366 676d 5f28 290a 2020   _get_cfgm_().  
+0001a950: 2020 2020 2020 6366 5f63 6163 6865 5b22        cf_cache["
+0001a960: 6c6f 6164 6564 5f64 6963 7473 225d 2e63  loaded_dicts"].c
+0001a970: 6c65 6172 2829 0a20 2020 2020 2020 2063  lear().        c
+0001a980: 665f 6361 6368 655b 2263 7572 7265 6e74  f_cache["current
+0001a990: 225d 203d 204e 6f6e 650a 2020 2020 2020  "] = None.      
+0001a9a0: 2020 6366 5f63 6163 6865 5b22 6465 6661    cf_cache["defa
+0001a9b0: 756c 7422 5d20 3d20 4e6f 6e65 0a20 2020  ult"] = None.   
+0001a9c0: 2020 2020 2063 665f 6361 6368 655b 2272       cf_cache["r
+0001a9d0: 6567 6973 7465 7265 6422 5d2e 636c 6561  egistered"].clea
+0001a9e0: 7228 290a 0a0a 6465 6620 7368 6f77 5f63  r()...def show_c
+0001a9f0: 6163 6865 2829 3a0a 2020 2020 2222 2253  ache():.    """S
+0001aa00: 686f 7720 7468 6520 6366 2073 7065 6373  how the cf specs
+0001aa10: 2063 6163 6865 2066 696c 6522 2222 0a20   cache file""". 
+0001aa20: 2020 2070 7269 6e74 2855 5345 525f 4346     print(USER_CF
+0001aa30: 5f43 4143 4845 5f46 494c 4529 0a0a 0a40  _CACHE_FILE)...@
+0001aa40: 4552 524f 5253 2e66 6f72 6d61 745f 6675  ERRORS.format_fu
+0001aa50: 6e63 7469 6f6e 5f64 6f63 7374 7269 6e67  nction_docstring
+0001aa60: 0a64 6566 2067 6574 5f63 665f 7370 6563  .def get_cf_spec
+0001aa70: 735f 6672 6f6d 5f6e 616d 6528 6e61 6d65  s_from_name(name
+0001aa80: 2c20 6572 726f 7273 3d22 7761 726e 2229  , errors="warn")
+0001aa90: 3a0a 2020 2020 2222 2247 6574 2061 2072  :.    """Get a r
+0001aaa0: 6567 6973 7465 7265 6420 4346 2073 7065  egistered CF spe
+0001aab0: 6373 2069 6e73 7461 6e63 6520 6672 6f6d  cs instance from
+0001aac0: 2069 7473 206e 616d 650a 0a20 2020 2050   its name..    P
+0001aad0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+0001aae0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e 616d  --------.    nam
+0001aaf0: 653a 2073 7472 0a20 2020 207b 6572 726f  e: str.    {erro
+0001ab00: 7273 7d0a 0a20 2020 2052 6574 7572 6e0a  rs}..    Return.
+0001ab10: 2020 2020 2d2d 2d2d 2d2d 0a20 2020 2043      ------.    C
+0001ab20: 4653 7065 6373 206f 7220 4e6f 6e65 0a20  FSpecs or None. 
+0001ab30: 2020 2020 2020 2049 7373 7565 2061 2077         Issue a w
+0001ab40: 6172 6e69 6e67 2069 6620 6e6f 7420 666f  arning if not fo
+0001ab50: 756e 640a 2020 2020 2222 220a 2020 2020  und.    """.    
+0001ab60: 6366 5f63 6163 6865 203d 205f 6765 745f  cf_cache = _get_
+0001ab70: 6361 6368 655f 2829 0a20 2020 2066 6f72  cache_().    for
+0001ab80: 2063 6673 7065 6373 2069 6e20 6366 5f63   cfspecs in cf_c
+0001ab90: 6163 6865 5b22 7265 6769 7374 6572 6564  ache["registered
+0001aba0: 225d 5b3a 3a2d 315d 3a0a 2020 2020 2020  "][::-1]:.      
+0001abb0: 2020 6966 2063 6673 7065 6373 5b22 7265    if cfspecs["re
+0001abc0: 6769 7374 6572 225d 5b22 6e61 6d65 225d  gister"]["name"]
+0001abd0: 2061 6e64 2063 6673 7065 6373 5b22 7265   and cfspecs["re
+0001abe0: 6769 7374 6572 225d 5b22 6e61 6d65 225d  gister"]["name"]
+0001abf0: 203d 3d20 6e61 6d65 2e6c 6f77 6572 2829   == name.lower()
+0001ac00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0001ac10: 7475 726e 2063 6673 7065 6373 0a20 2020  turn cfspecs.   
+0001ac20: 2065 7272 6f72 7320 3d20 4552 524f 5253   errors = ERRORS
+0001ac30: 5b65 7272 6f72 735d 0a20 2020 206d 7367  [errors].    msg
+0001ac40: 203d 2066 2249 6e76 616c 6964 2072 6567   = f"Invalid reg
+0001ac50: 6973 7472 6174 696f 6e20 6e61 6d65 2066  istration name f
+0001ac60: 6f72 2043 4620 7370 6563 733a 207b 6e61  or CF specs: {na
+0001ac70: 6d65 7d22 0a20 2020 2069 6620 6572 726f  me}".    if erro
+0001ac80: 7273 203d 3d20 2272 6169 7365 223a 0a20  rs == "raise":. 
+0001ac90: 2020 2020 2020 2072 6169 7365 2058 6f61         raise Xoa
+0001aca0: 4346 4572 726f 7228 6d73 6729 0a20 2020  CFError(msg).   
+0001acb0: 2065 6c69 6620 6572 726f 7273 203d 3d20   elif errors == 
+0001acc0: 2277 6172 6e22 3a0a 2020 2020 2020 2020  "warn":.        
+0001acd0: 786f 615f 7761 726e 286d 7367 290a 0a0a  xoa_warn(msg)...
+0001ace0: 6465 6620 6765 745f 6366 5f73 7065 6373  def get_cf_specs
+0001acf0: 5f65 6e63 6f64 696e 6728 6473 293a 0a20  _encoding(ds):. 
+0001ad00: 2020 2022 2222 4765 7420 7468 6520 6060     """Get the ``
+0001ad10: 6366 5f73 7065 6373 6060 2065 6e63 6f64  cf_specs`` encod
+0001ad20: 696e 6720 7661 6c75 650a 0a20 2020 2050  ing value..    P
+0001ad30: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+0001ad40: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 733a  --------.    ds:
+0001ad50: 2078 6172 7261 792e 4461 7461 4172 7261   xarray.DataArra
+0001ad60: 792c 2078 6172 7261 792e 4461 7461 7365  y, xarray.Datase
+0001ad70: 740a 0a20 2020 2052 6574 7572 6e0a 2020  t..    Return.  
+0001ad80: 2020 2d2d 2d2d 2d2d 0a20 2020 2073 7472    ------.    str
+0001ad90: 206f 7220 4e6f 6e65 0a0a 2020 2020 5365   or None..    Se
+0001ada0: 6520 616c 736f 0a20 2020 202d 2d2d 2d2d  e also.    -----
+0001adb0: 2d2d 2d0a 2020 2020 6765 745f 6366 5f73  ---.    get_cf_s
+0001adc0: 7065 6373 5f66 726f 6d5f 656e 636f 6469  pecs_from_encodi
+0001add0: 6e67 0a20 2020 2022 2222 0a20 2020 2069  ng.    """.    i
+0001ade0: 6620 6473 2069 7320 6e6f 7420 4e6f 6e65  f ds is not None
+0001adf0: 2061 6e64 206e 6f74 2069 7369 6e73 7461   and not isinsta
+0001ae00: 6e63 6528 6473 2c20 7374 7229 3a0a 2020  nce(ds, str):.  
+0001ae10: 2020 2020 2020 666f 7220 736f 7572 6365        for source
+0001ae20: 2069 6e20 6473 2e65 6e63 6f64 696e 672c   in ds.encoding,
+0001ae30: 2064 732e 6174 7472 733a 0a20 2020 2020   ds.attrs:.     
+0001ae40: 2020 2020 2020 2066 6f72 2061 7474 722c         for attr,
+0001ae50: 2076 616c 7565 2069 6e20 736f 7572 6365   value in source
+0001ae60: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+0001ae70: 2020 2020 2020 2020 2020 6966 2061 7474            if att
+0001ae80: 722e 6c6f 7765 7228 2920 3d3d 2022 6366  r.lower() == "cf
+0001ae90: 5f73 7065 6373 223a 0a20 2020 2020 2020  _specs":.       
+0001aea0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0001aeb0: 7572 6e20 7661 6c75 650a 0a0a 6465 6620  urn value...def 
+0001aec0: 6765 745f 6366 5f73 7065 6373 5f66 726f  get_cf_specs_fro
+0001aed0: 6d5f 656e 636f 6469 6e67 2864 7329 3a0a  m_encoding(ds):.
+0001aee0: 2020 2020 2222 2247 6574 2061 2072 6567      """Get a reg
+0001aef0: 6973 7465 7265 6420 4346 2073 7065 6373  istered CF specs
+0001af00: 2069 6e73 7461 6e63 6520 6672 6f6d 2074   instance from t
+0001af10: 6865 2060 6063 665f 7370 6563 7360 6020  he ``cf_specs`` 
+0001af20: 656e 636f 6469 6e67 2076 616c 7565 0a0a  encoding value..
+0001af30: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0001af40: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0001af50: 2020 6473 3a20 7861 7272 6179 2e44 6174    ds: xarray.Dat
+0001af60: 6141 7272 6179 2c20 7861 7272 6179 2e44  aArray, xarray.D
+0001af70: 6174 6173 6574 0a0a 2020 2020 5265 7475  ataset..    Retu
+0001af80: 726e 0a20 2020 202d 2d2d 2d2d 2d0a 2020  rn.    ------.  
+0001af90: 2020 4346 5370 6563 7320 6f72 204e 6f6e    CFSpecs or Non
+0001afa0: 650a 0a20 2020 2053 6565 2061 6c73 6f0a  e..    See also.
+0001afb0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0001afc0: 2067 6574 5f63 665f 7370 6563 735f 656e   get_cf_specs_en
+0001afd0: 636f 6469 6e67 0a20 2020 2022 2222 0a20  coding.    """. 
+0001afe0: 2020 2069 6620 6473 2069 7320 6e6f 7420     if ds is not 
+0001aff0: 4e6f 6e65 2061 6e64 206e 6f74 2069 7369  None and not isi
+0001b000: 6e73 7461 6e63 6528 6473 2c20 7374 7229  nstance(ds, str)
+0001b010: 3a0a 2020 2020 2020 2020 6e61 6d65 203d  :.        name =
+0001b020: 2067 6574 5f63 665f 7370 6563 735f 656e   get_cf_specs_en
+0001b030: 636f 6469 6e67 2864 7329 0a20 2020 2020  coding(ds).     
+0001b040: 2020 2069 6620 6e61 6d65 2069 7320 6e6f     if name is no
+0001b050: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0001b060: 2020 2020 7265 7475 726e 2067 6574 5f63      return get_c
+0001b070: 665f 7370 6563 735f 6672 6f6d 5f6e 616d  f_specs_from_nam
+0001b080: 6528 6e61 6d65 2c20 6572 726f 7273 3d22  e(name, errors="
+0001b090: 7761 726e 2229 0a0a 0a64 6566 2067 6574  warn")...def get
+0001b0a0: 5f64 6566 6175 6c74 5f63 665f 7370 6563  _default_cf_spec
+0001b0b0: 7328 6361 6368 653d 2272 7722 293a 0a20  s(cache="rw"):. 
+0001b0c0: 2020 2022 2222 4765 7420 7468 6520 6465     """Get the de
+0001b0d0: 6661 756c 7420 4346 2073 7065 6369 6669  fault CF specifi
+0001b0e0: 6361 7469 6f6e 730a 0a20 2020 2050 6172  cations..    Par
+0001b0f0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+0001b100: 2d2d 2d2d 2d2d 0a20 2020 2063 6163 6865  ------.    cache
+0001b110: 3a20 7374 722c 2062 6f6f 6c2c 204e 6f6e  : str, bool, Non
+0001b120: 650a 2020 2020 2020 2020 4361 6368 6520  e.        Cache 
+0001b130: 6465 6661 756c 7420 7370 6563 7320 6f6e  default specs on
+0001b140: 2064 6973 6b20 7769 7468 2070 6963 6b6c   disk with pickl
+0001b150: 696e 6720 666f 7220 6661 7374 206c 6f61  ing for fast loa
+0001b160: 6469 6e67 2e0a 2020 2020 2020 2020 4966  ding..        If
+0001b170: 2060 604e 6f6e 6560 602c 2069 7420 6465   ``None``, it de
+0001b180: 6661 756c 7473 2074 6f20 626f 6f6c 6561  faults to boolea
+0001b190: 6e20 6f70 7469 6f6e 203a 786f 616f 7074  n option :xoaopt
+0001b1a0: 696f 6e3a 6063 662e 6361 6368 6560 2e0a  ion:`cf.cache`..
+0001b1b0: 2020 2020 2020 2020 506f 7373 6962 6c65          Possible
+0001b1c0: 2073 7472 696e 6720 7661 6c75 6573 3a20   string values: 
+0001b1d0: 6060 2269 676e 6f72 6522 6060 2c20 6060  ``"ignore"``, ``
+0001b1e0: 2272 7722 6060 2c20 6060 2272 6561 6422  "rw"``, ``"read"
+0001b1f0: 6060 2c0a 2020 2020 2020 2020 6060 2277  ``,.        ``"w
+0001b200: 7269 7465 2260 602c 2060 6022 636c 6561  rite"``, ``"clea
+0001b210: 6e22 6060 2e0a 2020 2020 2020 2020 4966  n"``..        If
+0001b220: 2060 6054 7275 6560 602c 2069 7420 6973   ``True``, it is
+0001b230: 2073 6574 2074 6f20 6060 2272 7722 6060   set to ``"rw"``
+0001b240: 2e0a 2020 2020 2020 2020 4966 2060 6046  ..        If ``F
+0001b250: 616c 7365 6060 2c20 6974 2069 7320 7365  alse``, it is se
+0001b260: 7420 746f 2060 6022 6967 6e6f 7265 2260  t to ``"ignore"`
+0001b270: 602e 0a20 2020 2022 2222 0a20 2020 2069  `..    """.    i
+0001b280: 6620 6361 6368 6520 6973 204e 6f6e 653a  f cache is None:
+0001b290: 0a20 2020 2020 2020 2063 6163 6865 203d  .        cache =
+0001b2a0: 2067 6574 5f6f 7074 696f 6e28 2763 662e   get_option('cf.
+0001b2b0: 6361 6368 6527 290a 2020 2020 6966 2063  cache').    if c
+0001b2c0: 6163 6865 2069 7320 5472 7565 3a0a 2020  ache is True:.  
+0001b2d0: 2020 2020 2020 6361 6368 6520 3d20 2272        cache = "r
+0001b2e0: 7722 0a20 2020 2065 6c69 6620 6361 6368  w".    elif cach
+0001b2f0: 6520 6973 2046 616c 7365 3a0a 2020 2020  e is False:.    
+0001b300: 2020 2020 6361 6368 6520 3d20 2269 676e      cache = "ign
+0001b310: 6f72 6522 0a20 2020 2061 7373 6572 7420  ore".    assert 
+0001b320: 6361 6368 6520 696e 2028 2269 676e 6f72  cache in ("ignor
+0001b330: 6522 2c20 2272 7722 2c20 2272 6561 6422  e", "rw", "read"
+0001b340: 2c20 2277 7269 7465 222c 2022 636c 6561  , "write", "clea
+0001b350: 6e22 290a 2020 2020 6366 5f63 6163 6865  n").    cf_cache
+0001b360: 203d 205f 6765 745f 6361 6368 655f 2829   = _get_cache_()
+0001b370: 0a20 2020 2069 6620 6366 5f63 6163 6865  .    if cf_cache
+0001b380: 5b22 6465 6661 756c 7422 5d20 6973 206e  ["default"] is n
+0001b390: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0001b3a0: 2072 6574 7572 6e20 6366 5f63 6163 6865   return cf_cache
+0001b3b0: 5b22 6465 6661 756c 7422 5d0a 2020 2020  ["default"].    
+0001b3c0: 6366 7370 6563 7320 3d20 4e6f 6e65 0a0a  cfspecs = None..
+0001b3d0: 2020 2020 2320 5472 7920 6672 6f6d 2064      # Try from d
+0001b3e0: 6973 6b20 6361 6368 650a 2020 2020 6966  isk cache.    if
+0001b3f0: 2063 6163 6865 2069 6e20 2822 7265 6164   cache in ("read
+0001b400: 222c 2022 7277 2229 3a0a 2020 2020 2020  ", "rw"):.      
+0001b410: 2020 6966 206f 732e 7061 7468 2e65 7869    if os.path.exi
+0001b420: 7374 7328 5553 4552 5f43 465f 4341 4348  sts(USER_CF_CACH
+0001b430: 455f 4649 4c45 2920 616e 6420 280a 2020  E_FILE) and (.  
+0001b440: 2020 2020 2020 2020 2020 6f73 2e73 7461            os.sta
+0001b450: 7428 5f43 4647 4649 4c45 292e 7374 5f6d  t(_CFGFILE).st_m
+0001b460: 7469 6d65 203c 206f 732e 7374 6174 2855  time < os.stat(U
+0001b470: 5345 525f 4346 5f43 4143 4845 5f46 494c  SER_CF_CACHE_FIL
+0001b480: 4529 2e73 745f 6d74 696d 650a 2020 2020  E).st_mtime.    
+0001b490: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+0001b4a0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001b4b0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+0001b4c0: 6e28 5553 4552 5f43 465f 4341 4348 455f  n(USER_CF_CACHE_
+0001b4d0: 4649 4c45 2c20 2272 6222 2920 6173 2066  FILE, "rb") as f
+0001b4e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b4f0: 2020 2020 2020 6366 7370 6563 7320 3d20        cfspecs = 
+0001b500: 7069 636b 6c65 2e6c 6f61 6428 6629 0a20  pickle.load(f). 
+0001b510: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0001b520: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+0001b530: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b540: 2020 786f 615f 7761 726e 2822 4572 726f    xoa_warn("Erro
+0001b550: 7220 7768 696c 6520 6c6f 6164 696e 6720  r while loading 
+0001b560: 6361 6368 6564 2063 6620 7370 6563 733a  cached cf specs:
+0001b570: 2022 202b 2073 7472 2865 2e61 7267 7329   " + str(e.args)
+0001b580: 290a 0a20 2020 2023 2043 6f6d 7075 7465  )..    # Compute
+0001b590: 2069 7420 6672 6f6d 2073 6372 6174 6368   it from scratch
+0001b5a0: 0a20 2020 2069 6620 6366 7370 6563 7320  .    if cfspecs 
+0001b5b0: 6973 204e 6f6e 653a 0a0a 2020 2020 2020  is None:..      
+0001b5c0: 2020 2320 5365 7475 700a 2020 2020 2020    # Setup.      
+0001b5d0: 2020 6366 7370 6563 7320 3d20 4346 5370    cfspecs = CFSp
+0001b5e0: 6563 7328 290a 0a20 2020 2020 2020 2023  ecs()..        #
+0001b5f0: 2043 6163 6865 2069 7420 6f6e 2064 6973   Cache it on dis
+0001b600: 6b0a 2020 2020 2020 2020 6966 2063 6163  k.        if cac
+0001b610: 6865 2069 6e20 2822 7772 6974 6522 2c20  he in ("write", 
+0001b620: 2272 7722 293a 0a20 2020 2020 2020 2020  "rw"):.         
+0001b630: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001b640: 2020 2020 2020 2020 6361 6368 6564 6972          cachedir
+0001b650: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
+0001b660: 6d65 2855 5345 525f 4346 5f43 4143 4845  me(USER_CF_CACHE
+0001b670: 5f46 494c 4529 0a20 2020 2020 2020 2020  _FILE).         
+0001b680: 2020 2020 2020 2069 6620 6e6f 7420 6f73         if not os
+0001b690: 2e70 6174 682e 6578 6973 7473 2863 6163  .path.exists(cac
+0001b6a0: 6865 6469 7229 3a0a 2020 2020 2020 2020  hedir):.        
+0001b6b0: 2020 2020 2020 2020 2020 2020 6f73 2e6d              os.m
+0001b6c0: 616b 6564 6972 7328 6361 6368 6564 6972  akedirs(cachedir
+0001b6d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001b6e0: 2020 7769 7468 206f 7065 6e28 5553 4552    with open(USER
+0001b6f0: 5f43 465f 4341 4348 455f 4649 4c45 2c20  _CF_CACHE_FILE, 
+0001b700: 2277 6222 2920 6173 2066 3a0a 2020 2020  "wb") as f:.    
+0001b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b720: 7069 636b 6c65 2e64 756d 7028 6366 7370  pickle.dump(cfsp
+0001b730: 6563 732c 2066 290a 2020 2020 2020 2020  ecs, f).        
+0001b740: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+0001b750: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+0001b760: 2020 2020 2020 2020 2020 2078 6f61 5f77             xoa_w
+0001b770: 6172 6e28 2245 7272 6f72 2077 6869 6c65  arn("Error while
+0001b780: 2063 6163 6869 6e67 2063 6620 7370 6563   caching cf spec
+0001b790: 733a 2022 202b 2073 7472 2865 2e61 7267  s: " + str(e.arg
+0001b7a0: 7329 290a 0a20 2020 2063 665f 6361 6368  s))..    cf_cach
+0001b7b0: 655b 2264 6566 6175 6c74 225d 203d 2063  e["default"] = c
+0001b7c0: 6673 7065 6373 0a20 2020 2069 6620 6e6f  fspecs.    if no
+0001b7d0: 7420 6973 5f72 6567 6973 7465 7265 645f  t is_registered_
+0001b7e0: 6366 5f73 7065 6373 2863 6673 7065 6373  cf_specs(cfspecs
+0001b7f0: 293a 0a20 2020 2020 2020 2072 6567 6973  ):.        regis
+0001b800: 7465 725f 6366 5f73 7065 6373 2863 6673  ter_cf_specs(cfs
+0001b810: 7065 6373 290a 2020 2020 7265 7475 726e  pecs).    return
+0001b820: 2063 6673 7065 6373 0a0a 0a64 6566 2067   cfspecs...def g
+0001b830: 6574 5f63 665f 7370 6563 7328 6e61 6d65  et_cf_specs(name
+0001b840: 3d4e 6f6e 652c 2063 6163 6865 3d22 7277  =None, cache="rw
+0001b850: 2229 3a0a 2020 2020 2222 2247 6574 2074  "):.    """Get t
+0001b860: 6865 2063 7572 7265 6e74 206f 7220 6120  he current or a 
+0001b870: 7265 6769 7374 6572 6564 2043 4620 7370  registered CF sp
+0001b880: 6563 6966 6963 6174 696f 6e73 2069 6e73  ecifications ins
+0001b890: 7461 6e63 650a 0a20 2020 2050 6172 616d  tance..    Param
+0001b8a0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+0001b8b0: 2d2d 2d2d 0a20 2020 206e 616d 653a 2073  ----.    name: s
+0001b8c0: 7472 2c20 2263 7572 7265 6e74 222c 2022  tr, "current", "
+0001b8d0: 6465 6661 756c 7422 2c20 4e6f 6e65 2c20  default", None, 
+0001b8e0: 7861 7272 6179 2e44 6174 6173 6574 2c20  xarray.Dataset, 
+0001b8f0: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
+0001b900: 0a20 2020 2020 2020 2022 6465 6661 756c  .        "defaul
+0001b910: 7422 206d 6561 6e73 2074 6865 2064 6566  t" means the def
+0001b920: 6175 6c74 2078 6f61 2073 7065 6373 2e0a  ault xoa specs..
+0001b930: 2020 2020 2020 2020 2263 7572 7265 6e74          "current
+0001b940: 2220 6973 2065 7175 6976 616c 656e 7420  " is equivalent 
+0001b950: 746f 204e 6f6e 6520 616e 6420 6d65 616e  to None and mean
+0001b960: 7320 7468 6520 6375 7272 656e 7473 2073  s the currents s
+0001b970: 7065 6373 2c0a 2020 2020 2020 2020 7768  pecs,.        wh
+0001b980: 6963 6820 6465 6661 756c 7473 2074 6f20  ich defaults to 
+0001b990: 7468 6520 786f 6120 6465 6661 756c 7473  the xoa defaults
+0001b9a0: 210a 2020 2020 2020 2020 456c 7365 2072  !.        Else r
+0001b9b0: 6567 6973 7472 6174 696f 6e20 6e61 6d65  egistration name
+0001b9c0: 2066 6f72 2074 6865 7365 2073 7065 6373   for these specs
+0001b9d0: 206f 7220 6120 6461 7461 2061 7272 6179   or a data array
+0001b9e0: 206f 7220 6461 7461 7365 740a 2020 2020   or dataset.    
+0001b9f0: 2020 2020 7468 6174 2063 616e 2062 6520      that can be 
+0001ba00: 7573 6564 2074 6f20 6765 7420 7468 6520  used to get the 
+0001ba10: 7265 6769 7374 7261 7469 6f6e 206e 616d  registration nam
+0001ba20: 6520 6966 2069 7420 7365 7420 696e 2074  e if it set in t
+0001ba30: 6865 0a20 2020 2020 2020 203a 6174 7472  he.        :attr
+0001ba40: 3a60 6366 5f73 7065 6373 6020 6174 7472  :`cf_specs` attr
+0001ba50: 6962 7574 6520 6f72 2065 6e63 6f64 696e  ibute or encodin
+0001ba60: 672e 0a20 2020 2020 2020 2057 6865 6e20  g..        When 
+0001ba70: 7365 742c 2060 6063 6163 6865 6060 2069  set, ``cache`` i
+0001ba80: 7320 6967 6e6f 7265 642e 0a20 2020 2020  s ignored..     
+0001ba90: 2020 2052 6169 7365 7320 6120 3a63 6c61     Raises a :cla
+0001baa0: 7373 3a60 586f 6143 4645 7272 6f72 6020  ss:`XoaCFError` 
+0001bab0: 6973 2063 6173 6520 6f66 2069 6e76 616c  is case of inval
+0001bac0: 6964 206e 616d 652e 0a20 2020 2063 6163  id name..    cac
+0001bad0: 6865 3a20 7374 722c 2062 6f6f 6c2c 204e  he: str, bool, N
+0001bae0: 6f6e 650a 2020 2020 2020 2020 4361 6368  one.        Cach
+0001baf0: 6520 6465 6661 756c 7420 7370 6563 7320  e default specs 
+0001bb00: 6f6e 2064 6973 6b20 7769 7468 2070 6963  on disk with pic
+0001bb10: 6b6c 696e 6720 666f 7220 6661 7374 206c  kling for fast l
+0001bb20: 6f61 6469 6e67 2e0a 2020 2020 2020 2020  oading..        
+0001bb30: 4966 2060 604e 6f6e 6560 602c 2069 7420  If ``None``, it 
+0001bb40: 6465 6661 756c 7473 2074 6f20 626f 6f6c  defaults to bool
+0001bb50: 6561 6e20 6f70 7469 6f6e 203a 786f 616f  ean option :xoao
+0001bb60: 7074 696f 6e3a 6063 662e 6361 6368 6560  ption:`cf.cache`
+0001bb70: 2e0a 2020 2020 2020 2020 506f 7373 6962  ..        Possib
+0001bb80: 6c65 2073 7472 696e 6720 7661 6c75 6573  le string values
+0001bb90: 3a20 6060 2269 676e 6f72 6522 6060 2c20  : ``"ignore"``, 
+0001bba0: 6060 2272 7722 6060 2c20 6060 2272 6561  ``"rw"``, ``"rea
+0001bbb0: 6422 6060 2c20 6060 2277 7269 7465 2260  d"``, ``"write"`
+0001bbc0: 602e 0a20 2020 2020 2020 2049 6620 6060  `..        If ``
+0001bbd0: 5472 7565 6060 2c20 6974 2069 7320 7365  True``, it is se
+0001bbe0: 7420 746f 2060 6022 7277 2260 602e 0a20  t to ``"rw"``.. 
+0001bbf0: 2020 2020 2020 2049 6620 6060 4661 6c73         If ``Fals
+0001bc00: 6560 602c 2069 7420 6973 2073 6574 2074  e``, it is set t
+0001bc10: 6f20 6060 2269 676e 6f72 6522 6060 2e0a  o ``"ignore"``..
+0001bc20: 0a20 2020 2052 6574 7572 6e0a 2020 2020  .    Return.    
+0001bc30: 2d2d 2d2d 2d2d 0a20 2020 2043 4653 7065  ------.    CFSpe
+0001bc40: 6373 0a20 2020 2020 2020 204e 6f6e 6520  cs.        None 
+0001bc50: 6973 2072 6574 7572 6e20 6966 206e 6f20  is return if no 
+0001bc60: 7370 6563 7320 6172 6520 666f 756e 640a  specs are found.
+0001bc70: 0a20 2020 2052 6169 7365 0a20 2020 202d  .    Raise.    -
+0001bc80: 2d2d 2d2d 0a20 2020 2058 6f61 4346 4572  ----.    XoaCFEr
+0001bc90: 726f 720a 2020 2020 2020 2020 5768 656e  ror.        When
+0001bca0: 2060 606e 616d 6560 6020 6973 2070 726f   ``name`` is pro
+0001bcb0: 7669 6465 6420 6173 2061 2073 7472 696e  vided as a strin
+0001bcc0: 6720 616e 6420 6973 2069 6e76 616c 6964  g and is invalid
+0001bcd0: 2e0a 2020 2020 2222 220a 2020 2020 2320  ..    """.    # 
+0001bce0: 4578 706c 6963 6974 2072 6571 7565 7374  Explicit request
+0001bcf0: 0a20 2020 2069 6620 6e61 6d65 2069 7320  .    if name is 
+0001bd00: 4e6f 6e65 3a0a 2020 2020 2020 2020 6e61  None:.        na
+0001bd10: 6d65 203d 2022 6375 7272 656e 7422 0a20  me = "current". 
+0001bd20: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+0001bd30: 616e 6365 286e 616d 652c 2073 7472 2920  ance(name, str) 
+0001bd40: 6f72 206e 616d 6520 6e6f 7420 696e 2028  or name not in (
+0001bd50: 2263 7572 7265 6e74 222c 2022 6465 6661  "current", "defa
+0001bd60: 756c 7422 293a 0a0a 2020 2020 2020 2020  ult"):..        
+0001bd70: 2320 5265 6769 7374 6572 6564 206e 616d  # Registered nam
+0001bd80: 650a 2020 2020 2020 2020 6966 2069 7369  e.        if isi
+0001bd90: 6e73 7461 6e63 6528 6e61 6d65 2c20 7374  nstance(name, st
+0001bda0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0001bdb0: 7265 7475 726e 2067 6574 5f63 665f 7370  return get_cf_sp
+0001bdc0: 6563 735f 6672 6f6d 5f6e 616d 6528 6e61  ecs_from_name(na
+0001bdd0: 6d65 2c20 6572 726f 7273 3d22 7261 6973  me, errors="rais
+0001bde0: 6522 290a 0a20 2020 2020 2020 2023 204e  e")..        # N
+0001bdf0: 616d 6520 6173 2064 6174 6173 6574 206f  ame as dataset o
+0001be00: 7220 6461 7461 2061 7272 6179 2073 6f20  r data array so 
+0001be10: 7765 2067 7565 7373 2074 6865 206e 616d  we guess the nam
+0001be20: 650a 2020 2020 2020 2020 6366 7370 6563  e.        cfspec
+0001be30: 7320 3d20 6765 745f 6366 5f73 7065 6373  s = get_cf_specs
+0001be40: 5f66 726f 6d5f 656e 636f 6469 6e67 286e  _from_encoding(n
+0001be50: 616d 6529 0a20 2020 2020 2020 2069 6620  ame).        if 
+0001be60: 6366 7370 6563 733a 0a20 2020 2020 2020  cfspecs:.       
+0001be70: 2020 2020 2072 6574 7572 6e20 6366 7370       return cfsp
+0001be80: 6563 730a 2020 2020 2020 2020 656c 7365  ecs.        else
+0001be90: 3a0a 2020 2020 2020 2020 2020 2020 6e61  :.            na
+0001bea0: 6d65 203d 2022 6375 7272 656e 7422 0a0a  me = "current"..
+0001beb0: 2020 2020 2320 4e6f 7420 6e61 6d65 6420      # Not named 
+0001bec0: 3d3e 2063 7572 7265 6e74 206f 7220 6465  => current or de
+0001bed0: 6661 756c 7420 7370 6563 730a 2020 2020  fault specs.    
+0001bee0: 6966 206e 616d 6520 3d3d 2022 6375 7272  if name == "curr
+0001bef0: 656e 7422 3a0a 2020 2020 2020 2020 6366  ent":.        cf
+0001bf00: 5f63 6163 6865 203d 205f 6765 745f 6361  _cache = _get_ca
+0001bf10: 6368 655f 2829 0a20 2020 2020 2020 2069  che_().        i
+0001bf20: 6620 6366 5f63 6163 6865 5b22 6375 7272  f cf_cache["curr
+0001bf30: 656e 7422 5d20 6973 204e 6f6e 653a 0a20  ent"] is None:. 
+0001bf40: 2020 2020 2020 2020 2020 2063 665f 6361             cf_ca
+0001bf50: 6368 655b 2263 7572 7265 6e74 225d 203d  che["current"] =
+0001bf60: 2067 6574 5f64 6566 6175 6c74 5f63 665f   get_default_cf_
+0001bf70: 7370 6563 7328 290a 2020 2020 2020 2020  specs().        
+0001bf80: 6366 7370 6563 7320 3d20 6366 5f63 6163  cfspecs = cf_cac
+0001bf90: 6865 5b22 6375 7272 656e 7422 5d0a 2020  he["current"].  
+0001bfa0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001bfb0: 6366 7370 6563 7320 3d20 6765 745f 6465  cfspecs = get_de
+0001bfc0: 6661 756c 745f 6366 5f73 7065 6373 2829  fault_cf_specs()
+0001bfd0: 0a0a 2020 2020 7265 7475 726e 2063 6673  ..    return cfs
+0001bfe0: 7065 6373 0a0a 0a64 6566 2072 6567 6973  pecs...def regis
+0001bff0: 7465 725f 6366 5f73 7065 6373 282a 6172  ter_cf_specs(*ar
+0001c000: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
+0001c010: 2020 2022 2222 5265 6769 7374 6572 203a     """Register :
+0001c020: 636c 6173 733a 6043 4653 7065 6373 6020  class:`CFSpecs` 
+0001c030: 696e 2061 2062 616e 6b20 6f70 7469 6f6e  in a bank option
+0001c040: 616c 6c79 2077 6974 6820 6120 6e61 6d65  ally with a name
+0001c050: 2222 220a 2020 2020 6172 6773 203d 206c  """.    args = l
+0001c060: 6973 7428 6172 6773 290a 2020 2020 666f  ist(args).    fo
+0001c070: 7220 6e61 6d65 2c20 6366 7370 6563 7320  r name, cfspecs 
+0001c080: 696e 206b 7761 7267 732e 6974 656d 7328  in kwargs.items(
+0001c090: 293a 0a20 2020 2020 2020 2069 6620 6e6f  ):.        if no
+0001c0a0: 7420 6973 696e 7374 616e 6365 2863 6673  t isinstance(cfs
+0001c0b0: 7065 6373 2c20 4346 5370 6563 7329 3a0a  pecs, CFSpecs):.
+0001c0c0: 2020 2020 2020 2020 2020 2020 6366 7370              cfsp
+0001c0d0: 6563 7320 3d20 4346 5370 6563 7328 6366  ecs = CFSpecs(cf
+0001c0e0: 7370 6563 7329 0a20 2020 2020 2020 2063  specs).        c
+0001c0f0: 6673 7065 6373 2e6e 616d 6520 3d20 6e61  fspecs.name = na
+0001c100: 6d65 0a20 2020 2020 2020 2061 7267 732e  me.        args.
+0001c110: 6170 7065 6e64 2863 6673 7065 6373 290a  append(cfspecs).
+0001c120: 2020 2020 666f 7220 6366 7370 6563 7320      for cfspecs 
+0001c130: 696e 2061 7267 733a 0a20 2020 2020 2020  in args:.       
+0001c140: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+0001c150: 6365 2863 6673 7065 6373 2c20 4346 5370  ce(cfspecs, CFSp
+0001c160: 6563 7329 3a0a 2020 2020 2020 2020 2020  ecs):.          
+0001c170: 2020 6366 7370 6563 7320 3d20 4346 5370    cfspecs = CFSp
+0001c180: 6563 7328 6366 7370 6563 7329 0a20 2020  ecs(cfspecs).   
+0001c190: 2020 2020 2063 665f 6361 6368 6520 3d20       cf_cache = 
+0001c1a0: 5f67 6574 5f63 6163 6865 5f28 290a 2020  _get_cache_().  
+0001c1b0: 2020 2020 2020 6966 2063 6673 7065 6373        if cfspecs
+0001c1c0: 206e 6f74 2069 6e20 6366 5f63 6163 6865   not in cf_cache
+0001c1d0: 5b22 7265 6769 7374 6572 6564 225d 3a0a  ["registered"]:.
+0001c1e0: 2020 2020 2020 2020 2020 2020 6366 5f63              cf_c
+0001c1f0: 6163 6865 5b22 7265 6769 7374 6572 6564  ache["registered
+0001c200: 225d 2e61 7070 656e 6428 6366 7370 6563  "].append(cfspec
+0001c210: 7329 0a0a 0a64 6566 2067 6574 5f72 6567  s)...def get_reg
+0001c220: 6973 7465 7265 645f 6366 5f73 7065 6373  istered_cf_specs
+0001c230: 2863 7572 7265 6e74 3d54 7275 652c 2072  (current=True, r
+0001c240: 6576 6572 7365 3d54 7275 652c 206e 616d  everse=True, nam
+0001c250: 6564 3d46 616c 7365 293a 0a20 2020 2022  ed=False):.    "
+0001c260: 2222 4765 7420 7468 6520 6c69 7374 206f  ""Get the list o
+0001c270: 6620 7265 6769 7374 6572 6564 2043 4653  f registered CFS
+0001c280: 7065 6373 0a0a 2020 2020 5061 7261 6d65  pecs..    Parame
+0001c290: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0001c2a0: 2d2d 2d0a 2020 2020 6375 7272 656e 743a  ---.    current:
+0001c2b0: 2062 6f6f 6c0a 2020 2020 2020 2020 416c   bool.        Al
+0001c2c0: 736f 2069 6e63 6c75 6465 2074 6865 2063  so include the c
+0001c2d0: 7572 7265 6e74 2073 7065 6373 2069 6620  urrent specs if 
+0001c2e0: 616e 792c 2061 6c77 6179 7320 6174 2074  any, always at t
+0001c2f0: 6865 206c 6173 7420 706f 7369 7469 6f6e  he last position
+0001c300: 0a20 2020 2072 6576 6572 7365 3a20 626f  .    reverse: bo
+0001c310: 6f6c 0a20 2020 2020 2020 2052 6576 6572  ol.        Rever
+0001c320: 7365 2074 6865 206c 6973 740a 2020 2020  se the list.    
+0001c330: 6e61 6d65 643a 2062 6f6f 6c0a 2020 2020  named: bool.    
+0001c340: 2020 2020 4d61 6b65 2073 7572 6520 7468      Make sure th
+0001c350: 6520 7265 7475 726e 6564 2043 4653 7065  e returned CFSpe
+0001c360: 6373 2068 6176 6520 6120 7661 6c69 6420  cs have a valid 
+0001c370: 7265 6769 7374 7261 7469 6f6e 206e 616d  registration nam
+0001c380: 650a 0a20 2020 2052 6574 7572 6e0a 2020  e..    Return.  
+0001c390: 2020 2d2d 2d2d 2d2d 0a20 2020 206c 6973    ------.    lis
+0001c3a0: 740a 0a20 2020 2053 6565 2061 6c73 6f0a  t..    See also.
+0001c3b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0001c3c0: 2072 6567 6973 7465 725f 6366 5f73 7065   register_cf_spe
+0001c3d0: 6373 0a20 2020 2022 2222 0a20 2020 2063  cs.    """.    c
+0001c3e0: 665f 6361 6368 6520 3d20 5f67 6574 5f63  f_cache = _get_c
+0001c3f0: 6163 6865 5f28 290a 2020 2020 6366 6c20  ache_().    cfl 
+0001c400: 3d20 6366 5f63 6163 6865 5b22 7265 6769  = cf_cache["regi
+0001c410: 7374 6572 6564 225d 0a20 2020 2069 6620  stered"].    if 
+0001c420: 7265 7665 7273 653a 0a20 2020 2020 2020  reverse:.       
+0001c430: 2063 666c 203d 2063 666c 5b3a 3a2d 315d   cfl = cfl[::-1]
+0001c440: 0a20 2020 2069 6620 6375 7272 656e 7420  .    if current 
+0001c450: 616e 6420 6366 5f63 6163 6865 5b22 6375  and cf_cache["cu
+0001c460: 7272 656e 7422 5d20 6973 206e 6f74 204e  rrent"] is not N
+0001c470: 6f6e 653a 0a20 2020 2020 2020 2063 666c  one:.        cfl
+0001c480: 2e61 7070 656e 6428 6366 5f63 6163 6865  .append(cf_cache
+0001c490: 5b22 6375 7272 656e 7422 5d29 0a20 2020  ["current"]).   
+0001c4a0: 2069 6620 6e61 6d65 6420 6973 2046 616c   if named is Fal
+0001c4b0: 7365 3a0a 2020 2020 2020 2020 6366 6465  se:.        cfde
+0001c4c0: 6620 3d20 6765 745f 6465 6661 756c 745f  f = get_default_
+0001c4d0: 6366 5f73 7065 6373 2829 0a20 2020 2020  cf_specs().     
+0001c4e0: 2020 2069 6620 6366 6465 6620 6e6f 7420     if cfdef not 
+0001c4f0: 696e 2063 666c 3a0a 2020 2020 2020 2020  in cfl:.        
+0001c500: 2020 2020 6366 6c2e 6170 7065 6e64 2863      cfl.append(c
+0001c510: 6664 6566 290a 2020 2020 656c 7365 3a0a  fdef).    else:.
+0001c520: 2020 2020 2020 2020 6366 6c20 3d20 5b63          cfl = [c
+0001c530: 2066 6f72 2063 2069 6e20 6366 6c20 6966   for c in cfl if
+0001c540: 2063 2e6e 616d 655d 0a20 2020 2072 6574   c.name].    ret
+0001c550: 7572 6e20 6366 6c0a 0a0a 6465 6620 6973  urn cfl...def is
+0001c560: 5f72 6567 6973 7465 7265 645f 6366 5f73  _registered_cf_s
+0001c570: 7065 6373 286e 616d 6529 3a0a 2020 2020  pecs(name):.    
+0001c580: 2222 2243 6865 636b 2069 6620 6769 7665  """Check if give
+0001c590: 6e20 6366 2073 7065 6373 2073 6574 2069  n cf specs set i
+0001c5a0: 7320 7265 6769 7374 6572 6564 0a0a 2020  s registered..  
+0001c5b0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0001c5c0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0001c5d0: 6e61 6d65 3a20 7374 722c 2043 4653 7065  name: str, CFSpe
+0001c5e0: 6373 0a0a 2020 2020 5265 7475 726e 0a20  cs..    Return. 
+0001c5f0: 2020 202d 2d2d 2d2d 2d0a 2020 2020 626f     ------.    bo
+0001c600: 6f6c 0a20 2020 2022 2222 0a20 2020 2066  ol.    """.    f
+0001c610: 6f72 2063 6673 7065 6373 2069 6e20 6765  or cfspecs in ge
+0001c620: 745f 7265 6769 7374 6572 6564 5f63 665f  t_registered_cf_
+0001c630: 7370 6563 7328 293a 0a20 2020 2020 2020  specs():.       
+0001c640: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
+0001c650: 2020 6973 696e 7374 616e 6365 286e 616d    isinstance(nam
+0001c660: 652c 2073 7472 290a 2020 2020 2020 2020  e, str).        
+0001c670: 2020 2020 616e 6420 6366 7370 6563 735b      and cfspecs[
+0001c680: 2272 6567 6973 7465 7222 5d5b 226e 616d  "register"]["nam
+0001c690: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
+0001c6a0: 616e 6420 6366 7370 6563 735b 2272 6567  and cfspecs["reg
+0001c6b0: 6973 7465 7222 5d5b 226e 616d 6522 5d20  ister"]["name"] 
+0001c6c0: 3d3d 206e 616d 650a 2020 2020 2020 2020  == name.        
+0001c6d0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+0001c6e0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+0001c6f0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0001c700: 286e 616d 652c 2043 4653 7065 6373 2920  (name, CFSpecs) 
+0001c710: 616e 6420 6e61 6d65 2069 7320 6366 7370  and name is cfsp
+0001c720: 6563 733a 0a20 2020 2020 2020 2020 2020  ecs:.           
+0001c730: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+0001c740: 2072 6574 7572 6e20 4661 6c73 650a 0a0a   return False...
+0001c750: 6465 6620 6765 745f 6366 5f73 7065 6373  def get_cf_specs
+0001c760: 5f6d 6174 6368 696e 675f 7363 6f72 6528  _matching_score(
+0001c770: 6473 2c20 6366 7370 6563 7329 3a0a 2020  ds, cfspecs):.  
+0001c780: 2020 2222 2247 6574 2074 6865 206d 6174    """Get the mat
+0001c790: 6368 696e 6720 7363 6f72 6520 6265 7477  ching score betw
+0001c7a0: 6565 6e20 6473 2064 6174 615f 7661 7273  een ds data_vars
+0001c7b0: 2061 6e64 2063 6f6f 7264 206e 616d 6573   and coord names
+0001c7c0: 2061 6e64 2061 2043 4653 7065 6373 2069   and a CFSpecs i
+0001c7d0: 6e73 7461 6e63 6520 6e61 6d65 730a 0a20  nstance names.. 
+0001c7e0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0001c7f0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0001c800: 2064 733a 2078 6172 7261 792e 4461 7461   ds: xarray.Data
+0001c810: 7365 742c 2078 6172 7261 792e 4461 7461  set, xarray.Data
+0001c820: 4172 7261 790a 2020 2020 6366 5f73 7065  Array.    cf_spe
+0001c830: 6373 3a20 4346 5370 6563 730a 0a20 2020  cs: CFSpecs..   
+0001c840: 2052 6574 7572 6e0a 2020 2020 2d2d 2d2d   Return.    ----
+0001c850: 2d2d 0a20 2020 2066 6c6f 6174 0a20 2020  --.    float.   
+0001c860: 2020 2020 2041 2070 6572 6365 6e74 6167       A percentag
+0001c870: 6520 6f66 2074 6865 206e 756d 6265 7220  e of the number 
+0001c880: 6f66 2069 6465 6e74 6966 6965 6420 6461  of identified da
+0001c890: 7461 2061 7272 6179 7320 7673 0a20 2020  ta arrays vs.   
+0001c8a0: 2020 2020 2074 6865 2074 6f74 616c 206e       the total n
+0001c8b0: 756d 6265 7220 6f66 2064 6174 6120 6172  umber of data ar
+0001c8c0: 7261 7973 0a20 2020 2022 2222 0a20 2020  rays.    """.   
+0001c8d0: 2068 6974 203d 2030 0a20 2020 2074 6f74   hit = 0.    tot
+0001c8e0: 616c 203d 2030 0a20 2020 2066 6f72 2063  al = 0.    for c
+0001c8f0: 6174 2069 6e20 2264 6174 615f 7661 7273  at in "data_vars
+0001c900: 222c 2022 636f 6f72 6473 223a 0a20 2020  ", "coords":.   
+0001c910: 2020 2020 2063 666e 616d 6573 203d 205b       cfnames = [
+0001c920: 6366 7370 6563 735b 6361 745d 2e67 6574  cfspecs[cat].get
+0001c930: 5f6e 616d 6528 6e61 6d65 2c20 7370 6563  _name(name, spec
+0001c940: 6961 6c69 7a65 3d54 7275 6529 2066 6f72  ialize=True) for
+0001c950: 206e 616d 6520 696e 2063 6673 7065 6373   name in cfspecs
+0001c960: 5b63 6174 5d2e 6e61 6d65 735d 0a20 2020  [cat].names].   
+0001c970: 2020 2020 2069 6620 6e6f 7420 6861 7361       if not hasa
+0001c980: 7474 7228 6473 2c20 2264 6174 615f 7661  ttr(ds, "data_va
+0001c990: 7273 2229 3a20 2023 2044 6174 6141 7272  rs"):  # DataArr
+0001c9a0: 6179 0a20 2020 2020 2020 2020 2020 2064  ay.            d
+0001c9b0: 736e 616d 6573 203d 205b 6473 2e6e 616d  snames = [ds.nam
+0001c9c0: 655d 2069 6620 6473 2e6e 616d 6520 656c  e] if ds.name el
+0001c9d0: 7365 205b 5d0a 2020 2020 2020 2020 656c  se [].        el
+0001c9e0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001c9f0: 6473 6e61 6d65 7320 3d20 6c69 7374 2867  dsnames = list(g
+0001ca00: 6574 6174 7472 2864 732c 2063 6174 292e  etattr(ds, cat).
+0001ca10: 6b65 7973 2829 290a 2020 2020 2020 2020  keys()).        
+0001ca20: 6473 6e61 6d65 7320 3d20 5b63 6673 7065  dsnames = [cfspe
+0001ca30: 6373 2e73 676c 6f63 6174 6f72 2e70 6172  cs.sglocator.par
+0001ca40: 7365 5f61 7474 7228 226e 616d 6522 2c20  se_attr("name", 
+0001ca50: 6473 6e61 6d65 295b 305d 2066 6f72 2064  dsname)[0] for d
+0001ca60: 736e 616d 6520 696e 2064 736e 616d 6573  sname in dsnames
+0001ca70: 5d0a 2020 2020 2020 2020 746f 7461 6c20  ].        total 
+0001ca80: 2b3d 206c 656e 2864 736e 616d 6573 290a  += len(dsnames).
+0001ca90: 2020 2020 2020 2020 6869 7420 2b3d 206c          hit += l
+0001caa0: 656e 2873 6574 2864 736e 616d 6573 292e  en(set(dsnames).
+0001cab0: 696e 7465 7273 6563 7469 6f6e 2863 666e  intersection(cfn
+0001cac0: 616d 6573 2929 0a20 2020 2069 6620 746f  ames)).    if to
+0001cad0: 7461 6c20 3d3d 2030 3a0a 2020 2020 2020  tal == 0:.      
+0001cae0: 2020 7265 7475 726e 2030 0a20 2020 2072    return 0.    r
+0001caf0: 6574 7572 6e20 3130 3020 2a20 6869 7420  eturn 100 * hit 
+0001cb00: 2f20 746f 7461 6c0a 0a0a 6465 6620 696e  / total...def in
+0001cb10: 6665 725f 6366 5f73 7065 6373 2864 732c  fer_cf_specs(ds,
+0001cb20: 206e 616d 6564 3d46 616c 7365 293a 0a20   named=False):. 
+0001cb30: 2020 2022 2222 4765 7420 7468 6520 7265     """Get the re
+0001cb40: 6769 7374 6572 6564 2043 4653 7065 6373  gistered CFSpecs
+0001cb50: 2074 6861 7420 6172 6520 6265 7374 206d   that are best m
+0001cb60: 6174 6368 696e 6720 7468 6973 2064 6174  atching this dat
+0001cb70: 6173 6574 0a0a 2020 2020 5468 6973 2061  aset..    This a
+0001cb80: 6363 6f6d 706c 6973 6865 6420 7769 7468  ccomplished with
+0001cb90: 2073 6f6d 6520 6865 7572 6573 7469 6373   some heurestics
+0001cba0: 2e0a 2020 2020 4669 7273 742c 2074 6865  ..    First, the
+0001cbb0: 203a 6174 7472 3a60 6366 5f73 7065 6373   :attr:`cf_specs
+0001cbc0: 6020 676c 6f62 616c 2061 7474 7269 6275  ` global attribu
+0001cbd0: 7465 206f 7220 656e 636f 6469 6e67 206f  te or encoding o
+0001cbe0: 6620 7468 6520 6461 7461 7365 7420 6973  f the dataset is
+0001cbf0: 2063 6f6d 7061 7265 640a 2020 2020 7769   compared.    wi
+0001cc00: 7468 2074 6865 206e 616d 6520 6f66 2061  th the name of a
+0001cc10: 6c6c 2072 6567 6973 7465 7265 6420 6461  ll registered da
+0001cc20: 7461 7365 7473 2e0a 2020 2020 5365 636f  tasets..    Seco
+0001cc30: 6e64 2c20 6120 7363 6f72 6520 6261 7365  nd, a score base
+0001cc40: 6420 6f6e 2074 6865 206e 756d 6265 7220  d on the number 
+0001cc50: 6f66 2064 6174 615f 7661 7273 2061 6e64  of data_vars and
+0001cc60: 2063 6f6f 7264 206e 616d 6573 0a20 2020   coord names.   
+0001cc70: 2074 6861 7420 6172 6520 626f 7468 2069   that are both i
+0001cc80: 6e20 7468 6520 6366 7370 6563 7320 616e  n the cfspecs an
+0001cc90: 6420 7468 6520 6461 7461 7365 7420 6973  d the dataset is
+0001cca0: 2063 6f6d 7075 7465 6420 6279 203a 6675   computed by :fu
+0001ccb0: 6e63 3a60 6765 745f 6366 5f73 7065 6373  nc:`get_cf_specs
+0001ccc0: 5f6d 6174 6368 696e 675f 7363 6f72 6560  _matching_score`
+0001ccd0: 0a20 2020 2066 6f72 2074 6865 2072 6567  .    for the reg
+0001cce0: 6973 7465 7265 6420 696e 7374 616e 6365  istered instance
+0001ccf0: 732e 0a20 2020 2046 696e 616c 6c79 2c20  s..    Finally, 
+0001cd00: 6966 206e 6f20 6d61 7463 6869 6e67 2064  if no matching d
+0001cd10: 6174 6173 6574 2069 7320 666f 756e 642c  ataset is found,
+0001cd20: 2074 6865 2063 7572 7265 6e74 206f 6e65   the current one
+0001cd30: 2069 7320 7265 7475 726e 6564 2e0a 0a0a   is returned....
+0001cd40: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0001cd50: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0001cd60: 2020 6473 3a20 7861 7272 6179 2e44 6174    ds: xarray.Dat
+0001cd70: 6173 6574 2c20 7861 7272 6179 2e44 6174  aset, xarray.Dat
+0001cd80: 6141 7272 6179 0a20 2020 206e 616d 6564  aArray.    named
+0001cd90: 3a20 626f 6f6c 0a20 2020 2020 2020 204d  : bool.        M
+0001cda0: 616b 6520 7375 7265 2074 6865 2063 616e  ake sure the can
+0001cdb0: 6469 6461 7465 2043 4653 7065 6373 2068  didate CFSpecs h
+0001cdc0: 6176 6520 6120 6e61 6d65 0a0a 2020 2020  ave a name..    
+0001cdd0: 5265 7475 726e 0a20 2020 202d 2d2d 2d2d  Return.    -----
+0001cde0: 2d0a 2020 2020 4346 5370 6563 730a 2020  -.    CFSpecs.  
+0001cdf0: 2020 2020 2020 5468 6520 6d61 7463 6869        The matchi
+0001ce00: 6e67 2063 6620 7370 6563 7320 6f72 2074  ng cf specs or t
+0001ce10: 6865 2063 7572 7265 6e74 206f 6e65 730a  he current ones.
+0001ce20: 0a20 2020 2053 6565 2061 6c73 6f0a 2020  .    See also.  
+0001ce30: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2072    --------.    r
+0001ce40: 6567 6973 7465 725f 6366 5f73 7065 6373  egister_cf_specs
+0001ce50: 0a20 2020 2067 6574 5f72 6567 6973 7465  .    get_registe
+0001ce60: 7265 645f 6366 5f73 7065 6373 0a20 2020  red_cf_specs.   
+0001ce70: 2067 6574 5f63 665f 7370 6563 735f 6d61   get_cf_specs_ma
+0001ce80: 7463 6869 6e67 5f73 636f 7265 0a20 2020  tching_score.   
+0001ce90: 2067 6574 5f63 665f 7370 6563 730a 2020   get_cf_specs.  
+0001cea0: 2020 6765 745f 6366 5f73 7065 6373 0a20    get_cf_specs. 
+0001ceb0: 2020 2067 6574 5f63 665f 7370 6563 735f     get_cf_specs_
+0001cec0: 6672 6f6d 5f6e 616d 650a 2020 2020 6765  from_name.    ge
+0001ced0: 745f 6366 5f73 7065 6373 5f66 726f 6d5f  t_cf_specs_from_
+0001cee0: 656e 636f 6469 6e67 0a20 2020 2022 2222  encoding.    """
+0001cef0: 0a20 2020 2023 2042 7920 7265 6769 7374  .    # By regist
+0001cf00: 7261 7469 6f6e 206e 616d 6520 6669 7273  ration name firs
+0001cf10: 740a 2020 2020 6366 7370 6563 7320 3d20  t.    cfspecs = 
+0001cf20: 6765 745f 6366 5f73 7065 6373 5f66 726f  get_cf_specs_fro
+0001cf30: 6d5f 656e 636f 6469 6e67 2864 7329 0a20  m_encoding(ds). 
+0001cf40: 2020 2069 6620 6366 7370 6563 733a 0a20     if cfspecs:. 
+0001cf50: 2020 2020 2020 2072 6574 7572 6e20 6366         return cf
+0001cf60: 7370 6563 730a 0a20 2020 2023 2043 616e  specs..    # Can
+0001cf70: 6469 6461 7465 730a 2020 2020 6361 6e64  didates.    cand
+0001cf80: 6964 6174 6573 203d 2067 6574 5f72 6567  idates = get_reg
+0001cf90: 6973 7465 7265 645f 6366 5f73 7065 6373  istered_cf_specs
+0001cfa0: 286e 616d 6564 3d6e 616d 6564 290a 0a20  (named=named).. 
+0001cfb0: 2020 2023 2042 7920 6174 7472 6962 7574     # By attribut
+0001cfc0: 6573 0a20 2020 2061 7474 7273 203d 2064  es.    attrs = d
+0001cfd0: 6963 7428 6473 2e61 7474 7273 290a 2020  ict(ds.attrs).  
+0001cfe0: 2020 6174 7472 732e 7570 6461 7465 2864    attrs.update(d
+0001cff0: 732e 656e 636f 6469 6e67 290a 2020 2020  s.encoding).    
+0001d000: 6966 2061 7474 7273 3a0a 2020 2020 2020  if attrs:.      
+0001d010: 2020 666f 7220 6366 7370 6563 7320 696e    for cfspecs in
+0001d020: 2063 616e 6469 6461 7465 733a 0a20 2020   candidates:.   
+0001d030: 2020 2020 2020 2020 2066 6f72 2061 7474           for att
+0001d040: 722c 2070 6174 7465 726e 2069 6e20 6366  r, pattern in cf
+0001d050: 7370 6563 735b 2272 6567 6973 7465 7222  specs["register"
+0001d060: 5d5b 2261 7474 7273 225d 2e69 7465 6d73  ]["attrs"].items
+0001d070: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0001d080: 2020 2020 6966 2061 7474 7220 696e 2061      if attr in a
+0001d090: 7474 7273 3a0a 2020 2020 2020 2020 2020  ttrs:.          
+0001d0a0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+0001d0b0: 6e73 7461 6e63 6528 7061 7474 6572 6e2c  nstance(pattern,
+0001d0c0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+0001d0d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001d0e0: 6174 7465 726e 203d 205b 7061 7474 6572  attern = [patter
+0001d0f0: 6e5d 0a20 2020 2020 2020 2020 2020 2020  n].             
+0001d100: 2020 2020 2020 2066 6f72 2070 6174 2069         for pat i
+0001d110: 6e20 7061 7474 6572 6e3a 0a20 2020 2020  n pattern:.     
+0001d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d130: 2020 2069 6620 666e 6d61 7463 682e 666e     if fnmatch.fn
+0001d140: 6d61 7463 6828 7374 7228 6174 7472 735b  match(str(attrs[
+0001d150: 6174 7472 5d29 2e6c 6f77 6572 2829 2c20  attr]).lower(), 
+0001d160: 7061 742e 6c6f 7765 7228 2929 3a0a 2020  pat.lower()):.  
+0001d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d180: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001d190: 2063 6673 7065 6373 0a0a 2020 2020 2320   cfspecs..    # 
+0001d1a0: 4279 206d 6174 6368 696e 6720 7363 6f72  By matching scor
+0001d1b0: 650a 2020 2020 6265 7374 5f73 636f 7265  e.    best_score
+0001d1c0: 203d 202d 310a 2020 2020 666f 7220 6366   = -1.    for cf
+0001d1d0: 7370 6563 7320 696e 2063 616e 6469 6461  specs in candida
+0001d1e0: 7465 733a 0a20 2020 2020 2020 2073 636f  tes:.        sco
+0001d1f0: 7265 203d 2067 6574 5f63 665f 7370 6563  re = get_cf_spec
+0001d200: 735f 6d61 7463 6869 6e67 5f73 636f 7265  s_matching_score
+0001d210: 2864 732c 2063 6673 7065 6373 290a 2020  (ds, cfspecs).  
+0001d220: 2020 2020 2020 6966 2073 636f 7265 2021        if score !
+0001d230: 3d20 3020 616e 6420 7363 6f72 6520 3e20  = 0 and score > 
+0001d240: 6265 7374 5f73 636f 7265 3a0a 2020 2020  best_score:.    
+0001d250: 2020 2020 2020 2020 6265 7374 5f63 6673          best_cfs
+0001d260: 7065 6373 203d 2063 6673 7065 6373 0a20  pecs = cfspecs. 
+0001d270: 2020 2020 2020 2020 2020 2062 6573 745f             best_
+0001d280: 7363 6f72 6520 3d20 7363 6f72 650a 2020  score = score.  
+0001d290: 2020 6966 2062 6573 745f 7363 6f72 6520    if best_score 
+0001d2a0: 213d 202d 313a 0a20 2020 2020 2020 2072  != -1:.        r
+0001d2b0: 6574 7572 6e20 6265 7374 5f63 6673 7065  eturn best_cfspe
+0001d2c0: 6373 0a0a 2020 2020 2320 4661 6c6c 6261  cs..    # Fallba
+0001d2d0: 636b 2074 6f20 6465 6661 756c 7420 7370  ck to default sp
+0001d2e0: 6563 730a 2020 2020 6366 7370 6563 7320  ecs.    cfspecs 
+0001d2f0: 3d20 6765 745f 6366 5f73 7065 6373 2829  = get_cf_specs()
+0001d300: 0a20 2020 2069 6620 6e61 6d65 6420 616e  .    if named an
+0001d310: 6420 6e6f 7420 6366 7370 6563 732e 6e61  d not cfspecs.na
+0001d320: 6d65 3a0a 2020 2020 2020 2020 7265 7475  me:.        retu
+0001d330: 726e 0a20 2020 2072 6574 7572 6e20 6366  rn.    return cf
+0001d340: 7370 6563 730a 0a0a 6465 6620 6173 7369  specs...def assi
+0001d350: 676e 5f63 665f 7370 6563 7328 6473 2c20  gn_cf_specs(ds, 
+0001d360: 6e61 6d65 3d4e 6f6e 652c 2072 6567 6973  name=None, regis
+0001d370: 7465 723d 4661 6c73 6529 3a0a 2020 2020  ter=False):.    
+0001d380: 2222 2253 6574 2074 6865 2060 6063 665f  """Set the ``cf_
+0001d390: 7370 6563 7360 6020 656e 636f 6469 6e67  specs`` encoding
+0001d3a0: 2074 6f20 6060 6e61 6d65 6060 2069 6e20   to ``name`` in 
+0001d3b0: 616c 6c20 6461 7461 2076 6172 7320 616e  all data vars an
+0001d3c0: 6420 636f 6f72 6473 0a0a 2020 2020 5061  d coords..    Pa
+0001d3d0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+0001d3e0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6473 3a20  -------.    ds: 
+0001d3f0: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
+0001d400: 2c20 7861 7272 6179 2e44 6174 6173 6574  , xarray.Dataset
+0001d410: 0a20 2020 206e 616d 653a 204e 6f6e 652c  .    name: None,
+0001d420: 2073 7472 2c20 4346 5370 6563 732c 2078   str, CFSpecs, x
+0001d430: 6172 7261 792e 4461 7461 4172 7261 792c  array.DataArray,
+0001d440: 2078 6172 7261 792e 4461 7461 7365 740a   xarray.Dataset.
+0001d450: 2020 2020 2020 2020 4966 2061 203a 636c          If a :cl
+0001d460: 6173 733a 6043 4653 7065 6373 602c 2069  ass:`CFSpecs`, i
+0001d470: 7420 6d75 7374 2068 6176 6520 6120 7265  t must have a re
+0001d480: 6769 7374 7261 7469 6f6e 206e 616d 6520  gistration name 
+0001d490: 3a0a 0a20 2020 2020 2020 202e 2e20 636f  :..        .. co
+0001d4a0: 6465 2d62 6c6f 636b 3a3a 2069 6e69 0a0a  de-block:: ini..
+0001d4b0: 2020 2020 2020 2020 2020 2020 5b72 6567              [reg
+0001d4c0: 6973 7465 725d 0a20 2020 2020 2020 2020  ister].         
+0001d4d0: 2020 206e 616d 653d 7265 6769 7374 7261     name=registra
+0001d4e0: 7469 6f6e 5f6e 616d 650a 0a20 2020 2020  tion_name..     
+0001d4f0: 2020 2049 6620 6e6f 7420 7072 6f76 6964     If not provid
+0001d500: 6564 2c20 3a66 756e 633a 6069 6e66 6572  ed, :func:`infer
+0001d510: 5f63 665f 7370 6563 7360 2069 7320 6361  _cf_specs` is ca
+0001d520: 6c6c 6564 2074 6f20 696e 6665 720a 2020  lled to infer.  
+0001d530: 2020 2020 2020 7468 6520 6265 7374 206e        the best n
+0001d540: 616d 6564 2072 6567 6973 7465 7265 6420  amed registered 
+0001d550: 7370 6563 732e 0a0a 2020 2020 7265 6769  specs...    regi
+0001d560: 7374 6572 3a20 626f 6f6c 0a20 2020 2020  ster: bool.     
+0001d570: 2020 2052 6567 6973 7465 7220 7468 6520     Register the 
+0001d580: 7370 6563 7320 6966 206e 616d 6520 6973  specs if name is
+0001d590: 2061 206e 616d 6564 2c20 756e 7265 6769   a named, unregi
+0001d5a0: 7374 6572 6564 203a 636c 6173 733a 6043  stered :class:`C
+0001d5b0: 4653 7065 6373 6020 696e 7374 616e 6365  FSpecs` instance
+0001d5c0: 2e0a 0a20 2020 2052 6574 7572 6e0a 2020  ...    Return.  
+0001d5d0: 2020 2d2d 2d2d 2d2d 0a20 2020 2078 6172    ------.    xar
+0001d5e0: 7261 792e 4461 7461 7365 742c 2078 6172  ray.Dataset, xar
+0001d5f0: 7261 792e 4461 7461 4172 7261 790a 0a20  ray.DataArray.. 
+0001d600: 2020 2045 7861 6d70 6c65 0a20 2020 202d     Example.    -
+0001d610: 2d2d 2d2d 2d2d 0a20 2020 202e 2e20 6970  ------.    .. ip
+0001d620: 7974 686f 6e3a 3a20 7079 7468 6f6e 0a0a  ython:: python..
+0001d630: 2020 2020 2020 2020 4073 7570 7072 6573          @suppres
+0001d640: 730a 2020 2020 2020 2020 6672 6f6d 2078  s.        from x
+0001d650: 6f61 2e63 6620 696d 706f 7274 2061 7373  oa.cf import ass
+0001d660: 6967 6e5f 6366 5f73 7065 6373 0a20 2020  ign_cf_specs.   
+0001d670: 2020 2020 2040 7375 7070 7265 7373 0a20       @suppress. 
+0001d680: 2020 2020 2020 2069 6d70 6f72 7420 7861         import xa
+0001d690: 7272 6179 2061 7320 7872 0a20 2020 2020  rray as xr.     
+0001d6a0: 2020 2064 7320 3d20 7872 2e44 6174 6173     ds = xr.Datas
+0001d6b0: 6574 287b 2774 656d 7027 3a20 2827 6c6f  et({'temp': ('lo
+0001d6c0: 6e27 2c20 5b35 5d29 7d2c 2063 6f6f 7264  n', [5])}, coord
+0001d6d0: 733d 7b27 6c6f 6e27 3a20 5b36 5d7d 290a  s={'lon': [6]}).
+0001d6e0: 2020 2020 2020 2020 6173 7369 676e 5f63          assign_c
+0001d6f0: 665f 7370 6563 7328 6473 2c20 226d 7963  f_specs(ds, "myc
+0001d700: 726f 636f 2229 3b0a 2020 2020 2020 2020  roco");.        
+0001d710: 6473 2e65 6e63 6f64 696e 670a 2020 2020  ds.encoding.    
+0001d720: 2020 2020 6473 2e74 656d 702e 656e 636f      ds.temp.enco
+0001d730: 6469 6e67 0a20 2020 2020 2020 2064 732e  ding.        ds.
+0001d740: 6c6f 6e2e 656e 636f 6469 6e67 0a0a 2020  lon.encoding..  
+0001d750: 2020 2222 220a 2020 2020 2320 4e61 6d65    """.    # Name
+0001d760: 2061 7320 6120 4346 5370 6563 7320 696e   as a CFSpecs in
+0001d770: 7374 616e 6365 0a20 2020 2069 6620 6e61  stance.    if na
+0001d780: 6d65 2069 7320 4e6f 6e65 3a0a 2020 2020  me is None:.    
+0001d790: 2020 2020 6366 7370 6563 7320 3d20 696e      cfspecs = in
+0001d7a0: 6665 725f 6366 5f73 7065 6373 2864 732c  fer_cf_specs(ds,
+0001d7b0: 206e 616d 6564 3d54 7275 6529 0a20 2020   named=True).   
+0001d7c0: 2020 2020 2069 6620 6366 7370 6563 732e       if cfspecs.
+0001d7d0: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
+0001d7e0: 2020 6e61 6d65 203d 2063 6673 7065 6373    name = cfspecs
+0001d7f0: 2e6e 616d 650a 2020 2020 2020 2020 656c  .name.        el
+0001d800: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001d810: 7265 7475 726e 2064 730a 2020 2020 656c  return ds.    el
+0001d820: 6966 2068 6173 6174 7472 286e 616d 652c  if hasattr(name,
+0001d830: 2022 636f 6f72 6473 2229 3a20 2023 2066   "coords"):  # f
+0001d840: 726f 6d20 6120 6461 7461 7365 742f 6461  rom a dataset/da
+0001d850: 7461 6172 7261 790a 2020 2020 2020 2020  taarray.        
+0001d860: 6e61 6d65 203d 2067 6574 5f63 665f 7370  name = get_cf_sp
+0001d870: 6563 735f 656e 636f 6469 6e67 2864 7329  ecs_encoding(ds)
+0001d880: 0a20 2020 2020 2020 2069 6620 6e61 6d65  .        if name
+0001d890: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0001d8a0: 2020 2020 2020 7265 7475 726e 2064 730a        return ds.
+0001d8b0: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+0001d8c0: 7461 6e63 6528 6e61 6d65 2c20 7374 7229  tance(name, str)
+0001d8d0: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+0001d8e0: 206e 616d 652e 6e61 6d65 3a0a 2020 2020   name.name:.    
+0001d8f0: 2020 2020 2020 2020 786f 615f 7761 726e          xoa_warn
+0001d900: 2822 4346 5370 6563 7320 696e 7374 616e  ("CFSpecs instan
+0001d910: 6365 2068 6173 206e 6f20 7265 6769 7374  ce has no regist
+0001d920: 7261 7469 6f6e 206e 616d 6522 290a 2020  ration name").  
+0001d930: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001d940: 2064 730a 2020 2020 2020 2020 6966 2072   ds.        if r
+0001d950: 6567 6973 7465 7220 616e 6420 6e6f 7420  egister and not 
+0001d960: 6973 5f72 6567 6973 7465 7265 645f 6366  is_registered_cf
+0001d970: 5f73 7065 6373 286e 616d 6529 3a0a 2020  _specs(name):.  
+0001d980: 2020 2020 2020 2020 2020 7265 6769 7374            regist
+0001d990: 6572 5f63 665f 7370 6563 7328 6e61 6d65  er_cf_specs(name
+0001d9a0: 290a 2020 2020 2020 2020 6e61 6d65 203d  ).        name =
+0001d9b0: 206e 616d 652e 6e61 6d65 0a0a 2020 2020   name.name..    
+0001d9c0: 2320 5365 7420 6173 2065 6e63 6f64 696e  # Set as encodin
+0001d9d0: 670a 2020 2020 7461 7267 6574 7320 3d20  g.    targets = 
+0001d9e0: 5b64 735d 202b 205b 6473 5b6e 616d 655d  [ds] + [ds[name]
+0001d9f0: 2066 6f72 206e 616d 6520 696e 205f 6c69   for name in _li
+0001da00: 7374 5f78 725f 6e61 6d65 735f 2864 732c  st_xr_names_(ds,
+0001da10: 2064 696d 733d 4661 6c73 6529 5d0a 2020   dims=False)].  
+0001da20: 2020 666f 7220 7461 7267 6574 2069 6e20    for target in 
+0001da30: 7461 7267 6574 733a 0a20 2020 2020 2020  targets:.       
+0001da40: 2074 6172 6765 742e 656e 636f 6469 6e67   target.encoding
+0001da50: 2e75 7064 6174 6528 6366 5f73 7065 6373  .update(cf_specs
+0001da60: 3d6e 616d 6529 0a20 2020 2072 6574 7572  =name).    retur
+0001da70: 6e20 6473 0a0a 0a64 6566 2069 6e66 6572  n ds...def infer
+0001da80: 5f63 6f6f 7264 7328 6473 293a 0a20 2020  _coords(ds):.   
+0001da90: 2022 2222 496e 6665 7220 7768 6963 6820   """Infer which 
+0001daa0: 6f66 2074 6865 2064 6174 6120 6172 7261  of the data arra
+0001dab0: 7973 206f 6620 6120 6461 7461 7365 7420  ys of a dataset 
+0001dac0: 6172 6520 636f 6f72 6469 6e61 7465 730a  are coordinates.
+0001dad0: 0a20 2020 2057 6865 6e20 636f 6f72 6469  .    When coordi
+0001dae0: 6e61 7465 7320 6172 6520 666f 756e 642c  nates are found,
+0001daf0: 2069 7420 6d61 6b65 7320 7375 7265 2074   it makes sure t
+0001db00: 6865 7920 6172 6520 7265 6769 7374 6572  hey are register
+0001db10: 6564 2069 6e20 7468 6520 6461 7461 7365  ed in the datase
+0001db20: 740a 2020 2020 6173 2063 6f6f 7264 696e  t.    as coordin
+0001db30: 6461 7465 732e 0a0a 2020 2020 5061 7261  dates...    Para
+0001db40: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+0001db50: 2d2d 2d2d 2d0a 2020 2020 6473 3a20 7861  -----.    ds: xa
+0001db60: 7272 6179 2e44 6174 6173 6574 0a0a 2020  rray.Dataset..  
+0001db70: 2020 5365 6520 616c 736f 0a20 2020 202d    See also.    -
+0001db80: 2d2d 2d2d 2d2d 2d0a 2020 2020 4346 5370  -------.    CFSp
+0001db90: 6563 732e 696e 6665 725f 636f 6f72 6473  ecs.infer_coords
+0001dba0: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
+0001dbb0: 7572 6e20 6765 745f 6366 5f73 7065 6373  urn get_cf_specs
+0001dbc0: 2864 7329 2e69 6e66 6572 5f63 6f6f 7264  (ds).infer_coord
+0001dbd0: 7328 6473 290a 0a0a 696e 6665 725f 636f  s(ds)...infer_co
+0001dbe0: 6f72 6473 2e5f 5f64 6f63 5f5f 203d 2043  ords.__doc__ = C
+0001dbf0: 4653 7065 6373 2e69 6e66 6572 5f63 6f6f  FSpecs.infer_coo
+0001dc00: 7264 732e 5f5f 646f 635f 5f0a            rds.__doc__.
```

### Comparing `xoa-0.6.1/xoa/cfgm.py` & `xoa-0.7.0/xoa/cfgm.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,37 +30,33 @@
 from argparse import ArgumentParser
 from argparse import HelpFormatter as ArgHelpFormatter
 from argparse import _HelpAction
 from collections import OrderedDict
 from warnings import warn
 import logging
 
-import validate
+try:
+    import configobj.validate as validate
+except ImportError:
+    import validate
 from configobj import ConfigObj, flatten_errors
-from validate import (
-    ValidateError,
-    Validator,
-    VdtTypeError,
-    VdtValueTooBigError,
-    VdtValueTooSmallError,
-)
 
 from .__init__ import XoaError, XoaWarning, xoa_warn
 
 try:
     import numpy
 except ImportError:
     numpy = None
 
 
 class VdtWarning(XoaWarning):
     pass
 
 
-class XoaValidateError(ValidateError, XoaError):
+class XoaValidateError(validate.ValidateError, XoaError):
     pass
 
 
 class VdtSizeError(XoaValidateError):
     """List size is incorrect (nmin, nmax, odd, even or shape)"""
 
     pass
@@ -130,49 +126,51 @@
         # Handle single value
         if not isinstance(value, (list, tuple)):
             value = [value]
 
         # Do list checks
         n = kwargs.pop("n", None)
         if n is not None and len(value) != int(n):
-            raise VdtSizeError("Incorrect size: {}, {} values expected".format(len(value), n))
+            raise validate.VdtSizeError(
+                "Incorrect size: {}, {} values expected".format(len(value), n)
+            )
         nmin = kwargs.pop("nmin", None)
         if nmin is not None and len(value) < int(nmin):
-            raise VdtSizeError(
+            raise validate.VdtSizeError(
                 "Incorrect size: {}, at least {} values expected".format(len(value), nmin)
             )
         nmax = kwargs.pop("nmax", None)
         if nmax is not None and len(value) > int(nmax):
-            raise VdtSizeError(
+            raise validate.VdtSizeError(
                 "Incorrect size: {}, at most {} values expected".format(len(value), nmax)
             )
         odd = validate.is_boolean(kwargs.pop("odd", False))
         if odd and not len(value) % 2:
-            raise VdtSizeError(
+            raise validate.VdtSizeError(
                 "Incorrect size: {}, odd number of values expected".format(len(value))
             )
         even = validate.is_boolean(kwargs.pop("even", False))
         if even and len(value) % 2:
-            raise VdtSizeError(
+            raise validate.VdtSizeError(
                 "Incorrect size: {}, even number of values expected".format(len(value))
             )
 
         shape = kwargs.pop("shape", None)
         if shape is not None:
             if numpy is None:
                 warn("Cannot check shape, numpy package is missing")
             else:
                 try:
                     shape, vshape = list(map(int, shape)), numpy.shape(value)
                     if vshape != shape:
-                        raise VdtSizeError(
+                        raise validate.VdtSizeError(
                             "Incorrect shape: {}, {} shape expected".format(vshape, shape)
                         )
                 except Exception:
-                    raise ValidateError(
+                    raise validate.ValidateError(
                         "Cannot test value shape, this may be caused by "
                         "an irregular array-like shape. Error was:\n{}".format(
                             traceback.format_exc()
                         )
                     )
 
         # Preserve tuple type
@@ -194,15 +192,15 @@
     if value == "":
         value = default
     c = []
     # two possible delimiters: whitespaces and ','
     for v in value.split():
         c.extend(v.split(","))
     if len(c) != 4:
-        raise VdtTypeError(value)
+        raise validate.VdtTypeError(value)
     return list(map(float, c))
 
 
 def is_numerics(value, default=None, min=None, max=None, type="float", n=None):
     """Validation function of a tuple of numeric values"""
     if isinstance(value, str):
         value = value.strip("()[] ")
@@ -210,37 +208,37 @@
         return None
     if isinstance(value, list):
         value = tuple(value)
     elif isinstance(value, str):
         try:
             value = eval(value)
         except Exception:
-            raise VdtTypeError(value)
+            raise validate.VdtTypeError(value)
     if not isinstance(value, tuple):
         try:
             value = tuple(value)
         except Exception:
             value = (value,)
     if n is not None:
         if isinstance(n, str):
             n = int(n)
         if len(value) != n:
-            raise VdtTypeError(value)
+            raise validate.VdtTypeError(value)
     out = ()
     type = eval(type)
     if min is not None and isinstance(min, str):
         min = type(min)
     if max is not None and isinstance(max, str):
         max = type(max)
     for val in value:
         if isinstance(val, str):
             try:
                 val = type(val)
             except Exception:
-                raise VdtTypeError(value)
+                raise validate.VdtTypeError(value)
         if min is not None and val < min:
             val = type(min)
         if max is not None and val > max:
             val = type(max)
         out += (val,)
     return out
 
@@ -264,34 +262,34 @@
     """Validation function of an interval of coordinates (min,max[,bounds])"""
     if isinstance(value, str):
         value = value.strip("()[] ")
     if str(value) == "None":
         return None
     if not isinstance(value, str):
         if not isinstance(value, list):
-            raise VdtTypeError(value)
+            raise validate.VdtTypeError(value)
         value = ",".join(value)
     if value.startswith("("):
         value = value[1:]
     if value.endswith(")"):
         value = value[:-1]
     values = value.split(",")
     if len(values) < 2 or len(values) > 3:
-        raise VdtTypeError(value)
+        raise validate.VdtTypeError(value)
     out = ()
     for val in values[:2]:
         try:
             val = eval(val)
         except Exception:
             pass
         out += (val,)
     if len(values) == 3 and values[2]:
         m = re.search("([co]{1,2}[ne]{0,2})", values[2])
         if m is None:
-            raise VdtTypeError(value)
+            raise validate.VdtTypeError(value)
         out += (m.group(1),)
     return out
 
 
 def is_cmap(value, default=None):
     """Validation function that return a :`xoa.color.CmapAdapter`"""
     if str(value) == "None":
@@ -303,15 +301,15 @@
     if isinstance(value, list):
         from .color import cmap_custom
 
         return cmap_custom(value)
     return CmapAdapter(value)
 
 
-class VdtDateTimeError(ValidateError):
+class VdtDateTimeError(validate.ValidateError):
     pass
 
 
 def is_path(value, default="", expand=None):
     """Parse a value as a path
 
     Parameters
@@ -348,33 +346,33 @@
 # def is_timeunits(value, default="days since 1950-01-01"):
 #     """Validation function of standard time units"""
 #     from .atime import are_valid_units
 #     value = str(value)
 #     if value == "None" or not value:
 #         value = default
 #     if not are_valid_units(value):
-#         raise VdtTypeError(value)
+#         raise validate.VdtTypeError(value)
 #     return value
 
 
 def is_cdtime(value, min=None, max=None, default=None):
     """Validation function of a date (compatible with :func:`cdtime.s2c`)"""
     import cdtime
 
     value = str(value).strip()
     if not value[0].isdigit():
         return value.upper()
     try:
         value = cdtime.s2c(value)
     except Exception:
-        raise VdtTypeError(value)
+        raise validate.VdtTypeError(value)
     if min is not None and val < cdtime.s2c(min):
-        raise VdtValueTooSmallError(value)
+        raise validate.VdtValueTooSmallError(value)
     if max is not None and val > cdtime.s2c(max):
-        raise VdtValueTooBigError(value)
+        raise validate.VdtValueTooBigError(value)
     return value
 
 
 def is_timestamp(value, default=None):
     """Validation function of date as parsable by :func:`pandas.Timestamp`"""
     if str(value) == "None":
         return
@@ -448,31 +446,31 @@
     if str(value) == "None":
         return
     if isinstance(value, str):
         try:
             return validate.bool_dict[value.lower()]
         except KeyError:
             return value
-    if value == False:
+    if value is False:
         return False
-    elif value == True:
+    elif value is True:
         return True
     else:
-        raise VdtTypeError(value)
+        raise validate.VdtTypeError(value)
 
 
 def is_eval(value, default=None, unchanged_if_failed=True):
     """Validate a string that can be evaluated"""
     try:
         value = eval(str(value))
     except Exception:
         if unchanged_if_failed:
             return value
         else:
-            raise VdtTypeError(value)
+            raise validate.VdtTypeError(value)
     return value
 
 
 def is_color(value, default="k", alpha=False, as256=None):
     """Validate a matplotlib compatible color"""
     if str(value) == "None":
         return None
@@ -486,17 +484,17 @@
     try:
         return cc(_check256_(value, as256=as256))
     except Exception:
         if isinstance(value, str):
             try:
                 return cc(_check256_(eval(value), as256=as256))
             except Exception:
-                raise VdtTypeError(value)
+                raise validate.VdtTypeError(value)
 
-    raise VdtTypeError(value)
+    raise validate.VdtTypeError(value)
 
 
 def _check256_(val, as256=None):
     if isinstance(val, str):
         return val
     if as256 is None:
         as256 = any([v > 1 for v in val[:3]])
@@ -533,34 +531,34 @@
     value = value.strip()
     if value == "":
         return {}
     m = _re_funccall(value) or _re_acc(value)
     if not m:
         m = _re_set(value)
         if not m:
-            raise VdtTypeError(value)
+            raise validate.VdtTypeError(value)
         value = "dict(" + value + ")"
     if m:
         try:
             value = eval(value)
         except Exception:
-            raise VdtTypeError(value)
+            raise validate.VdtTypeError(value)
         if not isinstance(value, dict):
-            raise VdtTypeError(value)
+            raise validate.VdtTypeError(value)
         else:
             return value
-    raise VdtTypeError(value)
+    raise validate.VdtTypeError(value)
 
 
 # Define additionnal specifications
 # Value should be dict for internal use of this module (iterable, opttype, ...)
 # If value is not a dict, it is supposed to be the validator function
 
 
-#: Available VACUMM :mod:`configobj` validator specifications
+#: Available :mod:`configobj` validator specifications
 VALIDATOR_SPECS = {
     # copy of some validate.Validator.functions to later build plural forms
     "integer": validate.is_integer,
     "float": validate.is_float,
     "boolean": validate.is_boolean,
     "string": validate.is_string,
     "option": validate.is_option,
@@ -589,24 +587,22 @@
     "boolstr": is_boolstr
     # lists validators for these scalars will be automatically generated
 }
 
 #: Available :mod:`validate.Validator` validator functions
 VALIDATOR_FUNCTIONS = {}
 
-#: Available VACUMM :mod:`configobj` validator type names
+#: Available :mod:`configobj` validator type names
 VALIDATOR_TYPES = []
 
 
 def _update_registry_():
-
     # 1. Fix specs dicts
     # 2. Generate list validators
     for k, v in list(VALIDATOR_SPECS.items()):
-
         # Check type of spec
         if not isinstance(v, dict):
             v = dict(func=v)
             # Update specs mapping
             VALIDATOR_SPECS[k] = v
 
         # Check minimum settings
@@ -786,15 +782,15 @@
             if not self._configspec and warn_empty_specs:
                 xoa_warn("Empty Config specifications after filtering")
         self._cfgfilter = cfgfilter
         self._cfgfilter_default = cfgfilter_default
         self._configspecfile = self._configspec.filename
 
         # Validator
-        if isinstance(validator, Validator):
+        if isinstance(validator, validate.Validator):
             self._validator = validator
         else:
             self._validator = get_validator(functions=validator)
 
         # Makes sure that booleans have a default value
         self._boolean_false = boolean_false
         if boolean_false:
@@ -977,23 +973,20 @@
         if self._cfgfilter and cfgfilter:
             if not isinstance(cfgfilter, dict):
                 cfgfilter = self._cfgfilter
             filter_section(cfg, cfgfilter, self._cfgfilter_default)
 
         # Validation
         if validate and self._configspec:
-
             # Validation itself
             err = cfg.validate(self._validator, preserve_errors=True)
 
             # Loop on errors
             if isinstance(err, dict):
-
                 for sections, key, error in flatten_errors(cfg, err):
-
                     # Format explicit message
                     if len(sections):
                         section = "[" + "][".join(sections) + "] "
                     else:
                         section = ""
                     msg = "Config value error: {}{}: {}".format(
                         section,
@@ -1252,15 +1245,14 @@
                 nested=nested,
                 boolean_false=self._boolean_false,
                 validator=self.validator,
             )
 
         # Now create a configuration instance from passed options
         if parse:
-
             # Which args ?
             if args is None:
                 args = sys.argv[1:]
 
             # Parse
             options = parser.parse_args(list(args))
 
@@ -1513,19 +1505,17 @@
     s_optsep = r"(?:, +)"  # option separator
     s_desc = r"(?:  (.+))"
     s_tot = rf"^  (?:  )?((?:{s_sopt}|{s_lopt})(?:{s_optsep}" rf"(?:{s_sopt}|{s_lopt}))*){s_desc}?$"
     re_opt = re.compile(s_tot).match
     re_sec = re.compile(r"^(?:  )?([\w\s]+):(?: (.+))?$").match
     secname = None
     for line in shelp.splitlines():
-
         # Sections
         m = re_sec(line)
         if m and not line.lower().endswith("ex:"):
-
             secname = m.group(1).title().strip()
 
             # Usage
             if secname == "Usage" and m.group(2) is not None:
                 usage = m.group(2).strip()
                 if prog is None:
                     prog = os.path.basename(usage.split()[0])
@@ -1543,39 +1533,35 @@
                     rhelp.extend(["", "\t" + m.group(2)])
                     multiline = True
             continue
 
         # Options and other lines
         m = re_opt(line)
         if m:
-
             rhelp.extend(["", "\t.. cmdoption:: " + m.group(1), ""])
             multiline = True
             if m.group(2) is not None:
                 rhelp.append("\t\t" + m.group(2).strip())
 
         elif secname and secname.lower() == "positional arguments" and line.startswith(" " * 2):
-
             sline = line.split()
             rhelp.extend(["", "\t.. cmdoption:: " + sline[0], ""])
             multiline = True
             if len(sline) > 1:
                 rhelp.append("\t\t" + " ".join(sline[1:]))
 
         elif multiline and len(line.strip()) and line.startswith(" " * 3):
-
             indent = "\t\t"
             if secname == "Usage":
                 indent += "\t"
             rhelp.append(indent + line.strip())
         # elif secname==descname:
         #    rhelp.append('\t'+line)
 
         else:
-
             indent = ""
             if secname and secname == descname:
                 indent += "\t"
             rhelp.append(indent + line)
             multiline = False
             if secname == "Usage":
                 secname = descname
@@ -1667,15 +1653,15 @@
     spec = VALIDATOR_SPECS.get(
         funcname, dict(func=None, iterable=None, opttype=None, argtype=None)
     ).copy()
     spec.update(dict(funcname=funcname, args=args, kwargs=kwargs, default=default, type=funcname))
     return _attdict_(spec)
 
 
-def get_validator(functions=None, cls=Validator, **kwargs):
+def get_validator(functions=None, cls=validate.Validator, **kwargs):
     """Get a default validator"""
 
     # Init
     validator = cls(**kwargs)
 
     # This modules's validator functions are already wrapped
     validator.functions.update(VALIDATOR_FUNCTIONS)
@@ -1726,15 +1712,14 @@
 
 def _walker_argcfg_setcfg_(sec, key, cfg=None, options=None, nested=None):
     """Walker to set config values"""
     # Find genealogy
     parents = _parent_list_(sec, names=False)
     cfgkey = "_".join([p.name.strip("_") for p in parents] + [key])
     for option, value in options._get_kwargs():
-
         # Option not set
         if value is None:
             continue
 
         # Option matches key?
         if _opt2cfgname_(option, nested) != cfgkey.lower():
             continue
@@ -1814,14 +1799,15 @@
 
         - inline: inline comment only,
         - above: above comments only,
         - merge: merge inline and above comments,
         - auto: if one is empty use the other one, else use inline
 
     """
+
     # filter
     def strip(c):
         return c.strip().strip("#").strip()
 
     abcoms = list(map(strip, [c for c in sec.comments[key] if c is not None]))
     incoms = list(map(strip, [c for c in [sec.inline_comments[key]] if c is not None]))
 
@@ -2041,40 +2027,35 @@
     optrole="cfgopt",
     secrole="cfgsec",
     mode="basic",
     validator=None,
     dir_fmt=".. {conftype}:: {name}\n\n{desc}\n",
     desc_fmt_desc_item="| {key}: {val}\n",
 ):
-
     assert mode in ("basic", "values", "specs")
 
     # Name, values and type
     secnames = get_sec_names(cfg)
     specs = OrderedDict()
     if key in cfg.sections:  # section
-
         secnames.append(key)
         name = "[{}]".format("][".join(secnames))
         conftype = secrole
 
     else:  # option
-
         if secnames:
             name = "[{}] {}".format("][".join(secnames), key)
         else:
             name = key
         conftype = optrole
 
         if mode == "values":
-
             specs["default"] = cfg[key]
 
         elif mode == "specs":
-
             spec = get_spec(cfg[key], validator=validator)
             specs["default"] = spec["default"]
             func = spec["base_func"]
             funcpath = f"{func.__module__}.{func.__name__}"
             funcname = spec['funcname']
             specs["type"] = f":func:`{funcname} <{funcpath}>`"
             if spec["args"]:
@@ -2115,15 +2096,14 @@
     text = _redent(text, cfg.depth)
     lines.append(text)
 
 
 def print_short_help(parser, formatter=None, compressed=False):
     """Print all help of a parser instance but those of groups"""
     if isinstance(parser, ArgumentParser):
-
         if formatter is None:
             formatter = parser._get_formatter()
 
         # usage
         if compressed is True:
             compressed = [
                 "-h",
@@ -2186,15 +2166,14 @@
 # %% Sphinx extension
 
 re_ws = re.compile(r'\s+')
 re_split_2secs = re.compile(r'\]\s*\[').split
 
 
 def gen_cfgm_rst(app):
-
     if not app.config.cfgm_rst_file:
         return
 
     logging.info("Generating rst declarations for the ConfigManager")
 
     rst = app.config.cfgm_get_cfgm_func().to_rst(secrole="cfgmsec", optrole="cfgmopt")
 
@@ -2205,15 +2184,14 @@
     with open(outfile, "w") as f:
         f.write(rst)
 
     logging.info("Created: " + app.config.cfgm_rst_file)
 
 
 def gen_cfgm_cfg(app):
-
     if not app.config.cfgm_cfg_file:
         return
 
     logging.info("Generating the default config from the ConfigManager")
     cfg = app.config.cfgm_get_cfgm_func().defaults
     outfile = os.path.abspath(app.config.cfgm_cfg_file)
     outdir = os.path.dirname(outfile)
@@ -2239,15 +2217,14 @@
             sigdec = "[" * nsec + secname + "]" * nsec
     signode.clear()
     signode += addnodes.desc_name(sig, sigdec)
     return re_ws.sub(' ', sig)
 
 
 def setup(app):
-
     app.add_object_type(
         'cfgmopt',
         'cfgmopt',
         objname='configuration option',
         indextemplate='pair: %s; configuration option',
         parse_node=parse_node,
     )
```

### Comparing `xoa-0.6.1/xoa/cli.py` & `xoa-0.7.0/xoa/cli.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/color.py` & `xoa-0.7.0/xoa/color.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/coords.py` & `xoa-0.7.0/xoa/coords.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     """
     return xcf.get_cf_specs(da).search(da, 'lon', errors=errors)
 
 
 def is_lon(da, loc="any"):
     """Tell if a data array is identified as longitudes
 
-    Parameters    is_vertical
-
+    Parameters
+    ----------
     da: xarray.DataArray
 
     Return
     ------
     bool
 
     See also
@@ -405,41 +405,44 @@
     xoa.cf.CFSpecs.search_coord
     """
     cfspecs = xcf.get_cf_specs(da)
     return [cfspecs.search_coord(da, coord_name, errors=errors) for coord_name in coord_names]
 
 
 @misc.ERRORS.format_function_docstring
-def get_cf_dims(da, cf_args, allow_positional=False, positions='tzyx', errors="warn"):
+def get_cf_dims(da, cf_args, allow_positional=False, positions='tzyx', errors="warn", **kwargs):
     """Get the data array dimensions names from their type
 
     Parameters
     ----------
     da: xarray.DataArray
         Array to scan
     cf_args: str, list
         Letters among "x", "y", "z", "t" and "f",
         or generic CF names.
     allow_positional: bool
         Fall back to positional dimension of types if unkown.
     positions: str
         Default position per type starting from the end.
     {errors}
+    kwargs: dict
+        Extra parameters are passed to :meth:`xoa.cf.CFSpecs.get_dims` in addition to
+        the above parameters.
 
     Return
     ------
-    tuple
+    tuple(list) or list
         Tuple of dimension name or None when the dimension if not found
 
     See also
     --------
     xoa.cf.CFSpecs.get_dims
     """
     return xcf.get_cf_specs(da).get_dims(
-        da, cf_args, allow_positional=allow_positional, positions=positions, errors=errors
+        da, cf_args, allow_positional=allow_positional, positions=positions, errors=errors, **kwargs
     )
 
 
 @misc.ERRORS.format_function_docstring
 def get_xdim(da, errors="warn", **kwargs):
     """Get the dimension of X type
 
@@ -449,28 +452,26 @@
     ----------
     da: xarray.DataArray
         Array to scan
     positions: str
         Default position per type starting from the end.
     {errors}
     kwargs: dict
-        Extra parameters are passed to :func:`get_dims`
+        Extra parameters are passed to :func:`get_cf_dims`
 
     Return
     ------
     str or None
         The dimension name or None
 
     See also
     --------
     get_dims
     """
-    dims = get_cf_dims(da, "x", errors=errors)
-    if dims:
-        return dims[0]
+    return get_cf_dims(da, "x", errors=errors, **kwargs)
 
 
 @misc.ERRORS.format_function_docstring
 def get_ydim(da, errors="warn", **kwargs):
     """Get the dimension of Y type
 
     It is a simple call to :func:`get_dims` with ``dim_types="y"``
@@ -479,28 +480,26 @@
     ----------
     da: xarray.DataArray
         Array to scan
     positions: str
         Default position per type starting from the end.
     {errors}
     kwargs: dict
-        Extra parameters are passed to :func:`get_dims`
+        Extra parameters are passed to :func:`get_cf_dims`
 
     Return
     ------
     str or None
         The dimension name or None
 
     See also
     --------
     get_dims
     """
-    dims = get_cf_dims(da, "y", errors=errors)
-    if dims:
-        return dims[0]
+    return get_cf_dims(da, "y", errors=errors, **kwargs)
 
 
 @misc.ERRORS.format_function_docstring
 def get_zdim(da, errors="warn", **kwargs):
     """Get the dimension of Z type
 
     It is a simple call to :func:`get_dims` with ``dim_types="z"``
@@ -509,28 +508,26 @@
     ----------
     da: xarray.DataArray
         Array to scan
     positions: str
         Default position per type starting from the end.
     {errors}
     kwargs: dict
-        Extra parameters are passed to :func:`get_dims`
+        Extra parameters are passed to :func:`get_cf_dims`
 
     Return
     ------
     str or None
         The dimension name or None
 
     See also
     --------
-    get_dims
+    get_cf_dims
     """
-    dims = get_cf_dims(da, "z", errors=errors)
-    if dims:
-        return dims[0]
+    return get_cf_dims(da, "z", errors=errors, **kwargs)
 
 
 @misc.ERRORS.format_function_docstring
 def get_tdim(da, errors="warn", **kwargs):
     """Get the dimension of T type
 
     It is a simple call to :func:`get_dims` with ``dim_types="t"``
@@ -539,28 +536,26 @@
     ----------
     da: xarray.DataArray
         Array to scan
     positions: str
         Default position per type starting from the end.
     {errors}
     kwargs: dict
-        Extra parameters are passed to :func:`get_dims`
+        Extra parameters are passed to :func:`get_cf_dims`
 
     Return
     ------
     str or None
         The dimension name or None
 
     See also
     --------
-    get_dims
+    get_cf_dims
     """
-    dims = get_cf_dims(da, "t", errors=errors)
-    if dims:
-        return dims[0]
+    return get_cf_dims(da, "t", errors=errors, **kwargs)
 
 
 @misc.ERRORS.format_function_docstring
 def get_fdim(da, errors="warn", **kwargs):
     """Get the dimension of F type
 
     It is a simple call to :func:`get_dims` with ``dim_types="f"``
@@ -569,28 +564,26 @@
     ----------
     da: xarray.DataArray
         Array to scan
     positions: str
         Default position per type starting from the end.
     {errors}
     kwargs: dict
-        Extra parameters are passed to :func:`get_dims`
+        Extra parameters are passed to :func:`get_cf_dims`
 
     Return
     ------
     str or None
         The dimension name or None
 
     See also
     --------
-    get_dims
+    get_cf_dims
     """
-    dims = get_cf_dims(da, "f", errors=errors)
-    if dims:
-        return dims[0]
+    return get_cf_dims(da, "f", errors=errors, **kwargs)
 
 
 class transpose_modes(misc.IntEnumChoices, metaclass=misc.DefaultEnumMeta):
     """Supported :func:`transpose` modes"""
 
     #: Basic xarray transpose with :meth:`xarray.DataArray.transpose`
     classic = 0
@@ -875,15 +868,15 @@
         targets = list(da.coords.values())
         if isinstance(da, xr.Dataset):
             targets.extend(da.data_vars.values())
 
     # Loop on targets
     for target in targets:
         if "positive" in target.attrs:
-            positive = da.coords[zdim].attrs["positive"]
+            positive = target.attrs["positive"]
             return positive_attr[positive].name
 
     # Fall back to current CFSpecs
     cfspecs = xcf.get_cf_specs(da)
     return cfspecs["vertical"]["positive"]
```

### Comparing `xoa-0.6.1/xoa/dyn.py` & `xoa-0.7.0/xoa/dyn.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/filter.py` & `xoa-0.7.0/xoa/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import inspect
 import numpy as np
 import xarray as xr
 import numba
 
 from .__init__ import XoaError, xoa_warn
 from . import misc as xmisc
 from . import coords as xcoords
@@ -95,29 +96,29 @@
     15,
     8,
     3,
     1,
 ]
 
 
-def get_window_func(window, *args, **kwargs):
+def get_window_func(window, **kwargs):
     """Get a window function from its name
 
     Parameters
     ----------
     window: str, callable, list, array_like
         Specification to get the window function:
 
         - `callable`: used as is.
         - `str`: supposed to be function name of the :mod:`numpy` or
           :mod:`scipy.signal.windows` modules.
         - `list`, `array_like`: transformed to an array and interpolated
           onto ``size`` points.
 
-    args, kwargs:
+    kwargs:
         Argument passed to the low level window function at calling time.
 
     Return
     ------
     callable
         A function that only a ``size`` argument
 
@@ -125,20 +126,29 @@
     -------
     .. ipython:: python
 
         @suppress
         import matplotlib.pyplot as plt
         @suppress
         from xoa.filter import get_window_func
-        func0 = get_window_func("gaussian", 22, sym=True)
+        func0 = get_window_func("gaussian", std=22, sym=True)
         func1 = get_window_func([1, 2, 5, 2, 1])
         plt.plot(func0(100), label='Gaussian');
         plt.plot(func1(100), label='List/array');
         @savefig api.filter.get_window_func.png
         plt.legend();
+
+    See also
+    --------
+    scipy.signal.windows
+    numpy.bartlett
+    numpy.blackman
+    numpy.hamming
+    numpy.hanning
+    numpy.kaiser
     """
     # Explicit values so create a wrapper that interpolate them
     if isinstance(window, (list, np.ndarray)):
 
         def window_func(size):
             x = np.linspace(0, 1, size)
             xp = np.linspace(0, 1, len(window))
@@ -152,65 +162,38 @@
             func = getattr(np, window)
         else:
             import scipy.signal.windows as sw
 
             func = getattr(sw, window, None)
             if func is None:
                 raise XoaError(f'Invalid window name: {window}')
+
     else:
         func = window
 
     # Wrapper with args
-    if args or kwargs:
+    params = inspect.signature(func).parameters
+    if kwargs or "sym" in params or "std" in params or "p" in params or "sig" in params:
+        kwargs = kwargs.copy()
 
         def window_func(size):
-            return func(size, *args, **kwargs)
+            if "sym" in params and "sym" not in kwargs:
+                kwargs["sym"] = True
+            if "std" in params:
+                kwargs["std"] = size * kwargs.get("std", 1 / 6)
+            if "sig" in params:
+                kwargs["sig"] = size * kwargs.get("sig", 1 / 6)
+            if "p" in params and "p" not in kwargs:
+                kwargs["p"] = 1
+            return func(size, **kwargs)
 
         return window_func
     return func
 
 
-# def get_window_kernel(size, window, *args, **kwargs):
-#     """Generate an 1d kernel from a window name or function
-
-#     It first get the window function, then returns::
-
-#         window_func(size)
-
-#     Parameters
-#     ----------
-#     size: int
-#         Size of the output kernel
-#     window: str, callable, list, array_like
-#         Specification to get the window function:
-
-#         - `callable`: used as is.
-#         - `str`: supposed to be function name of the :mod:`numpy` or
-#           :mod:`scipy.signal.windows` modules.
-#         - `list`, `array_like`: transformed to an array and interpolated
-#           onto ``size`` points.
-
-#     Return
-#     ------
-#     np.ndarray
-#         1D kernel
-
-#     See also
-#     --------
-#     get_window_func
-#     """
-#     if isinstance(window, str):
-#         window = get_window_func(window, *args, **kwargs)
-#     elif isinstance(window, (list, np.ndarray)):
-#         x = np.linspace(0, 1, size)
-#         xp = np.linspace(0, 1, len(window))
-#         return np.interp(x, xp, window)
-#     return window(size)
-
-
 def generate_isotropic_kernel(shape, window_func, fill_value=0, npt=None):
     """Generate an nD istropic kernel given a shape and a window function
 
     Parameters
     ----------
     shape: int, tuple
         Shape of the desired kernel
@@ -242,14 +225,15 @@
         @savefig api.filter.generate_isotropic_kernel.png
         plt.colorbar();
 
     See also
     --------
     generate_orthogonal_kernel
     generate_kernel
+    scipy.signal.windows
     numpy.bartlett
     numpy.blackman
     numpy.hamming
     numpy.hanning
     numpy.kaiser
     numpy.interp
 
@@ -260,15 +244,15 @@
     # Normalised indices
     indices = np.indices(shape).astype('d')
     for i, width in enumerate(shape):
         indices[i] /= width - 1
         indices[i] -= 0.5
 
     # Distance from bounds with 0.5 at center and < 0 outside bounds
-    x = 0.5 - np.sqrt((indices ** 2).sum(axis=0))
+    x = 0.5 - np.sqrt((indices**2).sum(axis=0))
 
     # Window values
     if npt is None:
         npt = 2 * max(shape)
     fp = window_func(npt)
     xp = np.linspace(0, 1, npt)
 
@@ -334,25 +318,25 @@
 
 
 
     See also
     --------
     generate_isotropic_kernel
     generate_kernel
+    scipy.signal.windows
     numpy.bartlett
     numpy.blackman
     numpy.hamming
     numpy.hanning
     numpy.kaiser
     numpy.interp
 
     """
     kernel = None
     for k1d in kernels:
-
         # From scalar to 1d
         if np.isscalar(k1d):
             window_func = get_window_func(window_func)
             if isinstance(k1d, int):
                 k1d = window_func(k1d)
             else:  # Float case
                 size = int(k1d)
@@ -369,21 +353,15 @@
         else:
             kernel = np.tensordot(kernel[:, None], k1d[None], axes=1)
 
     return kernel
 
 
 def generate_kernel(
-    kernel,
-    data,
-    isotropic=False,
-    window_func="ones",
-    fill_value=0.0,
-    window_args=None,
-    window_kwargs=None,
+    kernel, data, window_func="ones", isotropic=False, fill_value=0.0, window_kwargs=None, **kwargs
 ):
     """Generate a kernel that is compatible with a given data array
 
     Parameters
     ----------
     kernel: xarray.DataArray, np.ndarray, int, list, dictorthokernels
         Ready to use kernel or specs to generate it.
@@ -398,24 +376,40 @@
         :func:`xoa.coords.transpose` to fit into the input data array.
     data: xarray.DataArray
         Data array that the kernel must be compatible with.
         If the kernel has more than one dimension, it is expanded with a size of 1
         for missing dimensions.
     isotropic: bool, tuple
         Tuple of the dimensions over which must be computed isotropically.
+    fill_value: float
+        Value used by :func:`generate_isotropic_kernel` to fill the isotropic kernel
+        in its corners.
+    window_func: str
+        Function to generate the kernel from its size by calling :func:`get_window_func`
+    window_kwargs: dict
+        Optional arguments passed to :func:`get_window_func`
+    kwargs: dict
+        Extra parameters are merged with `window_kwargs`
 
     Return
     ------
     xarray.DataArray
         Kernel array with suitable dimensions and shape
 
     See also
     --------
     generate_isotropic_kernel
     generate_orthogonal_kernel
+    get_window_func
+    scipy.signal.windows
+    numpy.bartlett
+    numpy.blackman
+    numpy.hamming
+    numpy.hanning
+    numpy.kaiser
     xoa.coords.transpose
     """
     # Isotropic
     if isotropic is True:
         isotropic = data.dims
 
     # Convert to tuple
@@ -432,15 +426,14 @@
 
     # Convert list to dict with dims
     elif isinstance(kernel, list):
         kernel = dict((dim, kernel) for dim in data.dims)
 
     # From an size or 1d kernel for given dimensions
     if isinstance(kernel, dict):
-
         # Isotropic parameter
         if isotropic:
             if isotropic is True:
                 isotropic = data.dims
             elif not set(isotropic).issubset(data.dims):
                 raise XoaError("invalid dimensions for isotropic keyword")
 
@@ -471,30 +464,30 @@
                     isokernel = kn
                 size = kn if np.isscalar(kn) else len(kn)
                 isokernels_sizes[dim] = size
 
         # Merge orthogonal kernels
         dims = ()
         kernel = None
+        window_kwargs = {} if window_kwargs is None else window_kwargs
+        if kwargs:
+            window_kwargs.update(kwargs)
         if orthokernels:
             dims += tuple(orthokernels.keys())
-            window_args = [] if window_args is None else window_args
-            window_kwargs = {} if window_kwargs is None else window_kwargs
-            window_func = get_window_func(window_func, *window_args, **window_kwargs)
+            window_func = get_window_func(window_func, **window_kwargs)
             sizes = tuple(orthokernels.values())
             kernel = generate_orthogonal_kernel(
                 sizes, window_func=window_func, fill_value=fill_value
             )
 
         # Build isotropic kernel
         if isokernel:
-
             # List/array
             if not np.isscalar(isokernel):
-                window_func = get_window_func(isokernel)
+                window_func = get_window_func(isokernel, **window_kwargs)
 
             # nD isotropic kernel
             isokernels = generate_isotropic_kernel(
                 tuple(isokernels_sizes.values()), window_func, fill_value=fill_value
             )
 
             # Update final kernel
@@ -595,15 +588,15 @@
     bad = weights <= kernel.sum() * np.clip(1e-6, 1 - na_thres, 1 - 1e-6)
     if normalize:
         weights = np.where(bad, 1, weights)
         cdata /= weights
     return np.where(bad, np.nan, cdata)
 
 
-def convolve(data, kernel, normalize=False, na_thres=0):
+def convolve(data, kernel, normalize=False, na_thres=0, kernel_kwargs=None, **kwargs):
     """N-dimensional convolution that takes care of nans
 
     Parameters
     ----------
     data: xarray.DataArray
         Array to filter
     kernel: int, tuple, numpy.ndarray, xarray.DataArray
@@ -614,14 +607,18 @@
     na_thres: float
         A float between 0 and 1 that defines the allowed level a NaN contamination.
         Examples of the behavioir at a single location:
 
             - `0`: Output is masked if a single NaN is found.
             - `0.5`: Output is masked only more than 50% of the input data are masked.
             - `1`: Output is masked if all input data are masked.
+    kernel_kwargs: dict, None
+        Extra parameters passed to :func:`generate_kernel`.
+    kwargs: dict
+        Extra parameters are merged with `kernel_kwargs`
 
     Return
     ------
     xarray.DataArray
         The filtered array with the same shape, attributes and coordinates
         as the input array.
 
@@ -630,15 +627,14 @@
     scipy.signal.convolve
     generate_kernel
 
     Example
     -------
     .. ipython:: python
 
-        @savefig api.filter.convolve.png
         @suppress
         import xarray as xr, numpy as np, matplotlib.pyplot as plt
         @suppress
         from xoa.filter import convolve
         data = xr.DataArray(np.random.normal(size=(50, 70)), dims=('y', 'x'))
         data[10:20, 10:20] = np.nan # introduce missing data
         kernel = dict(x=[1, 2, 5, 2, 1], y=[1, 2, 1])
@@ -647,22 +643,25 @@
         kw = dict(vmin=data.min(), vmax=data.max())
         data.plot.pcolormesh(ax=ax0, **kw);
         @savefig api.filter.convolve.png
         datac.plot.pcolormesh(ax=ax1, **kw);
 
     """
     # Adapt the kernel to the data
-    kernel = generate_kernel(kernel, data)
+    kernel_kwargs = kernel_kwargs if kernel_kwargs is not None else {}
+    if kwargs:
+        kernel_kwargs.update(kwargs)
+    kernel = generate_kernel(kernel, data, **kernel_kwargs)
 
     # Numpy convolution
     axis = data.get_axis_num(kernel.dims[0]) if kernel.ndim == 1 else None
     datac = _convolve_(data.data, kernel.data, normalize, na_thres, axis)
 
     # Format
-    return xr.DataArray(datac, coords=data.coords, attrs=data.attrs)
+    return xr.DataArray(datac, coords=data.coords, attrs=data.attrs, dims=data.dims)
 
 
 def _get_xydims_(data, xdim, ydim):
     if xdim is None:
         xdim = xcoords.get_xdims(data, 'x', allow_positional=False, errors="raise")
     else:
         assert xdim in data.dims, f"Invalid x dimension: {xdim}"
@@ -680,14 +679,34 @@
     return rmask
 
 
 def _convolve_and_fill_(data, kernel):
     return data.fillna(convolve(data, kernel, normalize=True, na_thres=1))
 
 
+def smooth(data, kernel, **kwargs):
+    """A short to ``convolve(data, kernel, normalize=True)``
+
+    See :func:`convolve` for the complete list of options.
+
+    Parameters
+    ----------
+    data: xarray.DataArray
+        Array to filter
+    kernel: int, tuple, numpy.ndarray, xarray.DataArray
+        Convolution kernel. See :func:`generate_kernel`.
+
+    See also
+    --------
+    convolve
+    """
+    kwargs["normalize"] = True
+    return convolve(data, kernel, **kwargs)
+
+
 def erode_mask(data, until=1, kernel=None):
     """Erode the horizontal mask using smoothing
 
     Missing values are filled with the smoothed field in a iterative way.
     Two cases:
 
         - Erode a fixed number of times.
```

### Comparing `xoa-0.6.1/xoa/geo.py` & `xoa-0.7.0/xoa/geo.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,15 +310,15 @@
     def __exit__(self, type, value, traceback):
         if self.switch_cdist:
             setattr(self.distmod, "cdist", self._old_cdist)
         if self.switch_pdist:
             setattr(self.distmod, "pdist", self._old_pdist)
 
 
-def get_extent(extent, margin=0, square=False):
+def get_extent(extent, margin=0, square=False, min_extent=None):
     """Compute the geographic extent in degrees
 
     Parameters
     ----------
     extent: xarray.DataArray, xarray.Dataset, dict, tuple, list
         Either:
 
@@ -327,14 +327,17 @@
         - A two-element tuple of longitudes and latitudes: ``(lon, lat)``
         - A extent list: ``[xmin, xmax, ymin, ymax]``.
     margin: float
         A relative fraction of the width and height that is used to set margins.
         For instance, a value of ``-0.1`` shrinks the box of 10% on each side.
     square: bool
         Force the box to be square in degrees.
+    min_extent: None, float, (float, float)
+        Minimal extent along x and y: ``(dx, dy)``.
+        If a single floating value is provided, it is valid for both x and y.
 
     Return
     ------
     list
         ``[xmin, xmax, ymin, ymax]``
 
     Example
@@ -364,20 +367,26 @@
         lon, lat = extent
         xmin = float(np.min(lon))
         xmax = float(np.max(lon))
         ymin = float(np.min(lat))
         ymax = float(np.max(lat))
 
     # Scale
-    if square or margin:
+    if square or margin or min_extent is not None:
         dx = xmax - xmin
         dy = ymax - ymin
         x0 = 0.5 * (xmin + xmax)
         y0 = 0.5 * (ymin + ymax)
-        if square:
+        if min_extent is not None:
+            if isinstance(min_extent, (float, int)):
+                min_extent = (min_extent, min_extent)
+            dx_min, dy_min = min_extent
+            dx = max(dx, dx_min)
+            dy = max(dy, dy_min)
+        if square and dy != 0:
             aspect = dx * math.cos(y0 * math.pi / 180) / dy
             if aspect > 1:
                 dy *= aspect
             else:
                 dx /= aspect
         xmargin = margin * dx
         ymargin = margin * dy
```

### Comparing `xoa-0.6.1/xoa/grid.py` & `xoa-0.7.0/xoa/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -531,18 +531,17 @@
     errors = misc.ERRORS[errors]
 
     # Find needed stuff
     cfspecs = cf.get_cf_specs(ds)
     dz = cfspecs.search(ds, 'dz', errors=errors)
     if dz is None:
         return ds
-    zdims = xcoords.get_cf_dims(dz, "z", errors=errors)
-    if zdims is None:
+    zdim = xcoords.get_cf_dims(dz, "z", errors=errors)
+    if zdim is None:
         return ds
-    zdim = zdims[0]
     positive = cfspecs["vertical"]["positive"]
     if positive is None:
         positive = xcoords.get_positive_attr(ds, zdim)
     if positive is None:
         msg = "Can't infer positive attribute from data dataset"
         if errors == "raise":
             raise XoaError(msg)
@@ -562,31 +561,38 @@
     # Compute depth
     depth = dz2depth(dz, positive=positive, zdim=zdim, ref=ref, ref_type=ref_type, centered=True)
 
     # Assign to dataset
     return ds.assign_coords(depth=depth)
 
 
-def to_rect(da, tol=1e-5):
-    """Convert a curvilinear coordinate array to a rectangular 1d coordinate array
+@misc.ERRORS.format_function_docstring
+def to_rect(da, tol=1e-5, errors="warn"):
+    """Convert the curvilinear coordinates of array/dataset to rectangular axis coordinates
 
-    It checks if the coordinates may be converted to 1D without loss of information.
+    It checks if the coordinates may be converted to 1D  axis without loss of information.
 
     Parameters
     ----------
     da: xarray.DataArray, xarray.Dataset
         In case of a dataset, it must contain longitudes and latitudes.
+    to: float
+        Absolute tolerance of the variability of a coordinate along its constant dimension
+        to consider it as a 1D axis coordinate.
+    {errors}
 
     Return
     ------
     xarray.DataArray, xarray.Dataset
     """
     da = da.copy()
     new_coords = {}
     rename_args = {}
+    da = cf.infer_coords(da)
+    errors = misc.ERRORS[errors]
     for name, coord in da.coords.items():
         if coord.ndim != 2:
             continue
         if xcoords.is_lon(coord):
             odim = xcoords.get_ydim(coord, errors="ignore")
         elif xcoords.is_lat(coord):
             odim = xcoords.get_xdim(coord, errors="ignore")
@@ -598,14 +604,22 @@
                 new_coords[name] = xr.DataArray(
                     coord.isel({odim: 0}).values, dims=name, attrs=coord.attrs
                 )
                 new_coords[name].encoding.update(coord.encoding)
                 dim = coord.dims[0] if coord.dims[1] == odim else coord.dims[1]
                 rename_args[dim] = name
                 break
+        else:
+            msg = (
+                "Cannot convert to curvilinear to rectangular grid since since coordinate "
+                f"'{name}' is not constant along one of its dimensions"
+            )
+            if errors == "errors":
+                raise XoaError(msg)
+            xoa_warn(msg)
     if new_coords:
         return (
             da.reset_coords(list(new_coords), drop=True)
             .rename(rename_args)
             .assign_coords(new_coords)
         )
     return da
```

### Comparing `xoa-0.6.1/xoa/interp.py` & `xoa-0.7.0/xoa/interp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Low level interpolation routines accelerated with numba
 
 The numerical inputs and outputs of all these routines are of scalar
 or numpy.ndarray type.
 """
-# Copyright 2020-2021 Shom
+# Copyright 2020-2022 Shom
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,87 +19,62 @@
 # limitations under the License.
 import os
 import math
 
 import numpy as np
 import numba
 
+from .num import ravel_index, unravel_index, get_iminmax
 from .geo import _haversine_
 
 NOT_CI = os.environ.get("CI", "false") == "false"
 
 
 # %% 1D routines
 
 
-@numba.njit(cache=NOT_CI)
-def get_iminmax(data1d):
-    """The first and last non nan values for a 1d array
-
-    Parameters
-    ----------
-    data1d: array_like(n)
-
-    Return
-    ------
-    int
-        Index of the first valid value
-    int
-        Index of the last valid value
-    """
-    imin = -1
-    imax = -1
-    n = len(data1d)
-    for i in range(n):
-        if imin < 0 and not np.isnan(data1d[i]):
-            imin = i
-        if imax < 0 and not np.isnan(data1d[n - 1 - i]):
-            imax = n - 1 - i
-        if imax > 0 and imin > 0:
-            break
-    return imin, imax
-
-
 @numba.njit(parallel=False, cache=NOT_CI)
-def nearest1d(vari, yi, yo, extrap="no"):
+def nearest1d(vari, yi, yo, eshapes, extrap="no"):
     """Nearest interpolation of nD data along an axis with varying coordinates
 
     Warning
     -------
     `nxi` must be either a multiple or a divisor of `nxo`,
     and multiple of `nxiy`.
 
     Parameters
     ----------
     vari: array_like(nxi, nyi)
     yi: array_like(nxiy, nyi)
     yo: array_like(nxo, nyo)
+    eshapes: array_like(3, ndim-1)
 
     Return
     ------
     array_like(nx, nyo): varo
         With `nx=max(nxi, nxo)`
     """
     # Shapes
-    nxi, nyi = vari.shape
-    nxiy = yi.shape[0]
-    nxi, nyi = vari.shape
-    nxo, nyo = yo.shape
-    nx = max(nxi, nxo)
+    nyo = yo.shape[1]
+    eshape = np.empty(eshapes.shape[1], eshapes.dtype)
+    for i in range(eshape.size):
+        eshape[i] = eshapes[:, i].max()
+    nx = np.prod(eshape)
 
     # Init output
     varo = np.full((nx, nyo), np.nan, dtype=vari.dtype)
 
     # Loop on the varying dimension
     for ix in numba.prange(nx):
 
-        # Index along x for coordinate arrays
-        ixi = min(nxi - 1, ix % nxi)
-        ixiy = min(nxiy - 1, ix % nxiy)
-        ixoy = min(nxo - 1, ix % nxo)
+        # Index along x for all arrays
+        ii = unravel_index(ix, eshape)
+        ixi = ravel_index(np.minimum(ii, eshapes[0] - 1), eshapes[0])
+        ixiy = ravel_index(np.minimum(ii, eshapes[1] - 1), eshapes[1])
+        ixoy = ravel_index(np.minimum(ii, eshapes[2] - 1), eshapes[2])
 
         # Loop on input grid
         iyimin, iyimax = get_iminmax(yi[ixiy])
         iyomin, iyomax = get_iminmax(yo[ixoy])
         for iyi in range(iyimin, iyimax):
 
             # Out of bounds
@@ -132,50 +107,52 @@
     if extrap != "no":
         varo = extrap1d(varo, extrap)
 
     return varo
 
 
 @numba.njit(parallel=False, cache=NOT_CI)
-def linear1d(vari, yi, yo, extrap="no"):
+def linear1d(vari, yi, yo, eshapes, extrap="no"):
     """Linear interpolation of nD data along an axis with varying coordinates
 
     Warning
     -------
     `nxi` must be either a multiple or a divisor of `nxo`,
     and multiple of `nxiy`.
 
     Parameters
     ----------
     vari: array_like(nxi, nyi)
     yi: array_like(nxiy, nyi)
     yo: array_like(nxo, nyo)
+    eshapes: array_like(3, ndim-1)
 
     Return
     ------
     array_like(nx, nyo): varo
         With `nx=max(nxi, nxo)`
     """
     # Shapes
-    nxi, nyi = vari.shape
-    nxiy = yi.shape[0]
-    nxi, nyi = vari.shape
-    nxo, nyo = yo.shape
-    nx = max(nxi, nxo)
+    nyo = yo.shape[1]
+    eshape = np.empty(eshapes.shape[1], eshapes.dtype)
+    for i in range(eshape.size):
+        eshape[i] = eshapes[:, i].max()
+    nx = np.prod(eshape)
 
     # Init output
     varo = np.full((nx, nyo), np.nan, dtype=vari.dtype)
 
     # Loop on the varying dimension
     for ix in numba.prange(nx):
 
-        # Index along x for coordinate arrays
-        ixi = min(nxi - 1, ix % nxi)
-        ixiy = min(nxiy - 1, ix % nxiy)
-        ixoy = min(nxo - 1, ix % nxo)
+        # Index along x for all arrays
+        ii = unravel_index(ix, eshape)
+        ixi = ravel_index(np.minimum(ii, eshapes[0] - 1), eshapes[0])
+        ixiy = ravel_index(np.minimum(ii, eshapes[1] - 1), eshapes[1])
+        ixoy = ravel_index(np.minimum(ii, eshapes[2] - 1), eshapes[2])
 
         # Loop on input grid
         iyimin, iyimax = get_iminmax(yi[ixiy])
         iyomin, iyomax = get_iminmax(yo[ixoy])
         for iyi in range(iyimin, iyimax):
 
             # Out of bounds
@@ -207,196 +184,208 @@
     if extrap != "no":
         varo = extrap1d(varo, extrap)
 
     return varo
 
 
 @numba.njit(parallel=False, cache=NOT_CI)
-def cubic1d(vari, yi, yo, extrap="no"):
+def cubic1d(vari, yi, yo, eshapes, extrap="no"):
     """Cubic interpolation of nD data along an axis with varying coordinates
 
     Warning
     -------
     `nxi` must be either a multiple or a divisor of `nxo`,
     and multiple of `nxiy`.
 
     Parameters
     ----------
     vari: array_like(nxi, nyi)
     yi: array_like(nxiy, nyi)
     yo: array_like(nxo, nyo)
+    eshapes: array_like(3, ndim-1)
 
     Return
     ------
     array_like(nx, nyo): varo
         With `nx=max(nxi, nxo)`
     """
     # Shapes
-    nxi, nyi = vari.shape
-    nxiy = yi.shape[0]
-    nxi, nyi = vari.shape
-    nxo, nyo = yo.shape
-    nx = max(nxi, nxo)
+    nyo = yo.shape[1]
+    eshape = np.empty(eshapes.shape[1], eshapes.dtype)
+    for i in range(eshape.size):
+        eshape[i] = eshapes[:, i].max()
+    nx = np.prod(eshape)
 
     # Init output
     varo = np.full((nx, nyo), np.nan, dtype=vari.dtype)
 
     # Loop on the varying dimension
     for ix in numba.prange(nx):
 
-        # Index along x for coordinate arrays
-        ixi = min(nxi - 1, ix % nxi)
-        ixiy = min(nxiy - 1, ix % nxiy)
-        ixoy = min(nxo - 1, ix % nxo)
+        # Index along x for all arrays
+        ii = unravel_index(ix, eshape)
+        ixi = ravel_index(np.minimum(ii, eshapes[0] - 1), eshapes[0])
+        ixiy = ravel_index(np.minimum(ii, eshapes[1] - 1), eshapes[1])
+        ixoy = ravel_index(np.minimum(ii, eshapes[2] - 1), eshapes[2])
 
         # Loop on input grid
         iyimin, iyimax = get_iminmax(yi[ixiy])
         iyomin, iyomax = get_iminmax(yo[ixoy])
         for iyi in range(iyimin, iyimax):
 
             # Out of bounds
             if yi[ixiy, iyi + 1] < yo[ixoy, iyomin]:
                 continue
             if yi[ixiy, iyi] > yo[ixoy, iyomax]:
                 break
 
             # Loop on output grid
-            for iyo in range(iyomin, nyo):
+            for iyo in range(iyomin, iyomax + 1):
 
                 dy0 = yo[ixoy, iyo] - yi[ixiy, iyi]
                 dy1 = yi[ixiy, iyi + 1] - yo[ixoy, iyo]
 
                 # Above
                 if dy1 < 0.0:  # above
                     break
 
+                # Below
+                if dy0 < 0.0:
+                    iyomin = iyo + 1
+
                 # Inside
                 if dy0 >= 0.0 and dy1 >= 0.0:
 
                     iyomin = iyo
                     mu = dy0 / (dy0 + dy1)
 
                     # Extrapolations
                     if iyi == iyimin:  # y0
-                        vc0 = 2 * vari[ix, iyi] - vari[ix, iyi + 1]
+                        vc0 = 2 * vari[ixi, iyi] - vari[ixi, iyi + 1]
                     else:
                         vc0 = vari[ixi, iyi - 1]
                     if iyi == iyimax - 1:  # y3
                         vc1 = 2 * vari[ixi, iyi + 1] - vari[ixi, iyi]
                     else:
                         vc1 = vari[ixi, iyi + 2]
 
                     # Interpolation
-                    varo[ix, iyo] = vc1 - vari[ix, iyi + 1] - vc0 + vari[ix, iyi]
-                    varo[ix, iyo] = mu ** 3 * varo[ix, iyo] + mu ** 2 * (
-                        vc0 - vari[ix, iyi] - varo[ix, iyo]
+                    varo[ix, iyo] = vc1 - vari[ixi, iyi + 1] - vc0 + vari[ixi, iyi]
+                    varo[ix, iyo] = mu**3 * varo[ix, iyo] + mu**2 * (
+                        vc0 - vari[ixi, iyi] - varo[ix, iyo]
                     )
-                    varo[ix, iyo] += mu * (vari[ix, iyi + 1] - vc0)
-                    varo[ix, iyo] += vari[ix, iyi]
+                    varo[ix, iyo] += mu * (vari[ixi, iyi + 1] - vc0)
+                    varo[ix, iyo] += vari[ixi, iyi]
 
     # Extrapolation
     if extrap != "no":
         varo = extrap1d(varo, extrap)
 
     return varo
 
 
 @numba.njit(parallel=False, cache=NOT_CI)
-def hermit1d(vari, yi, yo, extrap="no", bias=0.0, tension=0.0):
+def hermit1d(vari, yi, yo, eshapes, extrap="no", bias=0.0, tension=0.0):
     """Hermitian interp. of nD data along an axis with varying coordinates
 
     Warning
     -------
     `nxi` must be either a multiple or a divisor of `nxo`,
     and multiple of `nxiy`.
 
     Parameters
     ----------
     vari: array_like(nxi, nyi)
     yi: array_like(nxiy, nyi)
     yo: array_like(nxo, nyo)
+    eshapes: array_like(3, ndim-1)
     bias: float
     tension: float
 
     Return
     ------
     array_like(nx, nyo): varo
         With `nx=max(nxi, nxo)`
     """
     # Shapes
-    nxi, nyi = vari.shape
-    nxiy = yi.shape[0]
-    nxi, nyi = vari.shape
-    nxo, nyo = yo.shape
-    nx = max(nxi, nxo)
+    nyo = yo.shape[1]
+    eshape = np.empty(eshapes.shape[1], eshapes.dtype)
+    for i in range(eshape.size):
+        eshape[i] = eshapes[:, i].max()
+    nx = np.prod(eshape)
 
     # Init output
     varo = np.full((nx, nyo), np.nan, dtype=vari.dtype)
 
     # Loop on the varying dimension
     for ix in numba.prange(nx):
 
-        # Index along x for coordinate arrays
-        ixi = min(nxi - 1, ix % nxi)
-        ixiy = min(nxiy - 1, ix % nxiy)
-        ixoy = min(nxo - 1, ix % nxo)
+        # Index along x for all arrays
+        ii = unravel_index(ix, eshape)
+        ixi = ravel_index(np.minimum(ii, eshapes[0] - 1), eshapes[0])
+        ixiy = ravel_index(np.minimum(ii, eshapes[1] - 1), eshapes[1])
+        ixoy = ravel_index(np.minimum(ii, eshapes[2] - 1), eshapes[2])
 
         # Loop on input grid
         iyimin, iyimax = get_iminmax(yi[ixiy])
         iyomin, iyomax = get_iminmax(yo[ixoy])
         for iyi in range(iyimin, iyimax):
 
             # Out of bounds
             if yi[ixiy, iyi + 1] < yo[ixoy, iyomin]:
                 continue
             if yi[ixiy, iyi] > yo[ixoy, iyomax]:
                 break
 
             # Loop on output grid
-            for iyo in range(iyomin, nyo):
+            for iyo in range(iyomin, iyomax + 1):
 
                 dy0 = yo[ixoy, iyo] - yi[ixiy, iyi]
                 dy1 = yi[ixiy, iyi + 1] - yo[ixoy, iyo]
 
                 # Above
                 if dy1 < 0.0:  # above
                     break
 
+                # Below
+                if dy0 < 0.0:
+                    iyomin = iyo + 1
+
                 # Inside
                 if dy0 >= 0.0 and dy1 >= 0.0:
 
                     iyomin = iyo
                     mu = dy0 / (dy0 + dy1)
 
                     # Extrapolations
                     if iyi == iyimin:  # y0
-                        vc0 = 2 * vari[ix, iyi] - vari[ix, iyi + 1]
+                        vc0 = 2 * vari[ixi, iyi] - vari[ixi, iyi + 1]
                     else:
                         vc0 = vari[ixi, iyi - 1]
                     if iyi == iyimax - 1:  # y3
                         vc1 = 2 * vari[ixi, iyi + 1] - vari[ixi, iyi]
                     else:
                         vc1 = vari[ixi, iyi + 2]
 
                     # Interpolation
                     mu = dy0 / (dy0 + dy1)
-                    a0 = 2 * mu ** 3 - 3 * mu ** 2 + 1
-                    a1 = mu ** 3 - 2 * mu ** 2 + mu
-                    a2 = mu ** 3 - mu ** 2
-                    a3 = -2 * mu ** 3 + 3 * mu ** 2
-                    varo[ix, iyo] = a0 * vari[ix, iyi]
+                    a0 = 2 * mu**3 - 3 * mu**2 + 1
+                    a1 = mu**3 - 2 * mu**2 + mu
+                    a2 = mu**3 - mu**2
+                    a3 = -2 * mu**3 + 3 * mu**2
+                    varo[ix, iyo] = a0 * vari[ixi, iyi]
                     varo[ix, iyo] += a1 * (
-                        (vari[ix, iyi] - vc0) * (1 + bias) * (1 - tension) / 2
-                        + (vari[ix, iyi + 1] - vari[ix, iyi]) * (1 - bias) * (1 - tension) / 2
+                        (vari[ixi, iyi] - vc0) * (1 + bias) * (1 - tension) / 2
+                        + (vari[ixi, iyi + 1] - vari[ixi, iyi]) * (1 - bias) * (1 - tension) / 2
                     )
                     varo[ix, iyo] += a2 * (
-                        (vari[ix, iyi + 1] - vari[ix, iyi]) * (1 + bias) * (1 - tension) / 2
-                        + (vc1 - vari[ix, iyi + 1]) * (1 - bias) * (1 - tension) / 2
+                        (vari[ixi, iyi + 1] - vari[ixi, iyi]) * (1 + bias) * (1 - tension) / 2
+                        + (vc1 - vari[ixi, iyi + 1]) * (1 - bias) * (1 - tension) / 2
                     )
-                    varo[ix, iyo] += a3 * vari[ix, iyi + 1]
+                    varo[ix, iyo] += a3 * vari[ixi, iyi + 1]
 
     if extrap != "no":
         varo = extrap1d(varo, extrap)
 
     return varo
 
 
@@ -429,15 +418,15 @@
         if mode == "both" or mode == "top":
             varo[ix, iytop + 1 :] = varo[ix, iytop]
 
     return varo
 
 
 @numba.njit(parallel=False, cache=NOT_CI)
-def cellave1d(vari, yib, yob, extrap="no", conserv=False):
+def cellave1d(vari, yib, yob, eshapes, extrap="no", conserv=False):
     """Cell average regrid. of nD data along an axis with varying coordinates
 
     Warning
     -------
     `nxi` must be either a multiple or a divisor of `nxo`,
     and multiple of `nxiy`.
 
@@ -449,31 +438,39 @@
 
     Return
     ------
     array_like(nx, nyo): varo
         With `nx=max(nxi, nxo)`
     """
     # Shapes
-    nxi, nyib = vari.shape
-    nxiy, nyi = yib.shape
-    nxi, nyi = vari.shape
-    nxo, nyob = yob.shape
-    nx = max(nxi, nxo)
-    nyo = nyob - 1
+    # nxi, nyib = vari.shape
+    # nxiy, nyi = yib.shape
+    # nxi, nyi = vari.shape
+    # nxo, nyob = yob.shape
+    # nx = max(nxi, nxo)
+    # nyo = nyob - 1
+
+    nyi = vari.shape[1]
+    nyo = yob.shape[1] - 1
+    eshape = np.empty(eshapes.shape[1], eshapes.dtype)
+    for i in range(eshape.size):
+        eshape[i] = eshapes[:, i].max()
+    nx = np.prod(eshape)
 
     # Init output
     varo = np.zeros((nx, nyo), dtype=vari.dtype)
 
     # Loop on the varying dimension
     for ix in numba.prange(nx):
 
         # Index along x for coordinate arrays
-        ixi = min(nxi - 1, ix % nxi)
-        ixiy = min(nxiy - 1, ix % nxiy)
-        ixoy = min(nxo - 1, ix % nxo)
+        ii = unravel_index(ix, eshape)
+        ixi = ravel_index(np.minimum(ii, eshapes[0] - 1), eshapes[0])
+        ixiy = ravel_index(np.minimum(ii, eshapes[1] - 1), eshapes[1])
+        ixoy = ravel_index(np.minimum(ii, eshapes[2] - 1), eshapes[2])
 
         # Loop on output cells to be filled
         iyi0 = 0
         for iyo in range(nyo):
 
             if yob[ixoy, iyo] == yob[ixoy, iyo + 1]:
                 continue
@@ -505,15 +502,15 @@
 
                 # Contribution of intersection
                 dyio = min(yib1, yob[ixoy, iyo + 1]) - max(yib0, yob[ixoy, iyo])
                 if conserv and yib0 != yib1:
                     dyio = dyio / (yob[ixoy, iyo + 1] - yob[ixoy, iyo])
                 if not np.isnan(vari[ixi, iyi]):
                     wo = wo + dyio
-                    varo[ixi, iyo] += vari[ix, iyi] * dyio
+                    varo[ixi, iyo] += vari[ixi, iyi] * dyio
 
                 # Next input cell?
                 if yib1 >= yob[ixoy, iyo + 1]:
                     break
 
             # Normalize
             if not conserv:
@@ -600,15 +597,15 @@
     AA = c * d - a * f
     BB = -c * yy + b * d + xx * f - a * e
     CC = -yy * b + e * xx
     if abs(AA) < small:
         p1 = -CC / BB
         p2 = p1
     else:
-        DD = BB ** 2 - 4 * AA * CC
+        DD = BB**2 - 4 * AA * CC
         sDD = math.sqrt(DD)
         p1 = (-BB - sDD) / (2 * AA)
         p2 = (-BB + sDD) / (2 * AA)
 
     # Get q from p
     if abs(b + c * p1) > small:
         q1 = (xx - a * p1) / (b + c * p1)
@@ -962,7 +959,61 @@
                                 ) * (
                                     (1 - c[ie % nexz]) * (1 - kk) + c[ie % nexz] * kk
                                 ) * (
                                     (1 - d) * (1 - ll) + d * ll
                                 )
 
     return vo
+
+
+@numba.guvectorize(
+    [(numba.float64[:], numba.float64[:], numba.float64[:], numba.boolean, numba.float64[:])],
+    "(nz),(nz),(),()->()",
+)
+def isoslice(var, values, isoval, reverse, isovar):
+    """Extract data from var where values==isoval
+
+    Parameters
+    ----------
+    var: array_like
+        array from which the data are extracted
+    values: array_like
+        array on which a research of isoval is made
+    isoval: float
+        value of interest on which we perform research in values array
+    reverse: bool
+        search from the last index instead of the first one
+
+    Return
+    ------
+    isovar : array_like
+           Sliced array based on var where values==isoval
+
+    Example
+    -------
+
+    Let's define depth and temperature variables both in 3 dimensions (i,j,k)
+    where i and j are horizontal dimension and k the vertical one::
+
+        dep_at_t20 = isoslice(dep, temp, 20)   # depth at temperature=20°C
+        temp_at_z15 = isoslice(temp, dep, -15) # temperature at depth=-15m
+
+
+    """
+    nz = var.shape[-1]
+    isovar[0] = np.nan
+    if reverse:
+        istart, istop, istep = nz - 1, 1, -1
+    else:
+        istart, istop, istep = 0, nz - 2, 1
+
+    # From the top
+    for i in numba.prange(istart, istop + istep, istep):
+        if (values[i] >= isoval[0] and values[i + istep] <= isoval[0]) or (
+            values[i] <= isoval[0] and values[i + istep] >= isoval[0]
+        ):
+            if values[i + istep] == values[i]:
+                isovar[0] = values[i]
+            else:
+                isovar[0] = var[i + istep] + (isoval[0] - values[i + istep]) * (
+                    var[i] - var[i + istep]
+                ) / (values[i] - values[i + istep])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xoa-0.6.1/xoa/krig.py` & `xoa-0.7.0/xoa/krig.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/misc.py` & `xoa-0.7.0/xoa/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,27 +182,52 @@
     case_insensitive: bool
         Wether the treatment of string type choice should be case
         sensitive or not.
     parameter: None, str
         Parameter name, which defaults to the lower case class name
     description: str
         Short description of the parameter.
+    aliases: dict, None
+        Allowed alternate values for selected choices
     """
 
-    def __init__(self, choices, case_insensitive=True, parameter=None, description="Choices"):
+    def __init__(
+        self, choices, case_insensitive=True, parameter=None, description="Choices", aliases=None
+    ):
         self._ci = case_insensitive
         self._docs = {}
+        if aliases:
+            aa = {}
+            for key, values in aliases.items():
+                key = self._reformat_value_(key)
+                if not isinstance(values, (list, tuple)):
+                    values = [values]
+                else:
+                    values = list(values)
+                values = [self._reformat_value_(value) for value in values]
+                aa[key] = values
+            aliases = aa
         if isinstance(choices, dict):
             self._choices = []
             for value, doc in choices.items():
-                value = self._reformat_value_(value)
-                self._docs[value] = doc
+                value = doc_value = self._reformat_value_(value)
                 self._choices.append(value)
+                if aliases and value in aliases:
+                    doc_value = "|".join([repr(val) for val in ([value] + aliases[value])])
+                    self._choices.extend(aliases[value])
+                else:
+                    doc_value = repr(doc_value)
+                self._docs[doc_value] = doc
         else:
-            self._choices = [self._reformat_value_(value) for value in choices]
+            self._choices = []
+            for value in choices:
+                value = self._reformat_value_(value)
+                self._choices.append(value)
+                if aliases and value in aliases:
+                    self._choices.extend(aliases[value])
         self._parameter = self.__class__.__name__.lower() if parameter is None else parameter
         self._description = description
 
     @property
     def choices(self):
         return self._choices
 
@@ -217,15 +242,15 @@
             desc = self._description if self._description else 'choice'
             raise XoaError(
                 f"Invalid choice for \"{desc}\": {choice}. " f"Please choose one of: {self}"
             )
         return choice
 
     def __str__(self):
-        return ", ".join(self._choices)
+        return ", ".join([repr(choice) for choice in self._choices])
 
     def to_docstring(self, indent=4):
         """Convert to numpy-like docstring
 
         Parameters
         ----------
         indent: str, int
```

### Comparing `xoa-0.6.1/xoa/regrid.py` & `xoa-0.7.0/xoa/regrid.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 from . import interp
 
 
 class XoaRegridError(XoaError):
     pass
 
 
+# %% 1D
+
+
 class regrid1d_methods(misc.IntEnumChoices, metaclass=misc.DefaultEnumMeta):
     """Supported :func:`regrid1d` methods"""
 
     #: Linear interpolation (default)
     linear = 1
     #: Linear iterpolation (default)
     interp = 1  # compat
@@ -79,53 +82,66 @@
     #: Both below and above
     yes = 2
     #: Both below and above
     true = 2
 
 
 def _asfloat_(arr):
+    """We need arrays that are at least 1D and that are not dates, booleans or integers"""
     arr = np.asarray(arr)
+    arr = np.atleast_1d(arr)
     if arr.dtype.type is np.datetime64:
         arr = (arr - np.datetime64("1950-01-01", "us")) / np.timedelta64(1, "us")
     elif arr.dtype.char in 'il?':
         arr = arr.astype("d")
     return arr
 
 
 def _wrapper1d_(vari, *args, func_name, **kwargs):
     """To make sure arrays have a 2D shape
 
     Output array is reshaped back accordindly
     """
+
+    # The function to call
+    func = getattr(interp, func_name)
+
     # To 2D
-    vari = _asfloat_(vari)
-    eshape = vari.shape[:-1]
-    args = [_asfloat_(arr) for arr in args]
-    args = [np.reshape(arr, (-1, arr.shape[-1])) for arr in [vari] + args]
+    args = [vari] + list(args)
+    eshapes = []
+    for arr in args:
+        eshape = list(arr.shape[:-1])
+        if len(eshapes) and len(eshape) < len(eshapes[-1]):
+            eshape = [1] * (len(eshapes[-1]) - len(eshape)) + eshape
+        eshapes.append(eshape)
+    eshapes = np.array(eshapes, dtype='l')
+    args = [_asfloat_(arr).reshape(-1, arr.shape[-1]) for arr in args]
+    func_code = getattr(func, "func_code", getattr(func, "__code__"))
+    if "eshapes" in func_code.co_varnames[: func_code.co_argcount]:
+        args = args + [eshapes]
 
     # Call
-    func = getattr(interp, func_name)
     varo = func(*args, **kwargs)
 
     # From 2D
-    return varo.reshape(eshape + varo.shape[-1:])
+    return varo.reshape(tuple(eshapes.max(axis=0)) + varo.shape[-1:])
 
 
 def regrid1d(
     da,
     coord,
     method=None,
     dim=None,
     coord_in_name=None,
     edges=None,
     conserv=False,
     extrap="no",
     bias=0.0,
     tension=0.0,
-    dask='allowed',
+    dask='parallelized',
 ):
     """Regrid along a single dimension
 
     The input and output coordinates may vary along other dimensions,
     which useful for instance for vertical interpolation in coastal
     ocean models.
     Since it uses func:`xarray.apply_ufunc`, it support dask features.
@@ -158,21 +174,22 @@
         coordinates except along the interpolation dimension on which 1 is added.
     conserv: bool
         Use conservative regridding when using ``cellave`` method.
     extrap: str, int
         Extrapolation mode as one of the following:
         {extrap_modes.rst_with_links}
     dask: str
+        See :func:`xarray.apply_ufunc`.
 
     Returns
     -------
     xarray.DataArray
         Regridded array with ``coord`` as new coordinate array.
 
-    See also
+    See Also
     --------
     xoa.interp.nearest1d
     xoa.interp.linear2d
     xoa.interp.cubic2d
     xoa.interp.hermit1d
     xoa.interp.cellave1d
     xoa.interp.extrap1d
@@ -199,15 +216,15 @@
             dim_in = dim_out  # be cafeful, dim1 must be in input!
     assert dim_in in da.dims
     assert dim_out in coord.dims
 
     # Input coordinate
     if coord_in_name:
         assert coord_in_name in da.coords, 'Invalid coordinate'
-        coord_in = da.coords['coord_in_name']
+        coord_in = da.coords[coord_in_name]
     else:
         coord_in = cfspecs_in.search_coord_from_dim(da, dim_in, errors="raise")
         coord_in_name = coord_in.name
 
     # Coordinate arguments
     output_sizes = {dim_out: coord.sizes[dim_out]}
     input_core_dims = [[dim_in]]
@@ -280,29 +297,29 @@
 
     return da_out
 
 
 regrid1d.__doc__ = regrid1d.__doc__.format(**locals())
 
 
-def extrap1d(da, dim, mode, **kwargs):
+def extrap1d(da, dim, mode, dask='parallelized'):
     """Extrapolate along a single dimension
 
 
     Parameters
     ----------
     da: xarray.DataArray
         Array to interpolate
     dim:  str
         Dimension on which to operate.
     mode: str, int
         Extrapolation mode as one of the following:
         {extrap_modes.rst_with_links}
-    kwargs: dict
-        Extra arguments are passed to :func:`xarray.apply_ufunc`
+    dask: str
+        See :func:`xarray.apply_ufunc`.
 
     Returns
     -------
     xarray.DataArray
         Extrapolated array.
 
     See also
@@ -314,27 +331,86 @@
         _wrapper1d_,
         da,
         join="override",
         kwargs={"func_name": "extrap1d", "mode": str(extrap_modes[mode])},
         input_core_dims=[[dim]],
         output_core_dims=[[dim]],
         exclude_dims={dim},
+        dask=dask,
         dask_gufunc_kwargs={"output_sizes": da.sizes},
-        **kwargs,
     )
     da_out = da_out.transpose(*da.dims)
     da_out = da_out.assign_coords(da.coords)
     da_out.attrs.update(da.attrs)
     da_out.encoding.update(da.encoding)
     return da_out
 
 
 extrap1d.__doc__ = extrap1d.__doc__.format(**locals())
 
 
+def isoslice(da, values, isoval, dim, reverse=False, dask='parallelized', **kwargs):
+    """Extract data from var where values==isoval
+
+    Parameters
+    -----------
+    da: xarray.DataArray
+          array from which the data are extracted
+    values: array_like
+          array on which a research of isoval is made
+    isoval: float
+          value of interest on which we perform research in values array
+    dim: str
+          dimension shared by da and values on which the slice is made
+    dask: str
+        See :func:`xarray.apply_ufunc`.
+
+    Return
+    ------
+    isovar : array_like
+            Sliced array based on data where values==isoval
+
+    Example
+    -------
+
+    Let's define depth and temperature variables both in 3 dimensions (i,j,k)
+    where i and j are horizontal dimension and k the vertical one::
+
+        dep_at_t20 = isoslice(dep, temp, 20, "z")   # depth at temperature=20°C
+        temp_at_z15 = isoslice(temp, dep, -15, "z") # temperature at depth=-15m
+
+    See Also
+    --------
+    xoa.interp.isoslice
+    xarray.apply_ufunc
+    """
+
+    assert dim in da.dims
+    assert dim in values.dims
+
+    da_out = xr.apply_ufunc(
+        interp.isoslice,
+        da,
+        values,
+        isoval,
+        reverse,
+        join="override",
+        input_core_dims=[[dim], [dim], [], []],
+        exclude_dims={dim},
+        dask=dask,
+        **kwargs,
+    )
+    da_out.attrs.update(da.attrs)
+    da_out.encoding.update(da.encoding)
+    return da_out
+
+
+# %% 2D
+
+
 def grid2loc(da, loc, compat="warn"):
     """Interpolate a gridded data array to random locations
 
     ``da`` and ``loc`` must comply with CF conventions.
 
     Parameters
     ----------
@@ -356,15 +432,15 @@
         In case a requested coordinate is not found in the input dataset.
 
     Return
     ------
     xarray.dataArray
         The interpolated data array.
 
-    See also
+    See Also
     --------
     xoa.interp.grid2locs
     xoa.interp.grid2relloc
     xoa.interp.grid2rellocs
     xoa.interp.cell2relloc
     """
 
@@ -395,15 +471,15 @@
     glat = xcoords.get_lat(da)  # before to_rect
     dims_in = set(glon.dims).union(glat.dims)
     da_tmp = xgrid.to_rect(da)
     da_tmp = xcoords.reorder(da_tmp, order)
 
     # To numpy with singletons
     # - data
-    vi = da_tmp.data
+    vi = da_tmp.values
     for axis_type, axis in (("z", -3), ("t", -4)):
         if axis_type not in order:
             vi = np.expand_dims(vi, axis)
     vi = vi.reshape((-1,) + vi.shape[-4:])
     # - xy
     glon = xcoords.get_lon(da_tmp)  # after to_rect
     glat = xcoords.get_lat(da_tmp)  # after to_rect
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xoa-0.6.1/xoa/sigma.py` & `xoa-0.7.0/xoa/sigma.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,20 +19,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 
 import numpy as np
+import numba
+import xarray as xr
 
 from .__init__ import xoa_warn
 from . import misc
 from . import cf
 from . import coords as xcoords
 
+# %% Constants
+
 #: To convert from formula terms to CF names
 FORMULA_TERMS_TO_CF_NAMES = {
     'c': 'cs',  # C
     's': 'sig',
     'sigma': 'sig',
     'eta': 'ssh',
     'depth': 'bathy',
@@ -54,19 +58,111 @@
 )
 
 
 class XoaSigmaError(cf.XoaCFError):
     pass
 
 
-def atmosphere_sigma_coordinate(sig, ps, ptop, cache=None):
-    """Convert from sigma [0, 1] to altitude in an atmopsheric model
+# %% Low level routines
+
+
+@numba.njit(cache=True)
+def _atmosphere_sigma_(sigma, ps, ptop):
+    p = np.zeros(ps.shape + sigma.shape)
+    for k in numba.prange(sigma.shape[0]):
+        p[..., k] = ptop
+        p[..., k] = p[..., k] + sigma[k] * (ps - ptop)
+    return p
+
+
+@numba.njit(cache=True)
+def _ocean_sigma_(sigma, eta, depth):
+    z = np.zeros(eta.shape + sigma.shape)
+    for k in numba.prange(sigma.shape[0]):
+        z[..., k] = eta
+        z[..., k] = z[..., k] + sigma[k] * (eta + depth)
+    return z
+
+
+@numba.njit(cache=True)
+def _ocean_s_(s, eta, depth, depth_c, C):
+    z = np.zeros(eta.shape + s.shape)
+    for k in numba.prange(s.shape[0]):
+        z[..., k] = eta * (1 + s[k])
+        z[..., k] = z[..., k] + depth_c * s[k]
+        z[..., k] = z[..., k] + (depth - depth_c) * C[k]
+    return z
+
+
+@numba.njit(cache=True)
+def _ocean_s_g1_(s, eta, depth, depth_c, C):
+    z = np.zeros(eta.shape + s.shape)
+    for k in numba.prange(s.shape[0]):
+        S = depth_c * s[k]
+        S = S + (depth - depth_c) * C[k]
+        z[..., k] = S
+        z[..., k] = z[..., k] + eta * (1.0 + S / depth)
+    return z
+
+
+@numba.njit(cache=True)
+def _ocean_s_g2_(s, eta, depth, depth_c, C):
+    z = np.zeros(eta.shape + s.shape)
+    for k in numba.prange(s.shape[0]):
+        S = depth_c * s[k] + depth * C[k]
+        S = S / (depth + depth_c)
+        z[..., k] = S * (depth + eta)
+        z[..., k] = z[..., k] + eta
+    return z
+
+
+def _apply_ocean_s_(func, sig, ssh, bathy, hc, thetas, thetab, cs, cs_type, dask):
+    # Stetching curve
+    if cs is None:
+        if None in (thetas, thetab):
+            raise XoaSigmaError("thetas and thetab must be provided when cs is not")
+        cs = get_cs(sig, thetas, thetab, cs_type)
+
+    # Checks dims
+    if np.ndim(hc) and set(hc.dims) != set(bathy.dims):
+        raise XoaSigmaError("Incompatible dimensions between bathy and hc")
+
+    # Call core routine
+    zdim = sig.dims[0]
+    depth = xr.apply_ufunc(
+        func,
+        sig,
+        ssh,
+        bathy,
+        hc,
+        cs,
+        input_core_dims=[[zdim], [], [], [], [zdim]],
+        output_core_dims=[[zdim]],
+        exclude_dims={zdim},
+        dask=dask,
+        dask_gufunc_kwargs={"output_sizes": {zdim: sig.shape[0]}},
+    )
+
+    # Format
+    return cf.get_cf_specs(sig).format_data_var(
+        depth, "depth", format_coords=False, rename_dims=False
+    )
+
+
+# %% High level routines
+
+
+def atmosphere_sigma_coordinate(sig, ps, ptop, dask="parallelized", cache=None):
+    """Convert from sigma [0, 1] to pressure in an atmopsheric model
+
+    .. note:: This function is dask-aware since it delegates the core computation to
+        :func:`xarray.apply_ufunc`.
 
     Source:
-        `Ocean sigma coordinate  <http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html#_atmosphere_sigma_coordinate>`_
+        `Atmosphere sigma coordinate  <http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html#_atmosphere_sigma_coordinate>`_
 
     Formula:
         .. math::
 
             p = p_{top} + \\sigma * (p_{surf}-p_{top})
 
     Sigma standard name:
@@ -85,25 +181,42 @@
         Air pressure at top of model (:math:`p_{top}` | ``ptop``)
 
     Returns
     -------
     xarray.DataArray
         Air pressure in Pa (:math:`p`)
     """
-    # Compute
-    p = sig * (ps - ptop)
-    p = p + ptop
+
+    if cache is not None:
+        xoa_warn("The `cache` parameter is currently not used.")
+
+    # Call core routine
+    zdim = sig.dims[0]
+    p = xr.apply_ufunc(
+        _atmosphere_sigma_,
+        sig,
+        ps,
+        ptop,
+        input_core_dims=[[zdim], [], []],
+        output_core_dims=[[zdim]],
+        exclude_dims={zdim},
+        dask=dask,
+        dask_gufunc_kwargs={"output_sizes": {zdim: sig.shape[0]}},
+    )
 
     # Format
-    return cf.get_cf_specs(sig).format_data_var(p, "plev", format_coords=False)
+    return cf.get_cf_specs(sig).format_data_var(p, "plev", format_coords=False, rename_dims=False)
 
 
-def ocean_sigma_coordinate(sig, ssh, bathy, cache=None):
+def ocean_sigma_coordinate(sig, ssh, bathy, dask="parallelized", cache=None):
     """Convert from sigma [-1, 0] to negative depths in an ocean model
 
+    .. note:: This function is dask-aware since it delegates the core computation to
+        :func:`xarray.apply_ufunc`.
+
     Source:
         `Ocean sigma coordinate <http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html#_ocean_sigma_coordinate>`_
 
     Formula:
         .. math::
 
             z = \\eta + \\sigma * (\\eta+h)
@@ -124,22 +237,39 @@
         Positive sea floor depth (:math:`h` | ``depth``)
 
     Returns
     -------
     xarray.DataArray
         Negative depth below surface in m (:math:`z`)
     """
+    if cache is not None:
+        xoa_warn("The `cache` parameter is currently not used.")
+
     # Compute
     if not set(bathy.dims) <= set(ssh.dims):
         raise XoaSigmaError("Incompatible dimensions between bathy and ssh")
-    z = sig * (bathy + ssh)
-    z = z + ssh
+
+    # Call core routine
+    zdim = sig.dims[0]
+    depth = xr.apply_ufunc(
+        _ocean_sigma_,
+        sig,
+        ssh,
+        bathy,
+        input_core_dims=[[zdim], [], []],
+        output_core_dims=[[zdim]],
+        exclude_dims={zdim},
+        dask=dask,
+        dask_gufunc_kwargs={"output_sizes": {zdim: sig.shape[0]}},
+    )
 
     # Format
-    return cf.get_cf_specs(sig).format_data_var(z, "depth", format_coords=False)
+    return cf.get_cf_specs(sig).format_data_var(
+        depth, "depth", format_coords=False, rename_dims=False
+    )
 
 
 def get_cs(sig, thetas, thetab, cs_type=None):
     """Get a s-coordinate stretching curve
 
     Parameters
     ----------
@@ -161,22 +291,37 @@
     -------
     xarray.DataArray
         Stretching curve (:math:`C` | ``C``)
     """
     s, a, b = sig, thetas, thetab
     cs = np.sinh(s * a) * (1 - b) / np.sinh(a)
     cs = cs + b * (np.tanh(a * (s + 0.5)) / (2 * np.tanh(0.5 * a)) - 0.5)
+    cs.name = None
     if hasattr(cs, "coords"):
-        cs = cf.get_cf_specs(sig).format_data_var(cs, "cs", format_coords=False)
+        cs = cf.get_cf_specs(sig).format_data_var(cs, "cs", format_coords=False, rename_dims=False)
     return cs
 
 
-def ocean_s_coordinate(sig, ssh, bathy, hc, thetas, thetab, cs=None, cs_type=None, cache=None):
+def ocean_s_coordinate(
+    sig,
+    ssh,
+    bathy,
+    hc,
+    thetas=None,
+    thetab=None,
+    cs=None,
+    cs_type=None,
+    cache=None,
+    dask="parallelized",
+):
     """Convert from s [-1, 0] to depths in an ocean model
 
+    .. note:: This function is dask-aware since it delegates the core computation to
+        :func:`xarray.apply_ufunc`.
+
     Source:
         `Ocean s-coordinate <http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html#_ocean_s_coordinate>`_
 
     Formula:
         .. math::
 
             z & = \\eta*(1+s) + h_c*s + (h-h_c)*C
@@ -213,55 +358,46 @@
         from call to call.
 
     Returns
     -------
     xarray.DataArray
         Negative depth below surface in m (:math:`z`)
     """
-    # Check cache first
-    if cache:
-        zconst = cache['zconst']
-
-    else:  # Compute
-
-        # Stetching curve
-        if cs is None:
-            cs = get_cs(sig, thetas, thetab, cs_type)
-
-        # Constant part of the formula
-        if np.ndim(hc) and set(hc.dims) != set(bathy.dims):
-            raise XoaSigmaError("Incompatible dimensions between bathy and hc")
-        zconst = sig * hc
-        zconst = zconst + cs * (bathy - hc)
-
-        # Store in cache
-        if isinstance(cache, dict):
-            cache.update(zconst=zconst)
-
-    # Final computation
-    z = (sig + 1) * ssh + zconst
+    if cache is not None:
+        xoa_warn("The `cache` parameter is currently not used.")
 
-    # Format
-    return cf.get_cf_specs(sig).format_data_var(z, "depth", format_coords=False)
+    return _apply_ocean_s_(_ocean_s_, sig, ssh, bathy, hc, thetas, thetab, cs, cs_type, dask)
 
 
 def ocean_s_coordinate_g1(
-    sig, ssh, bathy, hc, thetas=None, thetab=None, cs=None, cs_type=None, cache=None
+    sig,
+    ssh,
+    bathy,
+    hc,
+    thetas=None,
+    thetab=None,
+    cs=None,
+    cs_type=None,
+    cache=None,
+    dask="parallelized",
 ):
     """Convert from s [-1, 0] generic form 1 to depths in an ocean model
 
+    .. note:: This function is dask-aware since it delegates the core computation to
+        :func:`xarray.apply_ufunc`.
+
     Source:
         `Ocean s-coordinate, generic form 1 <http://cfconventions.org/cf-conventions/cf-conventions.html#_ocean_s_coordinate_generic_form_1>`_
 
     Formula:
         .. math::
 
-            z & = \\eta*(1+s) + (\\eta + h * S)
+            z & = S + \\eta*(1+s) + (1 + S / h)
 
-            S & = \\frac{h_c s + h C}{h_c + h}
+            S & = h_c s + (h - h_c) C
 
             C & = (1-b)*\\frac{\\sinh(a*s)}{\\sinh(a)} +  b*\\left[\\frac{\\tanh(a*(s+0.5))}{2*\\tanh(0.5*a)} - 0.5\\right]
 
 
 
     Sigma standard name:
         ``ocean_s_coordinate_g2``
@@ -295,59 +431,44 @@
         from call to call.
 
     Returns
     -------
     xarray.DataArray
         Negative depth below surface in m (:math:`z`)
     """
-    s, h = sig, bathy
+    if cache is not None:
+        xoa_warn("The `cache` parameter is currently not used.")
 
-    # Check cache first
-    if cache:
-        S = cache['S']
-        Sh1 = cache['Sh1']
-
-    else:  # Compute
-
-        # Stetching curve
-        if cs is None:
-            if None in (thetas, thetab):
-                raise XoaSigmaError("thetas and thetas must be provided when " "cs is not")
-            cs = get_cs(sig, thetas, thetab, cs_type)
-
-        # Constant part of the formula
-        if np.ndim(hc) and set(hc.dims) != set(h.dims):
-            raise XoaSigmaError("Incompatible dimensions between bathy and hc")
-        S = s * hc + cs * (h - hc)
-        Sh1 = S / h
-        Sh1 = Sh1 + 1
-
-        # Store in cache
-        if isinstance(cache, dict):
-            cache.update(S=S, Sh1=Sh1)
-
-    # Final computation
-    z = S + Sh1 * ssh
-
-    # Format
-    return cf.get_cf_specs(sig).format_data_var(z, "depth", format_coords=False)
+    return _apply_ocean_s_(_ocean_s_g1_, sig, ssh, bathy, hc, thetas, thetab, cs, cs_type, dask)
 
 
 def ocean_s_coordinate_g2(
-    sig, ssh, bathy, hc, thetas=None, thetab=None, cs=None, cs_type=None, cache=None
+    sig,
+    ssh,
+    bathy,
+    hc,
+    thetas=None,
+    thetab=None,
+    cs=None,
+    cs_type=None,
+    cache=None,
+    dask="parallelized",
 ):
     """Convert from s [-1, 0] generic form 2 to depths in an ocean model
 
+    .. note:: This function is dask-aware since it delegates the core computation to
+        :func:`xarray.apply_ufunc`.
+
     Source:
         `Ocean s-coordinate, generic form 2 <http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html#_ocean_s_coordinate_generic_form_2>`_
 
     Formula:
         .. math::
 
-            z & = \\eta*(1+s) + (\\eta + h * S)
+            z & = \\eta + (\\eta + h) * S
 
             S & = \\frac{h_c s + h C}{h_c + h}
 
             C & = (1-b)*\\frac{\\sinh(a*s)}{\\sinh(a)} +  b*\\left[\\frac{\\tanh(a*(s+0.5))}{2*\\tanh(0.5*a)} - 0.5\\right]
 
     Sigma standard name:
         ``ocean_s_coordinate_g2``
@@ -381,63 +502,39 @@
         from call to call.
 
     Returns
     -------
     xarray.DataArray
         Negative depth below surface in m (:math:`z`)
     """
-    s, h = sig, bathy
+    if cache is not None:
+        xoa_warn("The `cache` parameter is currently not used.")
 
-    # Check cache first
-    if cache:
-        S = cache['S']
-        hS = cache['hS']
-
-    else:  # Compute
-
-        # Stetching curve
-        if cs is None:
-            if None in (thetas, thetab):
-                raise XoaSigmaError("thetas and thetas must be provided when cs is not")
-            cs = get_cs(sig, thetas, thetab, cs_type)
-
-        # Constant part of the formula
-        if np.ndim(hc) and set(hc.dims) != set(h.dims):
-            raise XoaSigmaError("Incompatible dimensions between bathy and hc")
-        S = s * hc + cs * h
-        S = S / (hc + h)
-        hS = S * h
-
-        # Store in cache
-        if isinstance(cache, dict):
-            cache.update(S=S, hS=hS)
+    return _apply_ocean_s_(_ocean_s_g2_, sig, ssh, bathy, hc, thetas, thetab, cs, cs_type, dask)
 
-    # Final computation
-    z = hS + (S + 1) * ssh
 
-    # Format
-    return cf.get_cf_specs(sig).format_data_var(z, "depth", format_coords=False)
+# %% File decoding
 
 
 def _ds_search_ci_(ds, name):
-    """Case insensitive search in data_vars and coords of a dataset
+    """Case insensitive search in data_vars, coords and attrs of a dataset
 
     Parameters
     ----------
     ds: xarray.Dataset
     name: str
         Requested name
 
     Returns
     -------
     str
         Real name
     """
     lname = name.lower()
-    for cat in "data_vars", "coords":
+    for cat in "data_vars", "coords", "attrs":
         pool = getattr(ds, cat)
         names = [nm for nm in pool.keys()]
         lnames = [nm.lower() for nm in names]
         if lname in lnames:
             return names[lnames.index(lname)]
 
 
@@ -534,22 +631,17 @@
 
         # Check standard_name and get loc
         if "standard_name" not in sig.attrs:
             raise XoaSigmaError(
                 "No standard_name attribute found in sigma/s " "variable name: " + sig.name
             )
         standard_name, loc = cfspecs.sglocator.parse_attr("standard_name", sig.standard_name)
+        # skip this one
         if standard_name not in SIGMA_COORDINATE_TYPES:
-            raise XoaSigmaError(
-                "Sigma/s coordinate not supported: "
-                + standard_name
-                + ". Supported coordinates: "
-                + " ".join(SIGMA_COORDINATE_TYPES)
-            )
-
+            continue
         # Get formula terms
         if "formula_terms" not in sig.attrs:
             raise XoaSigmaError(
                 f"Sigma/s type variable {sig.name} " "has no formula_term attribute"
             )
         formula_terms = decode_formula_terms(sig.formula_terms)
 
@@ -653,25 +745,25 @@
 
         for hloc in hlocs:
 
             terms = vterms if hsingle else vterms[hloc]
             hloc = cfspecs.sglocator.parse_loc_arg(hloc)
             sigma_type = terms.pop("type")
 
-            # Args: keys are cf names, values ara dataarrays
+            # Args: keys are cf names, values are dataarrays
             kwargs = {}
             for vname, cf_name in terms.items():
                 if cf_name in HORIZONTAL_TERMS:
                     vname = cfspecs.sglocator.format_attr("name", vname, hloc)
                 kwargs[cf_name] = ds[vname]
 
             # Compute depth/altitude/pressure
             func = getattr(sigma_module, sigma_type)
-            cache = {}
-            kwargs['cache'] = cache
+            # cache = {}
+            # kwargs['cache'] = cache
             height = func(**kwargs)
 
             # Format
             loc = (hloc or "") + (vloc or "")
             height = cfspecs.sglocator.format_dataarray(height, loc)
 
             # Transpose if approriate and set as coordinate
```

### Comparing `xoa-0.6.1/xoa/tests/test_cf.py` & `xoa-0.7.0/xoa/tests/test_cf.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,18 @@
         ("long_name", "My var at RHO location", ("My var", "rho")),
         ("long_name", "My var at rho location", ("My var", "rho")),
         ("name", "myvarrho", ("myvar", "rho")),
     ],
 )
 def test_cf_sglocator_parse_attr_with_valid_locations(attr, value, expected):
     assert (
-        cf.SGLocator(valid_locations=['u', 'rho'], name_format="{root}{loc}",).parse_attr(
-            attr, value
-        )
+        cf.SGLocator(
+            valid_locations=['u', 'rho'],
+            name_format="{root}{loc}",
+        ).parse_attr(attr, value)
         == expected
     )
 
 
 @pytest.mark.parametrize(
     "name,standard_name,long_name,loc",
     [
@@ -109,15 +110,17 @@
         ("long_name", "My var", "x", False),
         ("name", "myvar", "t", True),
         ("name", "myvar", "x", False),
     ],
 )
 def test_cf_sglocator_match_attr(attr, root, loc, expected):
     value = dict(
-        standard_name="my_var_at_t_location", long_name="My var at T location", name="myvar_t",
+        standard_name="my_var_at_t_location",
+        long_name="My var at T location",
+        name="myvar_t",
     )[attr]
     assert cf.SGLocator().match_attr(attr, value, root, loc) is expected
 
 
 @pytest.mark.parametrize(
     "attr,root,loc,expected",
     [
@@ -356,24 +359,30 @@
     cfspecs = cf.CFSpecs({"data_vars": {"temp": {"name": "temperature"}}})
     assert cfspecs.data_vars.get_name("temp", specialize=specialize) == expected
 
 
 def test_cf_cfspecs_get_attrs():
     cfspecs = cf.get_cf_specs()
     attrs = cfspecs.data_vars.get_attrs("temp", other="ok")
-    assert attrs["long_name"] == "Temperature"
+    assert attrs["long_name"] == "Sea water in situ temperature"
     assert attrs["other"] == "ok"
 
 
 def test_cf_cfspecs_get_loc_mapping():
 
     cf_dict0 = {
-        "sglocator": {"valid_locations": ["u", "v"],},
+        "sglocator": {
+            "valid_locations": ["u", "v"],
+        },
         "data_vars": {
-            "u": {"loc": "u", "add_loc": False, "add_coords_loc": {"lon": True, "x": True},},
+            "u": {
+                "loc": "u",
+                "add_loc": False,
+                "add_coords_loc": {"lon": True, "x": True},
+            },
             "bathy": {"add_loc": True},
         },
     }
     cf_specs0 = cf.CFSpecs(cf_dict0)
 
     ds0 = xr.Dataset(
         {"u": (("time", "y", "x"), np.ones((1, 2, 3))), "bathy": (("y", "x"), np.ones((2, 3)))},
@@ -440,15 +449,19 @@
     assert res is not None
     assert res.shape == (20,)
     assert res.name == "lon"
 
 
 @pytest.mark.parametrize("cf_name", ["temp", None])
 @pytest.mark.parametrize(
-    "in_name,in_attrs", [("temp", None), ("xxx", {"standard_name": "sea_water_temperature"}),],
+    "in_name,in_attrs",
+    [
+        ("temp", None),
+        ("xxx", {"standard_name": "sea_water_temperature"}),
+    ],
 )
 def test_cf_cfspecs_match_data_var(cf_name, in_name, in_attrs):
 
     lon = xr.DataArray(range(5), dims='lon', name='lon')
     temp = xr.DataArray(
         range(20, 25), dims='lon', coords={'lon': lon}, name=in_name, attrs=in_attrs
     )
@@ -457,31 +470,43 @@
         assert res == 'temp'
     else:
         assert res is True
 
 
 @pytest.mark.parametrize("cf_name", ["temp", None])
 @pytest.mark.parametrize(
-    "in_name,in_attrs", [("temp", None), ("xxx", {"standard_name": "sea_water_temperature"}),],
+    "in_name,in_attrs",
+    [
+        ("temp", None),
+        ("xxx", {"standard_name": "sea_water_temperature"}),
+    ],
 )
 def test_cf_cfspecs_search_data_var(cf_name, in_name, in_attrs):
 
     lon = xr.DataArray(range(5), dims='lon', name='lon')
     temp = xr.DataArray(
         range(20, 25), dims='lon', coords={'lon': lon}, name=in_name, attrs=in_attrs
     )
     ds = temp.to_dataset()
     assert cf.get_cf_specs().search_data_var(ds, cf_name, get="cf_name") == 'temp'
 
 
 def test_cf_cfspecs_cats_get_loc_arg():
 
     cf_dict0 = {
-        "sglocator": {"valid_locations": ["u", "v"],},
-        "data_vars": {"u": {"loc": "u", "add_loc": False, "add_coords_loc": {"lon": True},},},
+        "sglocator": {
+            "valid_locations": ["u", "v"],
+        },
+        "data_vars": {
+            "u": {
+                "loc": "u",
+                "add_loc": False,
+                "add_coords_loc": {"lon": True},
+            },
+        },
     }
     cf_specs0 = cf.CFSpecs(cf_dict0)
 
     ds0 = xr.Dataset(
         {"u": (("time", "y", "x"), np.ones((1, 2, 3))), "bathy": (("y", "x"), np.ones((2, 3)))},
         coords={
             "lon": (("y", "x"), np.ones((2, 3))),
@@ -503,15 +528,19 @@
     locations1 = cf_specs1.get_loc_mapping(ds0)
     assert cf_specs1.coords.get_loc_arg(ds0["lon"], locations=locations1) == "v"
 
 
 @pytest.mark.parametrize("cf_name", [None, "lon"])
 @pytest.mark.parametrize(
     "in_name,in_attrs",
-    [("lon", None), ("xxx", {"standard_name": "longitude"}), ("xxx", {"units": "degrees_east"}),],
+    [
+        ("lon", None),
+        ("xxx", {"standard_name": "longitude"}),
+        ("xxx", {"units": "degrees_east"}),
+    ],
 )
 def test_cf_cfspecs_cats_format_dataarray(cf_name, in_name, in_attrs):
 
     lon = xr.DataArray(range(5), dims=in_name, name=in_name, attrs=in_attrs)
     lon = cf.get_cf_specs().coords.format_dataarray(lon, cf_name)
     assert lon.name == "lon"
     assert lon.standard_name == "longitude"
@@ -535,17 +564,23 @@
     cfspecs = cf.CFSpecs(cfg)
     assert cfspecs.data_vars.get_allowed_names("banana") == ['banana', 'bonono', 'binini', 'bununu']
 
 
 def test_cf_cfspecs_format_obj_with_loc():
 
     cf_dict0 = {
-        "sglocator": {"valid_locations": ["u", "v"],},
+        "sglocator": {
+            "valid_locations": ["u", "v"],
+        },
         "data_vars": {
-            "u": {"loc": "u", "add_loc": False, "add_coords_loc": {"lon": True, "x": True},},
+            "u": {
+                "loc": "u",
+                "add_loc": False,
+                "add_coords_loc": {"lon": True, "x": True},
+            },
             "bathy": {"add_loc": True},
         },
     }
     cf_specs0 = cf.CFSpecs(cf_dict0)
 
     ds0 = xr.Dataset(
         {"u": (("time", "y", "x"), np.ones((1, 2, 3))), "bathy": (("y", "x"), np.ones((2, 3)))},
@@ -560,38 +595,39 @@
     assert "y" in ds.dims
     assert "u" in ds
     assert "bathy_u" in ds
 
 
 @pytest.mark.parametrize("cf_name", [None, "temp"])
 @pytest.mark.parametrize(
-    "in_name,in_attrs", [("temp", None), ("yyy", {"standard_name": "sea_water_temperature"}),],
+    "in_name,in_attrs",
+    [
+        ("temp", None),
+        ("yyy", {"standard_name": "sea_water_temperature"}),
+    ],
 )
 def test_cf_cfspecs_format_data_var(cf_name, in_name, in_attrs):
 
     lon = xr.DataArray(range(5), dims='xxx', name='xxx', attrs={'standard_name': 'longitude'})
     temp = xr.DataArray(
         range(20, 25), dims='xxx', coords={'xxx': lon}, name=in_name, attrs=in_attrs
     )
     temp = cf.get_cf_specs().format_data_var(temp, cf_name)
     assert temp.name == "temp"
     assert temp.standard_name == "sea_water_temperature"
-    assert temp.long_name == "Temperature"
+    assert temp.long_name == "Sea water in situ temperature"
     assert temp.units == "degrees_celsius"
     assert temp.lon.standard_name == "longitude"
 
 
 def test_cf_cfspecs_format_data_var_coord():
     da = xr.DataArray(0, attrs={'standard_name': 'longitude_at_u_location'})
     da = cf.get_cf_specs().format_data_var(da)
 
 
-#     assert da.name == "lon_u"
-
-
 def test_cf_cfspecs_format_data_var_specialize():
     da = xr.DataArray(1, name="salinity")
     cfspecs = cf.CFSpecs({'data_vars': {'sal': {'name': 'supersal'}}})
     da = cfspecs.format_data_var(da, specialize=True)
     assert da.name == "supersal"
     assert da.standard_name == "sea_water_salinity"
 
@@ -785,18 +821,18 @@
     lat = xr.DataArray([4, 5], dims='yy', attrs={'units': 'degrees_north'})
     depth = xr.DataArray([4, 5], dims='level', attrs={'axis': 'Z'})
     da = xr.DataArray(
         np.ones((2, 2, 2, 2)), dims=('r', 'level', 'yy', 'xi'), coords={'level': depth, 'yy': lat}
     )
 
     cfspecs = cf.get_cf_specs().coords
-    dims = cfspecs.get_dims(da, 'xyzt', allow_positional=True)
+    dims = cfspecs.get_dims(da, ['x', 'y', 'z', 't'], allow_positional=True)
     assert dims == ('xi', 'yy', 'level', 'r')
     dims = cfspecs.get_dims(da, 'f', errors="ignore")
-    assert dims == (None,)
+    assert dims is None
 
 
 def test_cf_cfspecs_infer_coords():
     ds = xr.Dataset({"temp": ("nx", [1, 2]), "lon": ("nx", [4, 5])})
     ds = cf.get_cf_specs().infer_coords(ds)
     assert "lon" in ds.coords
```

### Comparing `xoa-0.6.1/xoa/tests/test_coords.py` & `xoa-0.7.0/xoa/tests/test_coords.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/tests/test_dyn.py` & `xoa-0.7.0/xoa/tests/test_dyn.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/tests/test_filter.py` & `xoa-0.7.0/xoa/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/tests/test_geo.py` & `xoa-0.7.0/xoa/tests/test_geo.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/tests/test_grid.py` & `xoa-0.7.0/xoa/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/tests/test_interp.py` & `xoa-0.7.0/xoa/tests/test_interp.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,269 +7,273 @@
 import numpy as np
 import pytest
 
 from xoa import interp
 
 
 def vfunc(t=0, z=0, y=0, x=0):
-    """A function that returns a linear combination of coordinates
-    """
-    return 1.13*x + 2.35*y + 3.24*z - 0.65*t
+    """A function that returns a linear combination of coordinates"""
+    return 1.13 * x + 2.35 * y + 3.24 * z - 0.65 * t
 
 
 def round_as_time(arr, units="us", origin="1950-01-01"):
     arr = arr.astype(f"m8[{units}]")
     origin = np.datetime64(origin, units)
     arr = arr + origin
     return (arr - origin) / np.timedelta64(1, units)
 
 
 @functools.lru_cache()
 def get_interp1d_data(
-        yimin=-100., yimax=0., yomin=-90., yomax=10., irregular=True):
+    yimin=-100.0,
+    yimax=0.0,
+    yomin=-90.0,
+    yomax=10.0,
+    irregular=True,
+    nx=17,
+    nyi=15,
+    nyo=25,
+    mask=True,
+):
 
     np.random.seed(0)
 
     # coords
-    nx = 17
-    nyi = 15
-    nyo = 25
     yi = np.linspace(yimin, yimax, nyi)
     yo = np.linspace(yomin, yomax, nyo)
     x = np.linspace(0, 700, nx)
     yyi = np.resize(yi, (nx, nyi))
     yyo = np.resize(yo, (nx, nyo))
     if irregular:
-        dyi = (yi[1]-yi[0])*0.49
+        dyi = (yi[1] - yi[0]) * 0.49
         yyi += np.random.uniform(-dyi, dyi, (nx, nyi))
-        dyo = (yo[1]-yo[0])*0.49
+        dyo = (yo[1] - yo[0]) * 0.49
         yyo += +np.random.uniform(-dyo, dyo, (nx, nyo))
     xxi = np.resize(x, (nyi, nx)).T
     xxo = np.resize(x, (nyo, nx)).T
 
     # input
     xxi = np.resize(x, (nyi, nx)).T
     vari = vfunc(y=yyi, x=xxi)
-    vari[int(nx/3):int(2*nx/3), int(nyi/3):int(2*nyi/3)] = np.nan
+    if mask:
+        vari[int(nx / 3) : int(2 * nx / 3), int(nyi / 3) : int(2 * nyi / 3)] = np.nan
+
+    # shapes of extra dims
+    eshapes = np.vstack((vari.shape[:-1], yyi.shape[:-1], yyo.shape[:-1]))
 
-    return xxi, yyi, vari, xxo, yyo
+    return xxi, yyi, vari, xxo, yyo, eshapes
 
 
 def test_interp_nearest1d():
 
     # Get data
-    xxi, yyi, vari, xxo, yyo = get_interp1d_data()
+    xxi, yyi, vari, xxo, yyo, eshapes = get_interp1d_data()
 
     # Interpolation
-    varon = interp.nearest1d(vari, yyi, yyo)
-    yyon = interp.nearest1d(yyi, yyi, yyo)
-    xxon = interp.nearest1d(xxi, yyi, yyo)
+    varon = interp.nearest1d(vari, yyi, yyo, eshapes)
+    yyon = interp.nearest1d(yyi, yyi, yyo, eshapes)
+    xxon = interp.nearest1d(xxi, yyi, yyo, eshapes)
     varon_true = vfunc(y=yyon, x=xxon)
     varon_true[np.isnan(varon)] = np.nan
     np.testing.assert_allclose(varon_true, varon)
 
 
 def test_interp_linear1d():
 
     # Get data
-    xxi, yyi, vari, xxo, yyo = get_interp1d_data()
+    xxi, yyi, vari, xxo, yyo, eshapes = get_interp1d_data()
 
     # Interpolation
-    varol = interp.linear1d(vari, yyi, yyo)
+    varol = interp.linear1d(vari, yyi, yyo, eshapes)
     assert not np.isnan(varol).all()
     varol_true = vfunc(y=yyo, x=xxo)
     varol_true[np.isnan(varol)] = np.nan
     np.testing.assert_allclose(varol_true, varol)
 
 
 def test_interp_cubic1d():
 
     # Get data
-    xxi, yyi, vari, xxo, yyo = get_interp1d_data()
+    xxi, yyi, vari, xxo, yyo, eshapes = get_interp1d_data()
 
     # Interpolation
-    varoh = interp.cubic1d(vari, yyi, yyo)
+    varoh = interp.cubic1d(vari, yyi, yyo, eshapes)
     assert not np.isnan(varoh).all()
     assert np.nanmax(varoh) <= np.nanmax(vari)
     assert np.nanmin(varoh) >= np.nanmin(vari)
 
 
 def test_interp_hermit1d():
 
     # Get data
-    xxi, yyi, vari, xxo, yyo = get_interp1d_data()
+    xxi, yyi, vari, xxo, yyo, eshapes = get_interp1d_data()
 
     # Interpolation
-    varoh = interp.hermit1d(vari, yyi, yyo)
+    varoh = interp.hermit1d(vari, yyi, yyo, eshapes)
     assert not np.isnan(varoh).all()
     assert np.nanmax(varoh) <= np.nanmax(vari)
     assert np.nanmin(varoh) >= np.nanmin(vari)
 
 
 @pytest.mark.parametrize("method", ["nearest", "linear", "cubic", "hermit"])
 def test_interp1d_nans_in_coords(method):
 
     # Get data
-    xxi, yyi, vari, xxo, yyo = get_interp1d_data()
+    xxi, yyi, vari, xxo, yyo, eshapes = get_interp1d_data()
 
     # Add nans to coords
     yyin = yyi.copy()
     yyin[:, :3] = np.nan
     yyin[:, -3:] = np.nan
     yyon = yyo.copy()
     yyon[:, :3] = np.nan
     yyon[:, -3:] = np.nan
 
     # Interpolations
-    func = getattr(interp, method+"1d")
-    varol = func(vari[:, 3:-3], yyi[:, 3:-3], yyo[:, 3:-3])
-    varoln = func(vari, yyin, yyon)
+    func = getattr(interp, method + "1d")
+    varol = func(vari[:, 3:-3], yyi[:, 3:-3], yyo[:, 3:-3], eshapes)
+    varoln = func(vari, yyin, yyon, eshapes)
     np.testing.assert_allclose(varol, varoln[:, 3:-3])
 
 
+@pytest.mark.parametrize("method", ["nearest", "linear", "cubic", "hermit"])
+def test_interp_interp1d_eshapes(method):
 
-# def test_interp_cellave1d():
-
-#     # coords
-#     nx = 17
-#     nyi = 20
-#     nyo = 12
-#     yib = np.linspace(-1000., 0., nyi+1)
-#     yob = np.linspace(-1200, 200, nyo+1)
-#     xb = np.arange(nx+1)
-#     xxib, yyib = np.meshgrid(xb, yib)
-#     xxob, yyob = np.meshgrid(xb, yob)
-
-#     # input
-#     u, v = np.mgrid[-3:3:nx*1j, -3:3:nyi*1j]-2
-#     vari = np.asarray(u**2+v**2)
-#     vari[int(nx/3):int(2*nx/3), int(nyi/3):int(2*nyi/3)] = np.nan
-
-#     # conserv, no extrap
-#     varoc = interp.cellave1d(vari, yib, yob, conserv=1, extrap=0)
-#     sumi = np.nansum(vari*np.resize(np.diff(yib), vari.shape), axis=1)
-#     sumo = np.nansum(varoc*np.resize(np.diff(yob), varoc.shape), axis=1)
-#     np.testing.assert_allclose(sumi, sumo)
-
-#     # average, no extrap
-#     varoa = interp.cellave1d(vari, yib, yob, conserv=0, extrap=0)
-#     np.testing.assert_allclose([np.nanmin(vari), np.nanmax(vari)],
-#                                [np.nanmin(vari), np.nanmax(vari)])
-
-#     # average, extrap
-#     varoe = interp.cellave1d(vari, yib, yob, conserv=0, extrap=2)
-#     assert not np.isnan(varoe[0]).any()
-#     vv = varoa[0, ~np.isnan(varoa[0])]
-#     np.testing.assert_allclose(vv[[0, -1]], varoe[0, [0, -1]])
-
-
-# def test_interp_cellave1dx():
-
-#     # coords
-#     nx = 17
-#     nyi = 20
-#     nyo = 12
-#     yib = np.linspace(-1000., 0., nyi+1)
-#     yob = np.linspace(-1200, 200, nyo+1)
-#     yyib = np.resize(yib, (nx, nyi+1))
-#     dyi = (yib[1]-yib[0])*0.49
-#     np.random.seed(0)
-#     yyib += np.random.uniform(-dyi, dyi, yyib.shape)
-
-#     # input
-#     u, v = np.mgrid[-3:3:nx*1j, -3:3:nyi*1j]-2
-#     vari = np.asarray(u**2+v**2)
-#     vari[int(nx/3):int(2*nx/3), int(nyi/3):int(2*nyi/3)] = np.nan
-
-#     # conserv, no extrap
-#     varoc = interp.cellave1dx(vari, yyib, yob, conserv=1, extrap=0)
-#     sumi = np.nansum(vari*np.diff(yyib, axis=1), axis=1)
-#     sumo = np.nansum(varoc*np.resize(np.diff(yob), varoc.shape), axis=1)
-#     np.testing.assert_allclose(sumi, sumo)
-
-#     # average, no extrap
-#     interp.cellave1dx(vari, yyib, yob, conserv=0, extrap=0)
-
-#     # average, extrap
-#     varoe = interp.cellave1dx(vari, yyib, yob, conserv=0, extrap=2)
-#     assert not np.isnan(varoe[0]).any()
+    # Get data and func
+    xxi, yyi, vari, xxo, yyo, eshapes = get_interp1d_data(nx=18, mask=False, irregular=False)
+    eshapes = np.repeat([[3, 6]], 3, axis=0)
+    func = getattr(interp, method + "1d")
+
+    # Reference
+    varol_ref = func(vari, yyi, yyo, eshapes).reshape(3, 6, -1)
+
+    # missing dim 0 for vari
+    vari0 = vari.reshape(3, 6, -1)[0]
+    eshapes0 = eshapes.copy()
+    eshapes0[0, 0] = 1
+    varol0 = func(vari0, yyi, yyo, eshapes0).reshape(3, 6, -1)
+    np.testing.assert_allclose(varol_ref[0], varol0[0])
+    np.testing.assert_allclose(varol_ref[0], varol0[1])
+
+    # missing dim 1 for vari
+    vari1 = vari.reshape(3, 6, -1)[:, 0]
+    eshapes1 = eshapes.copy()
+    eshapes1[0, 1] = 1
+    varol1 = func(vari1, yyi, yyo, eshapes1).reshape(3, 6, -1)
+    np.testing.assert_allclose(varol_ref[:, 0], varol1[:, 0])
+    np.testing.assert_allclose(varol_ref[:, 0], varol1[:, 1])
+
+    # missing dim 0 for yyi
+    yyi0 = yyi.reshape(3, 6, -1)[0]
+    eshapes0 = eshapes.copy()
+    eshapes0[1, 0] = 1
+    varol0 = func(vari, yyi0, yyo, eshapes0).reshape(3, 6, -1)
+    np.testing.assert_allclose(varol_ref, varol0)
+
+    # missing dim 1 for yyi
+    yyi1 = yyi.reshape(3, 6, -1)[:, 0]
+    eshapes1 = eshapes.copy()
+    eshapes1[1, 1] = 1
+    varol1 = func(vari, yyi1, yyo, eshapes1).reshape(3, 6, -1)
+    np.testing.assert_allclose(varol_ref, varol1)
+
+    # missing dim 0 for yyo
+    yyo0 = yyo.reshape(3, 6, -1)[0]
+    eshapes0 = eshapes.copy()
+    eshapes0[2, 0] = 1
+    varol0 = func(vari, yyi, yyo0, eshapes0).reshape(3, 6, -1)
+    np.testing.assert_allclose(varol_ref, varol0)
+
+    # missing dim 1 for yyo
+    yyo1 = yyo.reshape(3, 6, -1)[:, 0]
+    eshapes1 = eshapes.copy()
+    eshapes1[2, 1] = 1
+    varol1 = func(vari, yyi, yyo1, eshapes1).reshape(3, 6, -1)
+    np.testing.assert_allclose(varol_ref, varol1)
 
 
 def test_interp_cellave1d():
 
     np.random.seed(0)
 
     # coords
     nx = 17
     nyi = 20
     nyo = 12
-    yib = np.linspace(-1000., 0., nyi+1)
-    yob = np.linspace(-1200, 200, nyo+1)
-    yyib = np.resize(yib, (nx, nyi+1))
-    dyi = (yib[1]-yib[0])*0.49
+    yib = np.linspace(-1000.0, 0.0, nyi + 1)
+    yob = np.linspace(-1200, 200, nyo + 1)
+    yyib = np.resize(yib, (nx, nyi + 1))
+    dyi = (yib[1] - yib[0]) * 0.49
     yyib += np.random.uniform(-dyi, dyi, yyib.shape)
-    yyob = np.resize(yob, (nx, nyo+1))
-    dyo = (yob[1]-yob[0])*0.49
+    yyob = np.resize(yob, (nx, nyo + 1))
+    dyo = (yob[1] - yob[0]) * 0.49
     yyob += np.random.uniform(-dyo, dyo, yyob.shape)
+    eshapes = np.full((3, 1), nx)
 
     # input
-    u, v = np.mgrid[-3:3:nx*1j, -3:3:nyi*1j]-2
-    vari = np.asarray(u**2+v**2)
-    vari[int(nx/3):int(2*nx/3), int(nyi/3):int(2*nyi/3)] = np.nan
+    u, v = np.mgrid[-3 : 3 : nx * 1j, -3 : 3 : nyi * 1j] - 2
+    vari = np.asarray(u**2 + v**2)
+    vari[int(nx / 3) : int(2 * nx / 3), int(nyi / 3) : int(2 * nyi / 3)] = np.nan
 
     # conserv, no extrap
-    varoc = interp.cellave1d(vari, yyib, yyob, conserv=True, extrap="no")
-    sumi = np.nansum(vari*np.diff(yyib, axis=1), axis=1)
-    sumo = np.nansum(varoc*np.diff(yyob, axis=1), axis=1)
+    varoc = interp.cellave1d(vari, yyib, yyob, eshapes, conserv=True, extrap="no")
+    sumi = np.nansum(vari * np.diff(yyib, axis=1), axis=1)
+    sumo = np.nansum(varoc * np.diff(yyob, axis=1), axis=1)
     np.testing.assert_allclose(sumi, sumo)
 
     # average, no extrap
-    interp.cellave1d(vari, yyib, yyob, conserv=0, extrap="no")
+    interp.cellave1d(vari, yyib, yyob, eshapes, conserv=0, extrap="no")
 
     # average, extrap
-    varoe = interp.cellave1d(vari, yyib, yyob, conserv=False, extrap="both")
+    varoe = interp.cellave1d(vari, yyib, yyob, eshapes, conserv=False, extrap="both")
     assert not np.isnan(varoe[0]).any()
 
 
 @pytest.mark.parametrize(
     "x,y,pt,qt",
-    [(0., 0, 0, 0),
-     (3, 1, 0, 1),
-     (2, 3, 1, 1),
-     (-1, 2, 1, 0),
-     (1., 1.5, .5, .5),
-     (-1, -1, -1, -1),
-     ])
+    [
+        (0.0, 0, 0, 0),
+        (3, 1, 0, 1),
+        (2, 3, 1, 1),
+        (-1, 2, 1, 0),
+        (1.0, 1.5, 0.5, 0.5),
+        (-1, -1, -1, -1),
+    ],
+)
 def test_interp_cell2relloc(x, y, pt, qt):
 
-    x1, y1 = 0., 0.
-    x2, y2 = 3., 1.
-    x3, y3 = 2., 3.
-    x4, y4 = -1., 2.
+    x1, y1 = 0.0, 0.0
+    x2, y2 = 3.0, 1.0
+    x3, y3 = 2.0, 3.0
+    x4, y4 = -1.0, 2.0
     p, q = interp.cell2relloc(x1, x2, x3, x4, y1, y2, y3, y4, x, y)
     assert p == pt
     assert q == qt
 
 
 @functools.lru_cache()
 def get_grid2locs_coords(nex=4, nexz=2, nxi=7, nyi=6, nzi=5, nti=4, no=10):
 
     np.random.seed(0)
 
-    tti, zzi, yyi, xxi = np.mgrid[0:nti-1:nti*1j, 0:nzi-1:nzi*1j,
-                                  0:nyi-1:nyi*1j, 0:nxi-1:nxi*1j]
+    tti, zzi, yyi, xxi = np.mgrid[
+        0 : nti - 1 : nti * 1j,
+        0 : nzi - 1 : nzi * 1j,
+        0 : nyi - 1 : nyi * 1j,
+        0 : nxi - 1 : nxi * 1j,
+    ]
 
     zzi = zzi[None]
     zzi = np.repeat(zzi, nexz, axis=0)
 
     xyztomin = -0.5
-    xo = np.random.uniform(xyztomin, nxi-1.5, no)
-    yo = np.random.uniform(xyztomin, nyi-1.5, no)
-    zo = np.random.uniform(xyztomin, nzi-1.5, no)
-    to = np.random.uniform(xyztomin, nti-1.5, no)
+    xo = np.random.uniform(xyztomin, nxi - 1.5, no)
+    yo = np.random.uniform(xyztomin, nyi - 1.5, no)
+    zo = np.random.uniform(xyztomin, nzi - 1.5, no)
+    to = np.random.uniform(xyztomin, nti - 1.5, no)
 
     tti = round_as_time(tti)
     to = round_as_time(to)
 
     return xxi, yyi, zzi, tti, xo, yo, to, zo
 
 
@@ -280,91 +284,107 @@
     nexz = 2
     nxi = 7
     nyi = 6
     nzi = 5
     nti = 4
     no = 10
     xxi, yyi, zzi, tti, xo, yo, to, zo = get_grid2locs_coords(
-        nex=nex, nexz=nexz, nxi=nxi, nyi=nyi, nzi=nzi, nti=nti, no=no)
+        nex=nex, nexz=nexz, nxi=nxi, nyi=nyi, nzi=nzi, nti=nti, no=no
+    )
 
     # Pure 1D axes
     xi = xxi[0, 0, 0:1, :]  # (nyix=1,nxi)
     yi = yyi[0, 0, :, 0:1]  # (nyi,nxiy=1)
     zi = zzi[0:1, 0:1, :, 0:1, 0:1]  # (nexz=1,ntiz=1,nzi,nyiz=1,nxiz=1)
     ti = tti[:, 0, 0, 0]  # (nti)
     vi = vfunc(tti, zzi, yyi, xxi)
-    vi = np.resize(vi, (nex, )+vi.shape[1:])  # (nex,nti,nzi,nyi,nxi)
+    vi = np.resize(vi, (nex,) + vi.shape[1:])  # (nex,nti,nzi,nyi,nxi)
     vo_truth = np.array(vfunc(to, zo, yo, xo))
     vo_interp = interp.grid2locs(xi, yi, zi, ti, vi, xo, yo, zo, to)
     assert vo_interp[0].shape == vo_truth.shape
     vo_truth[np.isnan(vo_interp[0])] = np.nan
     np.testing.assert_allclose(vo_interp[0], vo_truth)
 
     # Single point in space
     xi = xxi[0, 0, 0:1, :1]  # (nyix=1,nxi)
     yi = yyi[0, 0, :1, 0:1]  # (nyi,nxiy=1)
     zi = zzi[0:1, 0:1, :, 0:1, 0:1]  # (nexz=1,ntiz=1,nzi,nyiz=1,nxiz=1)
     ti = tti[:, 0, 0, 0]  # (nti)
     vi = vfunc(tti, zzi, yyi, xxi)[:, :, :, :1, :1]
-    vi = np.resize(vi, (nex, )+vi.shape[1:])  # (nex,nti,nzi,1,1)
+    vi = np.resize(vi, (nex,) + vi.shape[1:])  # (nex,nti,nzi,1,1)
     vo_truth = np.array(vfunc(to, zo, yi[0], xi[0]))
     vo_interp = interp.grid2locs(xi, yi, zi, ti, vi, xo, yo, zo, to)
     vo_truth[np.isnan(vo_interp[0])] = np.nan
     np.testing.assert_allclose(vo_interp[0], vo_truth)
 
     # Constant time
     xi = xxi[0, 0, 0:1, :]  # (nyix=1,nxi)
     yi = yyi[0, 0, :, 0:1]  # (nyi,nxiy=1)
     zi = zzi[0:1, 0:1, :, 0:1, 0:1]  # (ntiz=1,nzi,nyiz=1,nxiz=1)
     ti = tti[:1, 0, 0, 0]  # (1)
     vi = vfunc(tti, zzi, yyi, xxi)[:, :1, :, :, :]
-    vi = np.resize(vi, (nex, )+vi.shape[1:])  # (nex,1,nzi,nyi,nxi)
+    vi = np.resize(vi, (nex,) + vi.shape[1:])  # (nex,1,nzi,nyi,nxi)
     vo_truth = vfunc(ti, zo, yo, xo)
     vo_interp = interp.grid2locs(xi, yi, zi, ti, vi, xo, yo, zo, to)
     vo_truth[np.isnan(vo_interp[0])] = np.nan
     np.testing.assert_allclose(vo_interp[0], vo_truth)
 
     # Variable depth with 1D X/Y + T
     xi = xxi[0, 0, 0:1, :]  # (nyix=1,nxi)
     yi = yyi[0, 0, :, 0:1]  # (nyi,nxiy=1)
     zi = zzi[:, :, :, :, :]  # (nexz,ntiz=nti,nzi,nyiz=nyi,nxiz=nxi)
     ti = tti[:, 0, 0, 0]  # (nti)
     vi = vfunc(tti, zzi, yyi, xxi)
-    vi = np.resize(vi, (nex, )+vi.shape[1:])  # (nex,nti,nzi,nyi,nxi)
+    vi = np.resize(vi, (nex,) + vi.shape[1:])  # (nex,nti,nzi,nyi,nxi)
     vo_truth = vfunc(to, zo, yo, xo)
     vo_interp = interp.grid2locs(xi, yi, zi, ti, vi, xo, yo, zo, to)
     vo_truth[np.isnan(vo_interp[0])] = np.nan
     np.testing.assert_allclose(vo_interp[0], vo_truth)
 
     # 2D X/Y with no other axes (pure curvilinear)
     xi = xxi[0, 0]  # (nyix=nyi,nxi)
     yi = yyi[0, 0]  # (nyi,nxiy=nxi)
     zi = zzi[0:1, 0:1, 0:1, 0:1, 0:1]  # (nexz=1,ntiz=1,1,nyiz=1,nxiz=1)
     ti = tti[:1, 0, 0, 0]  # (1)
     vi = vfunc(tti, zzi, yyi, xxi)[:, :1, :1, :, :]
-    vi = np.resize(vi, (nex, )+vi.shape[1:])  # (nex,1,1,nyi,nxi)
+    vi = np.resize(vi, (nex,) + vi.shape[1:])  # (nex,1,1,nyi,nxi)
     vo_interp = interp.grid2locs(xi, yi, zi, ti, vi, xo, yo, zo, to)
-    vo_interp_rect = interp.grid2locs(
-        xi[:1], yi[:, :1], zi, ti, vi, xo, yo, zo, to)
+    vo_interp_rect = interp.grid2locs(xi[:1], yi[:, :1], zi, ti, vi, xo, yo, zo, to)
     vo_truth = vfunc(ti, zi.ravel()[0], yo, xo)
     vo_truth[np.isnan(vo_interp[0])] = np.nan
     np.testing.assert_allclose(vo_interp[0], vo_truth)
     vo_truth = vfunc(ti, zi.ravel()[0], yo, xo)
     vo_truth[np.isnan(vo_interp_rect[0])] = np.nan
     np.testing.assert_allclose(vo_interp_rect[0], vo_truth)
 
     # Same coordinates
     xi = xxi[0, 0, 0:1, :]  # (nyix=1,nxi)
     yi = yyi[0, 0, :, 0:1]  # (nyi,nxiy=1)
     zi = zzi[0:1, 0:1, :, 0:1, 0:1]  # (nexz=1,ntiz=1,nzi,nyiz=1,nxiz=1)
     ti = tti[:, 0, 0, 0]  # (nti)
     vi = vfunc(tti, zzi, yyi, xxi)
-    vi = np.resize(vi, (nex, )+vi.shape[1:])  # (nex,nti,nzi,nyi,nxi)
+    vi = np.resize(vi, (nex,) + vi.shape[1:])  # (nex,nti,nzi,nyi,nxi)
     tzyxo = np.meshgrid(ti, zi, yi, xi, indexing='ij')
     xo = tzyxo[3].ravel()
     yo = tzyxo[2].ravel()
     zo = tzyxo[1].ravel()
     to = tzyxo[0].ravel()
     vo_truth = vfunc(to, zo, yo, xo)
     vo_interp = interp.grid2locs(xi, yi, zi, ti, vi, xo, yo, zo, to)
     vo_truth[np.isnan(vo_interp[0])] = np.nan
     np.testing.assert_allclose(vo_interp[0], vo_truth)
+
+
+def test_interp_isoslice():
+
+    depth = np.linspace(-50, 0.0, 6)
+    values = np.linspace(10, 20.0, 6)
+    isoval = 15.0
+
+    isodepth = interp.isoslice(depth, values, isoval, False)
+    assert isodepth == -25.0
+    isodepth = interp.isoslice(depth, values, isoval, True)
+    assert isodepth == -25.0
+
+    depth = np.resize(depth, (2,) + depth.shape)
+    isodepth = interp.isoslice(depth, values, isoval, False)
+    np.testing.assert_allclose(isodepth, [-25.0, -25.0])
```

### Comparing `xoa-0.6.1/xoa/tests/test_misc.py` & `xoa-0.7.0/xoa/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `xoa-0.6.1/xoa/tests/test_regrid.py` & `xoa-0.7.0/xoa/tests/test_regrid.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from xoa import regrid
 from test_interp import get_grid2locs_coords, vfunc, get_interp1d_data
 
 
 def test_regrid_regrid1d():
 
     # Get some data
-    xxi, yyi, vari, xxo, yyo = get_interp1d_data()
+    xxi, yyi, vari, xxo, yyo, eshapes = get_interp1d_data()
 
     # Some inits
     nz1 = xxo.shape[1]
     nx, nz0 = xxi.shape
     nt = 2
     dep0 = xr.DataArray(yyi[0], dims='nz', name='nz')
     dep1 = xr.DataArray(yyo[0], dims='nk', name='nk')
@@ -50,18 +50,25 @@
     da_in = da_in.assign_coords({"time": time, "lon": lon, "depth": depth_in})
     da_out = regrid.regrid1d(da_in, depth_out, method="linear")
     assert da_out.dims == ('time', "lon", "nk")
     assert "depth" in da_out.coords
     assert not np.isnan(da_out).all()
 
     # same but transposed
-    da_in = da_in.transpose("time", "nz", "lon")
-    da_out = regrid.regrid1d(da_in, depth_out, method="linear")
-    assert da_out.dims == ('time', "nk", "lon")
-    assert not np.isnan(da_out).all()
+    da_in_t = da_in.transpose("time", "nz", "lon")
+    da_out_t = regrid.regrid1d(da_in_t, depth_out, method="linear")
+    assert da_out_t.dims == ('time', "nk", "lon")
+    assert not np.isnan(da_out_t).all()
+
+    # now we remove/add some dims
+    depth_in_ed = da_in_t.depth.broadcast_like(da_in_t).isel(lon=0).drop("lon")
+    da_in_ed = da_in_t.assign_coords({"depth": depth_in_ed})
+    da_out_ed = regrid.regrid1d(da_in_ed, depth_out, method="linear")
+    assert da_out_ed.dims == ('time', "nk", "lon")
+    np.testing.assert_allclose(da_out_ed.isel(lon=0), da_out_t.isel(lon=0))
 
 
 def test_regrid_regrid1d_time():
     time_in = xr.DataArray(np.arange("2000-01-01", "2000-01-03", dtype="M8[D]"), dims="time")
     data_in = xr.DataArray(np.arange(time_in.size), coords={"time": time_in})
     time_out = xr.DataArray(np.arange("2000-01-01", "2000-01-03", dtype="M8[h]"), dims="time")
     data_out = regrid.regrid1d(data_in, time_out)
@@ -80,15 +87,14 @@
         [-1, [1, 1, np.nan]],
         ['top', [np.nan, 1, 1]],
         ['both', [1, 1, 1]],
     ],
 )
 def test_regrid_extrap1d(mode, expected):
     nz, ny, nx = 4, 3, 5
-    zi = np.linspace(3, 10, nz)
     zi = xr.DataArray(np.arange(nz), dims="z")
     vi = xr.DataArray(np.ones((nz, ny, nx)), dims=('z', 'y', 'x'), coords={"z": zi})
     vi[:, 0] = np.nan
     vi[:, -1] = np.nan
     vi.attrs["long_name"] = "Long name"
     vi.name = "toto"
     vo = regrid.extrap1d(vi, "y", mode)
@@ -140,7 +146,28 @@
     assert vo_interp.dims == ("member", "time")
     assert "time" in vo_interp.coords
     assert "lon" in vo_interp.coords
     assert "member" in vo_interp.coords
     vo_truth[np.isnan(vo_interp[0].values)] = np.nan
     np.testing.assert_almost_equal(vo_interp[0], vo_truth)
     assert "long_name" in vo_interp.attrs
+
+
+def test_regrid_isoslice():
+
+    depth = xr.DataArray(np.linspace(-50, 0.0, 6), dims="z", attrs={"long_name": "Depth"})
+    values = xr.DataArray(np.linspace(10, 20.0, 6), dims="z")
+    isoval = 15.0
+
+    isodepth = regrid.isoslice(depth, values, isoval, "z")
+    assert isodepth == -25.0
+    assert isodepth.long_name == "Depth"
+
+    depth = np.resize(depth, (2,) + depth.shape).T
+    values = np.resize(values, (2,) + values.shape).T
+    depth = xr.DataArray(depth, dims=("z", "x"))
+    values = xr.DataArray(values, dims=("z", "x"))
+    isoval = xr.DataArray([15.0, 15.0], dims="x")
+    isodepth = regrid.isoslice(depth, values, isoval, "z")
+    np.testing.assert_allclose(isodepth, [-25.0, -25.0])
+    assert isodepth.dims == ("x",)
+    assert isodepth.shape == (2,)
```

### Comparing `xoa-0.6.1/xoa.egg-info/PKG-INFO` & `xoa-0.7.0/xoa.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: xoa
-Version: 0.6.1
+Version: 0.7.0
 Summary: xarray-based ocean analysis library
 Home-page: https://github.com/vacumm/xoa
 Author: Shom
 Author-email: stephane.raynaud@shom.fr
 License: Apache
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -21,53 +20,68 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 xoa - xarray-based ocean analysis library
 =========================================
 
-.. image:: https://anaconda.org/conda-forge/xoa/badges/installer/conda.svg
-    :alt: Install with conda
-    :target: https://conda.anaconda.org/conda-forge
-.. image:: https://github.com/VACUMM/xoa/actions/workflows/python-package-conda.yml/badge.svg
+.. image:: https://github.com/shom-fr/xoa/actions/workflows/python-package-conda.yml/badge.svg
     :alt: Install, linting and tests
+.. image:: https://anaconda.org/conda-forge/xoa/badges/version.svg
+    :alt: Available on conda-forge
+    :target: https://conda.anaconda.org/conda-forge/xoa
 .. image:: https://readthedocs.org/projects/docs/badge/?version=latest
     :alt: Documentation Status
     :target: https://xoa.readthedocs.io/en/latest/
 .. image:: https://anaconda.org/conda-forge/xoa/badges/downloads.svg
     :alt: Number of downloads on anaconda.org/conda-forge
     :target: https://anaconda.org/conda-forge/xoa/
 .. image:: https://pepy.tech/badge/xoa
     :alt: Number of downloads on pypi
     :target: https://pypi.org/project/xoa
+.. image:: https://anaconda.org/conda-forge/xoa/badges/platforms.svg
+    :alt: noarch
+    :target: https://anaconda.org/conda-forge/xoa
+.. image:: https://anaconda.org/conda-forge/xoa/badges/license.svg
+    :alt: Apache 2.0
+    :target: https://anaconda.org/conda-forge/xoa
 
 xoa is intended to help reading and manipulating observed
 and simulated ocean data.
 It is heavily based on `xarray <http://xarray.pydata.org/en/stable/>`_.
 For those who know it, it is the successor of
 `vacumm <https://github.com/VACUMM/vacumm>`_.
 
+Installation
+------------
+
+From conda::
+
+   conda install -c conda-forge xoa
+
+From pypi::
+
+   pip install xoa
+
 Documentation
 -------------
 
 The xoa documentation is currently generated and hosted by readthedocs:
 https://xoa.readthedocs.io
 
 Sources and help
 -----------------
 
 Sources are available on the xoa github page:
-https://github.com/VACUMM/xoa.
+https://github.com/shom-fr/xoa.
 Here you can also
-participate to `discussions <https://github.com/VACUMM/xoa/discussions>`_
+participate to `discussions <https://github.com/shom-fr/xoa/discussions>`_
 and post tickets for
-`requests <https://github.com/VACUMM/xoa/pulls>`_ and
-`issues <https://github.com/VACUMM/xoa/issues>`_.
+`requests <https://github.com/shom-fr/xoa/pulls>`_ and
+`issues <https://github.com/shom-fr/xoa/issues>`_.
 
 License
 -------
 
 xoa is a property of `Shom <https://www.shom.fr>`_
 and is published under the
 `Apache 2.0 license <https://www.apache.org/licenses/LICENSE-2.0>`_.
-
-
```

### Comparing `xoa-0.6.1/xoa.egg-info/SOURCES.txt` & `xoa-0.7.0/xoa.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 MANIFEST.in
 README.rst
 ROADMAP.rst
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
+.github/ISSUE_TEMPLATE.md
+.github/PULL_REQUEST_TEMPLATE.md
+.github/dependabot.yml
 .github/workflows/python-package-conda.yml
 .github/workflows/python-publish.yml
 bin/xoa
 doc/.nojekill
 doc/Makefile
 doc/accessors.rst
 doc/api.rst
@@ -61,17 +64,19 @@
 xoa/dyn.py
 xoa/filter.py
 xoa/geo.py
 xoa/grid.py
 xoa/interp.py
 xoa/krig.py
 xoa/misc.py
+xoa/num.py
 xoa/plot.py
 xoa/regrid.py
 xoa/sigma.py
+xoa/thermdyn.py
 xoa.egg-info/PKG-INFO
 xoa.egg-info/SOURCES.txt
 xoa.egg-info/dependency_links.txt
 xoa.egg-info/entry_points.txt
 xoa.egg-info/not-zip-safe
 xoa.egg-info/requires.txt
 xoa.egg-info/top_level.txt
@@ -94,8 +99,9 @@
 xoa/tests/test_dyn.py
 xoa/tests/test_filter.py
 xoa/tests/test_geo.py
 xoa/tests/test_grid.py
 xoa/tests/test_interp.py
 xoa/tests/test_misc.py
 xoa/tests/test_regrid.py
-xoa/tests/test_sigma.py
+xoa/tests/test_sigma.py
+xoa/tests/test_thermdyn.py
```

