# Comparing `tmp/visidata-2.9.tar.gz` & `tmp/visidata-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visidata-2.9.tar", last modified: Thu Jul 21 04:49:14 2022, max compression
+gzip compressed data, was "visidata-2.9.1.tar", last modified: Thu Jul 21 16:48:40 2022, max compression
```

## Comparing `visidata-2.9.tar` & `visidata-2.9.1.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxrwx---   0 kefala    (1000) kefala    (1000)        0 2022-07-21 04:49:14.850094 visidata-2.9/
--rw-rw----   0 kefala    (1000) kefala    (1000)    35147 2022-05-05 02:58:07.000000 visidata-2.9/LICENSE.gpl3
--rw-rw----   0 kefala    (1000) kefala    (1000)      156 2022-06-12 06:02:34.000000 visidata-2.9/MANIFEST.in
--rw-rw----   0 kefala    (1000) kefala    (1000)     4417 2022-07-21 04:49:14.850094 visidata-2.9/PKG-INFO
--rw-rw----   0 kefala    (1000) kefala    (1000)     2720 2022-07-21 04:48:26.000000 visidata-2.9/README.md
-drwxrwx---   0 kefala    (1000) kefala    (1000)        0 2022-07-21 04:49:14.834094 visidata-2.9/bin/
--rwxrwx---   0 kefala    (1000) kefala    (1000)      100 2022-06-12 06:02:26.000000 visidata-2.9/bin/vd
--rw-rw----   0 kefala    (1000) kefala    (1000)       38 2022-07-21 04:49:14.850094 visidata-2.9/setup.cfg
--rwxrwx---   0 kefala    (1000) kefala    (1000)     2116 2022-07-21 04:48:26.000000 visidata-2.9/setup.py
-drwxrwx---   0 kefala    (1000) kefala    (1000)        0 2022-07-21 04:49:14.842094 visidata-2.9/visidata/
--rw-rw----   0 kefala    (1000) kefala    (1000)     3879 2022-07-21 04:48:26.000000 visidata-2.9/visidata/__init__.py
--rw-rw----   0 kefala    (1000) kefala    (1000)       35 2022-06-12 06:02:34.000000 visidata-2.9/visidata/__main__.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    15286 2022-07-21 04:48:26.000000 visidata-2.9/visidata/_input.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4291 2022-06-12 06:02:42.000000 visidata-2.9/visidata/_open.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     8081 2022-07-21 04:48:26.000000 visidata-2.9/visidata/_types.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1040 2022-07-21 04:48:26.000000 visidata-2.9/visidata/_urlcache.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     6799 2022-07-21 04:48:26.000000 visidata-2.9/visidata/aggregators.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     9195 2022-07-21 04:48:26.000000 visidata-2.9/visidata/basesheet.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2060 2022-07-21 04:48:26.000000 visidata-2.9/visidata/bezier.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    29118 2022-07-21 04:48:26.000000 visidata-2.9/visidata/canvas.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     7882 2022-06-12 06:02:42.000000 visidata-2.9/visidata/canvas_text.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2936 2022-06-12 06:02:34.000000 visidata-2.9/visidata/choose.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     7656 2022-07-21 04:48:26.000000 visidata-2.9/visidata/clipboard.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     5855 2022-07-21 04:48:26.000000 visidata-2.9/visidata/cliptext.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    18541 2022-07-21 04:48:26.000000 visidata-2.9/visidata/cmdlog.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     5351 2022-07-21 04:48:26.000000 visidata-2.9/visidata/color.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1490 2022-06-12 06:02:34.000000 visidata-2.9/visidata/colorsheet.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    20954 2022-07-21 04:48:26.000000 visidata-2.9/visidata/column.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      990 2022-06-12 06:02:34.000000 visidata-2.9/visidata/customdate.py
-drwxrwx---   0 kefala    (1000) kefala    (1000)        0 2022-07-21 04:49:14.842094 visidata-2.9/visidata/ddw/
--rw-rw----   0 kefala    (1000) kefala    (1000)     7503 2022-06-12 06:02:42.000000 visidata-2.9/visidata/ddw/input.ddw
--rw-rw----   0 kefala    (1000) kefala    (1000)     4343 2022-06-12 06:02:34.000000 visidata-2.9/visidata/ddwplay.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     5106 2022-07-21 04:48:26.000000 visidata-2.9/visidata/deprecated.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4551 2022-06-12 06:02:34.000000 visidata-2.9/visidata/describe.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2699 2022-06-12 06:02:42.000000 visidata-2.9/visidata/editor.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1031 2022-06-12 06:02:34.000000 visidata-2.9/visidata/errors.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2896 2022-06-12 06:02:34.000000 visidata-2.9/visidata/expr.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     3143 2022-07-21 04:48:26.000000 visidata-2.9/visidata/extensible.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1026 2022-06-12 06:02:34.000000 visidata-2.9/visidata/fill.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     3566 2022-07-21 04:48:26.000000 visidata-2.9/visidata/form.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2242 2022-07-21 04:48:26.000000 visidata-2.9/visidata/freeze.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4483 2022-06-12 06:02:34.000000 visidata-2.9/visidata/freqtbl.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     7706 2022-06-12 06:02:34.000000 visidata-2.9/visidata/graph.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     5582 2022-06-12 06:02:42.000000 visidata-2.9/visidata/help.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1333 2022-06-12 06:02:34.000000 visidata-2.9/visidata/incr.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    11693 2022-07-21 04:48:26.000000 visidata-2.9/visidata/join.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2120 2022-06-12 06:02:34.000000 visidata-2.9/visidata/keys.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2013 2022-06-12 06:02:34.000000 visidata-2.9/visidata/layout.py
-drwxrwx---   0 kefala    (1000) kefala    (1000)        0 2022-07-21 04:49:14.846094 visidata-2.9/visidata/loaders/
--rw-rw----   0 kefala    (1000) kefala    (1000)        0 2020-11-29 22:19:31.000000 visidata-2.9/visidata/loaders/__init__.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    14751 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/_pandas.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4618 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/archive.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4020 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/arrow.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2299 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/csv.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1995 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/eml.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     3238 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/fixed_width.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      494 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/frictionless.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     5090 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/geojson.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2292 2022-06-12 06:02:34.000000 visidata-2.9/visidata/loaders/graphviz.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2232 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/hdf5.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     5062 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/html.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2423 2022-06-12 06:02:34.000000 visidata-2.9/visidata/loaders/http.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2101 2022-06-12 06:02:26.000000 visidata-2.9/visidata/loaders/imap.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     5314 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/json.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1253 2022-06-12 06:02:34.000000 visidata-2.9/visidata/loaders/lsv.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1700 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/markdown.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4655 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/mbtiles.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4067 2022-07-19 04:02:23.000000 visidata-2.9/visidata/loaders/mysql.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2916 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/npy.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2567 2022-06-12 06:02:34.000000 visidata-2.9/visidata/loaders/odf.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     8896 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/pandas_freqtbl.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      860 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/parquet.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    14150 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/pcap.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1674 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/pdf.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2606 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/png.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4126 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/postgres.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4844 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/rec.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1115 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/sas.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     3561 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/shp.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      741 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/spss.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     9153 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/sqlite.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      676 2022-06-12 06:02:34.000000 visidata-2.9/visidata/loaders/texttables.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     3316 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/tsv.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2910 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/ttf.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     8733 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/unzip_http.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      308 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/usv.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1151 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/vcf.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2731 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/vds.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      376 2022-06-12 06:02:34.000000 visidata-2.9/visidata/loaders/xlsb.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     6015 2022-07-21 04:48:26.000000 visidata-2.9/visidata/loaders/xlsx.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2974 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/xml.py
--rwxrwx---   0 kefala    (1000) kefala    (1000)     3517 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/xword.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1393 2022-06-12 06:02:42.000000 visidata-2.9/visidata/loaders/yaml.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     3338 2022-06-12 06:02:34.000000 visidata-2.9/visidata/macos.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2289 2022-07-21 04:48:26.000000 visidata-2.9/visidata/macros.py
--rwxrwx---   0 kefala    (1000) kefala    (1000)    12283 2022-07-21 04:48:26.000000 visidata-2.9/visidata/main.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    11231 2022-07-21 04:48:26.000000 visidata-2.9/visidata/mainloop.py
-drwxrwx---   0 kefala    (1000) kefala    (1000)        0 2022-07-21 04:49:14.850094 visidata-2.9/visidata/man/
--rw-rw----   0 kefala    (1000) kefala    (1000)    49478 2022-07-21 04:48:26.000000 visidata-2.9/visidata/man/vd.1
--rw-rw----   0 kefala    (1000) kefala    (1000)    54810 2022-07-21 04:48:26.000000 visidata-2.9/visidata/man/vd.txt
--rw-rw----   0 kefala    (1000) kefala    (1000)    49478 2022-07-21 04:48:26.000000 visidata-2.9/visidata/man/visidata.1
--rw-rw----   0 kefala    (1000) kefala    (1000)     3556 2022-07-21 04:48:26.000000 visidata-2.9/visidata/melt.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1050 2022-06-12 06:02:34.000000 visidata-2.9/visidata/memory.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    27567 2022-07-21 04:48:26.000000 visidata-2.9/visidata/menu.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    10229 2022-07-21 04:48:26.000000 visidata-2.9/visidata/metasheets.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      307 2022-06-12 06:02:26.000000 visidata-2.9/visidata/misc.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    10078 2022-07-21 04:48:26.000000 visidata-2.9/visidata/modify.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      868 2022-06-12 06:02:34.000000 visidata-2.9/visidata/motd.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    12024 2022-06-12 06:02:34.000000 visidata-2.9/visidata/movement.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    11247 2022-07-21 04:48:26.000000 visidata-2.9/visidata/path.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    11154 2022-07-21 04:48:26.000000 visidata-2.9/visidata/pivot.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     7911 2022-07-21 04:48:26.000000 visidata-2.9/visidata/plugins.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    14469 2022-07-21 04:48:26.000000 visidata-2.9/visidata/pyobj.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     5165 2022-07-21 04:48:26.000000 visidata-2.9/visidata/regex.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     7525 2022-07-21 04:48:26.000000 visidata-2.9/visidata/save.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4276 2022-06-12 06:02:34.000000 visidata-2.9/visidata/search.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     8827 2022-06-12 06:02:34.000000 visidata-2.9/visidata/selection.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    14495 2022-07-21 04:48:26.000000 visidata-2.9/visidata/settings.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    50125 2022-07-21 04:48:26.000000 visidata-2.9/visidata/sheets.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     9172 2022-07-21 04:48:26.000000 visidata-2.9/visidata/shell.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     5165 2022-06-12 06:02:34.000000 visidata-2.9/visidata/slide.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     3169 2022-06-12 06:02:34.000000 visidata-2.9/visidata/sort.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     7887 2022-07-21 04:48:26.000000 visidata-2.9/visidata/statusbar.py
-drwxrwx---   0 kefala    (1000) kefala    (1000)        0 2022-07-21 04:49:14.850094 visidata-2.9/visidata/tests/
--rw-rw----   0 kefala    (1000) kefala    (1000)        0 2019-02-23 16:28:56.000000 visidata-2.9/visidata/tests/__init__.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      489 2022-06-12 06:02:26.000000 visidata-2.9/visidata/tests/conftest.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4424 2022-07-21 04:48:26.000000 visidata-2.9/visidata/tests/test_commands.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     1878 2022-06-12 06:02:26.000000 visidata-2.9/visidata/tests/test_edittext.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      913 2022-06-12 06:02:26.000000 visidata-2.9/visidata/tests/test_path.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     3327 2022-06-12 06:02:34.000000 visidata-2.9/visidata/textsheet.py
--rw-rw----   0 kefala    (1000) kefala    (1000)    14993 2022-07-21 04:48:26.000000 visidata-2.9/visidata/threads.py
--rw-rw----   0 kefala    (1000) kefala    (1000)      947 2022-06-12 06:02:34.000000 visidata-2.9/visidata/transpose.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     3640 2022-07-21 04:48:26.000000 visidata-2.9/visidata/undo.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2942 2022-07-21 04:48:26.000000 visidata-2.9/visidata/unfurl.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     3614 2022-06-12 06:02:34.000000 visidata-2.9/visidata/utils.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     4559 2022-07-21 04:48:26.000000 visidata-2.9/visidata/vdobj.py
-drwxrwx---   0 kefala    (1000) kefala    (1000)        0 2022-07-21 04:49:14.850094 visidata-2.9/visidata/vendor/
--rw-rw----   0 kefala    (1000) kefala    (1000)    24527 2022-07-21 04:48:26.000000 visidata-2.9/visidata/vendor/appdirs.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     2162 2022-07-21 04:48:26.000000 visidata-2.9/visidata/window.py
--rw-rw----   0 kefala    (1000) kefala    (1000)     3294 2022-06-12 06:02:34.000000 visidata-2.9/visidata/wrappers.py
-drwxrwx---   0 kefala    (1000) kefala    (1000)        0 2022-07-21 04:49:14.842094 visidata-2.9/visidata.egg-info/
--rw-rw----   0 kefala    (1000) kefala    (1000)     4417 2022-07-21 04:49:14.000000 visidata-2.9/visidata.egg-info/PKG-INFO
--rw-rw----   0 kefala    (1000) kefala    (1000)     3036 2022-07-21 04:49:14.000000 visidata-2.9/visidata.egg-info/SOURCES.txt
--rw-rw----   0 kefala    (1000) kefala    (1000)        1 2022-07-21 04:49:14.000000 visidata-2.9/visidata.egg-info/dependency_links.txt
--rw-rw----   0 kefala    (1000) kefala    (1000)       51 2022-07-21 04:49:14.000000 visidata-2.9/visidata.egg-info/entry_points.txt
--rw-rw----   0 kefala    (1000) kefala    (1000)       64 2022-07-21 04:49:14.000000 visidata-2.9/visidata.egg-info/requires.txt
--rw-rw----   0 kefala    (1000) kefala    (1000)        9 2022-07-21 04:49:14.000000 visidata-2.9/visidata.egg-info/top_level.txt
+drwxrwx---   0 anja      (1000) anja      (1000)        0 2022-07-21 16:48:40.334184 visidata-2.9.1/
+-rw-rw----   0 anja      (1000) anja      (1000)    35147 2022-05-03 05:21:45.000000 visidata-2.9.1/LICENSE.gpl3
+-rw-rw----   0 anja      (1000) anja      (1000)      156 2022-07-06 04:56:40.000000 visidata-2.9.1/MANIFEST.in
+-rw-rw----   0 anja      (1000) anja      (1000)     3919 2022-07-21 16:48:40.334184 visidata-2.9.1/PKG-INFO
+-rw-rw----   0 anja      (1000) anja      (1000)     2722 2022-07-21 16:47:45.000000 visidata-2.9.1/README.md
+drwxrwx---   0 anja      (1000) anja      (1000)        0 2022-07-21 16:48:40.330184 visidata-2.9.1/bin/
+-rwxrwx---   0 anja      (1000) anja      (1000)      100 2022-05-03 05:21:45.000000 visidata-2.9.1/bin/vd
+-rw-rw----   0 anja      (1000) anja      (1000)       38 2022-07-21 16:48:40.334184 visidata-2.9.1/setup.cfg
+-rwxrwx---   0 anja      (1000) anja      (1000)     2118 2022-07-21 16:39:54.000000 visidata-2.9.1/setup.py
+drwxrwx---   0 anja      (1000) anja      (1000)        0 2022-07-21 16:48:40.330184 visidata-2.9.1/visidata/
+-rw-rw----   0 anja      (1000) anja      (1000)     3881 2022-07-21 16:39:54.000000 visidata-2.9.1/visidata/__init__.py
+-rw-rw----   0 anja      (1000) anja      (1000)       35 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/__main__.py
+-rw-rw----   0 anja      (1000) anja      (1000)    15286 2022-07-21 16:33:47.000000 visidata-2.9.1/visidata/_input.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4291 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/_open.py
+-rw-rw----   0 anja      (1000) anja      (1000)     8081 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/_types.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1040 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/_urlcache.py
+-rw-rw----   0 anja      (1000) anja      (1000)     6799 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/aggregators.py
+-rw-rw----   0 anja      (1000) anja      (1000)     9195 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/basesheet.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2060 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/bezier.py
+-rw-rw----   0 anja      (1000) anja      (1000)    29118 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/canvas.py
+-rw-rw----   0 anja      (1000) anja      (1000)     7882 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/canvas_text.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2936 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/choose.py
+-rw-rw----   0 anja      (1000) anja      (1000)     7656 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/clipboard.py
+-rw-rw----   0 anja      (1000) anja      (1000)     5855 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/cliptext.py
+-rw-rw----   0 anja      (1000) anja      (1000)    18541 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/cmdlog.py
+-rw-rw----   0 anja      (1000) anja      (1000)     5351 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/color.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1490 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/colorsheet.py
+-rw-rw----   0 anja      (1000) anja      (1000)    20954 2022-07-21 16:33:47.000000 visidata-2.9.1/visidata/column.py
+-rw-rw----   0 anja      (1000) anja      (1000)      990 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/customdate.py
+drwxrwx---   0 anja      (1000) anja      (1000)        0 2022-07-21 16:48:40.330184 visidata-2.9.1/visidata/ddw/
+-rw-rw----   0 anja      (1000) anja      (1000)     7503 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/ddw/input.ddw
+-rw-rw----   0 anja      (1000) anja      (1000)     4343 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/ddwplay.py
+-rw-rw----   0 anja      (1000) anja      (1000)     5106 2022-07-21 16:33:47.000000 visidata-2.9.1/visidata/deprecated.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4551 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/describe.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2699 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/editor.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1031 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/errors.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2896 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/expr.py
+-rw-rw----   0 anja      (1000) anja      (1000)     3143 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/extensible.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1026 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/fill.py
+-rw-rw----   0 anja      (1000) anja      (1000)     3566 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/form.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2242 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/freeze.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4483 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/freqtbl.py
+-rw-rw----   0 anja      (1000) anja      (1000)     7706 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/graph.py
+-rw-rw----   0 anja      (1000) anja      (1000)     5582 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/help.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1333 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/incr.py
+-rw-rw----   0 anja      (1000) anja      (1000)    11693 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/join.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2120 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/keys.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2013 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/layout.py
+drwxrwx---   0 anja      (1000) anja      (1000)        0 2022-07-21 16:48:40.334184 visidata-2.9.1/visidata/loaders/
+-rw-rw----   0 anja      (1000) anja      (1000)        0 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/loaders/__init__.py
+-rw-rw----   0 anja      (1000) anja      (1000)    14751 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/loaders/_pandas.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4618 2022-07-21 16:33:47.000000 visidata-2.9.1/visidata/loaders/archive.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4020 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/loaders/arrow.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2299 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/loaders/csv.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1995 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/eml.py
+-rw-rw----   0 anja      (1000) anja      (1000)     3238 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/fixed_width.py
+-rw-rw----   0 anja      (1000) anja      (1000)      494 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/frictionless.py
+-rw-rw----   0 anja      (1000) anja      (1000)     5090 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/geojson.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2292 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/graphviz.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2232 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/hdf5.py
+-rw-rw----   0 anja      (1000) anja      (1000)     5062 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/html.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2423 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/http.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2101 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/loaders/imap.py
+-rw-rw----   0 anja      (1000) anja      (1000)     5314 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/loaders/json.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1253 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/lsv.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1700 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/markdown.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4655 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/mbtiles.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4067 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/mysql.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2916 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/npy.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2567 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/odf.py
+-rw-rw----   0 anja      (1000) anja      (1000)     8896 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/pandas_freqtbl.py
+-rw-rw----   0 anja      (1000) anja      (1000)      860 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/loaders/parquet.py
+-rw-rw----   0 anja      (1000) anja      (1000)    14150 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/pcap.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1674 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/pdf.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2606 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/png.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4126 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/postgres.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4844 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/loaders/rec.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1115 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/sas.py
+-rw-rw----   0 anja      (1000) anja      (1000)     3561 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/shp.py
+-rw-rw----   0 anja      (1000) anja      (1000)      741 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/spss.py
+-rw-rw----   0 anja      (1000) anja      (1000)     9153 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/loaders/sqlite.py
+-rw-rw----   0 anja      (1000) anja      (1000)      676 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/loaders/texttables.py
+-rw-rw----   0 anja      (1000) anja      (1000)     3316 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/loaders/tsv.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2910 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/ttf.py
+-rw-rw----   0 anja      (1000) anja      (1000)     8741 2022-07-21 16:39:39.000000 visidata-2.9.1/visidata/loaders/unzip_http.py
+-rw-rw----   0 anja      (1000) anja      (1000)      308 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/loaders/usv.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1151 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/vcf.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2731 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/loaders/vds.py
+-rw-rw----   0 anja      (1000) anja      (1000)      376 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/xlsb.py
+-rw-rw----   0 anja      (1000) anja      (1000)     6015 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/loaders/xlsx.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2974 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/xml.py
+-rwxrwx---   0 anja      (1000) anja      (1000)     3517 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/xword.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1393 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/loaders/yaml.py
+-rw-rw----   0 anja      (1000) anja      (1000)     3338 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/macos.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2289 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/macros.py
+-rwxrwx---   0 anja      (1000) anja      (1000)    12285 2022-07-21 16:39:54.000000 visidata-2.9.1/visidata/main.py
+-rw-rw----   0 anja      (1000) anja      (1000)    11231 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/mainloop.py
+drwxrwx---   0 anja      (1000) anja      (1000)        0 2022-07-21 16:48:40.334184 visidata-2.9.1/visidata/man/
+-rw-rw----   0 anja      (1000) anja      (1000)    49478 2022-07-21 16:33:47.000000 visidata-2.9.1/visidata/man/vd.1
+-rw-rw----   0 anja      (1000) anja      (1000)    54810 2022-07-21 16:33:47.000000 visidata-2.9.1/visidata/man/vd.txt
+-rw-rw----   0 anja      (1000) anja      (1000)    49478 2022-07-21 16:33:47.000000 visidata-2.9.1/visidata/man/visidata.1
+-rw-rw----   0 anja      (1000) anja      (1000)     3556 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/melt.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1050 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/memory.py
+-rw-rw----   0 anja      (1000) anja      (1000)    27567 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/menu.py
+-rw-rw----   0 anja      (1000) anja      (1000)    10229 2022-07-21 16:33:47.000000 visidata-2.9.1/visidata/metasheets.py
+-rw-rw----   0 anja      (1000) anja      (1000)      307 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/misc.py
+-rw-rw----   0 anja      (1000) anja      (1000)    10078 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/modify.py
+-rw-rw----   0 anja      (1000) anja      (1000)      868 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/motd.py
+-rw-rw----   0 anja      (1000) anja      (1000)    12024 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/movement.py
+-rw-rw----   0 anja      (1000) anja      (1000)    11247 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/path.py
+-rw-rw----   0 anja      (1000) anja      (1000)    11154 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/pivot.py
+-rw-rw----   0 anja      (1000) anja      (1000)     7911 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/plugins.py
+-rw-rw----   0 anja      (1000) anja      (1000)    14469 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/pyobj.py
+-rw-rw----   0 anja      (1000) anja      (1000)     5165 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/regex.py
+-rw-rw----   0 anja      (1000) anja      (1000)     7525 2022-07-21 16:33:47.000000 visidata-2.9.1/visidata/save.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4276 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/search.py
+-rw-rw----   0 anja      (1000) anja      (1000)     8827 2022-07-06 04:56:40.000000 visidata-2.9.1/visidata/selection.py
+-rw-rw----   0 anja      (1000) anja      (1000)    14495 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/settings.py
+-rw-rw----   0 anja      (1000) anja      (1000)    50125 2022-07-21 16:33:47.000000 visidata-2.9.1/visidata/sheets.py
+-rw-rw----   0 anja      (1000) anja      (1000)     9172 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/shell.py
+-rw-rw----   0 anja      (1000) anja      (1000)     5165 2022-07-06 04:56:41.000000 visidata-2.9.1/visidata/slide.py
+-rw-rw----   0 anja      (1000) anja      (1000)     3169 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/sort.py
+-rw-rw----   0 anja      (1000) anja      (1000)     7887 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/statusbar.py
+drwxrwx---   0 anja      (1000) anja      (1000)        0 2022-07-21 16:48:40.334184 visidata-2.9.1/visidata/tests/
+-rw-rw----   0 anja      (1000) anja      (1000)        0 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/tests/__init__.py
+-rw-rw----   0 anja      (1000) anja      (1000)      489 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/tests/conftest.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4424 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/tests/test_commands.py
+-rw-rw----   0 anja      (1000) anja      (1000)     1878 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/tests/test_edittext.py
+-rw-rw----   0 anja      (1000) anja      (1000)      913 2022-05-03 05:21:45.000000 visidata-2.9.1/visidata/tests/test_path.py
+-rw-rw----   0 anja      (1000) anja      (1000)     3327 2022-07-06 04:56:41.000000 visidata-2.9.1/visidata/textsheet.py
+-rw-rw----   0 anja      (1000) anja      (1000)    14993 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/threads.py
+-rw-rw----   0 anja      (1000) anja      (1000)      947 2022-07-06 04:56:41.000000 visidata-2.9.1/visidata/transpose.py
+-rw-rw----   0 anja      (1000) anja      (1000)     3640 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/undo.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2942 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/unfurl.py
+-rw-rw----   0 anja      (1000) anja      (1000)     3614 2022-07-06 04:56:41.000000 visidata-2.9.1/visidata/utils.py
+-rw-rw----   0 anja      (1000) anja      (1000)     4559 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/vdobj.py
+drwxrwx---   0 anja      (1000) anja      (1000)        0 2022-07-21 16:48:40.334184 visidata-2.9.1/visidata/vendor/
+-rw-rw----   0 anja      (1000) anja      (1000)    24527 2022-07-21 16:33:21.000000 visidata-2.9.1/visidata/vendor/appdirs.py
+-rw-rw----   0 anja      (1000) anja      (1000)     2162 2022-07-21 16:33:47.000000 visidata-2.9.1/visidata/window.py
+-rw-rw----   0 anja      (1000) anja      (1000)     3294 2022-07-06 04:56:41.000000 visidata-2.9.1/visidata/wrappers.py
+drwxrwx---   0 anja      (1000) anja      (1000)        0 2022-07-21 16:48:40.330184 visidata-2.9.1/visidata.egg-info/
+-rw-rw----   0 anja      (1000) anja      (1000)     3919 2022-07-21 16:48:40.000000 visidata-2.9.1/visidata.egg-info/PKG-INFO
+-rw-rw----   0 anja      (1000) anja      (1000)     3036 2022-07-21 16:48:40.000000 visidata-2.9.1/visidata.egg-info/SOURCES.txt
+-rw-rw----   0 anja      (1000) anja      (1000)        1 2022-07-21 16:48:40.000000 visidata-2.9.1/visidata.egg-info/dependency_links.txt
+-rw-rw----   0 anja      (1000) anja      (1000)       50 2022-07-21 16:48:40.000000 visidata-2.9.1/visidata.egg-info/entry_points.txt
+-rw-rw----   0 anja      (1000) anja      (1000)       64 2022-07-21 16:48:40.000000 visidata-2.9.1/visidata.egg-info/requires.txt
+-rw-rw----   0 anja      (1000) anja      (1000)        9 2022-07-21 16:48:40.000000 visidata-2.9.1/visidata.egg-info/top_level.txt
```

### Comparing `visidata-2.9/LICENSE.gpl3` & `visidata-2.9.1/LICENSE.gpl3`

 * *Files identical despite different names*

### Comparing `visidata-2.9/PKG-INFO` & `visidata-2.9.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,16 @@
 Metadata-Version: 2.1
 Name: visidata
-Version: 2.9
+Version: 2.9.1
 Summary: terminal interface for exploring and arranging tabular data
 Home-page: https://visidata.org
+Download-URL: https://github.com/saulpw/visidata/tarball/2.9.1
 Author: Saul Pwanson
 Author-email: visidata@saul.pw
 License: GPLv3
-Download-URL: https://github.com/saulpw/visidata/tarball/2.9
-Description: 
-        # VisiData v2.9 [![twitter @VisiData][1.1]][1] [![CircleCI](https://circleci.com/gh/saulpw/visidata/tree/stable.svg?style=svg)](https://circleci.com/gh/saulpw/visidata/tree/stable) [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/saulpw/visidata)
-        
-        A terminal interface for exploring and arranging tabular data.
-        
-        ![Frequency table](http://visidata.org/freq-move-row.gif)
-        
-        VisiData supports tsv, csv, sqlite, json, xlsx (Excel), hdf5, and [many other formats](https://visidata.org/formats).
-        
-        ## Platform requirements
-        
-        - Linux, OS/X, or Windows (with WSL)
-        - Python 3.6+
-        - additional Python modules are required for certain formats and sources
-        
-        ## Install
-        
-        To install the latest release from PyPi:
-        
-            pip3 install visidata
-        
-        To install the cutting edge `develop` branch (no warranty expressed or implied):
-        
-            pip3 install git+https://github.com/saulpw/visidata.git@develop
-        
-        See [visidata.org/install](https://visidata.org/install) for detailed instructions for all available platforms and package managers.
-        
-        ### Usage
-        
-            $ vd <input>
-            $ <command> | vd
-        
-        Press `Ctrl+Q` to quit at any time.
-        
-        Hundreds of other commands and options are also available; see the documentation.
-        
-        ### Documentation
-        
-        * [VisiData documentation](https://visidata.org/docs)
-        * [Plugin Author's Guide and API Reference](https://visidata.org/docs/api)
-        * [Quick reference](https://visidata.org/man) (available within `vd` with `Ctrl+H`), which has a list of commands and options.
-        * [Intro to VisiData Tutorial](https://jsvine.github.io/intro-to-visidata/) by [Jeremy Singer-Vine](https://www.jsvine.com/)
-        
-        ### Help and Support
-        
-        If you have a question, issue, or suggestion regarding VisiData, please [create an issue on Github](https://github.com/saulpw/visidata/issues) or chat with us at #visidata on [irc.libera.chat](https://libera.chat/).
-        
-        If you use VisiData regularly, please [support me on Patreon](https://www.patreon.com/saulpw)!
-        
-        ## License
-        
-        Code in the `stable` branch of this repository, including the main `vd` application, loaders, and plugins, is available for use and redistribution under GPLv3.
-        
-        ## Credits
-        
-        VisiData is conceived and developed by Saul Pwanson `<vd@saul.pw>`.
-        
-        Anja Kefala `<anja.kefala@gmail.com>` maintains the documentation and packages for all platforms.
-        
-        Many thanks to numerous other [contributors](https://visidata.org/credits/), and to those wonderful users who provide feedback, for helping to make VisiData the awesome tool that it is.
-        
-        [1.1]: http://i.imgur.com/tXSoThF.png
-        [1]: http://www.twitter.com/VisiData
-        
-        <!-- Please don't remove this: Grab your social icons from https://github.com/carlsednaoui/gitsocial -->
-        
 Keywords: console tabular data spreadsheet terminal viewer textpunkcurses csv hdf5 h5 xlsx excel tsv
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -87,7 +21,76 @@
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.gpl3
+
+
+# VisiData v2.9.1 [![twitter @VisiData][1.1]][1] [![CircleCI](https://circleci.com/gh/saulpw/visidata/tree/stable.svg?style=svg)](https://circleci.com/gh/saulpw/visidata/tree/stable) [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/saulpw/visidata)
+
+A terminal interface for exploring and arranging tabular data.
+
+![Frequency table](http://visidata.org/freq-move-row.gif)
+
+VisiData supports tsv, csv, sqlite, json, xlsx (Excel), hdf5, and [many other formats](https://visidata.org/formats).
+
+## Platform requirements
+
+- Linux, OS/X, or Windows (with WSL)
+- Python 3.6+
+- additional Python modules are required for certain formats and sources
+
+## Install
+
+To install the latest release from PyPi:
+
+    pip3 install visidata
+
+To install the cutting edge `develop` branch (no warranty expressed or implied):
+
+    pip3 install git+https://github.com/saulpw/visidata.git@develop
+
+See [visidata.org/install](https://visidata.org/install) for detailed instructions for all available platforms and package managers.
+
+### Usage
+
+    $ vd <input>
+    $ <command> | vd
+
+Press `Ctrl+Q` to quit at any time.
+
+Hundreds of other commands and options are also available; see the documentation.
+
+### Documentation
+
+* [VisiData documentation](https://visidata.org/docs)
+* [Plugin Author's Guide and API Reference](https://visidata.org/docs/api)
+* [Quick reference](https://visidata.org/man) (available within `vd` with `Ctrl+H`), which has a list of commands and options.
+* [Intro to VisiData Tutorial](https://jsvine.github.io/intro-to-visidata/) by [Jeremy Singer-Vine](https://www.jsvine.com/)
+
+### Help and Support
+
+If you have a question, issue, or suggestion regarding VisiData, please [create an issue on Github](https://github.com/saulpw/visidata/issues) or chat with us at #visidata on [irc.libera.chat](https://libera.chat/).
+
+If you use VisiData regularly, please [support me on Patreon](https://www.patreon.com/saulpw)!
+
+## License
+
+Code in the `stable` branch of this repository, including the main `vd` application, loaders, and plugins, is available for use and redistribution under GPLv3.
+
+## Credits
+
+VisiData is conceived and developed by Saul Pwanson `<vd@saul.pw>`.
+
+Anja Kefala `<anja.kefala@gmail.com>` maintains the documentation and packages for all platforms.
+
+Many thanks to numerous other [contributors](https://visidata.org/credits/), and to those wonderful users who provide feedback, for helping to make VisiData the awesome tool that it is.
+
+[1.1]: http://i.imgur.com/tXSoThF.png
+[1]: http://www.twitter.com/VisiData
+
+<!-- Please don't remove this: Grab your social icons from https://github.com/carlsednaoui/gitsocial -->
+
+
```

### Comparing `visidata-2.9/README.md` & `visidata-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# VisiData v2.9 [![twitter @VisiData][1.1]][1] [![CircleCI](https://circleci.com/gh/saulpw/visidata/tree/stable.svg?style=svg)](https://circleci.com/gh/saulpw/visidata/tree/stable) [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/saulpw/visidata)
+# VisiData v2.9.1 [![twitter @VisiData][1.1]][1] [![CircleCI](https://circleci.com/gh/saulpw/visidata/tree/stable.svg?style=svg)](https://circleci.com/gh/saulpw/visidata/tree/stable) [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/saulpw/visidata)
 
 A terminal interface for exploring and arranging tabular data.
 
 ![Frequency table](http://visidata.org/freq-move-row.gif)
 
 VisiData supports tsv, csv, sqlite, json, xlsx (Excel), hdf5, and [many other formats](https://visidata.org/formats).
```

### Comparing `visidata-2.9/setup.py` & `visidata-2.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 from setuptools import setup
 # tox can't actually run python3 setup.py: https://github.com/tox-dev/tox/issues/96
 #from visidata import __version__
-__version__ = '2.9'
+__version__ = '2.9.1'
 
 setup(name='visidata',
       version=__version__,
       description='terminal interface for exploring and arranging tabular data',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       author='Saul Pwanson',
```

### Comparing `visidata-2.9/visidata/__init__.py` & `visidata-2.9.1/visidata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 'VisiData: a curses interface for exploring and arranging tabular data'
 
-__version__ = '2.9'
+__version__ = '2.9.1'
 __version_info__ = 'VisiData v' + __version__
 __author__ = 'Saul Pwanson <vd@saul.pw>'
 __status__ = 'Production/Stable'
 __copyright__ = 'Copyright (c) 2016-2021 ' + __author__
 
 
 class EscapeException(BaseException):
```

### Comparing `visidata-2.9/visidata/_input.py` & `visidata-2.9.1/visidata/_input.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/_open.py` & `visidata-2.9.1/visidata/_open.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/_types.py` & `visidata-2.9.1/visidata/_types.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/_urlcache.py` & `visidata-2.9.1/visidata/_urlcache.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/aggregators.py` & `visidata-2.9.1/visidata/aggregators.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/basesheet.py` & `visidata-2.9.1/visidata/basesheet.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/bezier.py` & `visidata-2.9.1/visidata/bezier.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/canvas.py` & `visidata-2.9.1/visidata/canvas.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/canvas_text.py` & `visidata-2.9.1/visidata/canvas_text.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/choose.py` & `visidata-2.9.1/visidata/choose.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/clipboard.py` & `visidata-2.9.1/visidata/clipboard.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/cliptext.py` & `visidata-2.9.1/visidata/cliptext.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/cmdlog.py` & `visidata-2.9.1/visidata/cmdlog.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/color.py` & `visidata-2.9.1/visidata/color.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/colorsheet.py` & `visidata-2.9.1/visidata/colorsheet.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/column.py` & `visidata-2.9.1/visidata/column.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/customdate.py` & `visidata-2.9.1/visidata/customdate.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/ddw/input.ddw` & `visidata-2.9.1/visidata/ddw/input.ddw`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/ddwplay.py` & `visidata-2.9.1/visidata/ddwplay.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/deprecated.py` & `visidata-2.9.1/visidata/deprecated.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/describe.py` & `visidata-2.9.1/visidata/describe.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/editor.py` & `visidata-2.9.1/visidata/editor.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/errors.py` & `visidata-2.9.1/visidata/errors.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/expr.py` & `visidata-2.9.1/visidata/expr.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/extensible.py` & `visidata-2.9.1/visidata/extensible.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/fill.py` & `visidata-2.9.1/visidata/fill.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/form.py` & `visidata-2.9.1/visidata/form.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/freeze.py` & `visidata-2.9.1/visidata/freeze.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/freqtbl.py` & `visidata-2.9.1/visidata/freqtbl.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/graph.py` & `visidata-2.9.1/visidata/graph.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/help.py` & `visidata-2.9.1/visidata/help.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/incr.py` & `visidata-2.9.1/visidata/incr.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/join.py` & `visidata-2.9.1/visidata/join.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/keys.py` & `visidata-2.9.1/visidata/keys.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/layout.py` & `visidata-2.9.1/visidata/layout.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/_pandas.py` & `visidata-2.9.1/visidata/loaders/_pandas.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/archive.py` & `visidata-2.9.1/visidata/loaders/archive.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/arrow.py` & `visidata-2.9.1/visidata/loaders/arrow.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/csv.py` & `visidata-2.9.1/visidata/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/eml.py` & `visidata-2.9.1/visidata/loaders/eml.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/fixed_width.py` & `visidata-2.9.1/visidata/loaders/fixed_width.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/geojson.py` & `visidata-2.9.1/visidata/loaders/geojson.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/graphviz.py` & `visidata-2.9.1/visidata/loaders/graphviz.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/hdf5.py` & `visidata-2.9.1/visidata/loaders/hdf5.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/html.py` & `visidata-2.9.1/visidata/loaders/html.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/http.py` & `visidata-2.9.1/visidata/loaders/http.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/imap.py` & `visidata-2.9.1/visidata/loaders/imap.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/json.py` & `visidata-2.9.1/visidata/loaders/json.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/lsv.py` & `visidata-2.9.1/visidata/loaders/lsv.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/markdown.py` & `visidata-2.9.1/visidata/loaders/markdown.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/mbtiles.py` & `visidata-2.9.1/visidata/loaders/mbtiles.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/mysql.py` & `visidata-2.9.1/visidata/loaders/mysql.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/npy.py` & `visidata-2.9.1/visidata/loaders/npy.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/odf.py` & `visidata-2.9.1/visidata/loaders/odf.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/pandas_freqtbl.py` & `visidata-2.9.1/visidata/loaders/pandas_freqtbl.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/parquet.py` & `visidata-2.9.1/visidata/loaders/parquet.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/pcap.py` & `visidata-2.9.1/visidata/loaders/pcap.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/pdf.py` & `visidata-2.9.1/visidata/loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/png.py` & `visidata-2.9.1/visidata/loaders/png.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/postgres.py` & `visidata-2.9.1/visidata/loaders/postgres.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/rec.py` & `visidata-2.9.1/visidata/loaders/rec.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/sas.py` & `visidata-2.9.1/visidata/loaders/sas.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/shp.py` & `visidata-2.9.1/visidata/loaders/shp.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/spss.py` & `visidata-2.9.1/visidata/loaders/spss.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/sqlite.py` & `visidata-2.9.1/visidata/loaders/sqlite.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/texttables.py` & `visidata-2.9.1/visidata/loaders/texttables.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/tsv.py` & `visidata-2.9.1/visidata/loaders/tsv.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/ttf.py` & `visidata-2.9.1/visidata/loaders/ttf.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/unzip_http.py` & `visidata-2.9.1/visidata/loaders/unzip_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import io
 import zlib
 import struct
 import fnmatch
 import pathlib
 import urllib.parse
 
-import urllib3
 
 __version__ = '0.5'
 
 
 def error(s):
     raise Exception(s)
 
@@ -95,14 +94,15 @@
     fmt_eocd64 = '<IQHHIIQQQQ'  # end of central directory ZIP64
     fmt_cdirentry = '<IHHHHIIIIHHHHHII'  # central directory entry
     fmt_localhdr = '<IHHHIIIIHH'  # local directory header
     magic_eocd64 = b'\x50\x4b\x06\x06'
     magic_eocd = b'\x50\x4b\x05\x06'
 
     def __init__(self, url):
+        import urllib3
         self.url = url
         self.http = urllib3.PoolManager()
         self.zip_size = 0
 
     def __enter__(self):
         return self
```

### Comparing `visidata-2.9/visidata/loaders/vcf.py` & `visidata-2.9.1/visidata/loaders/vcf.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/vds.py` & `visidata-2.9.1/visidata/loaders/vds.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/xlsx.py` & `visidata-2.9.1/visidata/loaders/xlsx.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/xml.py` & `visidata-2.9.1/visidata/loaders/xml.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/xword.py` & `visidata-2.9.1/visidata/loaders/xword.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/loaders/yaml.py` & `visidata-2.9.1/visidata/loaders/yaml.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/macos.py` & `visidata-2.9.1/visidata/macos.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/macros.py` & `visidata-2.9.1/visidata/macros.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/main.py` & `visidata-2.9.1/visidata/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # Usage: $0 [<options>] [<input> ...]
 #        $0 [<options>] --play <cmdlog> [--batch] [-w <waitsecs>] [-o <output>] [field=value ...]
 
-__version__ = '2.9'
+__version__ = '2.9.1'
 __version_info__ = 'saul.pw/VisiData v' + __version__
 
 from copy import copy
 import os
 import io
 import sys
 import locale
```

### Comparing `visidata-2.9/visidata/mainloop.py` & `visidata-2.9.1/visidata/mainloop.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/man/vd.1` & `visidata-2.9.1/visidata/man/vd.1`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/man/vd.txt` & `visidata-2.9.1/visidata/man/vd.txt`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/man/visidata.1` & `visidata-2.9.1/visidata/man/visidata.1`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/melt.py` & `visidata-2.9.1/visidata/melt.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/memory.py` & `visidata-2.9.1/visidata/memory.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/menu.py` & `visidata-2.9.1/visidata/menu.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/metasheets.py` & `visidata-2.9.1/visidata/metasheets.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/modify.py` & `visidata-2.9.1/visidata/modify.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/motd.py` & `visidata-2.9.1/visidata/motd.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/movement.py` & `visidata-2.9.1/visidata/movement.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/path.py` & `visidata-2.9.1/visidata/path.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/pivot.py` & `visidata-2.9.1/visidata/pivot.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/plugins.py` & `visidata-2.9.1/visidata/plugins.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/pyobj.py` & `visidata-2.9.1/visidata/pyobj.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/regex.py` & `visidata-2.9.1/visidata/regex.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/save.py` & `visidata-2.9.1/visidata/save.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/search.py` & `visidata-2.9.1/visidata/search.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/selection.py` & `visidata-2.9.1/visidata/selection.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/settings.py` & `visidata-2.9.1/visidata/settings.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/sheets.py` & `visidata-2.9.1/visidata/sheets.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/shell.py` & `visidata-2.9.1/visidata/shell.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/slide.py` & `visidata-2.9.1/visidata/slide.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/sort.py` & `visidata-2.9.1/visidata/sort.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/statusbar.py` & `visidata-2.9.1/visidata/statusbar.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/tests/test_commands.py` & `visidata-2.9.1/visidata/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/tests/test_edittext.py` & `visidata-2.9.1/visidata/tests/test_edittext.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/tests/test_path.py` & `visidata-2.9.1/visidata/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/textsheet.py` & `visidata-2.9.1/visidata/textsheet.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/threads.py` & `visidata-2.9.1/visidata/threads.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/transpose.py` & `visidata-2.9.1/visidata/transpose.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/undo.py` & `visidata-2.9.1/visidata/undo.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/unfurl.py` & `visidata-2.9.1/visidata/unfurl.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/utils.py` & `visidata-2.9.1/visidata/utils.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/vdobj.py` & `visidata-2.9.1/visidata/vdobj.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/vendor/appdirs.py` & `visidata-2.9.1/visidata/vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/window.py` & `visidata-2.9.1/visidata/window.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata/wrappers.py` & `visidata-2.9.1/visidata/wrappers.py`

 * *Files identical despite different names*

### Comparing `visidata-2.9/visidata.egg-info/PKG-INFO` & `visidata-2.9.1/visidata.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,16 @@
 Metadata-Version: 2.1
 Name: visidata
-Version: 2.9
+Version: 2.9.1
 Summary: terminal interface for exploring and arranging tabular data
 Home-page: https://visidata.org
+Download-URL: https://github.com/saulpw/visidata/tarball/2.9.1
 Author: Saul Pwanson
 Author-email: visidata@saul.pw
 License: GPLv3
-Download-URL: https://github.com/saulpw/visidata/tarball/2.9
-Description: 
-        # VisiData v2.9 [![twitter @VisiData][1.1]][1] [![CircleCI](https://circleci.com/gh/saulpw/visidata/tree/stable.svg?style=svg)](https://circleci.com/gh/saulpw/visidata/tree/stable) [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/saulpw/visidata)
-        
-        A terminal interface for exploring and arranging tabular data.
-        
-        ![Frequency table](http://visidata.org/freq-move-row.gif)
-        
-        VisiData supports tsv, csv, sqlite, json, xlsx (Excel), hdf5, and [many other formats](https://visidata.org/formats).
-        
-        ## Platform requirements
-        
-        - Linux, OS/X, or Windows (with WSL)
-        - Python 3.6+
-        - additional Python modules are required for certain formats and sources
-        
-        ## Install
-        
-        To install the latest release from PyPi:
-        
-            pip3 install visidata
-        
-        To install the cutting edge `develop` branch (no warranty expressed or implied):
-        
-            pip3 install git+https://github.com/saulpw/visidata.git@develop
-        
-        See [visidata.org/install](https://visidata.org/install) for detailed instructions for all available platforms and package managers.
-        
-        ### Usage
-        
-            $ vd <input>
-            $ <command> | vd
-        
-        Press `Ctrl+Q` to quit at any time.
-        
-        Hundreds of other commands and options are also available; see the documentation.
-        
-        ### Documentation
-        
-        * [VisiData documentation](https://visidata.org/docs)
-        * [Plugin Author's Guide and API Reference](https://visidata.org/docs/api)
-        * [Quick reference](https://visidata.org/man) (available within `vd` with `Ctrl+H`), which has a list of commands and options.
-        * [Intro to VisiData Tutorial](https://jsvine.github.io/intro-to-visidata/) by [Jeremy Singer-Vine](https://www.jsvine.com/)
-        
-        ### Help and Support
-        
-        If you have a question, issue, or suggestion regarding VisiData, please [create an issue on Github](https://github.com/saulpw/visidata/issues) or chat with us at #visidata on [irc.libera.chat](https://libera.chat/).
-        
-        If you use VisiData regularly, please [support me on Patreon](https://www.patreon.com/saulpw)!
-        
-        ## License
-        
-        Code in the `stable` branch of this repository, including the main `vd` application, loaders, and plugins, is available for use and redistribution under GPLv3.
-        
-        ## Credits
-        
-        VisiData is conceived and developed by Saul Pwanson `<vd@saul.pw>`.
-        
-        Anja Kefala `<anja.kefala@gmail.com>` maintains the documentation and packages for all platforms.
-        
-        Many thanks to numerous other [contributors](https://visidata.org/credits/), and to those wonderful users who provide feedback, for helping to make VisiData the awesome tool that it is.
-        
-        [1.1]: http://i.imgur.com/tXSoThF.png
-        [1]: http://www.twitter.com/VisiData
-        
-        <!-- Please don't remove this: Grab your social icons from https://github.com/carlsednaoui/gitsocial -->
-        
 Keywords: console tabular data spreadsheet terminal viewer textpunkcurses csv hdf5 h5 xlsx excel tsv
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -87,7 +21,76 @@
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.gpl3
+
+
+# VisiData v2.9.1 [![twitter @VisiData][1.1]][1] [![CircleCI](https://circleci.com/gh/saulpw/visidata/tree/stable.svg?style=svg)](https://circleci.com/gh/saulpw/visidata/tree/stable) [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/saulpw/visidata)
+
+A terminal interface for exploring and arranging tabular data.
+
+![Frequency table](http://visidata.org/freq-move-row.gif)
+
+VisiData supports tsv, csv, sqlite, json, xlsx (Excel), hdf5, and [many other formats](https://visidata.org/formats).
+
+## Platform requirements
+
+- Linux, OS/X, or Windows (with WSL)
+- Python 3.6+
+- additional Python modules are required for certain formats and sources
+
+## Install
+
+To install the latest release from PyPi:
+
+    pip3 install visidata
+
+To install the cutting edge `develop` branch (no warranty expressed or implied):
+
+    pip3 install git+https://github.com/saulpw/visidata.git@develop
+
+See [visidata.org/install](https://visidata.org/install) for detailed instructions for all available platforms and package managers.
+
+### Usage
+
+    $ vd <input>
+    $ <command> | vd
+
+Press `Ctrl+Q` to quit at any time.
+
+Hundreds of other commands and options are also available; see the documentation.
+
+### Documentation
+
+* [VisiData documentation](https://visidata.org/docs)
+* [Plugin Author's Guide and API Reference](https://visidata.org/docs/api)
+* [Quick reference](https://visidata.org/man) (available within `vd` with `Ctrl+H`), which has a list of commands and options.
+* [Intro to VisiData Tutorial](https://jsvine.github.io/intro-to-visidata/) by [Jeremy Singer-Vine](https://www.jsvine.com/)
+
+### Help and Support
+
+If you have a question, issue, or suggestion regarding VisiData, please [create an issue on Github](https://github.com/saulpw/visidata/issues) or chat with us at #visidata on [irc.libera.chat](https://libera.chat/).
+
+If you use VisiData regularly, please [support me on Patreon](https://www.patreon.com/saulpw)!
+
+## License
+
+Code in the `stable` branch of this repository, including the main `vd` application, loaders, and plugins, is available for use and redistribution under GPLv3.
+
+## Credits
+
+VisiData is conceived and developed by Saul Pwanson `<vd@saul.pw>`.
+
+Anja Kefala `<anja.kefala@gmail.com>` maintains the documentation and packages for all platforms.
+
+Many thanks to numerous other [contributors](https://visidata.org/credits/), and to those wonderful users who provide feedback, for helping to make VisiData the awesome tool that it is.
+
+[1.1]: http://i.imgur.com/tXSoThF.png
+[1]: http://www.twitter.com/VisiData
+
+<!-- Please don't remove this: Grab your social icons from https://github.com/carlsednaoui/gitsocial -->
+
+
```

### Comparing `visidata-2.9/visidata.egg-info/SOURCES.txt` & `visidata-2.9.1/visidata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

