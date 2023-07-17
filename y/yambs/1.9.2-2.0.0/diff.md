# Comparing `tmp/yambs-1.9.2.tar.gz` & `tmp/yambs-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.9.2.tar", last modified: Sat Jul  1 07:07:08 2023, max compression
+gzip compressed data, was "yambs-2.0.0.tar", last modified: Mon Jul 17 06:21:32 2023, max compression
```

## Comparing `yambs-1.9.2.tar` & `yambs-2.0.0.tar`

### file list

```diff
@@ -1,92 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.455123 yambs-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-01 07:05:50.000000 yambs-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-01 07:07:08.451123 yambs-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-07-01 07:05:50.000000 yambs-1.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-01 07:05:50.000000 yambs-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 07:07:08.455123 yambs-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-01 07:05:50.000000 yambs-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.443123 yambs-1.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-01 07:05:50.000000 yambs-1.9.2/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-01 07:05:50.000000 yambs-1.9.2/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/entry_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/targets_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/generate/variants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.451123 yambs-1.9.2/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-01 07:05:50.000000 yambs-1.9.2/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:07:08.447123 yambs-1.9.2/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 07:07:08.000000 yambs-1.9.2/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 06:20:21.000000 yambs-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-17 06:21:32.823221 yambs-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-17 06:20:21.000000 yambs-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-17 06:20:21.000000 yambs-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 06:21:32.823221 yambs-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-17 06:20:21.000000 yambs-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.815221 yambs-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-17 06:20:21.000000 yambs-2.0.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-17 06:20:21.000000 yambs-2.0.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.815221 yambs-2.0.0/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/includes/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/CommonConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/entry_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/targets_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/generate/variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.823221 yambs-2.0.0/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-17 06:20:21.000000 yambs-2.0.0/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:21:32.819221 yambs-2.0.0/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 06:21:32.000000 yambs-2.0.0/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.9.2/LICENSE` & `yambs-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/PKG-INFO` & `yambs-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.9.2
+Version: 2.0.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=9a21bcfc475707c132005e45f897b988
+    hash=002bf1ec758c597d37da825e56ca08c0
     =====================================
 -->
 
-# yambs ([1.9.2](https://pypi.org/project/yambs/))
+# yambs ([2.0.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -148,36 +148,53 @@
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mbs -h
 
-usage: mbs [-h] [--version] [-v] [-C DIR] {gen,native,uf2conv,noop} ...
+usage: mbs [-h] [--version] [-v] [-C DIR] {dist,gen,native,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
-  {gen,native,uf2conv,noop}
+  {dist,gen,native,uf2conv,noop}
                         set of available commands
+    dist                create a source distribution
     gen                 poll the source tree and generate any new build files
     native              generate build files for native-only target projects
-    uf2conv             Convert to UF2 or flash directly.
+    uf2conv             convert to UF2 or flash directly
     noop                command stub (does nothing)
 
 ```
 
 ## Sub-command Options
 
+### `dist`
+
+```
+$ ./venv3.11/bin/mbs dist -h
+
+usage: mbs dist [-h] [-c CONFIG] [-s]
+
+options:
+  -h, --help            show this help message and exit
+  -c CONFIG, --config CONFIG
+                        the path to the top-level configuration file (default:
+                        'yambs.yaml')
+  -s, --sources         set this flag to only capture source files
+
+```
+
 ### `gen`
 
 ```
 $ ./venv3.11/bin/mbs gen -h
 
 usage: mbs gen [-h] [-c CONFIG] [-i] [-w] [-s]
```

### Comparing `yambs-1.9.2/README.md` & `yambs-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=9a21bcfc475707c132005e45f897b988
+    hash=002bf1ec758c597d37da825e56ca08c0
     =====================================
 -->
 
-# yambs ([1.9.2](https://pypi.org/project/yambs/))
+# yambs ([2.0.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -125,36 +125,53 @@
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mbs -h
 
-usage: mbs [-h] [--version] [-v] [-C DIR] {gen,native,uf2conv,noop} ...
+usage: mbs [-h] [--version] [-v] [-C DIR] {dist,gen,native,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
-  {gen,native,uf2conv,noop}
+  {dist,gen,native,uf2conv,noop}
                         set of available commands
+    dist                create a source distribution
     gen                 poll the source tree and generate any new build files
     native              generate build files for native-only target projects
-    uf2conv             Convert to UF2 or flash directly.
+    uf2conv             convert to UF2 or flash directly
     noop                command stub (does nothing)
 
 ```
 
 ## Sub-command Options
 
+### `dist`
+
+```
+$ ./venv3.11/bin/mbs dist -h
+
+usage: mbs dist [-h] [-c CONFIG] [-s]
+
+options:
+  -h, --help            show this help message and exit
+  -c CONFIG, --config CONFIG
+                        the path to the top-level configuration file (default:
+                        'yambs.yaml')
+  -s, --sources         set this flag to only capture source files
+
+```
+
 ### `gen`
 
 ```
 $ ./venv3.11/bin/mbs gen -h
 
 usage: mbs gen [-h] [-c CONFIG] [-i] [-w] [-s]
```

### Comparing `yambs-1.9.2/pyproject.toml` & `yambs-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.9.2"
+version = "2.0.0"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.9.2/setup.py` & `yambs-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/tests/test_entry.py` & `yambs-2.0.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/aggregation/__init__.py` & `yambs-2.0.0/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/app.py` & `yambs-2.0.0/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/commands/all.py` & `yambs-2.0.0/yambs/commands/all.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=325e245e0e7b4e7366d426ca615de809
+# hash=f12a77b15954045668945389858afc26
 # =====================================
 
 """
 A module aggregating package commands.
 """
 
 # built-in
 from typing import List as _List
 from typing import Tuple as _Tuple
 
 # third-party
 from vcorelib.args import CommandRegister as _CommandRegister
 
 # internal
+from yambs.commands.dist import add_dist_cmd
 from yambs.commands.gen import add_gen_cmd
 from yambs.commands.native import add_native_cmd
 from yambs.commands.uf2conv import add_uf2conv_cmd
 
 
 def commands() -> _List[_Tuple[str, str, _CommandRegister]]:
     """Get this package's commands."""
 
     return [
         (
+            "dist",
+            "create a source distribution",
+            add_dist_cmd,
+        ),
+        (
             "gen",
             "poll the source tree and generate any new build files",
             add_gen_cmd,
         ),
         (
             "native",
             "generate build files for native-only target projects",
             add_native_cmd,
         ),
         (
             "uf2conv",
-            "Convert to UF2 or flash directly.",
+            "convert to UF2 or flash directly",
             add_uf2conv_cmd,
         ),
         ("noop", "command stub (does nothing)", lambda _: lambda _: 0),
     ]
```

### Comparing `yambs-1.9.2/yambs/commands/common.py` & `yambs-2.0.0/yambs/commands/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,27 +13,33 @@
 from rcmpy.watch.params import WatchParams
 
 # internal
 from yambs import PKG_NAME
 from yambs.config.common import DEFAULT_CONFIG
 
 
-def add_common_args(parser: _ArgumentParser) -> None:
-    """Add common command-line arguments to a parser."""
+def add_config_arg(parser: _ArgumentParser) -> None:
+    """Add an argument for specifying a configuration file."""
 
     parser.add_argument(
         "-c",
         "--config",
         type=_Path,
         default=DEFAULT_CONFIG,
         help=(
             "the path to the top-level configuration "
             "file (default: '%(default)s')"
         ),
     )
+
+
+def add_common_args(parser: _ArgumentParser) -> None:
+    """Add common command-line arguments to a parser."""
+
+    add_config_arg(parser)
     parser.add_argument(
         "-i",
         "--single-pass",
         action="store_true",
         help="only run a single watch iteration",
     )
     parser.add_argument(
```

### Comparing `yambs-1.9.2/yambs/commands/gen.py` & `yambs-2.0.0/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/commands/native.py` & `yambs-2.0.0/yambs/commands/native.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 from argparse import Namespace as _Namespace
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
 
 # internal
 from yambs.commands.common import add_common_args, run_watch
-from yambs.config.native import Native
+from yambs.config.native import load_native
 from yambs.environment.native import NativeBuildEnvironment
 
 
 def native_cmd(args: _Namespace) -> int:
     """Execute the native command."""
 
-    config = Native.load(
-        path=args.config, root=args.dir, package_config="native.yaml"
-    )
+    config = load_native(path=args.config, root=args.dir)
 
     NativeBuildEnvironment(config).generate(sources_only=args.sources)
 
     return run_watch(args, config.src_root, "native")
 
 
 def add_native_cmd(parser: _ArgumentParser) -> _CommandFunction:
```

### Comparing `yambs-1.9.2/yambs/commands/uf2conv.py` & `yambs-2.0.0/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/config/__init__.py` & `yambs-2.0.0/yambs/config/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 
 # internal
 from yambs.config.board import Board
 from yambs.config.common import CommonConfig
-from yambs.schemas import YambsDictCodec as _YambsDictCodec
 
 
-class Config(_YambsDictCodec, CommonConfig):
+class Config(CommonConfig):
     """The top-level configuration object for the package."""
 
     board_data: List[Board]
     boards_by_name: Dict[str, Board]
 
     def init(self, data: _JsonObject) -> None:
         """Initialize this instance."""
```

### Comparing `yambs-1.9.2/yambs/config/board.py` & `yambs-2.0.0/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/config/common.py` & `yambs-2.0.0/yambs/dist/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,65 @@
 """
-A module for common configuration interfaces.
+A module implementing interfaces for facilitating project distribution.
 """
 
 # built-in
 from pathlib import Path
-from typing import Any, Dict, Type, TypeVar
+from shutil import copy2, copytree, make_archive
 
 # third-party
-from vcorelib.dict import merge
-from vcorelib.dict.codec import BasicDictCodec as _BasicDictCodec
-from vcorelib.io import ARBITER as _ARBITER
-from vcorelib.io import DEFAULT_INCLUDES_KEY
-from vcorelib.io.types import JsonObject as _JsonObject
-from vcorelib.paths import Pathlike, find_file, normalize
+from vcorelib.paths.context import in_dir
 
 # internal
-from yambs import PKG_NAME
+from yambs.config.common import CommonConfig
 
-T = TypeVar("T", bound="CommonConfig")
-DEFAULT_CONFIG = f"{PKG_NAME}.yaml"
-
-
-class CommonConfig(_BasicDictCodec):
-    """A common, base configuration."""
-
-    data: Dict[str, Any]
-
-    root: Path
-    src_root: Path
-    build_root: Path
-    ninja_root: Path
-
-    def directory(self, name: str, mkdir: bool = True) -> Path:
-        """Get a configurable directory."""
-
-        name_root = Path(str(self.data[name]))
-        if not name_root.is_absolute():
-            name_root = self.root.joinpath(name_root)
-
-        if mkdir:
-            name_root.mkdir(parents=True, exist_ok=True)
-
-        return name_root
-
-    def init(self, data: _JsonObject) -> None:
-        """Initialize this instance."""
-
-        self.data = data
-        self.root = Path()
-
-        self.src_root = self.directory("src_root")
-        self.build_root = self.directory("build_root")
-        self.ninja_root = self.directory("ninja_out")
-
-    @classmethod
-    def load(
-        cls: Type[T],
-        path: Pathlike = DEFAULT_CONFIG,
-        package_config: str = DEFAULT_CONFIG,
-        root: Pathlike = None,
-    ) -> T:
-        """Load a configuration."""
-
-        src_config = find_file(package_config, package=PKG_NAME)
-        assert src_config is not None
-
-        data = merge(
-            _ARBITER.decode(
-                src_config,
-                includes_key=DEFAULT_INCLUDES_KEY,
-                require_success=True,
-            ).data,
-            _ARBITER.decode(path, includes_key=DEFAULT_INCLUDES_KEY).data,
-            # Always allow the project-specific configuration to override
-            # package data.
-            expect_overwrite=True,
-        )
-
-        result = cls.create(data)
-
-        if root is not None:
-            result.root = normalize(root)
-            result.root.mkdir(parents=True, exist_ok=True)
-
-        return result
+ARCHIVES = [
+    ("tar.gz", "gztar"),
+    ("tar.xz", "xztar"),
+    ("zip", "zip"),
+]
+
+
+def make_archives(tmp: Path, config: CommonConfig) -> None:
+    """Create a distribution that only contains sources."""
+
+    slug = str(config.project)
+
+    for ext, kind in ARCHIVES:
+        out = tmp.joinpath(f"{slug}.{ext}")
+        out.unlink(missing_ok=True)
+
+        with in_dir(tmp):
+            make_archive(slug, kind)
+
+        assert out.is_file(), out
+
+        final = config.dist_root.joinpath(out.name)
+        copy2(out, final.resolve())
+        out.unlink()
+
+        print(f"Created '{final}'.")
+
+
+def copy_source_tree(config: CommonConfig, dest: Path) -> None:
+    """
+    Copy necessary parts of the project source tree to some destination
+    directory.
+    """
+
+    root = config.root
+
+    for item in [
+        x
+        for x in [
+            config.src_root,
+            config.ninja_root,
+            root.joinpath("build.ninja"),
+            config.file,
+        ]
+        + [root.joinpath(x) for x in config.data.get("extra_dist", [])]
+        if x and x.exists()
+    ]:
+        if item.is_dir():
+            copytree(item, dest.joinpath(item.name))
+        else:
+            copy2(item, dest.joinpath(item.name))
```

### Comparing `yambs-1.9.2/yambs/data/includes/chips.yaml` & `yambs-2.0.0/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/data/includes/infineon.yaml` & `yambs-2.0.0/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/data/includes/microchip.yaml` & `yambs-2.0.0/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/data/schemas/Chip.yaml` & `yambs-2.0.0/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/data/schemas/Config.yaml` & `yambs-2.0.0/yambs/data/schemas/Config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -39,7 +39,12 @@
 
   architectures:
     type: object
     additionalProperties: false
     patternProperties:
       "^[a-zA-Z0-9-_.+]+$":
         $ref: package://yambs/schemas/Architecture.yaml
+
+  extra_third_party:
+    type: array
+    items:
+      type: string
```

### Comparing `yambs-1.9.2/yambs/data/schemas/Native.yaml` & `yambs-2.0.0/yambs/data/schemas/Native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/data/templates/rules.ninja.j2` & `yambs-2.0.0/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/data/uf2families.json` & `yambs-2.0.0/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/entry.py` & `yambs-2.0.0/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/environment/__init__.py` & `yambs-2.0.0/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/environment/native.py` & `yambs-2.0.0/yambs/environment/native.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # internal
 from yambs.aggregation import collect_files, populate_sources, sources_headers
 from yambs.config.native import Native
 from yambs.generate.common import get_jinja, render_template
 from yambs.generate.ninja import write_continuation
 from yambs.generate.ninja.format import render_format
 from yambs.generate.variants import generate as generate_variants
-from yambs.translation import BUILD_DIR_VAR, get_translator
+from yambs.translation import BUILD_DIR_PATH, get_translator
 
 
 def resolve_build_dir(build_root: Path, variant: str, path: Path) -> Path:
     """Resolve the build-directory variable in a path."""
-    return build_root.joinpath(variant, path.relative_to(BUILD_DIR_VAR))
+    return build_root.joinpath(variant, path.relative_to(BUILD_DIR_PATH))
 
 
 class NativeBuildEnvironment(LoggerMixin):
     """A class implementing a native-build environment."""
 
     def __init__(self, config: Native) -> None:
         """Initialize this instance."""
@@ -67,26 +67,46 @@
 
         return out
 
     def write_source_rules(self, stream: TextIO) -> Set[Path]:
         """Write source rules."""
         return {self.write_compile_line(stream, path) for path in self.regular}
 
+    def write_static_library_rule(
+        self, stream: TextIO, outputs: Set[Path]
+    ) -> Path:
+        """Create a rule for a static library output."""
+
+        lib = BUILD_DIR_PATH.joinpath(f"{self.config.project}.a")
+        line = f"build {lib}: ar "
+        offset = " " * len(line)
+
+        list_outputs = list(outputs)
+        stream.write(line + str(list_outputs[0]))
+        for file in list_outputs[1:]:
+            write_continuation(stream, offset)
+            stream.write(str(file))
+
+        stream.write(linesep + linesep)
+
+        return lib
+
     def write_app_rules(
         self, stream: TextIO, outputs: Set[Path]
     ) -> Dict[Path, Path]:
         """Write app rules."""
 
         elfs: Dict[Path, Path] = {}
 
+        # Create rules for linked executables.
         for path in self.apps:
             out = self.write_compile_line(stream, path)
 
             from_src = path.relative_to(self.config.src_root)
-            elf = Path(BUILD_DIR_VAR, from_src.with_suffix(".elf"))
+            elf = BUILD_DIR_PATH.joinpath(from_src.with_suffix(".elf"))
             elfs[path] = elf
             line = f"build {elf}: link "
             offset = " " * len(line)
 
             stream.write(line + str(out))
 
             for file in outputs:
@@ -95,14 +115,20 @@
 
             stream.write(linesep + linesep)
 
         line = "build ${variant}_apps: phony "
         offset = " " * len(line)
 
         elfs_list = list(elfs.values())
+
+        # Also update the static library (if necessary) when linking
+        # applications.
+        if outputs:
+            elfs_list.append(self.write_static_library_rule(stream, outputs))
+
         stream.write(line + str(elfs_list[0]))
         for elf in elfs_list[1:]:
             write_continuation(stream, offset)
             stream.write(str(elf))
         stream.write(linesep)
 
         return elfs
```

### Comparing `yambs-1.9.2/yambs/generate/__init__.py` & `yambs-2.0.0/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/generate/architectures.py` & `yambs-2.0.0/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/generate/boards.py` & `yambs-2.0.0/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/generate/chips.py` & `yambs-2.0.0/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/generate/common.py` & `yambs-2.0.0/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/generate/ninja/__init__.py` & `yambs-2.0.0/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/generate/ninja/format.py` & `yambs-2.0.0/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/generate/toolchains.py` & `yambs-2.0.0/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/generate/variants.py` & `yambs-2.0.0/yambs/generate/variants.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/schemas.py` & `yambs-2.0.0/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs/translation/__init__.py` & `yambs-2.0.0/yambs/translation/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # built-in
 from functools import lru_cache
 from pathlib import Path
 from typing import NamedTuple, Optional
 
 HEADER_EXTENSIONS = {".h", ".hpp"}
 BUILD_DIR_VAR = "$build_dir"
+BUILD_DIR_PATH = Path(BUILD_DIR_VAR)
 
 
 class SourceTranslator(NamedTuple):
     """
     A structure for keeping track of how source files become different types
     of output files.
     """
```

### Comparing `yambs-1.9.2/yambs/uf2/__init__.py` & `yambs-2.0.0/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.9.2/yambs.egg-info/PKG-INFO` & `yambs-2.0.0/yambs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.9.2
+Version: 2.0.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=9a21bcfc475707c132005e45f897b988
+    hash=002bf1ec758c597d37da825e56ca08c0
     =====================================
 -->
 
-# yambs ([1.9.2](https://pypi.org/project/yambs/))
+# yambs ([2.0.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -148,36 +148,53 @@
 following a specific convention), put your configuration data here.
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/mbs -h
 
-usage: mbs [-h] [--version] [-v] [-C DIR] {gen,native,uf2conv,noop} ...
+usage: mbs [-h] [--version] [-v] [-C DIR] {dist,gen,native,uf2conv,noop} ...
 
 Yet another meta build-system.
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
-  {gen,native,uf2conv,noop}
+  {dist,gen,native,uf2conv,noop}
                         set of available commands
+    dist                create a source distribution
     gen                 poll the source tree and generate any new build files
     native              generate build files for native-only target projects
-    uf2conv             Convert to UF2 or flash directly.
+    uf2conv             convert to UF2 or flash directly
     noop                command stub (does nothing)
 
 ```
 
 ## Sub-command Options
 
+### `dist`
+
+```
+$ ./venv3.11/bin/mbs dist -h
+
+usage: mbs dist [-h] [-c CONFIG] [-s]
+
+options:
+  -h, --help            show this help message and exit
+  -c CONFIG, --config CONFIG
+                        the path to the top-level configuration file (default:
+                        'yambs.yaml')
+  -s, --sources         set this flag to only capture source files
+
+```
+
 ### `gen`
 
 ```
 $ ./venv3.11/bin/mbs gen -h
 
 usage: mbs gen [-h] [-c CONFIG] [-i] [-w] [-s]
```

### Comparing `yambs-1.9.2/yambs.egg-info/SOURCES.txt` & `yambs-2.0.0/yambs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,33 @@
 yambs.egg-info/entry_points.txt
 yambs.egg-info/requires.txt
 yambs.egg-info/top_level.txt
 yambs/aggregation/__init__.py
 yambs/commands/__init__.py
 yambs/commands/all.py
 yambs/commands/common.py
+yambs/commands/dist.py
 yambs/commands/gen.py
 yambs/commands/native.py
 yambs/commands/uf2conv.py
 yambs/config/__init__.py
 yambs/config/board.py
 yambs/config/common.py
 yambs/config/native.py
 yambs/data/native.yaml
 yambs/data/uf2families.json
 yambs/data/yambs.yaml
 yambs/data/includes/chips.yaml
+yambs/data/includes/common.yaml
 yambs/data/includes/infineon.yaml
 yambs/data/includes/microchip.yaml
 yambs/data/schemas/Architecture.yaml
 yambs/data/schemas/Board.yaml
 yambs/data/schemas/Chip.yaml
+yambs/data/schemas/CommonConfig.yaml
 yambs/data/schemas/Config.yaml
 yambs/data/schemas/Native.yaml
 yambs/data/schemas/Toolchain.yaml
 yambs/data/schemas/Variant.yaml
 yambs/data/schemas/config_common.yaml
 yambs/data/schemas/entry_common.yaml
 yambs/data/schemas/targets_common.yaml
@@ -55,14 +58,15 @@
 yambs/data/templates/compile_commands.ninja.j2
 yambs/data/templates/native_all.ninja.j2
 yambs/data/templates/native_build.ninja.j2
 yambs/data/templates/native_rules.ninja.j2
 yambs/data/templates/rules.ninja.j2
 yambs/data/templates/toolchain.ninja.j2
 yambs/data/templates/variant.ninja.j2
+yambs/dist/__init__.py
 yambs/environment/__init__.py
 yambs/environment/native.py
 yambs/generate/__init__.py
 yambs/generate/architectures.py
 yambs/generate/boards.py
 yambs/generate/chips.py
 yambs/generate/common.py
```

