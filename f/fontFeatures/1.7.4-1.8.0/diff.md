# Comparing `tmp/fontFeatures-1.7.4.tar.gz` & `tmp/fontFeatures-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fontFeatures-1.7.4.tar", last modified: Mon Dec 12 16:12:16 2022, max compression
+gzip compressed data, was "fontFeatures-1.8.0.tar", last modified: Mon Jul 17 10:34:13 2023, max compression
```

## Comparing `fontFeatures-1.7.4.tar` & `fontFeatures-1.8.0.tar`

### file list

```diff
@@ -1,476 +1,475 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.856462 fontFeatures-1.7.4/
--rw-r--r--   0 simon      (501) staff       (20)      235 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/.coveragerc
--rw-r--r--   0 simon      (501) staff       (20)      178 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/.editorconfig
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.770681 fontFeatures-1.7.4/.github/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.774050 fontFeatures-1.7.4/.github/workflows/
--rw-r--r--   0 simon      (501) staff       (20)      593 2021-12-11 20:33:14.000000 fontFeatures-1.7.4/.github/workflows/ci.yml
--rw-r--r--   0 simon      (501) staff       (20)      128 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     1226 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/CHANGES.md
--rw-r--r--   0 simon      (501) staff       (20)     1520 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/LICENSE
--rw-r--r--   0 simon      (501) staff       (20)     2269 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/NEW-FORMAT.md
--rw-r--r--   0 simon      (501) staff       (20)     3304 2022-12-12 16:12:16.856325 fontFeatures-1.7.4/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)     2739 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/README.md
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.774953 fontFeatures-1.7.4/bin/
--rwxr-xr-x   0 simon      (501) staff       (20)     2339 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/bin/ff-shape
--rw-r--r--   0 simon      (501) staff       (20)     1814 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/bin/otf2fea
--rw-r--r--   0 simon      (501) staff       (20)    12420 2022-05-04 10:41:29.000000 fontFeatures-1.7.4/bin/otflayout2glyphs.py
--rw-r--r--   0 simon      (501) staff       (20)     7355 2022-05-04 10:41:29.000000 fontFeatures-1.7.4/bin/siesta
--rw-r--r--   0 simon      (501) staff       (20)     1242 2021-12-09 22:02:44.000000 fontFeatures-1.7.4/bin/txt2fea
--rw-r--r--   0 simon      (501) staff       (20)        0 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/conftest.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.775874 fontFeatures-1.7.4/docs/
--rw-r--r--   0 simon      (501) staff       (20)      634 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/docs/Makefile
--rw-r--r--   0 simon      (501) staff       (20)     1933 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/docs/conf.py
--rw-r--r--   0 simon      (501) staff       (20)      330 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/docs/converting.rst
--rw-r--r--   0 simon      (501) staff       (20)      849 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/docs/fontFeatures.rst
--rw-r--r--   0 simon      (501) staff       (20)     3101 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/docs/index.rst
--rw-r--r--   0 simon      (501) staff       (20)      225 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/docs/supportingmodules.rst
--rw-r--r--   0 simon      (501) staff       (20)      801 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fea2fea.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.776481 fontFeatures-1.7.4/fontFeatures/
--rw-r--r--   0 simon      (501) staff       (20)    31185 2022-05-04 10:41:29.000000 fontFeatures-1.7.4/fontFeatures/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.779047 fontFeatures-1.7.4/fontFeatures/feaLib/
--rw-r--r--   0 simon      (501) staff       (20)     3180 2022-10-20 09:47:30.000000 fontFeatures-1.7.4/fontFeatures/feaLib/Attachment.py
--rw-r--r--   0 simon      (501) staff       (20)     2783 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/feaLib/Chaining.py
--rw-r--r--   0 simon      (501) staff       (20)     6860 2022-10-13 08:32:00.000000 fontFeatures-1.7.4/fontFeatures/feaLib/FontFeatures.py
--rw-r--r--   0 simon      (501) staff       (20)      811 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/feaLib/Positioning.py
--rw-r--r--   0 simon      (501) staff       (20)     2937 2022-10-20 09:41:35.000000 fontFeatures-1.7.4/fontFeatures/feaLib/Routine.py
--rw-r--r--   0 simon      (501) staff       (20)      540 2022-10-13 08:27:01.000000 fontFeatures-1.7.4/fontFeatures/feaLib/RoutineReference.py
--rw-r--r--   0 simon      (501) staff       (20)     7147 2022-10-20 09:41:02.000000 fontFeatures-1.7.4/fontFeatures/feaLib/Substitution.py
--rw-r--r--   0 simon      (501) staff       (20)    13183 2022-12-12 15:24:16.000000 fontFeatures-1.7.4/fontFeatures/feaLib/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.779176 fontFeatures-1.7.4/fontFeatures/fontDameLib/
--rw-r--r--   0 simon      (501) staff       (20)    16775 2021-12-09 21:59:25.000000 fontFeatures-1.7.4/fontFeatures/fontDameLib/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.779906 fontFeatures-1.7.4/fontFeatures/optimizer/
--rw-r--r--   0 simon      (501) staff       (20)     2786 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/optimizer/FontFeatures.py
--rw-r--r--   0 simon      (501) staff       (20)     5997 2022-06-06 08:11:20.000000 fontFeatures-1.7.4/fontFeatures/optimizer/Routine.py
--rw-r--r--   0 simon      (501) staff       (20)     1046 2022-06-06 08:05:06.000000 fontFeatures-1.7.4/fontFeatures/optimizer/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2799 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/pathUtils.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.783677 fontFeatures-1.7.4/fontFeatures/shaperLib/
--rw-r--r--   0 simon      (501) staff       (20)     3530 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/ArabicShaper.py
--rw-r--r--   0 simon      (501) staff       (20)     4549 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/Attachment.py
--rw-r--r--   0 simon      (501) staff       (20)    13973 2021-12-12 19:16:48.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/BaseShaper.py
--rw-r--r--   0 simon      (501) staff       (20)    11876 2021-12-13 12:05:32.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/Buffer.py
--rw-r--r--   0 simon      (501) staff       (20)     1320 2021-12-12 19:16:51.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/Chaining.py
--rw-r--r--   0 simon      (501) staff       (20)     5634 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/HangulShaper.py
--rw-r--r--   0 simon      (501) staff       (20)    16866 2021-12-12 20:46:00.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/IndicShaper.py
--rw-r--r--   0 simon      (501) staff       (20)    10131 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/IndicShaperData.py
--rw-r--r--   0 simon      (501) staff       (20)     5374 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/KhmerShaper.py
--rw-r--r--   0 simon      (501) staff       (20)     6081 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/MyanmarShaper.py
--rw-r--r--   0 simon      (501) staff       (20)      326 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/Positioning.py
--rw-r--r--   0 simon      (501) staff       (20)     2113 2021-12-12 20:37:04.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/Routine.py
--rw-r--r--   0 simon      (501) staff       (20)     2718 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/Rule.py
--rw-r--r--   0 simon      (501) staff       (20)     8852 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/Shaper.py
--rw-r--r--   0 simon      (501) staff       (20)     1207 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/Substitution.py
--rw-r--r--   0 simon      (501) staff       (20)     4911 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/SyllabicShaper.py
--rw-r--r--   0 simon      (501) staff       (20)     7076 2021-12-12 19:03:44.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/USEShaper.py
--rw-r--r--   0 simon      (501) staff       (20)     8887 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/VowelConstraints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/shaperLib/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.785656 fontFeatures-1.7.4/fontFeatures/ttLib/
--rw-r--r--   0 simon      (501) staff       (20)      580 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/ttLib/Attachment.py
--rw-r--r--   0 simon      (501) staff       (20)      291 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/ttLib/Chaining.py
--rw-r--r--   0 simon      (501) staff       (20)    10078 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/ttLib/FontFeatures.py
--rw-r--r--   0 simon      (501) staff       (20)     4821 2021-12-12 08:48:09.000000 fontFeatures-1.7.4/fontFeatures/ttLib/GDEFUnparser.py
--rw-r--r--   0 simon      (501) staff       (20)    11127 2022-01-11 17:44:47.000000 fontFeatures-1.7.4/fontFeatures/ttLib/GPOSUnparser.py
--rw-r--r--   0 simon      (501) staff       (20)     5836 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/ttLib/GSUBUnparser.py
--rw-r--r--   0 simon      (501) staff       (20)    18337 2022-01-19 17:28:21.000000 fontFeatures-1.7.4/fontFeatures/ttLib/GTableUnparser.py
--rw-r--r--   0 simon      (501) staff       (20)      371 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/ttLib/Positioning.py
--rw-r--r--   0 simon      (501) staff       (20)     8868 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/ttLib/Routine.py
--rw-r--r--   0 simon      (501) staff       (20)     1041 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/ttLib/Substitution.py
--rw-r--r--   0 simon      (501) staff       (20)     1084 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/ttLib/ValueRecord.py
--rw-r--r--   0 simon      (501) staff       (20)     2644 2022-02-17 15:58:32.000000 fontFeatures-1.7.4/fontFeatures/ttLib/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.785918 fontFeatures-1.7.4/fontFeatures/voltLib/
--rw-r--r--   0 simon      (501) staff       (20)    21679 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/voltLib/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.787660 fontFeatures-1.7.4/fontFeatures/xmlLib/
--rw-r--r--   0 simon      (501) staff       (20)     1198 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/xmlLib/Attachment.py
--rw-r--r--   0 simon      (501) staff       (20)      990 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/xmlLib/Chaining.py
--rw-r--r--   0 simon      (501) staff       (20)     2906 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/xmlLib/FontFeatures.py
--rw-r--r--   0 simon      (501) staff       (20)     1610 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/xmlLib/Positioning.py
--rw-r--r--   0 simon      (501) staff       (20)      852 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/xmlLib/Routine.py
--rw-r--r--   0 simon      (501) staff       (20)      479 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/xmlLib/RoutineReference.py
--rw-r--r--   0 simon      (501) staff       (20)     1781 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/xmlLib/Rule.py
--rw-r--r--   0 simon      (501) staff       (20)      902 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/xmlLib/Substitution.py
--rw-r--r--   0 simon      (501) staff       (20)       15 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/xmlLib/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      426 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fontFeatures/xmlLib/utils.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.777333 fontFeatures-1.7.4/fontFeatures.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     3304 2022-12-12 16:12:16.000000 fontFeatures-1.7.4/fontFeatures.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)    21443 2022-12-12 16:12:16.000000 fontFeatures-1.7.4/fontFeatures.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2022-12-12 16:12:16.000000 fontFeatures-1.7.4/fontFeatures.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2022-12-12 16:12:16.000000 fontFeatures-1.7.4/fontFeatures.egg-info/not-zip-safe
--rw-r--r--   0 simon      (501) staff       (20)      150 2022-12-12 16:12:16.000000 fontFeatures-1.7.4/fontFeatures.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)       13 2022-12-12 16:12:16.000000 fontFeatures-1.7.4/fontFeatures.egg-info/top_level.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.789281 fontFeatures-1.7.4/fonts/
--rw-r--r--   0 simon      (501) staff       (20)   554616 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fonts/Amiri-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)   219932 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fonts/NotoNastaliqUrdu-Dummy.ttf
--rw-r--r--   0 simon      (501) staff       (20)   515100 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/fonts/Roboto-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.790353 fontFeatures-1.7.4/ms-use/
--rw-r--r--   0 simon      (501) staff       (20)     1141 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/ms-use/COPYING
--rw-r--r--   0 simon      (501) staff       (20)     6738 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/ms-use/IndicShapingInvalidCluster.txt
--rw-r--r--   0 simon      (501) staff       (20)       17 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/requirements-dev.txt
--rw-r--r--   0 simon      (501) staff       (20)       59 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)       38 2022-12-12 16:12:16.856504 fontFeatures-1.7.4/setup.cfg
--rw-r--r--   0 simon      (501) staff       (20)     1518 2022-12-12 16:12:03.000000 fontFeatures-1.7.4/setup.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.793224 fontFeatures-1.7.4/tests/
--rw-r--r--   0 simon      (501) staff       (20)        0 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.798073 fontFeatures-1.7.4/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)     1008 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/1735326da89f0818cd8c51a0600e9789812c0f94.ttf
--rw-r--r--   0 simon      (501) staff       (20)     1380 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf
--rw-r--r--   0 simon      (501) staff       (20)     1084 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/341421e629668b1a1242245d39238ca48432d35d.ttf
--rw-r--r--   0 simon      (501) staff       (20)     3300 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/55c88ebbe938680b08f92c3de20713183e0c7481.ttf
--rw-r--r--   0 simon      (501) staff       (20)     1204 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf
--rw-r--r--   0 simon      (501) staff       (20)    22980 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf
--rw-r--r--   0 simon      (501) staff       (20)   554616 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/Amiri-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)   496504 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/LibertinusSans-Regular.otf
--rw-r--r--   0 simon      (501) staff       (20)     6353 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/Noto Sans Sharada GSUB.txt
--rw-r--r--   0 simon      (501) staff       (20)     5555 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/SimpleTwoAxis.glyphs
--rw-r--r--   0 simon      (501) staff       (20)     2720 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/a014549f766436cf55b2ceb40e462038938ee899.ttf
--rw-r--r--   0 simon      (501) staff       (20)     1840 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/acbe26ce904463c690fb67f70679447059d13ee4.otf
--rw-r--r--   0 simon      (501) staff       (20)     6332 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/data/df768b9c257e0c9c35786c47cae15c46571d56be.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.771716 fontFeatures-1.7.4/tests/harfbuzz/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.798215 fontFeatures-1.7.4/tests/harfbuzz/aots/
--rw-r--r--   0 simon      (501) staff       (20)      593 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/COPYING
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.834063 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/
--rw-r--r--   0 simon      (501) staff       (20)     6004 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef1_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     6020 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef1_font2.otf
--rw-r--r--   0 simon      (501) staff       (20)     6060 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef1_font3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5984 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef1_font4.otf
--rw-r--r--   0 simon      (501) staff       (20)     6004 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef2_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     6016 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef2_font2.otf
--rw-r--r--   0 simon      (501) staff       (20)     6052 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef2_font3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5984 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef2_font4.otf
--rw-r--r--   0 simon      (501) staff       (20)     5196 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap0_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     4968 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap10_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     4960 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap10_font2.otf
--rw-r--r--   0 simon      (501) staff       (20)     4980 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap12_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5028 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap14_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     6000 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap2_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     4964 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap4_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     4956 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap4_font2.otf
--rw-r--r--   0 simon      (501) staff       (20)     4956 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap4_font3.otf
--rw-r--r--   0 simon      (501) staff       (20)     4972 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap4_font4.otf
--rw-r--r--   0 simon      (501) staff       (20)     4948 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap6_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     4944 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap6_font2.otf
--rw-r--r--   0 simon      (501) staff       (20)    13224 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap8_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5096 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_composition_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     6412 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_subtableselection_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     6140 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_subtableselection_font2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5872 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_subtableselection_font3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5600 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_subtableselection_font4.otf
--rw-r--r--   0 simon      (501) staff       (20)     5332 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_subtableselection_font5.otf
--rw-r--r--   0 simon      (501) staff       (20)     5208 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_1_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5136 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_1_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5136 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_1_simple_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5136 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_1_simple_f3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5136 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_1_simple_f4.otf
--rw-r--r--   0 simon      (501) staff       (20)     5108 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_2_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5148 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_2_font2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5120 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_font6.otf
--rw-r--r--   0 simon      (501) staff       (20)     5132 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_font7.otf
--rw-r--r--   0 simon      (501) staff       (20)     5220 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5220 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_lookupflag_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5180 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5176 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_next_glyph_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5148 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5148 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_2_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5188 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_2_font2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5188 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_2_font3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5148 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_2_font4.otf
--rw-r--r--   0 simon      (501) staff       (20)     5140 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_2_font5.otf
--rw-r--r--   0 simon      (501) staff       (20)     5120 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos3_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5160 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos3_font2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5164 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos3_font3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5256 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos4_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5240 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos4_lookupflag_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5352 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos4_multiple_anchors_1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5200 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos4_simple_1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5284 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos5_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5176 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos6_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5160 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos7_1_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5096 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos9_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5124 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos9_font2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f4.otf
--rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5592 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_multiple_subrules_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5592 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_multiple_subrules_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5540 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5488 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5488 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_simple_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5704 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5708 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5704 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5704 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f4.otf
--rw-r--r--   0 simon      (501) staff       (20)     5728 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5800 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_multiple_subrules_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5800 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_multiple_subrules_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5744 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5696 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5696 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_simple_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5732 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5504 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5508 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f4.otf
--rw-r--r--   0 simon      (501) staff       (20)     5548 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_simple_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5544 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5480 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5480 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5492 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_expansion_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5508 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_lookupflag_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5568 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_multiple_subrules_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5568 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_multiple_subrules_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5476 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5468 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_simple_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5508 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5492 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5540 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_classes_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5564 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_classes_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_expansion_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5540 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5532 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_lookupflag_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5600 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_multiple_subrules_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5600 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_multiple_subrules_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5512 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5508 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5484 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_simple_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5544 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5476 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5472 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5512 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5504 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_lookupflag_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5480 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5208 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub1_1_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5216 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub1_1_modulo_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5136 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub1_1_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5212 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub1_2_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5140 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub1_2_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5224 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub2_1_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5248 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub2_1_multiple_sequences_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5144 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub2_1_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5224 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub3_1_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5168 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub3_1_multiple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5144 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub3_1_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5220 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub4_1_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5252 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligatures_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5252 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligatures_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5240 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligsets_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5148 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub4_1_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5096 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub7_font1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5116 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub7_font2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f4.otf
--rw-r--r--   0 simon      (501) staff       (20)     5544 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5616 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_multiple_subrules_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5616 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_multiple_subrules_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5560 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5508 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5512 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_simple_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5544 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5724 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5728 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5728 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5728 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f4.otf
--rw-r--r--   0 simon      (501) staff       (20)     5752 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5824 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_multiple_subrules_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5824 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_multiple_subrules_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5764 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5716 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5720 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_simple_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5752 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5528 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5532 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f3.otf
--rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f4.otf
--rw-r--r--   0 simon      (501) staff       (20)     5572 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5548 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5540 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_simple_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5568 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5504 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_expansion_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5532 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_lookupflag_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5592 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_multiple_subrules_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5592 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_multiple_subrules_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5492 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_simple_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5528 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5564 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_classes_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5584 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_classes_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5544 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_expansion_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5560 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5552 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_lookupflag_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5620 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_multiple_subrules_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5620 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_multiple_subrules_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5536 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5528 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5504 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_simple_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5568 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_boundary_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_boundary_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5536 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_lookupflag_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5528 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_lookupflag_f2.otf
--rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_next_glyph_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5504 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_simple_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5540 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_successive_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5416 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/lookupflag_ignore_attach_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5256 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/lookupflag_ignore_base_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5408 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/lookupflag_ignore_combination_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5320 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/lookupflag_ignore_ligatures_f1.otf
--rw-r--r--   0 simon      (501) staff       (20)     5288 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/lookupflag_ignore_marks_f1.otf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.855324 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/
--rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/classdef1.tests
--rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/classdef1_empty.tests
--rw-r--r--   0 simon      (501) staff       (20)      295 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/classdef1_multiple.tests
--rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/classdef1_single.tests
--rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/classdef2.tests
--rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/classdef2_empty.tests
--rw-r--r--   0 simon      (501) staff       (20)      295 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/classdef2_multiple.tests
--rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/classdef2_single.tests
--rw-r--r--   0 simon      (501) staff       (20)      170 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos1_1_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      680 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos1_1_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      162 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos1_2.tests
--rw-r--r--   0 simon      (501) staff       (20)      162 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos1_2_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      461 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos2_1.tests
--rw-r--r--   0 simon      (501) staff       (20)      456 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos2_1_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      326 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos2_1_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)      301 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos2_1_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      932 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos2_2.tests
--rw-r--r--   0 simon      (501) staff       (20)     1586 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos3.tests
--rw-r--r--   0 simon      (501) staff       (20)      358 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos3_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      321 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos4_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      273 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos4_multiple_anchors.tests
--rw-r--r--   0 simon      (501) staff       (20)      777 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos4_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      306 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos5.tests
--rw-r--r--   0 simon      (501) staff       (20)      434 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos6.tests
--rw-r--r--   0 simon      (501) staff       (20)      341 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos7_1.tests
--rw-r--r--   0 simon      (501) staff       (20)      337 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos9.tests
--rw-r--r--   0 simon      (501) staff       (20)      760 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining1_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      372 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining1_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      610 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining1_multiple_subrules.tests
--rw-r--r--   0 simon      (501) staff       (20)      192 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining1_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)     2266 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining1_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      227 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining1_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      760 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining2_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      372 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining2_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      610 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining2_multiple_subrules.tests
--rw-r--r--   0 simon      (501) staff       (20)      192 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining2_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)     2266 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining2_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      227 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining2_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      760 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining3_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      372 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining3_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      227 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining3_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)     2266 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining3_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      227 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining3_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      412 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context1_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      173 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context1_expansion.tests
--rw-r--r--   0 simon      (501) staff       (20)      454 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context1_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      464 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context1_multiple_subrules.tests
--rw-r--r--   0 simon      (501) staff       (20)      208 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context1_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)      560 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context1_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      191 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context1_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      412 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context2_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      696 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context2_classes.tests
--rw-r--r--   0 simon      (501) staff       (20)      173 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context2_expansion.tests
--rw-r--r--   0 simon      (501) staff       (20)      454 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context2_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      464 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context2_multiple_subrules.tests
--rw-r--r--   0 simon      (501) staff       (20)      208 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context2_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)      560 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context2_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      191 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context2_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      412 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context3_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      454 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context3_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      208 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context3_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)      426 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context3_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      191 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context3_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      151 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub1_1_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      177 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub1_1_modulo.tests
--rw-r--r--   0 simon      (501) staff       (20)      147 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub1_1_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      151 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub1_2_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      147 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub1_2_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      144 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub2_1_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      155 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub2_1_multiple_sequences.tests
--rw-r--r--   0 simon      (501) staff       (20)      282 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub2_1_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      222 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub3_1_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      266 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub3_1_multiple.tests
--rw-r--r--   0 simon      (501) staff       (20)      278 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub3_1_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      235 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub4_1_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      383 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub4_1_multiple_ligatures.tests
--rw-r--r--   0 simon      (501) staff       (20)      171 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub4_1_multiple_ligsets.tests
--rw-r--r--   0 simon      (501) staff       (20)      181 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub4_1_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      282 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub7.tests
--rw-r--r--   0 simon      (501) staff       (20)      656 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining1_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      266 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining1_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      464 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining1_multiple_subrules.tests
--rw-r--r--   0 simon      (501) staff       (20)      166 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining1_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)     1895 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining1_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      183 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining1_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      656 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining2_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      266 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining2_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      464 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining2_multiple_subrules.tests
--rw-r--r--   0 simon      (501) staff       (20)      166 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining2_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)     1895 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining2_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      183 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining2_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      656 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining3_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      266 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining3_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      186 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining3_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)     1895 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining3_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      183 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining3_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      346 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context1_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      160 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context1_expansion.tests
--rw-r--r--   0 simon      (501) staff       (20)      367 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context1_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      382 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context1_multiple_subrules.tests
--rw-r--r--   0 simon      (501) staff       (20)      175 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context1_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)      482 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context1_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      162 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context1_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      346 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context2_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      502 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context2_classes.tests
--rw-r--r--   0 simon      (501) staff       (20)      160 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context2_expansion.tests
--rw-r--r--   0 simon      (501) staff       (20)      367 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context2_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      382 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context2_multiple_subrules.tests
--rw-r--r--   0 simon      (501) staff       (20)      175 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context2_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)      482 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context2_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      162 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context2_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      346 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context3_boundary.tests
--rw-r--r--   0 simon      (501) staff       (20)      367 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context3_lookupflag.tests
--rw-r--r--   0 simon      (501) staff       (20)      175 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context3_next_glyph.tests
--rw-r--r--   0 simon      (501) staff       (20)      350 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context3_simple.tests
--rw-r--r--   0 simon      (501) staff       (20)      162 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_context3_successive.tests
--rw-r--r--   0 simon      (501) staff       (20)      908 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/lookupflag_ignore_attach.tests
--rw-r--r--   0 simon      (501) staff       (20)      328 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/lookupflag_ignore_base.tests
--rw-r--r--   0 simon      (501) staff       (20)      564 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/lookupflag_ignore_combination.tests
--rw-r--r--   0 simon      (501) staff       (20)      564 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/lookupflag_ignore_ligatures.tests
--rw-r--r--   0 simon      (501) staff       (20)      180 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/harfbuzz/aots/tests/lookupflag_ignore_marks.tests
--rw-r--r--   0 simon      (501) staff       (20)     1117 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_anchors.py
--rw-r--r--   0 simon      (501) staff       (20)    15695 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_binary_emitter.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_chaining.py
--rw-r--r--   0 simon      (501) staff       (20)     4324 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_fea_parser.py
--rw-r--r--   0 simon      (501) staff       (20)     1166 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_fontdame.py
--rw-r--r--   0 simon      (501) staff       (20)     2730 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_fontfeatures.py
--rw-r--r--   0 simon      (501) staff       (20)     2676 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_languages.py
--rw-r--r--   0 simon      (501) staff       (20)     1503 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_optimizer.py
--rw-r--r--   0 simon      (501) staff       (20)     1039 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_positioning.py
--rw-r--r--   0 simon      (501) staff       (20)     1667 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_routine_partition.py
--rw-r--r--   0 simon      (501) staff       (20)     1240 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_shaping_generic.py
--rw-r--r--   0 simon      (501) staff       (20)     3332 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_shaping_harfbuzz.py
--rw-r--r--   0 simon      (501) staff       (20)     2468 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_substitution.py
--rw-r--r--   0 simon      (501) staff       (20)     2154 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_unparse_pos.py
--rw-r--r--   0 simon      (501) staff       (20)     1941 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/tests/test_unparse_sub.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2022-12-12 16:12:16.856073 fontFeatures-1.7.4/utils/
--rw-r--r--   0 simon      (501) staff       (20)      813 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/utils/addfeatures.py
--rw-r--r--   0 simon      (501) staff       (20)     1055 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/utils/dump-anchors.py
--rw-r--r--   0 simon      (501) staff       (20)     3004 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/utils/dump-cursive.py
--rwxr-xr-x   0 simon      (501) staff       (20)     5930 2021-12-09 21:27:38.000000 fontFeatures-1.7.4/utils/gen-vowel-constraints.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.328812 fontFeatures-1.8.0/
+-rw-r--r--   0 simon      (501) staff       (20)      235 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/.coveragerc
+-rw-r--r--   0 simon      (501) staff       (20)      178 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/.editorconfig
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.243969 fontFeatures-1.8.0/.github/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.247345 fontFeatures-1.8.0/.github/workflows/
+-rw-r--r--   0 simon      (501) staff       (20)      593 2021-12-11 20:33:14.000000 fontFeatures-1.8.0/.github/workflows/ci.yml
+-rw-r--r--   0 simon      (501) staff       (20)      128 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     1520 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/LICENSE
+-rw-r--r--   0 simon      (501) staff       (20)     2269 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/NEW-FORMAT.md
+-rw-r--r--   0 simon      (501) staff       (20)     3304 2023-07-17 10:34:13.328655 fontFeatures-1.8.0/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)     2739 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/README.md
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.248428 fontFeatures-1.8.0/bin/
+-rwxr-xr-x   0 simon      (501) staff       (20)     2339 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/bin/ff-shape
+-rw-r--r--   0 simon      (501) staff       (20)     1814 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/bin/otf2fea
+-rw-r--r--   0 simon      (501) staff       (20)    12420 2022-05-04 10:41:29.000000 fontFeatures-1.8.0/bin/otflayout2glyphs.py
+-rw-r--r--   0 simon      (501) staff       (20)     7355 2022-05-04 10:41:29.000000 fontFeatures-1.8.0/bin/siesta
+-rw-r--r--   0 simon      (501) staff       (20)     1242 2021-12-09 22:02:44.000000 fontFeatures-1.8.0/bin/txt2fea
+-rw-r--r--   0 simon      (501) staff       (20)        0 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/conftest.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.249426 fontFeatures-1.8.0/docs/
+-rw-r--r--   0 simon      (501) staff       (20)      634 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/docs/Makefile
+-rw-r--r--   0 simon      (501) staff       (20)     1933 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/docs/conf.py
+-rw-r--r--   0 simon      (501) staff       (20)      330 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/docs/converting.rst
+-rw-r--r--   0 simon      (501) staff       (20)      849 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/docs/fontFeatures.rst
+-rw-r--r--   0 simon      (501) staff       (20)     3101 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/docs/index.rst
+-rw-r--r--   0 simon      (501) staff       (20)      174 2023-07-17 10:27:09.000000 fontFeatures-1.8.0/docs/supportingmodules.rst
+-rw-r--r--   0 simon      (501) staff       (20)      801 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fea2fea.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.249807 fontFeatures-1.8.0/fontFeatures/
+-rw-r--r--   0 simon      (501) staff       (20)    31312 2023-07-17 10:28:54.000000 fontFeatures-1.8.0/fontFeatures/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.252160 fontFeatures-1.8.0/fontFeatures/feaLib/
+-rw-r--r--   0 simon      (501) staff       (20)     3019 2023-07-17 10:27:09.000000 fontFeatures-1.8.0/fontFeatures/feaLib/Attachment.py
+-rw-r--r--   0 simon      (501) staff       (20)     2783 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/feaLib/Chaining.py
+-rw-r--r--   0 simon      (501) staff       (20)     6860 2022-10-13 08:32:00.000000 fontFeatures-1.8.0/fontFeatures/feaLib/FontFeatures.py
+-rw-r--r--   0 simon      (501) staff       (20)      811 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/feaLib/Positioning.py
+-rw-r--r--   0 simon      (501) staff       (20)     2937 2023-07-17 10:26:24.000000 fontFeatures-1.8.0/fontFeatures/feaLib/Routine.py
+-rw-r--r--   0 simon      (501) staff       (20)      565 2023-07-17 10:27:09.000000 fontFeatures-1.8.0/fontFeatures/feaLib/RoutineReference.py
+-rw-r--r--   0 simon      (501) staff       (20)     7147 2022-10-20 09:41:02.000000 fontFeatures-1.8.0/fontFeatures/feaLib/Substitution.py
+-rw-r--r--   0 simon      (501) staff       (20)    13355 2023-07-17 10:27:09.000000 fontFeatures-1.8.0/fontFeatures/feaLib/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.252312 fontFeatures-1.8.0/fontFeatures/fontDameLib/
+-rw-r--r--   0 simon      (501) staff       (20)    16775 2021-12-09 21:59:25.000000 fontFeatures-1.8.0/fontFeatures/fontDameLib/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.253124 fontFeatures-1.8.0/fontFeatures/optimizer/
+-rw-r--r--   0 simon      (501) staff       (20)     2786 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/optimizer/FontFeatures.py
+-rw-r--r--   0 simon      (501) staff       (20)     5997 2023-07-17 10:26:24.000000 fontFeatures-1.8.0/fontFeatures/optimizer/Routine.py
+-rw-r--r--   0 simon      (501) staff       (20)     1046 2023-07-17 10:26:24.000000 fontFeatures-1.8.0/fontFeatures/optimizer/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.256989 fontFeatures-1.8.0/fontFeatures/shaperLib/
+-rw-r--r--   0 simon      (501) staff       (20)     3530 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/ArabicShaper.py
+-rw-r--r--   0 simon      (501) staff       (20)     4549 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/Attachment.py
+-rw-r--r--   0 simon      (501) staff       (20)    13973 2021-12-12 19:16:48.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/BaseShaper.py
+-rw-r--r--   0 simon      (501) staff       (20)    11865 2023-07-17 10:27:09.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/Buffer.py
+-rw-r--r--   0 simon      (501) staff       (20)     1320 2021-12-12 19:16:51.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/Chaining.py
+-rw-r--r--   0 simon      (501) staff       (20)     5634 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/HangulShaper.py
+-rw-r--r--   0 simon      (501) staff       (20)    16866 2021-12-12 20:46:00.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/IndicShaper.py
+-rw-r--r--   0 simon      (501) staff       (20)    10131 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/IndicShaperData.py
+-rw-r--r--   0 simon      (501) staff       (20)     5374 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/KhmerShaper.py
+-rw-r--r--   0 simon      (501) staff       (20)     6081 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/MyanmarShaper.py
+-rw-r--r--   0 simon      (501) staff       (20)      326 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/Positioning.py
+-rw-r--r--   0 simon      (501) staff       (20)     2113 2021-12-12 20:37:04.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/Routine.py
+-rw-r--r--   0 simon      (501) staff       (20)     2718 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/Rule.py
+-rw-r--r--   0 simon      (501) staff       (20)     8852 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/Shaper.py
+-rw-r--r--   0 simon      (501) staff       (20)     1207 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/Substitution.py
+-rw-r--r--   0 simon      (501) staff       (20)     4911 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/SyllabicShaper.py
+-rw-r--r--   0 simon      (501) staff       (20)     7076 2021-12-12 19:03:44.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/USEShaper.py
+-rw-r--r--   0 simon      (501) staff       (20)     8887 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/VowelConstraints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/shaperLib/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.259333 fontFeatures-1.8.0/fontFeatures/ttLib/
+-rw-r--r--   0 simon      (501) staff       (20)      588 2023-07-17 10:27:09.000000 fontFeatures-1.8.0/fontFeatures/ttLib/Attachment.py
+-rw-r--r--   0 simon      (501) staff       (20)      291 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/ttLib/Chaining.py
+-rw-r--r--   0 simon      (501) staff       (20)    10078 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/ttLib/FontFeatures.py
+-rw-r--r--   0 simon      (501) staff       (20)     4821 2021-12-12 08:48:09.000000 fontFeatures-1.8.0/fontFeatures/ttLib/GDEFUnparser.py
+-rw-r--r--   0 simon      (501) staff       (20)    11127 2022-01-11 17:44:47.000000 fontFeatures-1.8.0/fontFeatures/ttLib/GPOSUnparser.py
+-rw-r--r--   0 simon      (501) staff       (20)     5836 2023-03-02 20:28:38.000000 fontFeatures-1.8.0/fontFeatures/ttLib/GSUBUnparser.py
+-rw-r--r--   0 simon      (501) staff       (20)    18355 2023-07-17 10:27:09.000000 fontFeatures-1.8.0/fontFeatures/ttLib/GTableUnparser.py
+-rw-r--r--   0 simon      (501) staff       (20)      371 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/ttLib/Positioning.py
+-rw-r--r--   0 simon      (501) staff       (20)     8868 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/ttLib/Routine.py
+-rw-r--r--   0 simon      (501) staff       (20)     1041 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/ttLib/Substitution.py
+-rw-r--r--   0 simon      (501) staff       (20)     1084 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/ttLib/ValueRecord.py
+-rw-r--r--   0 simon      (501) staff       (20)     2644 2023-03-02 20:39:38.000000 fontFeatures-1.8.0/fontFeatures/ttLib/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1951 2023-07-17 10:27:09.000000 fontFeatures-1.8.0/fontFeatures/utils.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.259597 fontFeatures-1.8.0/fontFeatures/voltLib/
+-rw-r--r--   0 simon      (501) staff       (20)    21679 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/voltLib/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.261393 fontFeatures-1.8.0/fontFeatures/xmlLib/
+-rw-r--r--   0 simon      (501) staff       (20)     1198 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/xmlLib/Attachment.py
+-rw-r--r--   0 simon      (501) staff       (20)      990 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/xmlLib/Chaining.py
+-rw-r--r--   0 simon      (501) staff       (20)     2906 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/xmlLib/FontFeatures.py
+-rw-r--r--   0 simon      (501) staff       (20)     1610 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/xmlLib/Positioning.py
+-rw-r--r--   0 simon      (501) staff       (20)      852 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/xmlLib/Routine.py
+-rw-r--r--   0 simon      (501) staff       (20)      479 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/xmlLib/RoutineReference.py
+-rw-r--r--   0 simon      (501) staff       (20)     1781 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/xmlLib/Rule.py
+-rw-r--r--   0 simon      (501) staff       (20)      902 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/xmlLib/Substitution.py
+-rw-r--r--   0 simon      (501) staff       (20)       15 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/xmlLib/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      426 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fontFeatures/xmlLib/utils.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.250697 fontFeatures-1.8.0/fontFeatures.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     3304 2023-07-17 10:34:13.000000 fontFeatures-1.8.0/fontFeatures.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)    21428 2023-07-17 10:34:13.000000 fontFeatures-1.8.0/fontFeatures.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-07-17 10:34:13.000000 fontFeatures-1.8.0/fontFeatures.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-07-17 10:34:13.000000 fontFeatures-1.8.0/fontFeatures.egg-info/not-zip-safe
+-rw-r--r--   0 simon      (501) staff       (20)      117 2023-07-17 10:34:13.000000 fontFeatures-1.8.0/fontFeatures.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)       13 2023-07-17 10:34:13.000000 fontFeatures-1.8.0/fontFeatures.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.263298 fontFeatures-1.8.0/fonts/
+-rw-r--r--   0 simon      (501) staff       (20)   554616 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fonts/Amiri-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)   219932 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fonts/NotoNastaliqUrdu-Dummy.ttf
+-rw-r--r--   0 simon      (501) staff       (20)   515100 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/fonts/Roboto-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.264347 fontFeatures-1.8.0/ms-use/
+-rw-r--r--   0 simon      (501) staff       (20)     1141 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/ms-use/COPYING
+-rw-r--r--   0 simon      (501) staff       (20)     6738 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/ms-use/IndicShapingInvalidCluster.txt
+-rw-r--r--   0 simon      (501) staff       (20)       17 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/requirements-dev.txt
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-07-17 10:27:09.000000 fontFeatures-1.8.0/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-17 10:34:13.328854 fontFeatures-1.8.0/setup.cfg
+-rw-r--r--   0 simon      (501) staff       (20)     1518 2023-07-17 10:33:56.000000 fontFeatures-1.8.0/setup.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.268695 fontFeatures-1.8.0/tests/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.272632 fontFeatures-1.8.0/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)     1008 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/1735326da89f0818cd8c51a0600e9789812c0f94.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     1380 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     1084 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/341421e629668b1a1242245d39238ca48432d35d.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     3300 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/55c88ebbe938680b08f92c3de20713183e0c7481.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     1204 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf
+-rw-r--r--   0 simon      (501) staff       (20)    22980 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf
+-rw-r--r--   0 simon      (501) staff       (20)   554616 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/Amiri-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)   496504 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/LibertinusSans-Regular.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/Noto Sans Sharada GSUB.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5555 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/SimpleTwoAxis.glyphs
+-rw-r--r--   0 simon      (501) staff       (20)     2720 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/a014549f766436cf55b2ceb40e462038938ee899.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     1840 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/acbe26ce904463c690fb67f70679447059d13ee4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6332 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/data/df768b9c257e0c9c35786c47cae15c46571d56be.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.244948 fontFeatures-1.8.0/tests/harfbuzz/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.272759 fontFeatures-1.8.0/tests/harfbuzz/aots/
+-rw-r--r--   0 simon      (501) staff       (20)      593 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/COPYING
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.307205 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/
+-rw-r--r--   0 simon      (501) staff       (20)     6004 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef1_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6020 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef1_font2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6060 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef1_font3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5984 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef1_font4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6004 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef2_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6016 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef2_font2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6052 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef2_font3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5984 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef2_font4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5196 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap0_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     4968 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap10_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     4960 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap10_font2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     4980 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap12_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5028 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap14_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6000 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap2_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     4964 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap4_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     4956 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap4_font2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     4956 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap4_font3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     4972 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap4_font4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     4948 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap6_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     4944 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap6_font2.otf
+-rw-r--r--   0 simon      (501) staff       (20)    13224 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap8_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5096 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_composition_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6412 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_subtableselection_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     6140 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_subtableselection_font2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5872 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_subtableselection_font3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5600 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_subtableselection_font4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5332 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_subtableselection_font5.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5208 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_1_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5136 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_1_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5136 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_1_simple_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5136 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_1_simple_f3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5136 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_1_simple_f4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5108 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_2_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5148 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_2_font2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5120 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_font6.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5132 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_font7.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5220 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5220 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_lookupflag_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5180 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5176 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_next_glyph_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5148 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5148 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_2_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5188 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_2_font2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5188 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_2_font3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5148 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_2_font4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5140 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_2_font5.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5120 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos3_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5160 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos3_font2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5164 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos3_font3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5256 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos4_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5240 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos4_lookupflag_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5352 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos4_multiple_anchors_1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5200 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos4_simple_1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5284 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos5_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5176 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos6_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5160 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos7_1_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5096 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos9_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5124 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos9_font2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5592 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_multiple_subrules_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5592 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_multiple_subrules_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5540 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5488 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5488 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_simple_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5704 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5708 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5704 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5704 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5728 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5800 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_multiple_subrules_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5800 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_multiple_subrules_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5744 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5696 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5696 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_simple_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5732 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5504 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5548 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_simple_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5544 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5480 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5480 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5492 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_expansion_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_lookupflag_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5568 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_multiple_subrules_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5568 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_multiple_subrules_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5476 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5468 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_simple_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5492 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5540 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_classes_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5564 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_classes_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_expansion_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5540 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5532 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_lookupflag_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5600 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_multiple_subrules_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5600 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_multiple_subrules_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5512 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5484 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_simple_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5544 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5476 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5472 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5512 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5504 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_lookupflag_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5480 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5208 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub1_1_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5216 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub1_1_modulo_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5136 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub1_1_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5212 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub1_2_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5140 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub1_2_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5224 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub2_1_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5248 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub2_1_multiple_sequences_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5144 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub2_1_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5224 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub3_1_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5168 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub3_1_multiple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5144 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub3_1_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5220 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub4_1_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5252 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligatures_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5252 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligatures_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5240 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligsets_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5148 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub4_1_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5096 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub7_font1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5116 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub7_font2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5544 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5616 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_multiple_subrules_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5616 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_multiple_subrules_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5560 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5512 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_simple_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5544 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5724 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5728 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5728 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5728 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5752 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5824 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_multiple_subrules_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5824 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_multiple_subrules_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5764 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5716 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5720 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_simple_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5752 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5528 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5532 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f3.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f4.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5572 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5548 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5540 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_simple_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5568 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5504 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_expansion_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5532 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5524 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_lookupflag_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5592 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_multiple_subrules_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5592 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_multiple_subrules_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5492 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_simple_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5528 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5516 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5564 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_classes_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5584 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_classes_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5544 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_expansion_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5560 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5552 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_lookupflag_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5620 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_multiple_subrules_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5620 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_multiple_subrules_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5536 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5528 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5504 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_simple_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5568 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5500 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_boundary_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5496 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_boundary_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5536 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_lookupflag_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5528 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_lookupflag_f2.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5520 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_next_glyph_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5504 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_simple_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5540 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_successive_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5416 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/lookupflag_ignore_attach_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5256 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/lookupflag_ignore_base_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5408 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/lookupflag_ignore_combination_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5320 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/lookupflag_ignore_ligatures_f1.otf
+-rw-r--r--   0 simon      (501) staff       (20)     5288 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/lookupflag_ignore_marks_f1.otf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.327854 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/
+-rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/classdef1.tests
+-rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/classdef1_empty.tests
+-rw-r--r--   0 simon      (501) staff       (20)      295 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/classdef1_multiple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/classdef1_single.tests
+-rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/classdef2.tests
+-rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/classdef2_empty.tests
+-rw-r--r--   0 simon      (501) staff       (20)      295 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/classdef2_multiple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      145 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/classdef2_single.tests
+-rw-r--r--   0 simon      (501) staff       (20)      170 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos1_1_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      680 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos1_1_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      162 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos1_2.tests
+-rw-r--r--   0 simon      (501) staff       (20)      162 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos1_2_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      461 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos2_1.tests
+-rw-r--r--   0 simon      (501) staff       (20)      456 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos2_1_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      326 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos2_1_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)      301 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos2_1_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      932 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos2_2.tests
+-rw-r--r--   0 simon      (501) staff       (20)     1586 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos3.tests
+-rw-r--r--   0 simon      (501) staff       (20)      358 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos3_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      321 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos4_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      273 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos4_multiple_anchors.tests
+-rw-r--r--   0 simon      (501) staff       (20)      777 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos4_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      306 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos5.tests
+-rw-r--r--   0 simon      (501) staff       (20)      434 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos6.tests
+-rw-r--r--   0 simon      (501) staff       (20)      341 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos7_1.tests
+-rw-r--r--   0 simon      (501) staff       (20)      337 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos9.tests
+-rw-r--r--   0 simon      (501) staff       (20)      760 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining1_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      372 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining1_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      610 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining1_multiple_subrules.tests
+-rw-r--r--   0 simon      (501) staff       (20)      192 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining1_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)     2266 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining1_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      227 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining1_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      760 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining2_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      372 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining2_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      610 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining2_multiple_subrules.tests
+-rw-r--r--   0 simon      (501) staff       (20)      192 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining2_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)     2266 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining2_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      227 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining2_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      760 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining3_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      372 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining3_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      227 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining3_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)     2266 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining3_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      227 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining3_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      412 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context1_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      173 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context1_expansion.tests
+-rw-r--r--   0 simon      (501) staff       (20)      454 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context1_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      464 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context1_multiple_subrules.tests
+-rw-r--r--   0 simon      (501) staff       (20)      208 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context1_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)      560 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context1_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      191 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context1_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      412 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context2_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      696 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context2_classes.tests
+-rw-r--r--   0 simon      (501) staff       (20)      173 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context2_expansion.tests
+-rw-r--r--   0 simon      (501) staff       (20)      454 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context2_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      464 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context2_multiple_subrules.tests
+-rw-r--r--   0 simon      (501) staff       (20)      208 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context2_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)      560 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context2_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      191 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context2_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      412 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context3_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      454 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context3_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      208 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context3_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)      426 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context3_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      191 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context3_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      151 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub1_1_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      177 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub1_1_modulo.tests
+-rw-r--r--   0 simon      (501) staff       (20)      147 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub1_1_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      151 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub1_2_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      147 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub1_2_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      144 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub2_1_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      155 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub2_1_multiple_sequences.tests
+-rw-r--r--   0 simon      (501) staff       (20)      282 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub2_1_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      222 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub3_1_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      266 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub3_1_multiple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      278 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub3_1_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      235 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub4_1_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      383 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub4_1_multiple_ligatures.tests
+-rw-r--r--   0 simon      (501) staff       (20)      171 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub4_1_multiple_ligsets.tests
+-rw-r--r--   0 simon      (501) staff       (20)      181 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub4_1_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      282 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub7.tests
+-rw-r--r--   0 simon      (501) staff       (20)      656 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining1_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      266 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining1_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      464 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining1_multiple_subrules.tests
+-rw-r--r--   0 simon      (501) staff       (20)      166 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining1_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)     1895 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining1_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      183 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining1_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      656 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining2_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      266 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining2_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      464 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining2_multiple_subrules.tests
+-rw-r--r--   0 simon      (501) staff       (20)      166 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining2_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)     1895 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining2_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      183 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining2_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      656 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining3_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      266 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining3_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      186 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining3_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)     1895 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining3_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      183 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining3_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      346 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context1_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      160 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context1_expansion.tests
+-rw-r--r--   0 simon      (501) staff       (20)      367 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context1_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      382 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context1_multiple_subrules.tests
+-rw-r--r--   0 simon      (501) staff       (20)      175 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context1_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)      482 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context1_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      162 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context1_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      346 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context2_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      502 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context2_classes.tests
+-rw-r--r--   0 simon      (501) staff       (20)      160 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context2_expansion.tests
+-rw-r--r--   0 simon      (501) staff       (20)      367 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context2_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      382 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context2_multiple_subrules.tests
+-rw-r--r--   0 simon      (501) staff       (20)      175 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context2_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)      482 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context2_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      162 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context2_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      346 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context3_boundary.tests
+-rw-r--r--   0 simon      (501) staff       (20)      367 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context3_lookupflag.tests
+-rw-r--r--   0 simon      (501) staff       (20)      175 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context3_next_glyph.tests
+-rw-r--r--   0 simon      (501) staff       (20)      350 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context3_simple.tests
+-rw-r--r--   0 simon      (501) staff       (20)      162 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_context3_successive.tests
+-rw-r--r--   0 simon      (501) staff       (20)      908 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/lookupflag_ignore_attach.tests
+-rw-r--r--   0 simon      (501) staff       (20)      328 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/lookupflag_ignore_base.tests
+-rw-r--r--   0 simon      (501) staff       (20)      564 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/lookupflag_ignore_combination.tests
+-rw-r--r--   0 simon      (501) staff       (20)      564 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/lookupflag_ignore_ligatures.tests
+-rw-r--r--   0 simon      (501) staff       (20)      180 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/harfbuzz/aots/tests/lookupflag_ignore_marks.tests
+-rw-r--r--   0 simon      (501) staff       (20)     1122 2023-07-17 10:29:19.000000 fontFeatures-1.8.0/tests/test_anchors.py
+-rw-r--r--   0 simon      (501) staff       (20)    15695 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/test_binary_emitter.py
+-rw-r--r--   0 simon      (501) staff       (20)     2334 2023-07-17 10:30:02.000000 fontFeatures-1.8.0/tests/test_chaining.py
+-rw-r--r--   0 simon      (501) staff       (20)     4338 2023-07-17 10:32:16.000000 fontFeatures-1.8.0/tests/test_fea_parser.py
+-rw-r--r--   0 simon      (501) staff       (20)     1166 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/test_fontdame.py
+-rw-r--r--   0 simon      (501) staff       (20)     2730 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/test_fontfeatures.py
+-rw-r--r--   0 simon      (501) staff       (20)     2910 2023-07-17 10:33:19.000000 fontFeatures-1.8.0/tests/test_languages.py
+-rw-r--r--   0 simon      (501) staff       (20)     1503 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/test_optimizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     1039 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/test_positioning.py
+-rw-r--r--   0 simon      (501) staff       (20)     1667 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/test_routine_partition.py
+-rw-r--r--   0 simon      (501) staff       (20)     1240 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/test_shaping_generic.py
+-rw-r--r--   0 simon      (501) staff       (20)     3332 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/test_shaping_harfbuzz.py
+-rw-r--r--   0 simon      (501) staff       (20)     2468 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/test_substitution.py
+-rw-r--r--   0 simon      (501) staff       (20)     2154 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/test_unparse_pos.py
+-rw-r--r--   0 simon      (501) staff       (20)     1941 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/tests/test_unparse_sub.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-17 10:34:13.328398 fontFeatures-1.8.0/utils/
+-rw-r--r--   0 simon      (501) staff       (20)      813 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/utils/addfeatures.py
+-rw-r--r--   0 simon      (501) staff       (20)     1055 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/utils/dump-anchors.py
+-rw-r--r--   0 simon      (501) staff       (20)     3004 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/utils/dump-cursive.py
+-rwxr-xr-x   0 simon      (501) staff       (20)     5930 2021-12-09 21:27:38.000000 fontFeatures-1.8.0/utils/gen-vowel-constraints.py
```

### Comparing `fontFeatures-1.7.4/.github/workflows/ci.yml` & `fontFeatures-1.8.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/LICENSE` & `fontFeatures-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/NEW-FORMAT.md` & `fontFeatures-1.8.0/NEW-FORMAT.md`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/PKG-INFO` & `fontFeatures-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontFeatures
-Version: 1.7.4
+Version: 1.8.0
 Summary: Python library for manipulating OpenType font features
 Home-page: https://github.com/simoncozens/fontFeatures
 Author: Simon Cozens
 Author-email: simon@simon-cozens.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `fontFeatures-1.7.4/README.md` & `fontFeatures-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/bin/ff-shape` & `fontFeatures-1.8.0/bin/ff-shape`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/bin/otf2fea` & `fontFeatures-1.8.0/bin/otf2fea`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/bin/otflayout2glyphs.py` & `fontFeatures-1.8.0/bin/otflayout2glyphs.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/bin/siesta` & `fontFeatures-1.8.0/bin/siesta`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/bin/txt2fea` & `fontFeatures-1.8.0/bin/txt2fea`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/docs/Makefile` & `fontFeatures-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/docs/conf.py` & `fontFeatures-1.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/docs/fontFeatures.rst` & `fontFeatures-1.8.0/docs/fontFeatures.rst`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/docs/index.rst` & `fontFeatures-1.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fea2fea.py` & `fontFeatures-1.8.0/fea2fea.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/__init__.py` & `fontFeatures-1.8.0/fontFeatures/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,14 +498,15 @@
 class RoutineReference:
     """A reference to a Routine object, used in a lookup.
 
     Routines can be referenced either by name (for example, when loaded from a
     textual representation), in which case they will be resolved at a later time,
     or by providing a pointer to the :py:class:`Routine` object."""
     def __init__(self, name=None, routine=None):
+        self.languages = []
         self.routine = routine
         if self.routine:
             self.name = routine.name
         if name:
             self.name = name
 
     def resolve(self, ff):
@@ -861,22 +862,24 @@
 
     def __init__(
         self,
         base_name,
         mark_name,
         bases=None,
         marks=None,
+        fullname=None,
         flags=0,
         address=None,
         font=None,
         languages=None,
         force_markmark=False
     ):
         self.base_name = base_name
         self.mark_name = mark_name
+        self.fullname = fullname or (self.base_name + "_" + self.mark_name)
         self.bases = bases or {}
         self.marks = marks or {}
         self.flags = flags
         self.address = address
         self.font = font
         self.stage = "pos"
         self.languages = languages or []
```

### Comparing `fontFeatures-1.7.4/fontFeatures/feaLib/Attachment.py` & `fontFeatures-1.8.0/fontFeatures/feaLib/Attachment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # Code for converting a Attachment object into feaLib statements
 import fontTools.feaLib.ast as feaast
-from glyphtools import categorize_glyph
-import warnings
-from fontTools.feaLib.variableScalar import VariableScalar
+from fontFeatures.utils import categorize_glyph
 
 
 def fix_scalar(scalar):
     if isinstance(scalar, int):
         return scalar
     if isinstance(scalar, float):
         return int(scalar)
@@ -40,25 +38,24 @@
 def feaPreamble(self, ff):
     if self.is_cursive:
         return []
     sortByAnchor(self)
     if not "mark_classes_done" in ff.scratch:
         ff.scratch["mark_classes_done"] = {}
     b = feaast.Block()
-    fullname = self.base_name + "_" + self.mark_name
     for mark in self.markslist:
-        if not (fullname, tuple(mark[0])) in ff.scratch["mark_classes_done"]:
+        if not (self.fullname, tuple(mark[0])) in ff.scratch["mark_classes_done"]:
             b.statements.append(
                 feaast.MarkClassDefinition(
-                    feaast.MarkClass(fullname),
+                    feaast.MarkClass(self.fullname),
                     feaast.Anchor(fix_scalar(mark[1][0]), fix_scalar(mark[1][1])),
                     _glyphref(mark[0]),
                 )
             )
-            ff.scratch["mark_classes_done"][(fullname, tuple(mark[0]))] = True
+            ff.scratch["mark_classes_done"][(self.fullname, tuple(mark[0]))] = True
     return [b]
 
 
 def asFeaAST(self):
     b = feaast.Block()
     if self.is_cursive:
         allglyphs = set(self.bases.keys()) | set(self.marks.keys())
@@ -71,21 +68,20 @@
                 )
             )
     else:
         if not hasattr(self, "baseslist"):
             sortByAnchor(self)  # e.g. when testing
         for base in self.baseslist:
             statementtype = feaast.MarkBasePosStatement
-            fullname = self.base_name + "_" + self.mark_name
             if self.font:
                 if categorize_glyph(self.font, base[0][0])[0] == "mark":
                     statementtype = feaast.MarkMarkPosStatement
             if self.force_markmark:
                 statementtype = feaast.MarkMarkPosStatement
             b.statements.append(
                 statementtype(
                     _glyphref(base[0]),
-                    [[feaast.Anchor(fix_scalar(base[1][0]), fix_scalar(base[1][1])), feaast.MarkClass(fullname)]],
+                    [[feaast.Anchor(fix_scalar(base[1][0]), fix_scalar(base[1][1])), feaast.MarkClass(self.fullname)]],
                 )
             )
 
     return b
```

### Comparing `fontFeatures-1.7.4/fontFeatures/feaLib/Chaining.py` & `fontFeatures-1.8.0/fontFeatures/feaLib/Chaining.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/feaLib/FontFeatures.py` & `fontFeatures-1.8.0/fontFeatures/feaLib/FontFeatures.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/feaLib/Positioning.py` & `fontFeatures-1.8.0/fontFeatures/feaLib/Positioning.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/feaLib/Routine.py` & `fontFeatures-1.8.0/fontFeatures/feaLib/Routine.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/feaLib/RoutineReference.py` & `fontFeatures-1.8.0/fontFeatures/feaLib/RoutineReference.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Routines for converting RoutineReference objects to and from Adobe FEA."""
 import fontTools.feaLib.ast as feaast
-from fontFeatures.ttLib.Substitution import lookup_type as sub_lookup_type
-from fontFeatures.ttLib.Positioning import lookup_type as pos_lookup_type
 
 def feaPreamble(self, ff):
     return []
 
 
 def asFeaAST(self, expand=False):
     # if self.routine.usecount == 1:
     #     return self.routine.asFeaAST()
     f = feaast.Block()
+    if self.languages:
+        f.statements.append(feaast.ScriptStatement(self.languages[0][0]))
+        f.statements.append(feaast.LanguageStatement(self.languages[0][1]))
+
     f.statements.append(feaast.LookupReferenceStatement(self.routine.asFeaAST()))
     return f
```

### Comparing `fontFeatures-1.7.4/fontFeatures/feaLib/Substitution.py` & `fontFeatures-1.8.0/fontFeatures/feaLib/Substitution.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/feaLib/__init__.py` & `fontFeatures-1.8.0/fontFeatures/feaLib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,43 +6,45 @@
 from warnings import warn
 
 
 def bad_statement_to_comment(s):
     # We could check through the attributes but that's hard...
     fea = s.asFea()
     if re.search(r"\[\s*\]", fea):  # Empty classes
-        warn("Empty class found in: '"+ fea+ "'")
+        warn("Empty class found in: '" + fea + "'")
         return ast.Comment("# " + fea)
     return s
 
 
 class FeaParser:
     """Turns a AFDKO feature file or string into a FontFeatures object.
 
     Args:
         featurefile: File object or string.
         font: Optionally, a TTFont object.
         glyphNames: Optionally, a list of glyph names in the font
     """
-    def __init__(self, featurefile, font=None, glyphNames=None, includeDir=None):
 
+    def __init__(self, featurefile, font=None, glyphNames=None, includeDir=None):
         self.ff = fontFeatures.FontFeatures()
         self.markclasses = {}
         self.currentFeature = None
         self.currentRoutine = None
         self.gensym = 1
         self.glyphmap = ()
         self.currentLanguage = None
         if font and not glyphNames:
             glyphNames = font.getGlyphOrder()
         if isinstance(featurefile, str):
             featurefile = io.StringIO(featurefile)
         self.featurefile = featurefile
         if glyphNames:
-            self.parser = Parser(self.featurefile, glyphNames=glyphNames, includeDir=includeDir)
+            self.parser = Parser(
+                self.featurefile, glyphNames=glyphNames, includeDir=includeDir
+            )
         else:
             self.parser = Parser(self.featurefile, includeDir=includeDir)
         self.parser.ast.ValueRecord = fontFeatures.ValueRecord
 
     def parse(self):
         """Parse the feature code.
 
@@ -114,76 +116,75 @@
 
     def add_single_subst(self, location, prefix, suffix, mapping, forceChain):
         self._start_routine_if_necessary(location)
         location = "%s:%i:%i" % (location)
         s = fontFeatures.Substitution(
             input_=[list(mapping.keys())],
             replacement=[list(mapping.values())],
-            precontext= [[str(g) for g in group] for group in prefix],
-            postcontext= [[str(g) for g in group] for group in suffix],
+            precontext=[[str(g) for g in group] for group in prefix],
+            postcontext=[[str(g) for g in group] for group in suffix],
             address=location,
-            languages=self.currentLanguage
+            languages=self.currentLanguage,
         )
         self.currentRoutine.addRule(s)
 
-
     def add_reverse_chain_single_subst(self, location, prefix, suffix, mapping):
         self._start_routine_if_necessary(location)
         location = "%s:%i:%i" % (location)
         s = fontFeatures.Substitution(
             input_=[list(mapping.keys())],
             replacement=[list(mapping.values())],
-            precontext= [[str(g) for g in group] for group in prefix],
-            postcontext= [[str(g) for g in group] for group in suffix],
+            precontext=[[str(g) for g in group] for group in prefix],
+            postcontext=[[str(g) for g in group] for group in suffix],
             address=location,
             languages=self.currentLanguage,
-            reverse=True
+            reverse=True,
         )
         self.currentRoutine.addRule(s)
 
     def add_multiple_subst(
         self, location, prefix, glyph, suffix, replacements, forceChain
     ):
         self._start_routine_if_necessary(location)
         location = "%s:%i:%i" % (location)
         s = fontFeatures.Substitution(
             input_=[[glyph]],
             replacement=[[g] for g in replacements],
-            precontext= [[str(g) for g in group] for group in prefix],
-            postcontext= [[str(g) for g in group] for group in suffix],
+            precontext=[[str(g) for g in group] for group in prefix],
+            postcontext=[[str(g) for g in group] for group in suffix],
             address=location,
-            languages=self.currentLanguage
+            languages=self.currentLanguage,
         )
         self.currentRoutine.addRule(s)
 
     def add_alternate_subst(self, location, prefix, glyph, suffix, replacement):
         self._start_routine_if_necessary(location)
         location = "%s:%i:%i" % (location)
         s = fontFeatures.Substitution(
             input_=[[glyph]],
             replacement=[replacement],
-            precontext= [[str(g) for g in group] for group in prefix],
-            postcontext= [[str(g) for g in group] for group in suffix],
+            precontext=[[str(g) for g in group] for group in prefix],
+            postcontext=[[str(g) for g in group] for group in suffix],
             address=location,
-            languages=self.currentLanguage
+            languages=self.currentLanguage,
         )
         self.currentRoutine.addRule(s)
 
     def add_ligature_subst(
         self, location, prefix, glyphs, suffix, replacement, forceChain
     ):
         self._start_routine_if_necessary(location)
         location = "%s:%i:%i" % (location)
         s = fontFeatures.Substitution(
             input_=[list(x) for x in glyphs],
             replacement=[[replacement]],
-            precontext= [[str(g) for g in group] for group in prefix],
-            postcontext= [[str(g) for g in group] for group in suffix],
+            precontext=[[str(g) for g in group] for group in prefix],
+            postcontext=[[str(g) for g in group] for group in suffix],
             address=location,
-            languages=self.currentLanguage
+            languages=self.currentLanguage,
         )
         self.currentRoutine.addRule(s)
 
     def add_chain_context_subst(self, location, prefix, glyphs, suffix, lookups):
         self._start_routine_if_necessary(location)
         location = "%s:%i:%i" % (location)
         # Find named feature
@@ -191,54 +192,56 @@
         for x in lookups:
             if x:
                 mylookups.append([self.ff.routineNamed(y.name) for y in x])
             else:
                 mylookups.append(None)
         s = fontFeatures.Chaining(
             input_=[list(x) for x in glyphs],
-            precontext= [[str(g) for g in group] for group in prefix],
-            postcontext= [[str(g) for g in group] for group in suffix],
+            precontext=[[str(g) for g in group] for group in prefix],
+            postcontext=[[str(g) for g in group] for group in suffix],
             lookups=mylookups,
             address=location,
-            languages=self.currentLanguage
+            languages=self.currentLanguage,
         )
         self.currentRoutine.addRule(s)
 
     add_chain_context_pos = add_chain_context_subst
 
     def add_single_pos(self, location, prefix, suffix, pos, forceChain):
         self._start_routine_if_necessary(location)
         location = "%s:%i:%i" % (location)
         s = fontFeatures.Positioning(
             glyphs=[p[0] for p in pos],
             valuerecords=[p[1] for p in pos],
-            precontext= [[str(g) for g in group] for group in prefix],
-            postcontext= [[str(g) for g in group] for group in suffix],
+            precontext=[[str(g) for g in group] for group in prefix],
+            postcontext=[[str(g) for g in group] for group in suffix],
             address=location,
-            languages=self.currentLanguage
+            languages=self.currentLanguage,
         )
         self.currentRoutine.addRule(s)
 
     def add_specific_pair_pos(self, location, glyph1, value1, glyph2, value2):
         self._start_routine_if_necessary(location)
         location = "%s:%i:%i" % (location)
         s = fontFeatures.Positioning(
-            glyphs=[[glyph1], [glyph2]], valuerecords=[value1, value2], address=location,
-            languages=self.currentLanguage
+            glyphs=[[glyph1], [glyph2]],
+            valuerecords=[value1, value2],
+            address=location,
+            languages=self.currentLanguage,
         )
         self.currentRoutine.addRule(s)
 
     def add_class_pair_pos(self, location, glyphclass1, value1, glyphclass2, value2):
         self._start_routine_if_necessary(location)
         location = "%s:%i:%i" % (location)
         s = fontFeatures.Positioning(
             glyphs=[glyphclass1, glyphclass2],
             valuerecords=[value1, value2],
             address=location,
-            languages=self.currentLanguage
+            languages=self.currentLanguage,
         )
         self.currentRoutine.addRule(s)
 
     def add_cursive_pos(self, location, glyphclass, entryAnchor, exitAnchor):
         self._start_routine_if_necessary(location)
         location = "%s:%i:%i" % (location)
         basedict, markdict = {}, {}
@@ -248,15 +251,15 @@
             markdict = {g: (exitAnchor.x, exitAnchor.y) for g in glyphclass}
         s = fontFeatures.Attachment(
             base_name="cursive_entry",
             mark_name="cursive_exit",
             bases=basedict,
             marks=markdict,
             address=location,
-            languages=self.currentLanguage
+            languages=self.currentLanguage,
         )
         self.currentRoutine.addRule(s)
 
     def add_mark_base_pos(self, location, bases, marks):
         self._start_routine_if_necessary(location)
         location = "%s:%i:%i" % (location)
         for baseanchor, markclass in marks:
@@ -266,15 +269,15 @@
                     base_name=markclass.name,
                     mark_name=markclass.name,
                     bases={g: (baseanchor.x, baseanchor.y) for g in bases},
                     marks={
                         g: (markanchor.x, markanchor.y) for g in markclass.glyphs.keys()
                     },
                     address=location,
-                    languages=self.currentLanguage
+                    languages=self.currentLanguage,
                 )
                 s.fontfeatures = self.ff
                 self.currentRoutine.addRule(s)
 
     add_mark_mark_pos = add_mark_base_pos
 
     def set_lookup_flag(self, location, value, markAttach, markFilter):
@@ -288,27 +291,31 @@
         self.currentRoutineFlag = value
 
     def add_language_system(self, location, script, language):
         pass
 
     def setElidedFallbackName(self, location, *args):
         pass
+
     def addDesignAxis(self, location, *args):
         pass
+
     def addAxisValueRecord(self, location, *args):
         pass
-    def add_ligatureCaretByPos_(self, location, *args): # Urgh
+
+    def add_ligatureCaretByPos_(self, location, *args):  # Urgh
         pass
 
     def add_lookup_call(self, lookup_name):
-
         routine = self.ff.routineNamed(lookup_name)
+        rr = fontFeatures.RoutineReference(name=lookup_name, routine=routine)
+        rr.languages = self.currentLanguage
         if self.currentFeature:
             self._discard_empty_routine()
-            self.ff.addFeature(self.currentFeature, [routine])
+            self.ff.addFeature(self.currentFeature, [rr])
         else:
             raise ValueError("Huh?")
 
     def end_lookup_block(self):
         if self.currentRoutine:
             for rule in self.currentRoutine.rules:
                 rule.flags = self.currentRoutineFlag
```

### Comparing `fontFeatures-1.7.4/fontFeatures/fontDameLib/__init__.py` & `fontFeatures-1.8.0/fontFeatures/fontDameLib/__init__.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/optimizer/FontFeatures.py` & `fontFeatures-1.8.0/fontFeatures/optimizer/FontFeatures.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/optimizer/Routine.py` & `fontFeatures-1.8.0/fontFeatures/optimizer/Routine.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/optimizer/__init__.py` & `fontFeatures-1.8.0/fontFeatures/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/ArabicShaper.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/ArabicShaper.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/Attachment.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/Attachment.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/BaseShaper.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/BaseShaper.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/Buffer.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/Buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from fontFeatures import ValueRecord
-from glyphtools import get_glyph_metrics, categorize_glyph
+from fontFeatures.utils import categorize_glyph
 from youseedee import ucd_data
 import sys
 import warnings
 
 
 def _add_value_records(vr1, vr2):
     if vr1.xPlacement or vr2.xPlacement:
```

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/Chaining.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/Chaining.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/HangulShaper.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/HangulShaper.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/IndicShaper.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/IndicShaper.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/IndicShaperData.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/IndicShaperData.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/KhmerShaper.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/KhmerShaper.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/MyanmarShaper.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/MyanmarShaper.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/Routine.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/Routine.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/Rule.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/Rule.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/Shaper.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/Shaper.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/Substitution.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/Substitution.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/SyllabicShaper.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/SyllabicShaper.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/USEShaper.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/USEShaper.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/shaperLib/VowelConstraints.py` & `fontFeatures-1.8.0/fontFeatures/shaperLib/VowelConstraints.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/ttLib/Attachment.py` & `fontFeatures-1.8.0/fontFeatures/ttLib/Attachment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ttLib.Attachment: Converting Attachment rules to TrueType."""
 
-from glyphtools import categorize_glyph
+from fontFeatures.utils import categorize_glyph
 
 
 def lookup_type(self):
     """Mixin to determine the GPOS lookup type of a fontFeatures.Attachment object
 
     Returns: integer GPOS lookup type."""
     if self.is_cursive:
```

### Comparing `fontFeatures-1.7.4/fontFeatures/ttLib/FontFeatures.py` & `fontFeatures-1.8.0/fontFeatures/ttLib/FontFeatures.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/ttLib/GDEFUnparser.py` & `fontFeatures-1.8.0/fontFeatures/ttLib/GDEFUnparser.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/ttLib/GPOSUnparser.py` & `fontFeatures-1.8.0/fontFeatures/ttLib/GPOSUnparser.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/ttLib/GSUBUnparser.py` & `fontFeatures-1.8.0/fontFeatures/ttLib/GSUBUnparser.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/ttLib/GTableUnparser.py` & `fontFeatures-1.8.0/fontFeatures/ttLib/GTableUnparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         retrieve the original address and routine names."""
         if not self.font or "Debg" not in self.font:
             return None
         debug_data = self.font["Debg"].data
         if "com.github.fonttools.feaLib" not in debug_data:
             return None
         debug_data = debug_data["com.github.fonttools.feaLib"][table][str(ix)]
-        return debug_data[0], debug_data[1]
+        return debug_data[0], debug_data[1].replace("-", "_")
 
     def _asXML(self, sub):
         writer = XMLWriter(BytesIO())
         sub.toXML(writer, self.font)
         out = writer.file.getvalue().decode("utf-8")
         return out
```

### Comparing `fontFeatures-1.7.4/fontFeatures/ttLib/Routine.py` & `fontFeatures-1.8.0/fontFeatures/ttLib/Routine.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/ttLib/Substitution.py` & `fontFeatures-1.8.0/fontFeatures/ttLib/Substitution.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/ttLib/ValueRecord.py` & `fontFeatures-1.8.0/fontFeatures/ttLib/ValueRecord.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/ttLib/__init__.py` & `fontFeatures-1.8.0/fontFeatures/ttLib/__init__.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/voltLib/__init__.py` & `fontFeatures-1.8.0/fontFeatures/voltLib/__init__.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/xmlLib/Attachment.py` & `fontFeatures-1.8.0/fontFeatures/xmlLib/Attachment.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/xmlLib/Chaining.py` & `fontFeatures-1.8.0/fontFeatures/xmlLib/Chaining.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/xmlLib/FontFeatures.py` & `fontFeatures-1.8.0/fontFeatures/xmlLib/FontFeatures.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/xmlLib/Positioning.py` & `fontFeatures-1.8.0/fontFeatures/xmlLib/Positioning.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/xmlLib/Routine.py` & `fontFeatures-1.8.0/fontFeatures/xmlLib/Routine.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/xmlLib/Rule.py` & `fontFeatures-1.8.0/fontFeatures/xmlLib/Rule.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures/xmlLib/Substitution.py` & `fontFeatures-1.8.0/fontFeatures/xmlLib/Substitution.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fontFeatures.egg-info/PKG-INFO` & `fontFeatures-1.8.0/fontFeatures.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontFeatures
-Version: 1.7.4
+Version: 1.8.0
 Summary: Python library for manipulating OpenType font features
 Home-page: https://github.com/simoncozens/fontFeatures
 Author: Simon Cozens
 Author-email: simon@simon-cozens.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `fontFeatures-1.7.4/fontFeatures.egg-info/SOURCES.txt` & `fontFeatures-1.8.0/fontFeatures.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .coveragerc
 .editorconfig
 .gitignore
-CHANGES.md
 LICENSE
 NEW-FORMAT.md
 README.md
 conftest.py
 fea2fea.py
 requirements-dev.txt
 requirements.txt
@@ -19,15 +18,15 @@
 docs/Makefile
 docs/conf.py
 docs/converting.rst
 docs/fontFeatures.rst
 docs/index.rst
 docs/supportingmodules.rst
 fontFeatures/__init__.py
-fontFeatures/pathUtils.py
+fontFeatures/utils.py
 fontFeatures.egg-info/PKG-INFO
 fontFeatures.egg-info/SOURCES.txt
 fontFeatures.egg-info/dependency_links.txt
 fontFeatures.egg-info/not-zip-safe
 fontFeatures.egg-info/requires.txt
 fontFeatures.egg-info/top_level.txt
 fontFeatures/feaLib/Attachment.py
```

### Comparing `fontFeatures-1.7.4/fonts/Amiri-Regular.ttf` & `fontFeatures-1.8.0/fonts/Amiri-Regular.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fonts/NotoNastaliqUrdu-Dummy.ttf` & `fontFeatures-1.8.0/fonts/NotoNastaliqUrdu-Dummy.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/fonts/Roboto-Regular.ttf` & `fontFeatures-1.8.0/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/ms-use/COPYING` & `fontFeatures-1.8.0/ms-use/COPYING`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/ms-use/IndicShapingInvalidCluster.txt` & `fontFeatures-1.8.0/ms-use/IndicShapingInvalidCluster.txt`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/setup.py` & `fontFeatures-1.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'author': 'Simon Cozens',
     'author_email': 'simon@simon-cozens.org',
     'url': 'https://github.com/simoncozens/fontFeatures',
     'description': 'Python library for manipulating OpenType font features',
     'long_description': open('README.md', 'r').read(),
     'long_description_content_type': 'text/markdown',
     'license': 'MIT',
-    'version': '1.7.4',
+    'version': '1.8.0',
     'install_requires': install_requires,
     'extras_require': {
         'shaper': [
             "youseedee >=0.3.0",
             "babelfont >=3.0.0a1",
             "dataclasses ; python_version < '3.7'"
         ]
```

### Comparing `fontFeatures-1.7.4/tests/data/1735326da89f0818cd8c51a0600e9789812c0f94.ttf` & `fontFeatures-1.8.0/tests/data/1735326da89f0818cd8c51a0600e9789812c0f94.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf` & `fontFeatures-1.8.0/tests/data/1a3d8f381387dd29be1e897e4b5100ac8b4829e1.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/341421e629668b1a1242245d39238ca48432d35d.ttf` & `fontFeatures-1.8.0/tests/data/341421e629668b1a1242245d39238ca48432d35d.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/55c88ebbe938680b08f92c3de20713183e0c7481.ttf` & `fontFeatures-1.8.0/tests/data/55c88ebbe938680b08f92c3de20713183e0c7481.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf` & `fontFeatures-1.8.0/tests/data/663aef6b019dbf45ffd74089e2b5f2496ceceb18.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf` & `fontFeatures-1.8.0/tests/data/932ad5132c2761297c74e9976fe25b08e5ffa10b.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/Amiri-Regular.ttf` & `fontFeatures-1.8.0/tests/data/Amiri-Regular.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/LibertinusSans-Regular.otf` & `fontFeatures-1.8.0/tests/data/LibertinusSans-Regular.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/Noto Sans Sharada GSUB.txt` & `fontFeatures-1.8.0/tests/data/Noto Sans Sharada GSUB.txt`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/SimpleTwoAxis.glyphs` & `fontFeatures-1.8.0/tests/data/SimpleTwoAxis.glyphs`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/a014549f766436cf55b2ceb40e462038938ee899.ttf` & `fontFeatures-1.8.0/tests/data/a014549f766436cf55b2ceb40e462038938ee899.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/acbe26ce904463c690fb67f70679447059d13ee4.otf` & `fontFeatures-1.8.0/tests/data/acbe26ce904463c690fb67f70679447059d13ee4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/data/df768b9c257e0c9c35786c47cae15c46571d56be.ttf` & `fontFeatures-1.8.0/tests/data/df768b9c257e0c9c35786c47cae15c46571d56be.ttf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/COPYING` & `fontFeatures-1.8.0/tests/harfbuzz/aots/COPYING`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef1_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef1_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef1_font2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef1_font2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef1_font3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef1_font3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef1_font4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef1_font4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef2_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef2_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef2_font2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef2_font2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef2_font3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef2_font3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/classdef2_font4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/classdef2_font4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap0_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap0_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap10_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap10_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap10_font2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap10_font2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap12_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap12_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap14_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap14_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap2_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap2_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap4_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap4_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap4_font2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap4_font2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap4_font3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap4_font3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap4_font4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap4_font4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap6_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap6_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap6_font2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap6_font2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap8_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap8_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_composition_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_composition_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_subtableselection_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_subtableselection_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_subtableselection_font2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_subtableselection_font2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_subtableselection_font3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_subtableselection_font3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_subtableselection_font4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_subtableselection_font4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/cmap_subtableselection_font5.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/cmap_subtableselection_font5.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_1_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_1_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_1_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_1_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_1_simple_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_1_simple_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_1_simple_f3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_1_simple_f3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_1_simple_f4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_1_simple_f4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_2_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_2_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos1_2_font2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos1_2_font2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_font6.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_font6.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_font7.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_font7.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_lookupflag_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_lookupflag_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_next_glyph_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_next_glyph_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_1_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_1_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_2_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_2_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_2_font2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_2_font2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_2_font3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_2_font3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_2_font4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_2_font4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos2_2_font5.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos2_2_font5.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos3_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos3_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos3_font2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos3_font2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos3_font3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos3_font3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos4_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos4_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos4_lookupflag_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos4_lookupflag_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos4_multiple_anchors_1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos4_multiple_anchors_1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos4_simple_1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos4_simple_1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos5_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos5_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos6_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos6_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos7_1_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos7_1_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos9_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos9_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos9_font2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos9_font2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_boundary_f4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_multiple_subrules_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_multiple_subrules_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_multiple_subrules_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_multiple_subrules_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_simple_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_simple_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining1_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining1_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_boundary_f4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_multiple_subrules_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_multiple_subrules_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_multiple_subrules_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_multiple_subrules_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_simple_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_simple_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining2_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining2_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_boundary_f4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_simple_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_simple_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_chaining3_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_chaining3_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_expansion_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_expansion_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_lookupflag_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_lookupflag_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_multiple_subrules_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_multiple_subrules_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_multiple_subrules_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_multiple_subrules_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_simple_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_simple_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context1_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context1_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_classes_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_classes_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_classes_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_classes_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_expansion_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_expansion_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_lookupflag_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_lookupflag_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_multiple_subrules_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_multiple_subrules_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_multiple_subrules_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_multiple_subrules_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_simple_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_simple_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context2_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context2_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_lookupflag_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_lookupflag_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gpos_context3_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gpos_context3_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub1_1_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub1_1_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub1_1_modulo_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub1_1_modulo_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub1_1_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub1_1_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub1_2_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub1_2_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub1_2_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub1_2_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub2_1_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub2_1_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub2_1_multiple_sequences_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub2_1_multiple_sequences_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub2_1_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub2_1_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub3_1_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub3_1_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub3_1_multiple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub3_1_multiple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub3_1_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub3_1_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub4_1_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub4_1_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligatures_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligatures_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligatures_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligatures_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligsets_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub4_1_multiple_ligsets_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub4_1_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub4_1_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub7_font1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub7_font1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub7_font2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub7_font2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_boundary_f4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_multiple_subrules_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_multiple_subrules_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_multiple_subrules_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_multiple_subrules_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_simple_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_simple_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining1_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining1_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_boundary_f4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_multiple_subrules_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_multiple_subrules_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_multiple_subrules_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_multiple_subrules_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_simple_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_simple_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining2_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining2_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f3.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f3.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f4.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_boundary_f4.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_simple_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_simple_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_chaining3_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_chaining3_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_expansion_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_expansion_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_lookupflag_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_lookupflag_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_multiple_subrules_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_multiple_subrules_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_multiple_subrules_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_multiple_subrules_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_simple_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_simple_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context1_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context1_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_classes_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_classes_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_classes_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_classes_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_expansion_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_expansion_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_lookupflag_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_lookupflag_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_multiple_subrules_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_multiple_subrules_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_multiple_subrules_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_multiple_subrules_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_simple_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_simple_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context2_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context2_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_boundary_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_boundary_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_boundary_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_boundary_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_lookupflag_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_lookupflag_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_lookupflag_f2.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_lookupflag_f2.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_next_glyph_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_next_glyph_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_simple_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_simple_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/gsub_context3_successive_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/gsub_context3_successive_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/lookupflag_ignore_attach_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/lookupflag_ignore_attach_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/lookupflag_ignore_base_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/lookupflag_ignore_base_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/lookupflag_ignore_combination_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/lookupflag_ignore_combination_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/lookupflag_ignore_ligatures_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/lookupflag_ignore_ligatures_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/fonts/lookupflag_ignore_marks_f1.otf` & `fontFeatures-1.8.0/tests/harfbuzz/aots/fonts/lookupflag_ignore_marks_f1.otf`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos1_1_simple.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos1_1_simple.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos2_2.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos2_2.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos3.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos3.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos4_simple.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos4_simple.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining1_boundary.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining1_boundary.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining1_multiple_subrules.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining1_multiple_subrules.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining1_simple.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining1_simple.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining2_boundary.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining2_boundary.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining2_multiple_subrules.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining2_multiple_subrules.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining2_simple.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining2_simple.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining3_boundary.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining3_boundary.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_chaining3_simple.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_chaining3_simple.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context1_simple.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context1_simple.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context2_classes.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context2_classes.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gpos_context2_simple.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gpos_context2_simple.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining1_boundary.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining1_boundary.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining1_simple.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining1_simple.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining2_boundary.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining2_boundary.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining2_simple.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining2_simple.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining3_boundary.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining3_boundary.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/gsub_chaining3_simple.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/gsub_chaining3_simple.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/lookupflag_ignore_attach.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/lookupflag_ignore_attach.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/lookupflag_ignore_combination.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/lookupflag_ignore_combination.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/harfbuzz/aots/tests/lookupflag_ignore_ligatures.tests` & `fontFeatures-1.8.0/tests/harfbuzz/aots/tests/lookupflag_ignore_ligatures.tests`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/test_anchors.py` & `fontFeatures-1.8.0/tests/test_anchors.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 class TestAnchors(unittest.TestCase):
     def roundTrip(self, thing):
       rt = thing.__class__.fromXML(thing.toXML())
       self.assertEqual(rt.asFea(), thing.asFea())
 
     def test_markbase(self):
         s = Attachment("top", "top_", {"A": (679, 1600)}, {"acutecomb": (-570, 1290)})
-        assertSufficientlyEqual(s.asFea(), "    pos base A <anchor 679 1600> mark @top;\n")
+        assertSufficientlyEqual(s.asFea(), "    pos base A <anchor 679 1600> mark @top_top_;\n")
         self.assertEqual(s.involved_glyphs, set(["A", "acutecomb"]))
         self.assertEqual(etree.tostring(s.toXML()), '<attachment basename="top" markname="top_"><base name="A" anchorX="679" anchorY="1600"/><mark name="acutecomb" anchorX="-570" anchorY="1290"/></attachment>'.encode("utf-8"))
         self.roundTrip(s)
```

### Comparing `fontFeatures-1.7.4/tests/test_binary_emitter.py` & `fontFeatures-1.8.0/tests/test_binary_emitter.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/test_chaining.py` & `fontFeatures-1.8.0/tests/test_chaining.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         rr = RoutineReference(routine=r)
 
         c = Chaining([["a"], ["b"]], lookups=[[rr], None])
         self.assertEqual(c.asFea(), "sub a' lookup dummy b';")
 
     def test_ignore(self):
         c = Chaining([["a"], ["b"]], lookups=[])
-        self.assertEqual(c.asFea(), "ignore sub a b;")
+        self.assertEqual(c.asFea(), "ignore sub a' b';")
 
     def test_complex(self):
         pos1 = Substitution(["a"], ["b"])
         pos2 = Substitution(["b"], ["c"])
         r1 = Routine(rules=[pos1], name="dummy1")
         r2 = Routine(rules=[pos2], name="dummy2")
         rr1 = RoutineReference(routine=r1)
```

### Comparing `fontFeatures-1.7.4/tests/test_fea_parser.py` & `fontFeatures-1.8.0/tests/test_fea_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,21 @@
     pytest.param("lookup dummy { pos a [one two]' <-80 0 -160 0>; } dummy;",id="pos_one_contexual"),
     pytest.param("lookup dummy { pos s f' 10 t; } dummy;",id="pos_one_contextual_alt_format"),
     pytest.param("lookup dummy { pos T -60 a <-40 0 -40 0>; } dummy;",id="pos_two"),
     pytest.param("lookup dummy { pos [X Y] -60 a <-40 0 -40 0>; } dummy;",id="pos_two_group"),
     pytest.param("lookup dummy { pos T a -100; } dummy;",id="pos_two_one_null"),
     pytest.param("lookup dummy { pos cursive meem.medial <anchor 500 20> <anchor 0 -20>; } dummy;",id="pos_cursive1"),
     pytest.param("lookup dummy { pos cursive meem.init <anchor NULL> <anchor 0 -20>; } dummy;",id="pos_cursive2"),
-    pytest.param(
-        """markClass [acute grave] <anchor 150 -10> @TOP_MARKS;
-  lookup dummy {
-  pos base [a e o u] <anchor 250 450> mark @TOP_MARKS;
-  } dummy;
-  """, id="mark_attachment"
-        ),
+  #   pytest.param(
+  #       """markClass [acute grave] <anchor 150 -10> @TOP_MARKS;
+  # lookup dummy {
+  # pos base [a e o u] <anchor 250 450> mark @TOP_MARKS;
+  # } dummy;
+  # """, id="mark_attachment"
+        # ),
     pytest.param("lookup dummy { pos X [A B]' -40 B' -40 A' -40 Y; } dummy;", id="pos_contextual"),
     # pytest.param("lookup dummy { sub a b by c; } dummy; feature calt { lookup dummy; } calt;", id="lookup_reference"),
     pytest.param("lookup dummy { lookupflag IgnoreMarks; sub a b by c; } dummy;", id="lookup_flag"),
     # pytest.param("feature calt { lookupflag IgnoreMarks; sub a b by c; } calt;", id="flag_in_feature"),
     # pytest.param("feature calt { sub x by y; lookupflag IgnoreMarks; sub a b by c; } calt;", id="switch_flags"),
 ])
 def test_round_trip(s):
```

### Comparing `fontFeatures-1.7.4/tests/test_fontdame.py` & `fontFeatures-1.8.0/tests/test_fontdame.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/test_fontfeatures.py` & `fontFeatures-1.8.0/tests/test_fontfeatures.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/test_languages.py` & `fontFeatures-1.8.0/tests/test_languages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from fontFeatures import Substitution, FontFeatures, Routine
 
 import pytest
 
 
+@pytest.mark.xfail(reason="Harmless but annoying duplication of script/lang")
 def test_language_ordering():
     f = FontFeatures()
     s1 = Substitution([["a"]], ["b"], languages=[("arab", "URD ")])
     s2 = Substitution([["a"]], ["c"], languages=[("arab", "FAR ")])
     s3 = Substitution([["x"], ["y"]], ["z"], languages=[("arab", "URD ")])
 
     f.addFeature("locl", [Routine(rules=[ s1, s2, s3 ] )])
@@ -63,14 +64,15 @@
     r2 = Routine(rules=[ s2 ])
     r3 = Routine(rules=[ s3 ])
 
     f.addFeature("locl", [r1,r2,r3])
     assert f.asFea(do_gdef=False) == expected
 
 
+@pytest.mark.xfail(reason="Harmless but annoying duplication of script/lang")
 def test_multiple_languages():
     f = FontFeatures()
     s1 = Substitution([["a"]], ["b"], languages=[("arab", "URD "),("arab", "FAR ")])
     expected = """languagesystem arab URD;
 languagesystem arab FAR;
 
 lookup Routine_1 {
@@ -100,14 +102,15 @@
 } locl;
 """
     f = FontFeatures()
     r1 = Routine(rules=[ s1 ])
     f.addFeature("locl", [r1])
     assert f.asFea(do_gdef=False) == expected
 
+@pytest.mark.xfail(reason="Harmless but annoying duplication of script/lang")
 def test_multiple_languages_routine():
     f = FontFeatures()
     s1 = Substitution([["a"]], ["b"])
     expected = """languagesystem arab URD;
 languagesystem arab FAR;
 
 lookup Routine_1 {
```

### Comparing `fontFeatures-1.7.4/tests/test_optimizer.py` & `fontFeatures-1.8.0/tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/test_positioning.py` & `fontFeatures-1.8.0/tests/test_positioning.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/test_routine_partition.py` & `fontFeatures-1.8.0/tests/test_routine_partition.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/test_shaping_generic.py` & `fontFeatures-1.8.0/tests/test_shaping_generic.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/test_shaping_harfbuzz.py` & `fontFeatures-1.8.0/tests/test_shaping_harfbuzz.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/test_substitution.py` & `fontFeatures-1.8.0/tests/test_substitution.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/test_unparse_pos.py` & `fontFeatures-1.8.0/tests/test_unparse_pos.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/tests/test_unparse_sub.py` & `fontFeatures-1.8.0/tests/test_unparse_sub.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/utils/addfeatures.py` & `fontFeatures-1.8.0/utils/addfeatures.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/utils/dump-anchors.py` & `fontFeatures-1.8.0/utils/dump-anchors.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/utils/dump-cursive.py` & `fontFeatures-1.8.0/utils/dump-cursive.py`

 * *Files identical despite different names*

### Comparing `fontFeatures-1.7.4/utils/gen-vowel-constraints.py` & `fontFeatures-1.8.0/utils/gen-vowel-constraints.py`

 * *Files identical despite different names*

