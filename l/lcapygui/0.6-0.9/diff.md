# Comparing `tmp/lcapygui-0.6.tar.gz` & `tmp/lcapygui-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcapygui-0.6.tar", last modified: Tue Apr 11 21:09:29 2023, max compression
+gzip compressed data, was "lcapygui-0.9.tar", last modified: Mon Jul 17 20:22:56 2023, max compression
```

## Comparing `lcapygui-0.6.tar` & `lcapygui-0.9.tar`

### file list

```diff
@@ -1,80 +1,95 @@
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.452365 lcapygui-0.6/
--rw-rw-r--   0 mph       (1000) mph       (1000)      933 2023-04-11 21:09:29.452365 lcapygui-0.6/PKG-INFO
--rw-rw-r--   0 mph       (1000) mph       (1000)      361 2023-04-11 21:09:29.000000 lcapygui-0.6/README.md
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.448365 lcapygui-0.6/lcapygui/
--rw-rw-r--   0 mph       (1000) mph       (1000)      567 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      443 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/annotation.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      246 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/annotations.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.448365 lcapygui-0.6/lcapygui/components/
--rw-rw-r--   0 mph       (1000) mph       (1000)       99 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       89 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/admittance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      620 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/annotation.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      169 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/bipole.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      641 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/bjt.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       88 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/capacitor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/cccs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/ccvs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    12801 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/component.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3762 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/connection.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      177 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/controlledcomponent.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      107 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/cpe.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3368 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/cpt_maker.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/current_source.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      758 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/diode.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      136 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/ferritebead.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       88 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/impedance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       87 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/inductor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      215 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/jfet.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1610 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/mosfet.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3953 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/opamp.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      188 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/opencircuit.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      132 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/port.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      110 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/resistor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4522 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/sketch.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3342 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/svgparse.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1401 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/transistor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/vccs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/vcvs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/voltage_source.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      365 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/components/wire.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1237 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/node.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1842 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/nodes.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.448365 lcapygui-0.6/lcapygui/scripts/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/scripts/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1621 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/scripts/lcapytk.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.448365 lcapygui-0.6/lcapygui/ui/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1825 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/preferences.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.452365 lcapygui-0.6/lcapygui/ui/tk/
--rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2939 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/cpt_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4648 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/cpt_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1800 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/drawing.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1390 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/equations_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4003 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/expr_advanced_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1798 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/expr_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      187 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/exprimage.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1760 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/help_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1206 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/inspect_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2239 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/labelentries.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      846 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/lateximage.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    19504 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/lcapytk.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     9431 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/lcapytkm.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      251 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/message_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      907 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/node_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      788 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/plot_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2323 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/plot_properties_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4324 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/preferences_dialog.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4078 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/tk/sketcher.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    20204 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/uimodelbase.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    15207 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui/ui/uimodelmph.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-04-11 21:09:29.448365 lcapygui-0.6/lcapygui.egg-info/
--rw-rw-r--   0 mph       (1000) mph       (1000)      933 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/PKG-INFO
--rw-rw-r--   0 mph       (1000) mph       (1000)     2123 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/SOURCES.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)        1 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/dependency_links.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)       60 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/entry_points.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)      150 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/requires.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)        9 2023-04-11 21:09:29.000000 lcapygui-0.6/lcapygui.egg-info/top_level.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)      103 2023-04-11 21:09:29.000000 lcapygui-0.6/pyproject.toml
--rw-rw-r--   0 mph       (1000) mph       (1000)      287 2023-04-11 21:09:29.452365 lcapygui-0.6/setup.cfg
--rw-rw-r--   0 mph       (1000) mph       (1000)     1348 2023-04-11 21:09:29.000000 lcapygui-0.6/setup.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:22:56.697250 lcapygui-0.9/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      933 2023-07-17 20:22:56.697250 lcapygui-0.9/PKG-INFO
+-rw-rw-r--   0 mph       (1000) mph       (1000)      361 2023-07-17 20:22:56.000000 lcapygui-0.9/README.md
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:22:56.693250 lcapygui-0.9/lcapygui/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      567 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      443 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/annotation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      246 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/annotations.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:22:56.693250 lcapygui-0.9/lcapygui/components/
+-rw-rw-r--   0 mph       (1000) mph       (1000)       99 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       89 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/admittance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      620 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/annotation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      341 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/bipole.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      641 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/bjt.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      315 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/capacitor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/cccs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      162 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/ccvs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    13524 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/component.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3762 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/connection.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      177 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/controlledcomponent.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      107 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/cpe.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3368 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/cpt_maker.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/current_source.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      510 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/diode.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      136 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/ferritebead.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       88 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/impedance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      283 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/inductor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      215 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/jfet.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1610 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/mosfet.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3962 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/opamp.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      188 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/opencircuit.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      132 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/port.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      216 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/resistor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4522 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/sketch.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3342 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/svgparse.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1401 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/transistor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/vccs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      104 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/vcvs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      331 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/voltage_source.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      365 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/components/wire.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1237 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/node.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1842 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/nodes.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:22:56.697250 lcapygui-0.9/lcapygui/scripts/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/scripts/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1878 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/scripts/lcapytk.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:22:56.697250 lcapygui-0.9/lcapygui/ui/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1825 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/preferences.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:22:56.697250 lcapygui-0.9/lcapygui/ui/tk/
+-rw-rw-r--   0 mph       (1000) mph       (1000)        0 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1220 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/approximate_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2939 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/cpt_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4980 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/cpt_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1800 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/drawing.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      768 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/edit_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2693 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/edit_values_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1390 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/equations_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      716 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/expr_attributes_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      425 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/expr_calc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    12941 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/expr_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      187 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/exprimage.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1760 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/help_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1206 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/inspect_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2373 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/labelentries.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      846 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/lateximage.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    23079 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/lcapytk.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     9431 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/lcapytkm.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1174 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/limit_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2342 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/menu.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      251 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/message_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1631 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/multiplot_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      907 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/node_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      788 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/plot_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2323 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/plot_properties_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4324 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/preferences_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1679 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/python_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4078 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/sketcher.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2490 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/state_space_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1189 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/subs_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      892 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/transfer_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2011 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/transfer_function_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1448 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/twoport_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3864 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/twoport_select_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      435 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/tk/working_dialog.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    20476 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/uimodelbase.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    17327 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui/ui/uimodelmph.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2023-07-17 20:22:56.693250 lcapygui-0.9/lcapygui.egg-info/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      933 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui.egg-info/PKG-INFO
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2628 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui.egg-info/SOURCES.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)        1 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui.egg-info/dependency_links.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)       60 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui.egg-info/entry_points.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)      150 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui.egg-info/requires.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)        9 2023-07-17 20:22:56.000000 lcapygui-0.9/lcapygui.egg-info/top_level.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)      103 2023-07-17 20:22:56.000000 lcapygui-0.9/pyproject.toml
+-rw-rw-r--   0 mph       (1000) mph       (1000)      287 2023-07-17 20:22:56.697250 lcapygui-0.9/setup.cfg
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1348 2023-07-17 20:22:56.000000 lcapygui-0.9/setup.py
```

### Comparing `lcapygui-0.6/PKG-INFO` & `lcapygui-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcapygui
-Version: 0.6
+Version: 0.9
 Summary: A GUI for lcapy
 Home-page: https://github.com/mph-/lcapy-gui
 Author: Michael Hayes, Jordan Hay
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mph-/lcapy-gui
 Description: # lcapy-gui
```

### Comparing `lcapygui-0.6/lcapygui/__init__.py` & `lcapygui-0.9/lcapygui/__init__.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/components/annotation.py` & `lcapygui-0.9/lcapygui/components/annotation.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/components/bjt.py` & `lcapygui-0.9/lcapygui/components/bjt.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/components/component.py` & `lcapygui-0.9/lcapygui/components/component.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,32 @@
               'voltage_label': 'Voltage label',
               'current_label': 'Current label',
               'flow_label': 'Flow label',
               'color': 'Color',
               'attrs': 'Attributes'}
     extra_fields = {}
     has_value = True
-    netitem_args = ()
+
+    voltage_keys = ('v', 'v_', 'v^', 'v_>', 'v_<', 'v^>', 'v^<',
+                    'v<', 'v>')
+    current_keys = ('i', 'i_', 'i^', 'i_>',  'i_<', 'i^>', 'i^<',
+                    'i>_', 'i<_', 'i>^', 'i<^', 'i>', 'i<', 'ir')
+    flow_keys = ('f', 'f_', 'f^', 'f_>',  'f_<', 'f^>', 'f^<',
+                 'f>_', 'f<_', 'f>^', 'f<^', 'f>', 'f<')
+    label_keys = ('l', 'l_', 'l^')
+    annotation_keys = ('a', 'a_', 'a^')
+
+    # These are not passed to the sktecher.
+    ignore_keys = ('left', 'right', 'up', 'down', 'size', 'rotate',
+                   'pinnodes', 'pinnames', 'pins', 'pinlabels',
+                   'mirrorinputs', 'free', 'ignore', 'nosim', 'arrow',
+                   'startarrow', 'endarrow', 'bus', 'anchor', 'fixed')
+
+    all_keys = voltage_keys + current_keys + flow_keys + \
+        label_keys + annotation_keys + ignore_keys
 
     # TODO: add class methods to construct Component from
     # an Lcapy cpt or from a cpt type.
 
     def __init__(self, kind='', style='', name=None, nodes=None, opts=None):
 
         if nodes is None:
@@ -91,23 +108,18 @@
                 except:
                     self.scale = 1.0
             elif k == 'mirror':
                 self.mirror = True
             elif k == 'invert':
                 self.invert = True
             elif k == 'kind':
-                self.kind = '-' + v
+                self.kind += '-' + v
             elif k == 'style':
                 self.style = v
-            elif k in ('f', 'i', 'v'):
-                # TODO, handle labels.
-                pass
-            elif k in ('left', 'right', 'up', 'down', 'size', 'rotate',
-                       'pinnodes', 'pinnames', 'pins', 'pinlabels',
-                       'mirrorinputs'):
+            elif k in self.all_keys:
                 pass
             else:
                 if v == '':
                     parts.append(k)
                 else:
                     parts.append(k + '=' + v)
         self.attrs = ', '.join(parts)
@@ -450,14 +462,21 @@
     def netitem_nodes(self, node_names):
 
         parts = []
         for node_name in node_names:
             parts.append(node_name)
         return parts
 
+    @property
+    def netitem_args(self):
+
+        if self.cpt_kind == '':
+            return ()
+        return (self.cpt_kind, )
+
     def netitem(self, node_names, x1, y1, x2, y2, step=1):
 
         parts = [self.name]
         parts.extend(self.netitem_nodes(node_names))
         if self.type in ('E', 'G'):
             # Need to use known nodes to start with.
             parts.extend([node_names[0], node_names[1]])
```

### Comparing `lcapygui-0.6/lcapygui/components/connection.py` & `lcapygui-0.9/lcapygui/components/connection.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/components/cpt_maker.py` & `lcapygui-0.9/lcapygui/components/cpt_maker.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 class CptMaker:
 
     cpts = {
         'C': Capacitor,
         'CPE': CPE,
         'D': Diode,
         'E': VCVS,
-        'Opamp': Opamp,
+        'opamp': Opamp,
         'F': CCCS,
         'FB': FerriteBead,
         'G': VCCS,
         'H': CCVS,
         'I': CurrentSource,
         'J': JFET,
         'L': Inductor,
```

### Comparing `lcapygui-0.6/lcapygui/components/mosfet.py` & `lcapygui-0.9/lcapygui/components/mosfet.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/components/opamp.py` & `lcapygui-0.9/lcapygui/components/opamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .component import Component
-from numpy import array, sqrt
+from numpy import array, sqrt, nan
 from numpy.linalg import norm
 
 
 def point_in_triangle(x, y, x0, y0, x1, y1, x2, y2):
 
     s = (x0 - x2) * (y - y2) - (y0 - y2) * (x - x2)
     t = (x1 - x0) * (y - y0) - (y1 - y0) * (x - x0)
@@ -61,15 +61,15 @@
 
         # TODO: handle rotation
 
         xo = (x2 + x1) / 2 + r * 5 / 2
         yo = (y2 + y1) / 2
 
         positions = array(((xo, yo),
-                           (0, 0),
+                           (nan, nan),
                            (x1, y1),
                            (x1, y2)))
         return positions
 
     @property
     def midpoint(self):
```

### Comparing `lcapygui-0.6/lcapygui/components/sketch.py` & `lcapygui-0.9/lcapygui/components/sketch.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/components/svgparse.py` & `lcapygui-0.9/lcapygui/components/svgparse.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/components/transistor.py` & `lcapygui-0.9/lcapygui/components/transistor.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/node.py` & `lcapygui-0.9/lcapygui/node.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/nodes.py` & `lcapygui-0.9/lcapygui/nodes.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/scripts/lcapytk.py` & `lcapygui-0.9/lcapygui/scripts/lcapytk.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Usage: lcapy-tk [infile.sch]
 """
 
 from argparse import ArgumentParser
 import sys
 from lcapygui import LcapyTk
+from lcapy import expr as lcapify
 
 
 def schtex_exception(type, value, tb):
     if hasattr(sys, 'ps1') or not sys.stderr.isatty():
         # We are not in interactive mode or we don't have a tty-like
         # device, so call the default hook
         sys.__excepthook__(type, value, tb)
@@ -36,23 +37,30 @@
                         version=__doc__.split('\n')[0])
     parser.add_argument('--pdb', action='store_true',
                         default=False,
                         help="enter python debugger on exception")
     parser.add_argument('--debug', type=int,
                         dest='debug', default=None,
                         help="enable debugging")
+    parser.add_argument('--expr', type=str,
+                        dest='expr', default=None,
+                        help="Lcapy expression")
     parser.add_argument('filenames', type=str, nargs='*',
                         help='schematic filename(s)', default=[])
 
     args = parser.parse_args()
 
     if args.pdb:
         sys.excepthook = schtex_exception
 
     e = LcapyTk(args.filenames, debug=args.debug)
+
+    if args.expr is not None:
+        e.show_expr_dialog(lcapify(args.expr))
+
     e.display()
 
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `lcapygui-0.6/lcapygui/ui/preferences.py` & `lcapygui-0.9/lcapygui/ui/preferences.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/ui/tk/cpt_dialog.py` & `lcapygui-0.9/lcapygui/ui/tk/cpt_dialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,75 +5,75 @@
 class CptDialog:
 
     def __init__(self, cpt, update=None):
 
         self.cpt = cpt
         self.update = update
 
-        self.master = Tk()
-        self.master.title(cpt.name)
+        self.window = Tk()
+        self.window.title(cpt.name)
 
         row = 0
 
         self.kind_var = None
         if cpt.kind is not None:
-            self.kind_var = StringVar(self.master)
+            self.kind_var = StringVar(self.window)
             self.kind_var.set(cpt.kind)
 
-            kind_label = Label(self.master, text='Kind: ')
-            kind_option = OptionMenu(self.master, self.kind_var,
+            kind_label = Label(self.window, text='Kind: ')
+            kind_option = OptionMenu(self.window, self.kind_var,
                                      *cpt.kinds.keys())
 
             kind_label.grid(row=row)
             kind_option.grid(row=row, column=1)
             row += 1
 
-        self.name_var = StringVar(self.master)
+        self.name_var = StringVar(self.window)
         self.name_var.set(cpt.name)
 
-        name_label = Label(self.master, text='Name: ')
-        name_entry = Entry(self.master, textvariable=self.name_var,
+        name_label = Label(self.window, text='Name: ')
+        name_entry = Entry(self.window, textvariable=self.name_var,
                            command=self.on_update)
 
         name_label.grid(row=row)
         name_entry.grid(row=row, column=1)
         row += 1
 
-        self.value_var = StringVar(self.master)
+        self.value_var = StringVar(self.window)
         value = cpt.value
         if value is None:
             value = cpt.name
         self.value_var.set(value)
 
-        value_label = Label(self.master, text='Value: ')
-        value_entry = Entry(self.master, textvariable=self.value_var,
+        value_label = Label(self.window, text='Value: ')
+        value_entry = Entry(self.window, textvariable=self.value_var,
                             command=self.on_update)
 
         value_label.grid(row=row)
         value_entry.grid(row=row, column=1)
         row += 1
 
         self.initial_value_var = None
         if isinstance(cpt, (Capacitor, Inductor)):
 
             ivlabel = 'v0'
             if isinstance(cpt, Inductor):
                 ivlabel = 'i0'
 
-            self.initial_value_var = StringVar(self.master)
+            self.initial_value_var = StringVar(self.window)
 
-            initial_value_label = Label(self.master, text=ivlabel + ': ')
+            initial_value_label = Label(self.window, text=ivlabel + ': ')
             initial_value_entry = Entry(
-                self.master, textvariable=self.initial_value_var,
+                self.window, textvariable=self.initial_value_var,
                 command=self.on_update)
             initial_value_label.grid(row=row)
             initial_value_entry.grid(row=row, column=1)
             row += 1
 
-        button = Button(self.master, text="OK", command=self.on_ok)
+        button = Button(self.window, text="OK", command=self.on_ok)
         button.grid(row=row)
 
     def on_update(self, arg=None):
 
         if self.kind_var is not None:
             kind = self.kind_var.get()
             if kind == '':
@@ -96,8 +96,8 @@
         if self.update:
             self.update(self.cpt)
 
     def on_ok(self):
 
         self.on_update()
 
-        self.master.destroy()
+        self.window.destroy()
```

### Comparing `lcapygui-0.6/lcapygui/ui/tk/cpt_properties_dialog.py` & `lcapygui-0.9/lcapygui/ui/tk/cpt_properties_dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     def __init__(self, ui, cpt, update=None, title=''):
 
         self.cpt = cpt
         self.gcpt = cpt.gcpt
         self.update = update
         self.ui = ui
 
-        self.master = Tk()
-        self.master.title(title)
+        self.window = Tk()
+        self.window.title(title)
 
         entries = []
         if self.gcpt.kinds != {}:
             kind_name = self.gcpt.kinds[self.gcpt.kind]
             entries.append(LabelEntry(
                 'kind', 'Kind', kind_name, list(self.gcpt.kinds.values()),
                 command=self.on_update))
@@ -54,17 +54,17 @@
             entries.append(LabelEntry(k, v, getattr(self.gcpt, k),
                                       command=self.on_update))
 
         for k, v in self.gcpt.extra_fields.items():
             entries.append(LabelEntry(k, v, getattr(self.gcpt, k),
                                       command=self.on_update))
 
-        self.labelentries = LabelEntries(self.master, ui, entries)
+        self.labelentries = LabelEntries(self.window, ui, entries)
 
-        button = Button(self.master, text="OK", command=self.on_ok)
+        button = Button(self.window, text="OK", command=self.on_ok)
         button.grid(row=self.labelentries.row)
 
     def on_update(self, arg=None):
 
         if self.gcpt.kinds != {}:
             kind = self.gcpt.inv_kinds[self.labelentries.get('kind')]
             if self.gcpt.kind != kind:
@@ -81,34 +81,45 @@
         else:
             self.ui.show_error_dialog('Cannot change component type')
 
         for m, arg in enumerate(self.gcpt.args):
             if arg == 'Control':
                 continue
             value = self.labelentries.get(arg)
+            if value == '':
+                value = self.gcpt.name
             self.cpt.args[m] = value
 
         try:
             if self.cpt.is_capacitor:
                 v0 = self.labelentries.get('v0')
                 self.cpt.args[-1] = v0
                 if v0 == '':
                     v0 = None
                 else:
-                    v0 = float(v0)
+                    try:
+                        v0 = float(v0)
+                    except ValueError:
+                        # Symbolic
+                        pass
+
                 cpt = self.cpt.cpt
                 # Create new oneport (this should be improved).
                 self.cpt._cpt = cpt.__class__(cpt.C, v0)
             elif self.cpt.is_inductor:
                 i0 = self.labelentries.get('i0')
                 self.cpt.args[-1] = i0
                 if i0 == '':
                     i0 = None
                 else:
-                    i0 = float(i0)
+                    try:
+                        i0 = float(i0)
+                    except ValueError:
+                        # Symbolic
+                        pass
                 cpt = self.cpt.cpt
                 # Create new oneport (this should be improved).
                 self.cpt._cpt = cpt.__class__(cpt.L, i0)
         except KeyError:
             pass
 
         try:
@@ -125,8 +136,8 @@
         if self.update:
             self.update(self.cpt)
 
     def on_ok(self):
 
         self.on_update()
 
-        self.master.destroy()
+        self.window.destroy()
```

### Comparing `lcapygui-0.6/lcapygui/ui/tk/drawing.py` & `lcapygui-0.9/lcapygui/ui/tk/drawing.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/ui/tk/equations_dialog.py` & `lcapygui-0.9/lcapygui/ui/tk/equations_dialog.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,35 +24,35 @@
                 k = k.latex()
 
             s += '$' + k + '$: & $' + v.latex() + '$\\\\ \n'
 
         s += '\\end{tabular}\n'
         self.s = s
 
-        self.master = Tk()
-        self.master.title(title)
+        self.window = Tk()
+        self.window.title(title)
 
-        self.expr_label = Label(self.master, text='')
+        self.expr_label = Label(self.window, text='')
         self.expr_label.grid(row=0)
 
-        button = Button(self.master, text="LaTeX", command=self.on_latex)
+        button = Button(self.window, text="LaTeX", command=self.on_latex)
         button.grid(row=1, sticky='w')
 
         self.update()
 
     def update(self):
 
         try:
             self.show_img()
         except Exception as e:
             self.expr_label.config(text=e)
 
     def show_img(self):
 
         png_filename = LatexImage(self.s).image()
-        img = ImageTk.PhotoImage(Image.open(png_filename), master=self.master)
+        img = ImageTk.PhotoImage(Image.open(png_filename), master=self.window)
         self.expr_label.config(image=img)
         self.expr_label.photo = img
 
     def on_latex(self):
 
         self.ui.show_message_dialog(self.s)
```

### Comparing `lcapygui-0.6/lcapygui/ui/tk/help_dialog.py` & `lcapygui-0.9/lcapygui/ui/tk/help_dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,12 +39,12 @@
 For further information about Lcapy, see
  <a href="https://lcapy-gui.readthedocs.io"> https://lcapy-gui.readthedocs.io </a>
 and  <a href="https://lcapy.readthedocs.io"> https://lcapy.readthedocs.io </a>
 """
 
     def __init__(self):
 
-        master = Tk()
-        master.title('Help!')
-        html_label = HTMLLabel(master, html=self.message)
+        window = Tk()
+        window.title('Help!')
+        html_label = HTMLLabel(window, html=self.message)
         html_label.pack(fill="both", expand=True)
         html_label.fit_height()
```

### Comparing `lcapygui-0.6/lcapygui/ui/tk/inspect_dialog.py` & `lcapygui-0.9/lcapygui/ui/tk/inspect_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 class InspectDialog:
 
     def __init__(self, uimodel, cpt, title=''):
 
         self.uimodel = uimodel
         self.cpt = cpt
 
-        self.master = Tk()
-        self.master.title(title)
+        self.window = Tk()
+        self.window.title(title)
 
         buttons = [('Voltage', self.on_voltage),
                    ('Current', self.on_current),
                    ('Component impedance', self.on_impedance),
                    ('Component admittance', self.on_admittance),
                    ('Thevenin impedance', self.on_thevenin_impedance),
                    ('Norton admittance', self.on_norton_admittance)]
         for b in buttons:
-            button = Button(self.master, text=b[0], command=b[1])
+            button = Button(self.window, text=b[0], command=b[1])
             button.pack()
 
     def on_voltage(self):
 
         self.uimodel.inspect_voltage(self.cpt)
 
     def on_current(self):
```

### Comparing `lcapygui-0.6/lcapygui/ui/tk/labelentries.py` & `lcapygui-0.9/lcapygui/ui/tk/labelentries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 from tkinter import StringVar, Label, Entry, OptionMenu
 from tkinter.ttk import Checkbutton
 
 
 class LabelEntry:
 
-    def __init__(self, name, text, default, options=None, command=None):
+    def __init__(self, name, text, default, options=None,
+                 command=None, **kwargs):
 
         self.name = name
         self.text = text
         if default is None:
             default = 'None'
         self.default = default
         self.cls = default.__class__
         self.options = options
         self.command = command
+        # width, etc.
+        self.kwargs = kwargs
 
 
 class LabelEntries(dict):
 
-    def __init__(self, master, ui, entries):
+    def __init__(self, window, ui, entries):
 
         self.row = 0
         self.ui = ui
 
         for labelentry in entries:
 
-            var = StringVar(master)
+            var = StringVar(window)
             var.set(labelentry.default)
             self[labelentry.name] = (var, labelentry.cls)
 
-            label = Label(master, text=labelentry.text + ': ', anchor='w')
+            label = Label(window, text=labelentry.text + ': ', anchor='w')
             if isinstance(labelentry.options, (tuple, list)):
                 entry = OptionMenu(
-                    master, var, *labelentry.options,
+                    window, var, *labelentry.options,
                     command=labelentry.command)
             else:
                 if isinstance(labelentry.default, bool):
                     entry = Checkbutton(
-                        master, variable=var, command=labelentry.command)
+                        window, variable=var, command=labelentry.command)
                 else:
-                    entry = Entry(master, textvariable=var)
+                    entry = Entry(window, textvariable=var,
+                                  **labelentry.kwargs)
+
                     # if labelentry.command:
                     #    var.trace_add('write', labelentry.command)
                     if labelentry.command:
                         entry.bind('<Return>', labelentry.command)
 
             label.grid(row=self.row, sticky='w')
             entry.grid(row=self.row, column=1, sticky='w')
```

### Comparing `lcapygui-0.6/lcapygui/ui/tk/lateximage.py` & `lcapygui-0.9/lcapygui/ui/tk/lateximage.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/ui/tk/lcapytkm.py` & `lcapygui-0.9/lcapygui/ui/tk/lcapytkm.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/ui/tk/plot_dialog.py` & `lcapygui-0.9/lcapygui/ui/tk/node_properties_dialog.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from tkinter import Tk, StringVar, Label, Entry, Button
 
 
-class PlotDialog:
+class NodePropertiesDialog:
 
-    def __init__(self, node, update=None):
+    def __init__(self, node, update=None, title=''):
 
         self.node = node
         self.update = update
 
-        self.master = Tk()
+        self.window = Tk()
+        self.window.title(title)
 
         row = 0
 
-        self.name_var = StringVar(self.master)
+        self.name_var = StringVar(self.window)
         self.name_var.set(node.name)
 
-        name_label = Label(self.master, text='Name: ')
-        name_entry = Entry(self.master, textvariable=self.name_var)
+        name_label = Label(self.window, text='Name: ')
+        name_entry = Entry(self.window, textvariable=self.name_var)
 
         name_label.grid(row=row)
         name_entry.grid(row=row, column=1)
         row += 1
 
-        button = Button(self.master, text="OK", command=self.on_update)
+        button = Button(self.window, text="OK", command=self.on_update)
         button.grid(row=row)
 
     def on_update(self):
 
-        self.node.name = self.name_var.get()
+        node_name = self.name_var.get()
 
-        self.master.destroy()
+        self.window.destroy()
 
-        if self.update:
+        if self.node.name != node_name and self.update:
+            self.node.name = node_name
             self.update(self.node)
```

### Comparing `lcapygui-0.6/lcapygui/ui/tk/plot_properties_dialog.py` & `lcapygui-0.9/lcapygui/ui/tk/plot_properties_dialog.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 class PlotPropertiesDialog:
 
     def __init__(self, expr, ui):
 
         self.expr = expr
         self.ui = ui
 
-        self.master = Tk()
-        self.master.title('Plot properties')
+        self.window = Tk()
+        self.window.title('Plot properties')
 
         entries = [LabelEntry('min', 'Min', 0.0),
                    LabelEntry('max', 'Max', 1.0),
                    LabelEntry('points', 'Points', 200)]
 
         self.symbols = []
         for key in expr.symbols:
@@ -30,17 +30,17 @@
 
         kinds = []
         for key, val in plots.items():
             if hasattr(expr, val):
                 kinds.append(key)
 
         entries.append(LabelEntry('kind', 'Plot type', 'Plot', kinds))
-        self.labelentries = LabelEntries(self.master, ui, entries)
+        self.labelentries = LabelEntries(self.window, ui, entries)
 
-        button = Button(self.master, text="Plot", command=self.on_update)
+        button = Button(self.window, text="Plot", command=self.on_update)
         button.grid(row=self.labelentries.row)
 
     def on_update(self):
 
         points = linspace(self.labelentries.get('min'),
                           self.labelentries.get('max'),
                           self.labelentries.get('points'))
```

### Comparing `lcapygui-0.6/lcapygui/ui/tk/preferences_dialog.py` & `lcapygui-0.9/lcapygui/ui/tk/preferences_dialog.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 class PreferencesDialog:
 
     def __init__(self, ui, update):
 
         self.model = ui.model
         self.update = update
 
-        self.master = Tk()
-        self.master.title('Preferences')
+        self.window = Tk()
+        self.window.title('Preferences')
 
         entries = [LabelEntry('label_nodes', 'Node labels',
                               self.model.preferences.label_nodes,
                               ('all', 'none', 'alpha', 'pins',
                                'primary'), command=self.on_update),
                    LabelEntry('draw_nodes', 'Nodes',
                               self.model.preferences.draw_nodes,
@@ -54,17 +54,17 @@
                               command=self.on_update),
                    LabelEntry('snap_grid', 'Snap to grid',
                               self.model.preferences.snap_grid,
                               ('true', 'false'),
                               command=self.on_update),
                    ]
 
-        self.labelentries = LabelEntries(self.master, ui, entries)
+        self.labelentries = LabelEntries(self.window, ui, entries)
 
-        button = Button(self.master, text="OK", command=self.on_ok)
+        button = Button(self.window, text="OK", command=self.on_ok)
         button.grid(row=self.labelentries.row)
 
     def on_update(self, arg=None):
 
         self.model.preferences.label_nodes = self.labelentries.get(
             'label_nodes')
         self.model.preferences.draw_nodes = self.labelentries.get('draw_nodes')
@@ -87,10 +87,10 @@
             # Could check for changes
             self.update()
 
     def on_ok(self):
 
         self.on_update()
 
-        self.master.destroy()
+        self.window.destroy()
 
         self.model.preferences.save()
```

### Comparing `lcapygui-0.6/lcapygui/ui/tk/sketcher.py` & `lcapygui-0.9/lcapygui/ui/tk/sketcher.py`

 * *Files identical despite different names*

### Comparing `lcapygui-0.6/lcapygui/ui/uimodelbase.py` & `lcapygui-0.9/lcapygui/ui/uimodelbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ..annotations import Annotations
 from .preferences import Preferences
 from ..components.opamp import Opamp
 from ..components.cpt_maker import cpt_make_from_cpt, cpt_make_from_type, cpt_remake
 
 from copy import copy
 from math import atan2, degrees, sqrt
+from numpy import nan, isnan
 from lcapy import Circuit, expr
 from lcapy.mnacpts import Cpt
 from lcapy.nodes import parse_nodes
 from lcapy.schemmisc import Pos
 from lcapy.opts import Opts
 
 
@@ -34,15 +35,15 @@
         'v': ('v', 'Voltage source', 'V', ''),
         'w': ('w', 'Wire', 'W', ''),
         'e': ('e', 'VCVS', 'E', ''),
         'f': ('f', 'CCCS', 'F', ''),
         'g': ('g', 'VCCS', 'G', ''),
         'h': ('h', 'CCVS', 'H', ''),
         'o': ('o', 'Open circuit', 'O', ''),
-        'opamp': ('', 'Opamp', 'Opamp', ''),
+        'opamp': ('', 'Opamp', 'opamp', ''),
         'p': ('p', 'Port', 'P', ''),
         'y': ('y', 'Admittance', 'Y', ''),
         'z': ('z', 'Impedance', 'Z', ''),
         'cpe': ('', 'CPE', 'CPE', ''),
     }
 
     connection_map = {
@@ -62,15 +63,15 @@
     }
 
     def __init__(self, ui):
 
         self.circuit = Circuit()
         self.ui = ui
         self._analysis_circuit = None
-        self.filename = ''
+        self.pathname = ''
         self.voltage_annotations = Annotations()
         self.selected = None
         self.last_expr = None
         self.preferences = Preferences()
         self.dirty = False
         self.history = []
         self.clipboard = None
@@ -122,15 +123,15 @@
                 ymin = node.y
             if node.y > ymax:
                 ymax = node.y
         return xmin, ymin, xmax, ymax
 
     def choose_cpt_name(self, cpt_type):
 
-        if cpt_type == 'Opamp':
+        if cpt_type == 'opamp':
             cpt_type = 'E'
 
         num = 1
         while True:
             name = cpt_type + str(num)
             if name not in self.circuit.elements:
                 return name
@@ -185,14 +186,15 @@
             # This should also delete the annotations.
             cpt.undraw()
             redraw = False
         except AttributeError:
             pass
 
         self.circuit.remove(cpt.name)
+        self.invalidate()
 
         if redraw:
             self.ui.clear()
             self.redraw()
 
     def cpt_draw(self, cpt):
 
@@ -345,37 +347,37 @@
 
     def draw(self, cpt, **kwargs):
 
         if cpt is None:
             return
         cpt.draw(**kwargs)
 
-    def export(self, filename):
+    def export(self, pathname):
 
         cct = self.circuit
-        cct.draw(filename)
+        cct.draw(pathname)
 
     def invalidate(self):
 
         self._analysis_circuit = None
 
-    def load(self, filename):
+    def load(self, pathname):
 
         from lcapy import Circuit
 
-        self.filename = filename
+        self.pathname = pathname
 
-        with open(filename) as f:
+        with open(pathname) as f:
             line = f.readline()
             if line.startswith(r'\begin{tikz'):
                 self.ui.show_error_dialog('Cannot load Circuitikz macro file')
                 return
 
         try:
-            circuit = Circuit(filename)
+            circuit = Circuit(pathname)
         except Exception as e:
             self.exception(e)
             return
 
         return self.load_from_circuit(circuit)
 
     def load_from_circuit(self, circuit):
@@ -385,15 +387,18 @@
         for cpt in self.circuit.elements.values():
             if cpt.type == 'XX' and 'nodes' in cpt.opts:
                 positions = parse_nodes(cpt.opts['nodes'])
                 break
 
         if positions is not None:
             for k, v in self.circuit.nodes.items():
-                v.pos = positions[k]
+                try:
+                    v.pos = positions[k]
+                except KeyError:
+                    v.pos = None
 
         else:
 
             # Node positions not defined.
 
             sch = self.circuit.sch
 
@@ -475,28 +480,30 @@
             if cpt.type == 'XX' and cpt._string.startswith('; nodes='):
                 self.circuit.remove(cpt.name)
 
     def rotate(self, angle):
         # TODO
         pass
 
-    def save(self, filename):
+    def save(self, pathname):
 
         s = self.schematic()
 
-        with open(filename, 'w') as fhandle:
+        with open(pathname, 'w') as fhandle:
             fhandle.write(s)
         self.dirty = False
 
     def schematic(self):
 
         s = '# Created by ' + self.ui.NAME + ' V' + self.ui.version + '\n'
 
         # Define node positions
-        foo = [str(node) for node in self.circuit.nodes.values()]
+        foo = [str(node) for node in self.circuit.nodes.values()
+               if not isnan(node.pos.x)]
+
         s += '; nodes={' + ', '.join(foo) + '}' + '\n'
 
         for cpt in self.circuit.elements.values():
             s += str(cpt) + '\n'
 
         # FIXME, remove other preference string
         # Note, need a newline so string treated as a netlist string
@@ -511,28 +518,32 @@
             return
 
         all_node_names = list(self.circuit.nodes)
         node_names = []
         positions = gcpt.assign_positions(x1, y1, x2, y2)
 
         for m, position in enumerate(positions):
+            if position is None:
+                continue
+
             node = self.circuit.nodes.by_position(position)
             if node is None:
                 node_name = gcpt.choose_node_name(m, all_node_names)
                 all_node_names.append(node_name)
             else:
                 node_name = node.name
             node_names.append(node_name)
 
         netitem = gcpt.netitem(node_names, x1, y1, x2, y2, self.STEP)
 
         if self.ui.debug:
             print('Adding ' + netitem)
 
         cct = self.circuit.add(netitem)
+        self.invalidate()
         cpt = cct[cpt_name]
 
         for m, position in enumerate(positions):
             cpt.nodes[m].pos = Pos(position)
 
         attr_string = netitem.split(';', 1)[1]
         gcpt.update(nodes=cpt.nodes, opts=Opts(attr_string))
```

### Comparing `lcapygui-0.6/lcapygui/ui/uimodelmph.py` & `lcapygui-0.9/lcapygui/ui/uimodelmph.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from .uimodelbase import UIModelBase
 from lcapy.mnacpts import Cpt
 from lcapy import Circuit
+from os.path import basename
+from warnings import warn
 
 
 class Cursor:
 
     def __init__(self, ui, x, y):
 
         self.sketcher = ui.sketcher
@@ -137,33 +139,62 @@
                 return cpt
 
         return None
 
     def closest_node(self, x, y):
 
         for node in self.circuit.nodes.values():
+            if node.pos is None:
+                # This happens with opamps.  Node 0 is the default
+                # reference pin.
+                warn('Ignoring node %s with no position' % node.name)
+                continue
             x1, y1 = node.pos.x, node.pos.y
             rsq = (x1 - x)**2 + (y1 - y)**2
             if rsq < 0.1:
                 return node
         return None
 
+    def create_state_space(self, cpt):
+
+        ss = self.circuit.ss
+        self.ui.show_state_space_dialog(ss)
+
+    def create_transfer_function(self, cpt):
+
+        self.ui.show_transfer_function_dialog(cpt)
+
+    def create_twoport(self, cpt, kind):
+
+        self.ui.show_twoport_dialog(cpt, kind)
+
     def exception(self, e):
         message = str(e)
-        if self.filename != '':
-            message += ' in ' + self.filename
+        if self.pathname != '':
+            message += ' in ' + self.pathname
         self.ui.show_error_dialog(message)
         if self.ui.debug:
             import pdb
             pdb.set_trace()
 
-    def unselect(self):
+    def new_name(self, pathname):
 
-        self.cursors.remove()
-        self.ui.refresh()
+        from os.path import splitext
+
+        base, ext = splitext(pathname)
+        parts = base.split('_')
+        if len(parts) == 0:
+            suffix = '1'
+        else:
+            try:
+                suffix = str(int(parts[-1]) + 1)
+                base = '_'.join(parts[0:-1])
+            except ValueError:
+                suffix = '1'
+        return base + '_' + suffix + ext
 
     def on_add_node(self, x, y):
 
         # Snap to known node then snap to grid.
         node = self.closest_node(x, y)
         if node is None:
             if self.preferences.snap_grid == 'true':
@@ -228,35 +259,20 @@
         xmin, ymin, xmax, ymax = bbox
 
         self.ui.set_view(xmin - 2, ymin - 2, xmax + 2, ymax + 2)
         self.ui.refresh()
 
     def on_clone(self):
 
-        def new_name(filename):
-
-            from os.path import splitext
-
-            base, ext = splitext(filename)
-            parts = base.split('_')
-            if len(parts) == 0:
-                suffix = '1'
-            else:
-                try:
-                    suffix = str(int(parts[-1]) + 1)
-                    base = '_'.join(parts[0:-1])
-                except ValueError:
-                    suffix = '1'
-            return base + '_' + suffix + ext
-
-        filename = new_name(self.filename)
-        self.save(filename)
+        pathname = self.new_name(self.pathname)
+        self.save(pathname)
 
         model = self.ui.new()
-        model.load(filename)
+        model.load(pathname)
+        filename = basename(pathname)
         self.ui.set_filename(filename)
         self.ui.refresh()
 
     def on_close(self):
 
         self.ui.quit()
 
@@ -285,40 +301,52 @@
             # Node name may have changed...
             pass
 
         self.redraw()
         self.cursors.draw()
         self.ui.refresh()
 
-    def on_debug(self):
+    def on_create_state_space(self):
 
-        s = ''
-        s += 'Netlist.........\n'
-        s += self.schematic() + '\n'
-        s += 'Nodes...........\n'
-        s += self.circuit.nodes.debug() + '\n'
-        s += 'Cursors.........\n'
-        s += self.cursors.debug() + '\n'
-        s += 'Selected.........\n'
-        s += str(self.selected) + '\n'
-        self.ui.show_message_dialog(s, 'Debug')
+        self.create_state_space(self.selected)
+
+    def on_create_transfer_function(self):
+
+        self.create_transfer_function(self.selected)
+
+    def on_create_twoport(self, kind):
+
+        self.create_twoport(self.selected, kind)
 
     def on_cut(self):
 
         if self.selected is None:
             return
         if not self.cpt_selected:
             return
 
         self.cut(self.selected)
 
         self.cursors.draw()
 
         self.ui.refresh()
 
+    def on_debug(self):
+
+        s = ''
+        s += 'Netlist.........\n'
+        s += self.schematic() + '\n'
+        s += 'Nodes...........\n'
+        s += self.circuit.nodes.debug() + '\n'
+        s += 'Cursors.........\n'
+        s += self.cursors.debug() + '\n'
+        s += 'Selected.........\n'
+        s += str(self.selected) + '\n'
+        self.ui.show_message_dialog(s, 'Debug')
+
     def on_delete(self):
 
         if self.selected is None:
             return
         if not self.cpt_selected:
             # Handle node deletion later
             return
@@ -330,20 +358,32 @@
         self.ui.refresh()
 
     def on_describe(self):
 
         self.ui.show_message_dialog(self.circuit.description(),
                                     title='Description')
 
+    def on_expand(self):
+
+        cct = self.circuit.expand()
+        self.on_show_new_circuit(cct)
+
     def on_export(self):
 
-        filename = self.ui.export_file_dialog(self.filename)
-        if filename == '':
+        pathname = self.ui.export_file_dialog(self.pathname)
+        if pathname == '':
             return
-        self.export(filename)
+        self.export(pathname)
+
+    def on_expression(self):
+
+        from lcapy import expr
+
+        e = self.last_expr if self.last_expr is not None else expr(0)
+        self.ui.show_expr_dialog(e)
 
     def on_help(self):
 
         self.ui.show_help_dialog()
 
     def on_inspect(self):
 
@@ -357,15 +397,17 @@
                                     title=self.selected.name)
 
     def on_inspect_current(self):
 
         if not self.selected or not self.cpt_selected:
             return
 
+        win = self.ui.show_working_dialog('Calculating voltage')
         self.inspect_current(self.selected)
+        win.destroy()
 
     def on_inspect_norton_admittance(self):
 
         if not self.selected or not self.cpt_selected:
             return
 
         self.inspect_norton_admittance(self.selected)
@@ -378,15 +420,17 @@
         self.inspect_thevenin_impedance(self.selected)
 
     def on_inspect_voltage(self):
 
         if not self.selected or not self.cpt_selected:
             return
 
+        win = self.ui.show_working_dialog('Calculating voltage')
         self.inspect_voltage(self.selected)
+        win.destroy()
 
     def on_laplace_model(self):
 
         cct = self.circuit.s_model()
         self.on_show_new_circuit(cct)
 
     def on_left_click(self, x, y):
@@ -409,23 +453,44 @@
 
     def on_left_double_click(self, x, y):
 
         self.on_right_click(x, y)
 
     def on_load(self, initial_dir='.'):
 
-        filename = self.ui.open_file_dialog(initial_dir)
-        if filename == '' or filename == ():
+        pathname = self.ui.open_file_dialog(initial_dir)
+        if pathname == '' or pathname == ():
             return
 
         model = self.ui.new()
-        model.load(filename)
-        self.ui.set_filename(filename)
+        model.load(pathname)
+        self.ui.set_filename(pathname)
         self.ui.refresh()
 
+    def on_manipulation_kill(self):
+
+        # Could have a dialog to select what to kill
+
+        cct = self.circuit.kill()
+        self.on_show_new_circuit(cct)
+
+    def on_manipulation_remove_sources(self):
+
+        # Could have a dialog to select what to remove
+
+        # Remove independent sources
+        cct = self.circuit.copy()
+        cct = cct.copy()
+        values = list(cct.elements.values())
+        for cpt in values:
+            if cpt.is_independent_source:
+                cct.remove(cpt.name)
+
+        self.on_show_new_circuit(cct)
+
     def on_mesh_equations(self):
 
         if self.ground_node is None:
             self.ui.show_info_dialog('Suggest adding a ground node.')
 
         try:
             la = self.analysis_circuit.loop_analysis()
@@ -436,24 +501,29 @@
         eqns = la.mesh_equations()
         self.ui.show_equations_dialog(eqns, 'Mesh equations')
 
     def on_move(self, xshift, yshift):
 
         self.move(xshift, yshift)
 
-    def on_netlist(self):
+    def on_simple_netlist(self):
 
         netlist = []
         lines = self.circuit.netlist().split('\n')
         for line in lines:
             parts = line.split(';')
             netlist.append(parts[0].strip())
         s = '\n'.join(netlist)
         self.ui.show_message_dialog(s, 'Netlist')
 
+    def on_netlist(self):
+
+        s = self.schematic()
+        self.ui.show_message_dialog(s, 'Netlist')
+
     def on_nodal_equations(self):
 
         if self.ground_node is None:
             self.ui.show_info_dialog('Suggest adding a ground node.')
 
         try:
             na = self.analysis_circuit.nodal_analysis()
@@ -534,35 +604,35 @@
 
     def on_rotate(self, angle):
 
         self.rotate(angle)
 
     def on_save(self):
 
-        filename = self.filename
-        if filename == '':
+        pathname = self.pathname
+        if pathname == '':
             return
-        self.save(filename)
-        self.ui.save(filename)
+        self.save(pathname)
+        self.ui.save(pathname)
 
     def on_save_as(self):
 
-        filename = self.ui.save_file_dialog(self.filename)
-        if filename == '' or filename == ():
+        pathname = self.ui.save_file_dialog(self.pathname)
+        if pathname == '' or pathname == ():
             return
-        self.save(filename)
-        self.ui.save(filename)
+        self.save(pathname)
+        self.ui.save(pathname)
 
     def on_screenshot(self):
 
-        filename = self.ui.export_file_dialog(self.filename,
+        pathname = self.ui.export_file_dialog(self.pathname,
                                               default_ext='.png')
-        if filename == '' or filename == ():
+        if pathname == '' or pathname == ():
             return
-        self.ui.screenshot(filename)
+        self.ui.screenshot(pathname)
 
     def on_select(self, x, y):
 
         cpt = self.closest_cpt(x, y)
 
         if cpt is None:
             node = self.closest_node(x, y)
@@ -575,14 +645,19 @@
             self.select(None)
 
     def on_show_new_circuit(self, cct):
 
         model = self.ui.new()
         model.load_from_circuit(cct)
 
+        pathname = self.new_name(self.pathname)
+        filename = basename(pathname)
+        self.ui.set_filename(filename)
+        self.ui.refresh()
+
     def on_undo(self):
 
         self.undo()
         self.ui.refresh()
 
     def on_unselect(self):
 
@@ -603,7 +678,12 @@
         cct.draw(schtex_filename)
 
         with open(schtex_filename) as f:
             content = f.read()
         remove(schtex_filename)
 
         self.ui.show_message_dialog(content)
+
+    def unselect(self):
+
+        self.cursors.remove()
+        self.ui.refresh()
```

### Comparing `lcapygui-0.6/lcapygui.egg-info/PKG-INFO` & `lcapygui-0.9/lcapygui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcapygui
-Version: 0.6
+Version: 0.9
 Summary: A GUI for lcapy
 Home-page: https://github.com/mph-/lcapy-gui
 Author: Michael Hayes, Jordan Hay
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mph-/lcapy-gui
 Description: # lcapy-gui
```

### Comparing `lcapygui-0.6/lcapygui.egg-info/SOURCES.txt` & `lcapygui-0.9/lcapygui.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -47,26 +47,41 @@
 lcapygui/scripts/__init__.py
 lcapygui/scripts/lcapytk.py
 lcapygui/ui/__init__.py
 lcapygui/ui/preferences.py
 lcapygui/ui/uimodelbase.py
 lcapygui/ui/uimodelmph.py
 lcapygui/ui/tk/__init__.py
+lcapygui/ui/tk/approximate_dialog.py
 lcapygui/ui/tk/cpt_dialog.py
 lcapygui/ui/tk/cpt_properties_dialog.py
 lcapygui/ui/tk/drawing.py
+lcapygui/ui/tk/edit_dialog.py
+lcapygui/ui/tk/edit_values_dialog.py
 lcapygui/ui/tk/equations_dialog.py
-lcapygui/ui/tk/expr_advanced_dialog.py
+lcapygui/ui/tk/expr_attributes_dialog.py
+lcapygui/ui/tk/expr_calc.py
 lcapygui/ui/tk/expr_dialog.py
 lcapygui/ui/tk/exprimage.py
 lcapygui/ui/tk/help_dialog.py
 lcapygui/ui/tk/inspect_dialog.py
 lcapygui/ui/tk/labelentries.py
 lcapygui/ui/tk/lateximage.py
 lcapygui/ui/tk/lcapytk.py
 lcapygui/ui/tk/lcapytkm.py
+lcapygui/ui/tk/limit_dialog.py
+lcapygui/ui/tk/menu.py
 lcapygui/ui/tk/message_dialog.py
+lcapygui/ui/tk/multiplot_dialog.py
 lcapygui/ui/tk/node_properties_dialog.py
 lcapygui/ui/tk/plot_dialog.py
 lcapygui/ui/tk/plot_properties_dialog.py
 lcapygui/ui/tk/preferences_dialog.py
-lcapygui/ui/tk/sketcher.py
+lcapygui/ui/tk/python_dialog.py
+lcapygui/ui/tk/sketcher.py
+lcapygui/ui/tk/state_space_dialog.py
+lcapygui/ui/tk/subs_dialog.py
+lcapygui/ui/tk/transfer_dialog.py
+lcapygui/ui/tk/transfer_function_dialog.py
+lcapygui/ui/tk/twoport_dialog.py
+lcapygui/ui/tk/twoport_select_dialog.py
+lcapygui/ui/tk/working_dialog.py
```

### Comparing `lcapygui-0.6/setup.py` & `lcapygui-0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setup(
     name='lcapygui',
     packages=find_packages(include=[
         "lcapygui",
         "lcapygui.*"
     ]),
-    version="0.6",
+    version="0.9",
     description="A GUI for lcapy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Michael Hayes, Jordan Hay",
     license="MIT",
     url="https://github.com/mph-/lcapy-gui",
     project_urls={
@@ -27,15 +27,15 @@
     ],
     install_requires=[
         "setuptools",
         "importlib",
         "importlib-metadata",
         "importlib-resources",
         "pathlib",
-        "lcapy>=1.14",
+        "lcapy>=1.15",
         "numpy",
         "tk",
         "pillow>=9.4.0",
         "matplotlib",
         "svgpathtools",
         "svgpath2mpl",
         "tkhtmlview"
```

