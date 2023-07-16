# Comparing `tmp/ork.build-0.0.54.tar.gz` & `tmp/ork.build-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ork.build-0.0.54.tar", last modified: Sun Jul 16 23:15:10 2023, max compression
+gzip compressed data, was "ork.build-0.0.55.tar", last modified: Sun Jul 16 23:23:06 2023, max compression
```

## Comparing `ork.build-0.0.54.tar` & `ork.build-0.0.55.tar`

### file list

```diff
@@ -1,461 +1,461 @@
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.737815 ork.build-0.0.54/
--rw-r--r--   0 michael    (501) wheel        (0)    16892 2023-07-16 23:15:10.737339 ork.build-0.0.54/PKG-INFO
--rw-r--r--   0 michael    (501) wheel        (0)    16493 2023-07-16 20:17:09.000000 ork.build-0.0.54/README.md
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.548921 ork.build-0.0.54/bin_priv/
--rw-r--r--   0 michael    (501) wheel        (0)        0 2023-07-14 17:52:14.000000 ork.build-0.0.54/bin_priv/__init__.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      375 2023-07-15 05:41:15.000000 ork.build-0.0.54/bin_priv/_obt_dep_completions.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      418 2023-07-15 05:41:15.000000 ork.build-0.0.54/bin_priv/_obt_dep_completions_shell.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      322 2023-07-15 05:41:15.000000 ork.build-0.0.54/bin_priv/_obt_subspace_completions.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      332 2023-07-15 05:43:34.000000 ork.build-0.0.54/bin_priv/obt.dep.build.all.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1965 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.dep.build.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1312 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.dep.findtext.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1810 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.dep.info.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      779 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.dep.list.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     3223 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.dep.replacetext.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      206 2023-07-15 05:41:15.000000 ork.build-0.0.54/bin_priv/obt.dep.require.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      840 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.dep.shell.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2298 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.dep.status.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1612 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.docker.build.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1107 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.docker.info.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1240 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.docker.kill.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2422 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.docker.launch.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      780 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.docker.list.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1429 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.docker.method.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      708 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.ext.find.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1311 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.find.in.dep.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      649 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.find.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1099 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.host.info.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1839 2023-07-15 05:41:15.000000 ork.build-0.0.54/bin_priv/obt.installedacontainers.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       83 2023-07-14 17:52:14.000000 ork.build-0.0.54/bin_priv/obt.ix.udevrules.reload.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      977 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.litex.env.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      241 2023-07-14 17:52:14.000000 ork.build-0.0.54/bin_priv/obt.litex.zephyrriscv-env.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     1406 2023-07-15 05:41:15.000000 ork.build-0.0.54/bin_priv/obt.litex.zephyrriscv-sample.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       97 2023-07-14 17:52:14.000000 ork.build-0.0.54/bin_priv/obt.lsttys.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     6545 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.lsusbx.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       99 2023-07-14 17:52:14.000000 ork.build-0.0.54/bin_priv/obt.lsvideo.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1262 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.osx.macho.fixup.libs.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      359 2023-07-15 05:41:15.000000 ork.build-0.0.54/bin_priv/obt.osx.macho.showinstallname.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      350 2023-07-15 05:41:15.000000 ork.build-0.0.54/bin_priv/obt.osx.macho.showlibs.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      163 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.pip.install.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1782 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.replace.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1377 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.sdk.info.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      955 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.sdk.install.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1640 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.subspace.build.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1341 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.subspace.launch.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      802 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.subspace.list.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1262 2023-07-15 05:45:21.000000 ork.build-0.0.54/bin_priv/obt.target.info.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2901 2023-07-15 05:43:34.000000 ork.build-0.0.54/bin_priv/obt.vivado.getsites.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2566 2023-07-15 05:43:34.000000 ork.build-0.0.54/bin_priv/obt.vivado.launch.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2441 2023-07-15 05:59:32.000000 ork.build-0.0.54/bin_priv/obt.vscode.create.debug.task.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.551735 ork.build-0.0.54/bin_pub/
--rwxr-xr-x   0 michael    (501) wheel        (0)     5554 2023-07-15 05:31:23.000000 ork.build-0.0.54/bin_pub/obt.create.env.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     8060 2023-07-16 20:17:09.000000 ork.build-0.0.54/bin_pub/obt.init.env.py
--rw-r--r--   0 michael    (501) wheel        (0)      445 2023-07-16 20:17:09.000000 ork.build-0.0.54/bin_pub/obt.ix.installdeps.gentoo.py
--rw-r--r--   0 michael    (501) wheel        (0)     2936 2023-07-16 20:17:09.000000 ork.build-0.0.54/bin_pub/obt.ix.installdeps.linuxcnc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2764 2023-07-16 20:17:09.000000 ork.build-0.0.54/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py
--rw-r--r--   0 michael    (501) wheel        (0)     3161 2023-07-16 20:17:09.000000 ork.build-0.0.54/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py
--rw-r--r--   0 michael    (501) wheel        (0)      446 2023-07-16 20:17:09.000000 ork.build-0.0.54/bin_pub/obt.osx.installdeps.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1670 2023-07-16 20:17:09.000000 ork.build-0.0.54/bin_pub/obt.versions.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.521646 ork.build-0.0.54/examples/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.552042 ork.build-0.0.54/examples/dep-overrides/
--rw-r--r--   0 michael    (501) wheel        (0)     1530 2023-07-15 05:45:21.000000 ork.build-0.0.54/examples/dep-overrides/orkid.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.555222 ork.build-0.0.54/examples/litex1/
--rwxr-xr-x   0 michael    (501) wheel        (0)     4642 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex1/arty.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      389 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex1/bit2svf_nexysv.tcl
--rw-r--r--   0 michael    (501) wheel        (0)    11759 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex1/cmod_a7_platform.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     3002 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex1/cmod_a7_target.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     4526 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex1/nexys_video.py
--rw-r--r--   0 michael    (501) wheel        (0)      628 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex1/nexysv.cfg
--rwxr-xr-x   0 michael    (501) wheel        (0)      247 2023-07-15 05:45:21.000000 ork.build-0.0.54/examples/litex1/soc_arty.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2559 2023-07-15 05:45:21.000000 ork.build-0.0.54/examples/litex1/soc_nexysv.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.558575 ork.build-0.0.54/examples/litex_zephyrtest/
--rw-r--r--   0 michael    (501) wheel        (0)      213 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex_zephyrtest/CMakeLists.txt
--rw-r--r--   0 michael    (501) wheel        (0)    11415 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex_zephyrtest/LICENSE
--rw-r--r--   0 michael    (501) wheel        (0)     1015 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex_zephyrtest/README.rst
--rwxr-xr-x   0 michael    (501) wheel        (0)      315 2023-07-15 05:41:15.000000 ork.build-0.0.54/examples/litex_zephyrtest/build.py
--rw-r--r--   0 michael    (501) wheel        (0)      111 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex_zephyrtest/main.c
--rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex_zephyrtest/prj.conf
--rw-r--r--   0 michael    (501) wheel        (0)      703 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex_zephyrtest/sample.yaml
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.558977 ork.build-0.0.54/examples/litex_zephyrtest/src/
--rw-r--r--   0 michael    (501) wheel        (0)     2515 2022-09-08 21:51:23.000000 ork.build-0.0.54/examples/litex_zephyrtest/src/main.c
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.529648 ork.build-0.0.54/modules/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.644793 ork.build-0.0.54/modules/dep/
--rw-r--r--   0 michael    (501) wheel        (0)      718 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/dep/_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     8257 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/dep/_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1276 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/_nnsvs.py
--rw-r--r--   0 michael    (501) wheel        (0)     1910 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/apitrace.py
--rw-r--r--   0 michael    (501) wheel        (0)     1776 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/dep/arachnepnr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1663 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/arm64_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1580 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/arm64_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2051 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/assimp.py
--rw-r--r--   0 michael    (501) wheel        (0)     1712 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/astcencoder.py
--rw-r--r--   0 michael    (501) wheel        (0)     1675 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/audiofile.py
--rw-r--r--   0 michael    (501) wheel        (0)     1611 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/avr_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     2206 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/avr_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2209 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/avr_libc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1793 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/bazel.py
--rw-r--r--   0 michael    (501) wheel        (0)     1302 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/blosc.py
--rw-r--r--   0 michael    (501) wheel        (0)     9272 2023-07-15 05:58:02.000000 ork.build-0.0.54/modules/dep/boost.py
--rw-r--r--   0 michael    (501) wheel        (0)     1248 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/bullet.py
--rw-r--r--   0 michael    (501) wheel        (0)     2004 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/calf.py
--rw-r--r--   0 michael    (501) wheel        (0)     1541 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/cgal.py
--rw-r--r--   0 michael    (501) wheel        (0)     2422 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/clang.py
--rw-r--r--   0 michael    (501) wheel        (0)     1408 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/cmake.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1428 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/cpppeglib.py
--rw-r--r--   0 michael    (501) wheel        (0)     1632 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/cppzmq.py
--rw-r--r--   0 michael    (501) wheel        (0)     1563 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/csvparser.py
--rw-r--r--   0 michael    (501) wheel        (0)     1257 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/cuda.py
--rw-r--r--   0 michael    (501) wheel        (0)     1684 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/dep/curlpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     1757 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/cycles.py
--rw-r--r--   0 michael    (501) wheel        (0)     1579 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/depthaicore.py
--rw-r--r--   0 michael    (501) wheel        (0)      992 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/drawtext.py
--rw-r--r--   0 michael    (501) wheel        (0)     1491 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/easyprof.py
--rw-r--r--   0 michael    (501) wheel        (0)     1454 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/eigen.py
--rw-r--r--   0 michael    (501) wheel        (0)     2047 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/embree.py
--rw-r--r--   0 michael    (501) wheel        (0)     1871 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/faust.py
--rw-r--r--   0 michael    (501) wheel        (0)     1577 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/dep/fcollada.py
--rw-r--r--   0 michael    (501) wheel        (0)     1737 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/ffmpeg.py
--rw-r--r--   0 michael    (501) wheel        (0)     1997 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/flatcam.py
--rw-r--r--   0 michael    (501) wheel        (0)     1676 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/fltk.py
--rw-r--r--   0 michael    (501) wheel        (0)     1891 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/fluidsynth.py
--rw-r--r--   0 michael    (501) wheel        (0)     1866 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/frameretrace.py
--rw-r--r--   0 michael    (501) wheel        (0)     1438 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/gcode_gpr.py
--rw-r--r--   0 michael    (501) wheel        (0)     2148 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/dep/giflib.py
--rw-r--r--   0 michael    (501) wheel        (0)     1175 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/gitpython.py
--rw-r--r--   0 michael    (501) wheel        (0)     2601 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/glfw.py
--rw-r--r--   0 michael    (501) wheel        (0)     1544 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/glm.py
--rw-r--r--   0 michael    (501) wheel        (0)      894 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/gnutar.py
--rw-r--r--   0 michael    (501) wheel        (0)      756 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/houdini.py
--rw-r--r--   0 michael    (501) wheel        (0)     1731 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/dep/icestorm.py
--rw-r--r--   0 michael    (501) wheel        (0)     2898 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/igl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1767 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/irix65_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     6593 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/irix65_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1150 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/irrlicht.py
--rw-r--r--   0 michael    (501) wheel        (0)     3478 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/ispc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2331 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/ispctexc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1316 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/jpegturbo.py
--rw-r--r--   0 michael    (501) wheel        (0)     1719 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/klein.py
--rw-r--r--   0 michael    (501) wheel        (0)     1079 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/lapack.py
--rw-r--r--   0 michael    (501) wheel        (0)     1065 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/lemongraph.py
--rw-r--r--   0 michael    (501) wheel        (0)     1301 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/lexertl14.py
--rw-r--r--   0 michael    (501) wheel        (0)     1664 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/dep/libcurl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1701 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/libfive.py
--rw-r--r--   0 michael    (501) wheel        (0)     1490 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/libpqpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     1425 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/libsocket.py
--rw-r--r--   0 michael    (501) wheel        (0)     1419 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/libsurvive.py
--rw-r--r--   0 michael    (501) wheel        (0)     7892 2023-07-15 05:58:02.000000 ork.build-0.0.54/modules/dep/libtorch.py
--rw-r--r--   0 michael    (501) wheel        (0)     1926 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/linuxcnc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2487 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/litex.py
--rw-r--r--   0 michael    (501) wheel        (0)     2529 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/llvm.py
--rw-r--r--   0 michael    (501) wheel        (0)     1339 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/lm32_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1066 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/lm32_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2937 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/dep/lua.py
--rw-r--r--   0 michael    (501) wheel        (0)     2135 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/dep/luajit.py
--rw-r--r--   0 michael    (501) wheel        (0)     1664 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/m68k_amiga_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1555 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/m68k_amiga_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     3841 2023-07-15 06:16:54.000000 ork.build-0.0.54/modules/dep/minetest.py
--rw-r--r--   0 michael    (501) wheel        (0)     2009 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/moltenvk.py
--rw-r--r--   0 michael    (501) wheel        (0)     1244 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/nextpnr.py
--rw-r--r--   0 michael    (501) wheel        (0)     2121 2023-07-16 20:17:09.000000 ork.build-0.0.54/modules/dep/ngc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1426 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/nlohmannjson.py
--rw-r--r--   0 michael    (501) wheel        (0)     1633 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/dep/nss.py
--rw-r--r--   0 michael    (501) wheel        (0)     1464 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/nsync_cpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     3022 2023-07-16 20:17:09.000000 ork.build-0.0.54/modules/dep/nvtt.py
--rw-r--r--   0 michael    (501) wheel        (0)     1562 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/ocio.py
--rw-r--r--   0 michael    (501) wheel        (0)     2587 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/oiio.py
--rw-r--r--   0 michael    (501) wheel        (0)     1738 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/oneapimkl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1407 2023-07-15 07:36:59.000000 ork.build-0.0.54/modules/dep/openblas.py
--rw-r--r--   0 michael    (501) wheel        (0)     2857 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/dep/opencv.py
--rw-r--r--   0 michael    (501) wheel        (0)     1358 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/opencv_contrib.py
--rw-r--r--   0 michael    (501) wheel        (0)     1217 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/opendb.py
--rw-r--r--   0 michael    (501) wheel        (0)     1556 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/openexr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1332 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/openjpeg.py
--rw-r--r--   0 michael    (501) wheel        (0)     1270 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/openroad.py
--rw-r--r--   0 michael    (501) wheel        (0)     1791 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/opensubdiv.py
--rw-r--r--   0 michael    (501) wheel        (0)     1447 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/openvdb.py
--rw-r--r--   0 michael    (501) wheel        (0)     1376 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/openvr.py
--rw-r--r--   0 michael    (501) wheel        (0)     5239 2023-07-16 20:17:09.000000 ork.build-0.0.54/modules/dep/orkid.py
--rw-r--r--   0 michael    (501) wheel        (0)     1306 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/osgeolaszip.py
--rw-r--r--   0 michael    (501) wheel        (0)     1495 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/osgeoliblas.py
--rw-r--r--   0 michael    (501) wheel        (0)     1345 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/osgeoproj.py
--rw-r--r--   0 michael    (501) wheel        (0)     1543 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/osgeotiff.py
--rw-r--r--   0 michael    (501) wheel        (0)     1447 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/osl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1249 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/ozzanim.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1619 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/pangolin.py
--rw-r--r--   0 michael    (501) wheel        (0)     1874 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/parsertl14.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.523347 ork.build-0.0.54/modules/dep/patches/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.522462 ork.build-0.0.54/modules/dep/patches/boost/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.645957 ork.build-0.0.54/modules/dep/patches/boost/chg/
--rw-r--r--   0 michael    (501) wheel        (0)    22151 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/dep/patches/boost/chg/darwin.jam
--rw-r--r--   0 michael    (501) wheel        (0)     1111 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/dep/patches/boost/chg/project-config.jam
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.646483 ork.build-0.0.54/modules/dep/patches/boost/ori/
--rw-r--r--   0 michael    (501) wheel        (0)    22062 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/dep/patches/boost/ori/darwin.jam
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.649109 ork.build-0.0.54/modules/dep/patches/gcc/
--rw-r--r--   0 michael    (501) wheel        (0)   116535 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/dep/patches/gcc/gcc.sgifixes.patch
--rw-r--r--   0 michael    (501) wheel        (0)      522 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch
--rw-r--r--   0 michael    (501) wheel        (0)      475 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/dep/patches/gcc/gcc.sgifixlibstdcpp02.patch
--rw-r--r--   0 michael    (501) wheel        (0)      801 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/dep/patches/gcc/newlib.sgifixes.patch
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.523156 ork.build-0.0.54/modules/dep/patches/giflib/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.649627 ork.build-0.0.54/modules/dep/patches/giflib/chg/
--rw-r--r--   0 michael    (501) wheel        (0)     5546 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/dep/patches/giflib/chg/Makefile
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.650134 ork.build-0.0.54/modules/dep/patches/giflib/ori/
--rw-r--r--   0 michael    (501) wheel        (0)     4712 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/dep/patches/giflib/ori/Makefile
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.523673 ork.build-0.0.54/modules/dep/patches/pillar/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.650643 ork.build-0.0.54/modules/dep/patches/pillar/chg/
--rw-r--r--   0 michael    (501) wheel        (0)     1660 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/dep/patches/pillar/chg/markdown.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.651144 ork.build-0.0.54/modules/dep/patches/pillar/ori/
--rw-r--r--   0 michael    (501) wheel        (0)     1645 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/dep/patches/pillar/ori/markdown.py
--rw-r--r--   0 michael    (501) wheel        (0)     1748 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/dep/pillar.py
--rw-r--r--   0 michael    (501) wheel        (0)     2152 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/pkgconfig.py
--rw-r--r--   0 michael    (501) wheel        (0)     1362 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/portaudio.py
--rw-r--r--   0 michael    (501) wheel        (0)     2133 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/postgresql.py
--rw-r--r--   0 michael    (501) wheel        (0)     1989 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/premake.py
--rw-r--r--   0 michael    (501) wheel        (0)     1526 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/ptex.py
--rw-r--r--   0 michael    (501) wheel        (0)     1298 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/pugixml.py
--rw-r--r--   0 michael    (501) wheel        (0)     1488 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/pybind11.py
--rw-r--r--   0 michael    (501) wheel        (0)     1521 2023-07-16 20:17:09.000000 ork.build-0.0.54/modules/dep/pydefaults.py
--rw-r--r--   0 michael    (501) wheel        (0)      822 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/pyopengl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1954 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/pyqt5.py
--rw-r--r--   0 michael    (501) wheel        (0)      814 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/pyside2.py
--rw-r--r--   0 michael    (501) wheel        (0)     7471 2023-07-15 08:06:28.000000 ork.build-0.0.54/modules/dep/python.py
--rw-r--r--   0 michael    (501) wheel        (0)     5932 2023-07-15 05:58:02.000000 ork.build-0.0.54/modules/dep/qt5.py
--rw-r--r--   0 michael    (501) wheel        (0)     1781 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/qt5ct.py
--rw-r--r--   0 michael    (501) wheel        (0)     5913 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/qt5forpython.py
--rw-r--r--   0 michael    (501) wheel        (0)     1942 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/rapidjson.py
--rw-r--r--   0 michael    (501) wheel        (0)     3538 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/realsense2.py
--rw-r--r--   0 michael    (501) wheel        (0)     1032 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/root.py
--rw-r--r--   0 michael    (501) wheel        (0)     1344 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/rtmidi.py
--rw-r--r--   0 michael    (501) wheel        (0)     1345 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/rv32_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1069 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/rv32_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1355 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/sigslot.py
--rw-r--r--   0 michael    (501) wheel        (0)     1215 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/simavr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1370 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/sse2neon.py
--rw-r--r--   0 michael    (501) wheel        (0)     2929 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/dep/tbb.py
--rw-r--r--   0 michael    (501) wheel        (0)     6552 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/dep/tflite.py
--rw-r--r--   0 michael    (501) wheel        (0)     3343 2023-07-15 06:17:46.000000 ork.build-0.0.54/modules/dep/ue5.py
--rw-r--r--   0 michael    (501) wheel        (0)     6344 2023-07-15 06:17:57.000000 ork.build-0.0.54/modules/dep/ue5_cesium.py
--rw-r--r--   0 michael    (501) wheel        (0)     1669 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/unittestpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     2361 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/usd.py
--rw-r--r--   0 michael    (501) wheel        (0)     1289 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/vhacd.py
--rw-r--r--   0 michael    (501) wheel        (0)     1316 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/vivado.py
--rw-r--r--   0 michael    (501) wheel        (0)     2962 2023-07-15 06:17:29.000000 ork.build-0.0.54/modules/dep/vpf.py
--rw-r--r--   0 michael    (501) wheel        (0)     1892 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/dep/vrx.py
--rw-r--r--   0 michael    (501) wheel        (0)     1972 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/vst3sdk.py
--rw-r--r--   0 michael    (501) wheel        (0)     4325 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/vulkan.py
--rw-r--r--   0 michael    (501) wheel        (0)     2772 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/wt4.py
--rw-r--r--   0 michael    (501) wheel        (0)     2144 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/dep/xatlas.py
--rw-r--r--   0 michael    (501) wheel        (0)     1107 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/dep/yarl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1887 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/dep/yosys.py
--rw-r--r--   0 michael    (501) wheel        (0)     1922 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/dep/zephyr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1719 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/dep/zmq.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.528222 ork.build-0.0.54/modules/docker/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.652148 ork.build-0.0.54/modules/docker/amigadev/
--rw-r--r--   0 michael    (501) wheel        (0)     1042 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/amigadev/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     2813 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/amigadev/amigadev.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.655265 ork.build-0.0.54/modules/docker/amigadev/test1/
--rw-r--r--   0 michael    (501) wheel        (0)      280 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/amigadev/test1/Makefile
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.655750 ork.build-0.0.54/modules/docker/amigadev/test1/S/
--rw-r--r--   0 michael    (501) wheel        (0)        8 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/amigadev/test1/S/Startup-Sequence
--rwxr-xr-x   0 michael    (501) wheel        (0)      418 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/amigadev/test1/_build.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      527 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/amigadev/test1/build.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.656695 ork.build-0.0.54/modules/docker/amigadev/test1/libs/
--rw-r--r--   0 michael    (501) wheel        (0)     4688 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/amigadev/test1/libs/mathieeedoubbas.library
--rw-r--r--   0 michael    (501) wheel        (0)    15728 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library
--rw-r--r--   0 michael    (501) wheel        (0)     5351 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/amigadev/test1/main.cpp
--rwxr-xr-x   0 michael    (501) wheel        (0)     1177 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/amigadev/test1/test_fsuae.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      391 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/amigadev/test1/test_vamos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.657676 ork.build-0.0.54/modules/docker/androiddev/
--rw-r--r--   0 michael    (501) wheel        (0)     1679 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/androiddev/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     2071 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/androiddev/androiddev.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.662774 ork.build-0.0.54/modules/docker/cicd/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.669273 ork.build-0.0.54/modules/docker/cicd/bin/
--rw-r--r--   0 michael    (501) wheel        (0)        1 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/bin/__init__.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      457 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/bin/build_master_image.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      276 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/bin/build_worker_android_image.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      271 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/bin/build_worker_ub20_image.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      271 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/bin/build_worker_ub22_image.py
--rw-r--r--   0 michael    (501) wheel        (0)      644 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/bin/ci_common.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       66 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/bin/launch_attached.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       64 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/bin/launch_detached.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       83 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/bin/launch_testnossl.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       46 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/bin/terminate.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     1188 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/bin/test_worker_android.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1235 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/bin/test_worker_ub20.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1255 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/bin/test_worker_ub22.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.677872 ork.build-0.0.54/modules/docker/cicd/ci_impl/
--rw-r--r--   0 michael    (501) wheel        (0)      307 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/TODO.txt
--rw-r--r--   0 michael    (501) wheel        (0)     9906 2023-07-15 05:59:09.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/_masterimpl.py
--rw-r--r--   0 michael    (501) wheel        (0)     6829 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/_watcher.py
--rw-r--r--   0 michael    (501) wheel        (0)     1087 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/_workerimpl.py
--rw-r--r--   0 michael    (501) wheel        (0)     3772 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/_zmqssh.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.680480 ork.build-0.0.54/modules/docker/cicd/ci_impl/assets/
--rw-r--r--   0 michael    (501) wheel        (0)    71033 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/assets/OrkidLogo.png
--rw-r--r--   0 michael    (501) wheel        (0)     1778 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/assets/index.template
--rw-r--r--   0 michael    (501) wheel        (0)     3091 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/assets/variant.template
--rw-r--r--   0 michael    (501) wheel        (0)     4134 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/badge.py
--rw-r--r--   0 michael    (501) wheel        (0)      218 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/dummy.svg
--rw-r--r--   0 michael    (501) wheel        (0)     2881 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/httphandler.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1768 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/master.py
--rw-r--r--   0 michael    (501) wheel        (0)     2597 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/orkbb.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1538 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/process_log.py
--rw-r--r--   0 michael    (501) wheel        (0)     7766 2023-07-15 05:58:48.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/scheduler.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/spin.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/start-master.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/start-worker.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     7710 2023-07-15 05:58:58.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/worker.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     4005 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/worker_build_branch.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1335 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/ci_impl/worker_fetch_branch.py
--rw-r--r--   0 michael    (501) wheel        (0)     1708 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/cicd/cicd.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.681919 ork.build-0.0.54/modules/docker/cicd/conf/
--rw-r--r--   0 michael    (501) wheel        (0)      420 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/conf/nginx_app.conf
--rw-r--r--   0 michael    (501) wheel        (0)      898 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/conf/nginx_ssl.conf
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.685681 ork.build-0.0.54/modules/docker/cicd/container-scripts/
--rwxr-xr-x   0 michael    (501) wheel        (0)     2542 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py
--rw-r--r--   0 michael    (501) wheel        (0)     2626 2023-07-16 20:17:09.000000 ork.build-0.0.54/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py
--rw-r--r--   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/container-scripts/spin.sh
--rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/container-scripts/start-master.sh
--rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/container-scripts/start-worker.sh
--rw-r--r--   0 michael    (501) wheel        (0)       20 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/container-scripts/worker.bashrc
--rw-r--r--   0 michael    (501) wheel        (0)      221 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/container-scripts/worker.test.sh
--rw-r--r--   0 michael    (501) wheel        (0)     1126 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/docker-compose-nossl.yml
--rw-r--r--   0 michael    (501) wheel        (0)     1222 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/docker-compose.yml
--rw-r--r--   0 michael    (501) wheel        (0)     2043 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/master.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     1045 2023-07-15 07:01:02.000000 ork.build-0.0.54/modules/docker/cicd/master.json
--rw-r--r--   0 michael    (501) wheel        (0)      228 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/readme.md
--rw-r--r--   0 michael    (501) wheel        (0)     3551 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/worker-android.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/worker-ub20.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/worker-ub22.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/worker20.json
--rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/cicd/worker22.json
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.688029 ork.build-0.0.54/modules/docker/ps1dev/
--rw-r--r--   0 michael    (501) wheel        (0)     1019 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/ps1dev/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     2268 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/ps1dev/Makefile.cfg
--rwxr-xr-x   0 michael    (501) wheel        (0)      223 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/ps1dev/fetch.sh
--rw-r--r--   0 michael    (501) wheel        (0)     2750 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/ps1dev/ps1dev.py
--rw-r--r--   0 michael    (501) wheel        (0)       71 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/ps1dev/readme.md
--rwxr-xr-x   0 michael    (501) wheel        (0)      756 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/ps1dev/setup.sh
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.688378 ork.build-0.0.54/modules/docker/ps1dev/testprograms/
--rw-r--r--   0 michael    (501) wheel        (0)      890 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/ps1dev/testprograms/project.mk
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.689016 ork.build-0.0.54/modules/docker/ps1dev/testprograms/test1/
--rw-r--r--   0 michael    (501) wheel        (0)       86 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/ps1dev/testprograms/test1/Makefile
--rw-r--r--   0 michael    (501) wheel        (0)     7821 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/ps1dev/testprograms/test1/test1.c
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.689849 ork.build-0.0.54/modules/docker/realsense2/
--rw-r--r--   0 michael    (501) wheel        (0)     2325 2023-02-05 19:12:10.000000 ork.build-0.0.54/modules/docker/realsense2/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     3446 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/realsense2/realsense2.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.691414 ork.build-0.0.54/modules/docker/sagemath/
--rw-r--r--   0 michael    (501) wheel        (0)     2646 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/sagemath/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)      347 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/sagemath/docker-compose.yml
--rwxr-xr-x   0 michael    (501) wheel        (0)      100 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/sagemath/entrypoint.sh
--rw-r--r--   0 michael    (501) wheel        (0)     2757 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/sagemath/sagemath.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.693242 ork.build-0.0.54/modules/docker/tflow2gpu/
--rwxr-xr-x   0 michael    (501) wheel        (0)     2775 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/tflow2gpu/Dockerfile
--rwxr-xr-x   0 michael    (501) wheel        (0)      519 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/tflow2gpu/test_mediapipe.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     2533 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/tflow2gpu/test_multi_gpu.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1715 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/tflow2gpu/test_single_gpu.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2483 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/tflow2gpu/tflow2gpu.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.693885 ork.build-0.0.54/modules/docker/ub-focal/
--rw-r--r--   0 michael    (501) wheel        (0)      517 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/docker/ub-focal/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     1702 2023-07-15 05:59:22.000000 ork.build-0.0.54/modules/docker/ub-focal/ub-focal.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.695447 ork.build-0.0.54/modules/host/
--rw-r--r--   0 michael    (501) wheel        (0)     1181 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/host/aarch64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)     1629 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/host/aarch64-macos.py
--rw-r--r--   0 michael    (501) wheel        (0)     1409 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/host/x86_64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)     2165 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/host/x86_64-macos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.697435 ork.build-0.0.54/modules/sdk/
--rw-r--r--   0 michael    (501) wheel        (0)     4088 2023-07-15 05:43:34.000000 ork.build-0.0.54/modules/sdk/aarch64-android.py
--rw-r--r--   0 michael    (501) wheel        (0)     1678 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/sdk/aarch64-ios.py
--rw-r--r--   0 michael    (501) wheel        (0)      776 2023-07-16 23:12:45.000000 ork.build-0.0.54/modules/sdk/aarch64-macos.py
--rw-r--r--   0 michael    (501) wheel        (0)      222 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/sdk/cuda.py
--rw-r--r--   0 michael    (501) wheel        (0)      618 2023-07-15 05:42:23.000000 ork.build-0.0.54/modules/sdk/x86_64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)      619 2023-07-16 23:12:52.000000 ork.build-0.0.54/modules/sdk/x86_64-macos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.698866 ork.build-0.0.54/modules/subspace/
--rw-r--r--   0 michael    (501) wheel        (0)     7785 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/subspace/conda.py
--rw-r--r--   0 michael    (501) wheel        (0)     1227 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/subspace/host.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.699177 ork.build-0.0.54/modules/subspace/nnsvs/
--rwxr-xr-x   0 michael    (501) wheel        (0)     3419 2023-07-15 05:41:15.000000 ork.build-0.0.54/modules/subspace/nnsvs/test.py
--rw-r--r--   0 michael    (501) wheel        (0)     4513 2023-07-15 05:54:20.000000 ork.build-0.0.54/modules/subspace/nnsvs.py
--rw-r--r--   0 michael    (501) wheel        (0)     1187 2023-07-15 05:45:21.000000 ork.build-0.0.54/modules/subspace/yo.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.701090 ork.build-0.0.54/modules/target/
--rw-r--r--   0 michael    (501) wheel        (0)      558 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/target/aarch64-android.py
--rw-r--r--   0 michael    (501) wheel        (0)      551 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/target/aarch64-ios.py
--rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/target/aarch64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/target/aarch64-macos.py
--rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/target/x86_64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build-0.0.54/modules/target/x86_64-macos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.530805 ork.build-0.0.54/scripts/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.724495 ork.build-0.0.54/scripts/obt/
--rw-r--r--   0 michael    (501) wheel        (0)       67 2023-02-05 19:12:10.000000 ork.build-0.0.54/scripts/obt/__init__.py
--rw-r--r--   0 michael    (501) wheel        (0)    12350 2023-07-15 05:51:25.000000 ork.build-0.0.54/scripts/obt/_dep_build.py
--rw-r--r--   0 michael    (501) wheel        (0)     1460 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/_dep_dl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1619 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/_dep_enumerate.py
--rw-r--r--   0 michael    (501) wheel        (0)     8444 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/_dep_fetch.py
--rw-r--r--   0 michael    (501) wheel        (0)     2872 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/_dep_impl.py
--rw-r--r--   0 michael    (501) wheel        (0)     4734 2023-07-15 09:08:14.000000 ork.build-0.0.54/scripts/obt/_dep_node.py
--rw-r--r--   0 michael    (501) wheel        (0)    13516 2023-07-15 05:54:20.000000 ork.build-0.0.54/scripts/obt/_dep_provider.py
--rw-r--r--   0 michael    (501) wheel        (0)     3450 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/_dep_x.py
--rw-r--r--   0 michael    (501) wheel        (0)    13033 2023-07-15 08:10:41.000000 ork.build-0.0.54/scripts/obt/_envutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1925 2022-09-08 21:51:24.000000 ork.build-0.0.54/scripts/obt/_globals.py
--rw-r--r--   0 michael    (501) wheel        (0)     5607 2023-07-15 05:42:23.000000 ork.build-0.0.54/scripts/obt/buildtrace.py
--rw-r--r--   0 michael    (501) wheel        (0)     2975 2023-07-15 05:52:48.000000 ork.build-0.0.54/scripts/obt/cmake.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.725503 ork.build-0.0.54/scripts/obt/cnc/
--rw-r--r--   0 michael    (501) wheel        (0)        2 2023-02-05 19:12:10.000000 ork.build-0.0.54/scripts/obt/cnc/__init__.py
--rw-r--r--   0 michael    (501) wheel        (0)     7782 2023-02-05 19:12:10.000000 ork.build-0.0.54/scripts/obt/cnc/saf.py
--rw-r--r--   0 michael    (501) wheel        (0)     8668 2023-07-15 05:49:59.000000 ork.build-0.0.54/scripts/obt/command.py
--rw-r--r--   0 michael    (501) wheel        (0)     1486 2022-09-08 21:51:24.000000 ork.build-0.0.54/scripts/obt/common.py
--rw-r--r--   0 michael    (501) wheel        (0)      803 2022-09-08 21:51:24.000000 ork.build-0.0.54/scripts/obt/config.py
--rw-r--r--   0 michael    (501) wheel        (0)     8068 2022-09-08 21:51:24.000000 ork.build-0.0.54/scripts/obt/deco.py
--rw-r--r--   0 michael    (501) wheel        (0)      849 2023-07-15 05:37:57.000000 ork.build-0.0.54/scripts/obt/dep.py
--rw-r--r--   0 michael    (501) wheel        (0)     2756 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/docker.py
--rw-r--r--   0 michael    (501) wheel        (0)     1266 2023-07-15 08:33:20.000000 ork.build-0.0.54/scripts/obt/env.py
--rw-r--r--   0 michael    (501) wheel        (0)     1806 2023-07-15 05:43:34.000000 ork.build-0.0.54/scripts/obt/executors.py
--rw-r--r--   0 michael    (501) wheel        (0)     1241 2023-07-15 05:41:15.000000 ork.build-0.0.54/scripts/obt/gen_pkgconfig.py
--rw-r--r--   0 michael    (501) wheel        (0)     5172 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/git.py
--rw-r--r--   0 michael    (501) wheel        (0)     2876 2023-07-15 06:14:59.000000 ork.build-0.0.54/scripts/obt/host.py
--rw-r--r--   0 michael    (501) wheel        (0)      268 2022-09-08 21:51:24.000000 ork.build-0.0.54/scripts/obt/libav.py
--rw-r--r--   0 michael    (501) wheel        (0)      927 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/litex.py
--rw-r--r--   0 michael    (501) wheel        (0)      285 2023-07-15 05:37:17.000000 ork.build-0.0.54/scripts/obt/log.py
--rw-r--r--   0 michael    (501) wheel        (0)     2849 2023-07-15 05:43:34.000000 ork.build-0.0.54/scripts/obt/macos.py
--rw-r--r--   0 michael    (501) wheel        (0)      141 2023-07-15 05:41:15.000000 ork.build-0.0.54/scripts/obt/macos_homebrew.py
--rw-r--r--   0 michael    (501) wheel        (0)     1080 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/make.py
--rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:24.000000 ork.build-0.0.54/scripts/obt/math.py
--rw-r--r--   0 michael    (501) wheel        (0)     2040 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/module.py
--rw-r--r--   0 michael    (501) wheel        (0)      145 2022-09-08 21:51:24.000000 ork.build-0.0.54/scripts/obt/net.py
--rw-r--r--   0 michael    (501) wheel        (0)     1194 2023-07-15 05:41:15.000000 ork.build-0.0.54/scripts/obt/osrelease.py
--rw-r--r--   0 michael    (501) wheel        (0)      983 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/patch.py
--rw-r--r--   0 michael    (501) wheel        (0)     9592 2023-07-16 20:17:09.000000 ork.build-0.0.54/scripts/obt/path.py
--rw-r--r--   0 michael    (501) wheel        (0)     8544 2023-07-15 05:41:15.000000 ork.build-0.0.54/scripts/obt/pathtools.py
--rw-r--r--   0 michael    (501) wheel        (0)      668 2023-07-15 05:43:34.000000 ork.build-0.0.54/scripts/obt/pip.py
--rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:24.000000 ork.build-0.0.54/scripts/obt/pybind11.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1341 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/scp.py
--rw-r--r--   0 michael    (501) wheel        (0)     1755 2023-07-15 06:15:14.000000 ork.build-0.0.54/scripts/obt/sdk.py
--rw-r--r--   0 michael    (501) wheel        (0)     4538 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/search.py
--rw-r--r--   0 michael    (501) wheel        (0)     3241 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/subspace.py
--rw-r--r--   0 michael    (501) wheel        (0)     1342 2023-07-15 06:16:16.000000 ork.build-0.0.54/scripts/obt/target.py
--rw-r--r--   0 michael    (501) wheel        (0)     1559 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/template.py
--rw-r--r--   0 michael    (501) wheel        (0)     6511 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/utils.py
--rw-r--r--   0 michael    (501) wheel        (0)     2080 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/wget.py
--rw-r--r--   0 michael    (501) wheel        (0)      591 2023-07-15 05:45:21.000000 ork.build-0.0.54/scripts/obt/xcode.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.728441 ork.build-0.0.54/scripts/ork.build.egg-info/
--rw-r--r--   0 michael    (501) wheel        (0)    16892 2023-07-16 23:15:10.000000 ork.build-0.0.54/scripts/ork.build.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) wheel        (0)    12158 2023-07-16 23:15:10.000000 ork.build-0.0.54/scripts/ork.build.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) wheel        (0)        1 2023-07-16 23:15:10.000000 ork.build-0.0.54/scripts/ork.build.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) wheel        (0)       14 2023-07-16 23:15:10.000000 ork.build-0.0.54/scripts/ork.build.egg-info/requires.txt
--rw-r--r--   0 michael    (501) wheel        (0)        4 2023-07-16 23:15:10.000000 ork.build-0.0.54/scripts/ork.build.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) wheel        (0)       38 2023-07-16 23:15:10.737900 ork.build-0.0.54/setup.cfg
--rw-r--r--   0 michael    (501) wheel        (0)     1966 2023-07-16 23:15:00.000000 ork.build-0.0.54/setup.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.730258 ork.build-0.0.54/tests/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.733378 ork.build-0.0.54/tests/docker-gpu/
--rw-r--r--   0 michael    (501) wheel        (0)      411 2022-09-08 21:51:24.000000 ork.build-0.0.54/tests/docker-gpu/Dockerfile
--rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build-0.0.54/tests/docker-gpu/build.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      358 2022-09-08 21:51:24.000000 ork.build-0.0.54/tests/docker-gpu/launch_glmark.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      369 2022-09-08 21:51:24.000000 ork.build-0.0.54/tests/docker-gpu/launch_nvtopo.sh
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.735624 ork.build-0.0.54/tests/docker-gpu-tensorflow/
--rw-r--r--   0 michael    (501) wheel        (0)      505 2022-09-08 21:51:24.000000 ork.build-0.0.54/tests/docker-gpu-tensorflow/Dockerfile
--rwxr-xr-x   0 michael    (501) wheel        (0)       55 2022-09-08 21:51:24.000000 ork.build-0.0.54/tests/docker-gpu-tensorflow/build.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      379 2022-09-08 21:51:24.000000 ork.build-0.0.54/tests/docker-gpu-tensorflow/launch_nvtopo.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      391 2022-09-08 21:51:24.000000 ork.build-0.0.54/tests/docker-gpu-tensorflow/launch_tf.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     1543 2023-07-15 05:41:15.000000 ork.build-0.0.54/tests/litex1_nx4.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      178 2023-07-15 05:45:21.000000 ork.build-0.0.54/tests/osx_rpaths.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:15:10.736588 ork.build-0.0.54/tests/pytorch/
--rwxr-xr-x   0 michael    (501) wheel        (0)      916 2023-07-15 05:43:34.000000 ork.build-0.0.54/tests/pytorch/install.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1190 2023-07-15 06:00:28.000000 ork.build-0.0.54/tests/pytorch/training.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.347958 ork.build-0.0.55/
+-rw-r--r--   0 michael    (501) wheel        (0)    16892 2023-07-16 23:23:06.347349 ork.build-0.0.55/PKG-INFO
+-rw-r--r--   0 michael    (501) wheel        (0)    16493 2023-07-16 20:17:09.000000 ork.build-0.0.55/README.md
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.167010 ork.build-0.0.55/bin_priv/
+-rw-r--r--   0 michael    (501) wheel        (0)        0 2023-07-14 17:52:14.000000 ork.build-0.0.55/bin_priv/__init__.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      375 2023-07-15 05:41:15.000000 ork.build-0.0.55/bin_priv/_obt_dep_completions.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      418 2023-07-15 05:41:15.000000 ork.build-0.0.55/bin_priv/_obt_dep_completions_shell.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      322 2023-07-15 05:41:15.000000 ork.build-0.0.55/bin_priv/_obt_subspace_completions.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      332 2023-07-15 05:43:34.000000 ork.build-0.0.55/bin_priv/obt.dep.build.all.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1965 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.dep.build.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1312 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.dep.findtext.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1810 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.dep.info.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      779 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.dep.list.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     3223 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.dep.replacetext.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      206 2023-07-15 05:41:15.000000 ork.build-0.0.55/bin_priv/obt.dep.require.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      840 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.dep.shell.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2298 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.dep.status.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1612 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.docker.build.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1107 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.docker.info.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1240 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.docker.kill.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2422 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.docker.launch.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      780 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.docker.list.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1429 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.docker.method.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      708 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.ext.find.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1311 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.find.in.dep.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      649 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.find.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1099 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.host.info.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1839 2023-07-15 05:41:15.000000 ork.build-0.0.55/bin_priv/obt.installedacontainers.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       83 2023-07-14 17:52:14.000000 ork.build-0.0.55/bin_priv/obt.ix.udevrules.reload.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      977 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.litex.env.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      241 2023-07-14 17:52:14.000000 ork.build-0.0.55/bin_priv/obt.litex.zephyrriscv-env.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1406 2023-07-15 05:41:15.000000 ork.build-0.0.55/bin_priv/obt.litex.zephyrriscv-sample.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       97 2023-07-14 17:52:14.000000 ork.build-0.0.55/bin_priv/obt.lsttys.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     6545 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.lsusbx.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       99 2023-07-14 17:52:14.000000 ork.build-0.0.55/bin_priv/obt.lsvideo.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1262 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.osx.macho.fixup.libs.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      359 2023-07-15 05:41:15.000000 ork.build-0.0.55/bin_priv/obt.osx.macho.showinstallname.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      350 2023-07-15 05:41:15.000000 ork.build-0.0.55/bin_priv/obt.osx.macho.showlibs.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      163 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.pip.install.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1782 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.replace.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1377 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.sdk.info.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      955 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.sdk.install.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1640 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.subspace.build.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1341 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.subspace.launch.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      802 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.subspace.list.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1262 2023-07-15 05:45:21.000000 ork.build-0.0.55/bin_priv/obt.target.info.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2901 2023-07-15 05:43:34.000000 ork.build-0.0.55/bin_priv/obt.vivado.getsites.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2566 2023-07-15 05:43:34.000000 ork.build-0.0.55/bin_priv/obt.vivado.launch.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2441 2023-07-15 05:59:32.000000 ork.build-0.0.55/bin_priv/obt.vscode.create.debug.task.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.171078 ork.build-0.0.55/bin_pub/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     5554 2023-07-15 05:31:23.000000 ork.build-0.0.55/bin_pub/obt.create.env.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     8060 2023-07-16 20:17:09.000000 ork.build-0.0.55/bin_pub/obt.init.env.py
+-rw-r--r--   0 michael    (501) wheel        (0)      445 2023-07-16 20:17:09.000000 ork.build-0.0.55/bin_pub/obt.ix.installdeps.gentoo.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2936 2023-07-16 20:17:09.000000 ork.build-0.0.55/bin_pub/obt.ix.installdeps.linuxcnc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2764 2023-07-16 20:17:09.000000 ork.build-0.0.55/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3161 2023-07-16 20:17:09.000000 ork.build-0.0.55/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py
+-rw-r--r--   0 michael    (501) wheel        (0)      446 2023-07-16 20:17:09.000000 ork.build-0.0.55/bin_pub/obt.osx.installdeps.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1670 2023-07-16 20:17:09.000000 ork.build-0.0.55/bin_pub/obt.versions.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.135159 ork.build-0.0.55/examples/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.171579 ork.build-0.0.55/examples/dep-overrides/
+-rw-r--r--   0 michael    (501) wheel        (0)     1530 2023-07-15 05:45:21.000000 ork.build-0.0.55/examples/dep-overrides/orkid.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.175480 ork.build-0.0.55/examples/litex1/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     4642 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex1/arty.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      389 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex1/bit2svf_nexysv.tcl
+-rw-r--r--   0 michael    (501) wheel        (0)    11759 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex1/cmod_a7_platform.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     3002 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex1/cmod_a7_target.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     4526 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex1/nexys_video.py
+-rw-r--r--   0 michael    (501) wheel        (0)      628 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex1/nexysv.cfg
+-rwxr-xr-x   0 michael    (501) wheel        (0)      247 2023-07-15 05:45:21.000000 ork.build-0.0.55/examples/litex1/soc_arty.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2559 2023-07-15 05:45:21.000000 ork.build-0.0.55/examples/litex1/soc_nexysv.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.178876 ork.build-0.0.55/examples/litex_zephyrtest/
+-rw-r--r--   0 michael    (501) wheel        (0)      213 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex_zephyrtest/CMakeLists.txt
+-rw-r--r--   0 michael    (501) wheel        (0)    11415 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex_zephyrtest/LICENSE
+-rw-r--r--   0 michael    (501) wheel        (0)     1015 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex_zephyrtest/README.rst
+-rwxr-xr-x   0 michael    (501) wheel        (0)      315 2023-07-15 05:41:15.000000 ork.build-0.0.55/examples/litex_zephyrtest/build.py
+-rw-r--r--   0 michael    (501) wheel        (0)      111 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex_zephyrtest/main.c
+-rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex_zephyrtest/prj.conf
+-rw-r--r--   0 michael    (501) wheel        (0)      703 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex_zephyrtest/sample.yaml
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.179284 ork.build-0.0.55/examples/litex_zephyrtest/src/
+-rw-r--r--   0 michael    (501) wheel        (0)     2515 2022-09-08 21:51:23.000000 ork.build-0.0.55/examples/litex_zephyrtest/src/main.c
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.142959 ork.build-0.0.55/modules/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.258203 ork.build-0.0.55/modules/dep/
+-rw-r--r--   0 michael    (501) wheel        (0)      718 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/dep/_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8257 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/dep/_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1276 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/_nnsvs.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1910 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/apitrace.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1776 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/dep/arachnepnr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1663 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/arm64_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1580 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/arm64_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2051 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/assimp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1712 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/astcencoder.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1675 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/audiofile.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1611 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/avr_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2206 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/avr_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2209 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/avr_libc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1793 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/bazel.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1302 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/blosc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     9272 2023-07-15 05:58:02.000000 ork.build-0.0.55/modules/dep/boost.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1248 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/bullet.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2004 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/calf.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1541 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/cgal.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2422 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/clang.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1408 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/cmake.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1428 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/cpppeglib.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1632 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/cppzmq.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1563 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/csvparser.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1257 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/cuda.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1684 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/dep/curlpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1757 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/cycles.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1579 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/depthaicore.py
+-rw-r--r--   0 michael    (501) wheel        (0)      992 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/drawtext.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1491 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/easyprof.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1454 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/eigen.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2047 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/embree.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1871 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/faust.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1577 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/dep/fcollada.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1737 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/ffmpeg.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1997 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/flatcam.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1676 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/fltk.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1891 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/fluidsynth.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1866 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/frameretrace.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1438 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/gcode_gpr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2148 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/dep/giflib.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1175 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/gitpython.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2601 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/glfw.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1544 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/glm.py
+-rw-r--r--   0 michael    (501) wheel        (0)      894 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/gnutar.py
+-rw-r--r--   0 michael    (501) wheel        (0)      756 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/houdini.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1731 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/dep/icestorm.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2898 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/igl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1767 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/irix65_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6593 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/irix65_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1150 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/irrlicht.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3478 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/ispc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2331 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/ispctexc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1316 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/jpegturbo.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1719 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/klein.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1079 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/lapack.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1065 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/lemongraph.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1301 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/lexertl14.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1664 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/dep/libcurl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1701 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/libfive.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1490 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/libpqpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1425 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/libsocket.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1419 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/libsurvive.py
+-rw-r--r--   0 michael    (501) wheel        (0)     7892 2023-07-15 05:58:02.000000 ork.build-0.0.55/modules/dep/libtorch.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1926 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/linuxcnc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2487 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/litex.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2529 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/llvm.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1339 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/lm32_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1066 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/lm32_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2937 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/dep/lua.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2135 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/dep/luajit.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1664 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/m68k_amiga_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1555 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/m68k_amiga_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3841 2023-07-15 06:16:54.000000 ork.build-0.0.55/modules/dep/minetest.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2009 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/moltenvk.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1244 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/nextpnr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2121 2023-07-16 20:17:09.000000 ork.build-0.0.55/modules/dep/ngc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1426 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/nlohmannjson.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1633 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/dep/nss.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1464 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/nsync_cpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3022 2023-07-16 20:17:09.000000 ork.build-0.0.55/modules/dep/nvtt.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1562 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/ocio.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2587 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/oiio.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1738 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/oneapimkl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1407 2023-07-15 07:36:59.000000 ork.build-0.0.55/modules/dep/openblas.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2857 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/dep/opencv.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1358 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/opencv_contrib.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1217 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/opendb.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1556 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/openexr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1332 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/openjpeg.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1270 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/openroad.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1791 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/opensubdiv.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1447 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/openvdb.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1376 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/openvr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5239 2023-07-16 20:17:09.000000 ork.build-0.0.55/modules/dep/orkid.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1306 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/osgeolaszip.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1495 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/osgeoliblas.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1345 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/osgeoproj.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1543 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/osgeotiff.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1447 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/osl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1249 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/ozzanim.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1619 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/pangolin.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1874 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/parsertl14.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.137276 ork.build-0.0.55/modules/dep/patches/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.136348 ork.build-0.0.55/modules/dep/patches/boost/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.259344 ork.build-0.0.55/modules/dep/patches/boost/chg/
+-rw-r--r--   0 michael    (501) wheel        (0)    22151 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/dep/patches/boost/chg/darwin.jam
+-rw-r--r--   0 michael    (501) wheel        (0)     1111 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/dep/patches/boost/chg/project-config.jam
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.259839 ork.build-0.0.55/modules/dep/patches/boost/ori/
+-rw-r--r--   0 michael    (501) wheel        (0)    22062 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/dep/patches/boost/ori/darwin.jam
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.262090 ork.build-0.0.55/modules/dep/patches/gcc/
+-rw-r--r--   0 michael    (501) wheel        (0)   116535 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/dep/patches/gcc/gcc.sgifixes.patch
+-rw-r--r--   0 michael    (501) wheel        (0)      522 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch
+-rw-r--r--   0 michael    (501) wheel        (0)      475 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/dep/patches/gcc/gcc.sgifixlibstdcpp02.patch
+-rw-r--r--   0 michael    (501) wheel        (0)      801 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/dep/patches/gcc/newlib.sgifixes.patch
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.137107 ork.build-0.0.55/modules/dep/patches/giflib/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.262582 ork.build-0.0.55/modules/dep/patches/giflib/chg/
+-rw-r--r--   0 michael    (501) wheel        (0)     5546 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/dep/patches/giflib/chg/Makefile
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.263063 ork.build-0.0.55/modules/dep/patches/giflib/ori/
+-rw-r--r--   0 michael    (501) wheel        (0)     4712 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/dep/patches/giflib/ori/Makefile
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.137777 ork.build-0.0.55/modules/dep/patches/pillar/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.263595 ork.build-0.0.55/modules/dep/patches/pillar/chg/
+-rw-r--r--   0 michael    (501) wheel        (0)     1660 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/dep/patches/pillar/chg/markdown.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.264063 ork.build-0.0.55/modules/dep/patches/pillar/ori/
+-rw-r--r--   0 michael    (501) wheel        (0)     1645 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/dep/patches/pillar/ori/markdown.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1748 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/dep/pillar.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2152 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/pkgconfig.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1362 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/portaudio.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2133 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/postgresql.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1989 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/premake.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1526 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/ptex.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1298 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/pugixml.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1488 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/pybind11.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1521 2023-07-16 20:17:09.000000 ork.build-0.0.55/modules/dep/pydefaults.py
+-rw-r--r--   0 michael    (501) wheel        (0)      822 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/pyopengl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1954 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/pyqt5.py
+-rw-r--r--   0 michael    (501) wheel        (0)      814 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/pyside2.py
+-rw-r--r--   0 michael    (501) wheel        (0)     7471 2023-07-15 08:06:28.000000 ork.build-0.0.55/modules/dep/python.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5932 2023-07-15 05:58:02.000000 ork.build-0.0.55/modules/dep/qt5.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1781 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/qt5ct.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5913 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/qt5forpython.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1942 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/rapidjson.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3538 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/realsense2.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1032 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/root.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1344 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/rtmidi.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1345 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/rv32_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1069 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/rv32_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1355 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/sigslot.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1215 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/simavr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1370 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/sse2neon.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2929 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/dep/tbb.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6552 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/dep/tflite.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3343 2023-07-15 06:17:46.000000 ork.build-0.0.55/modules/dep/ue5.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6344 2023-07-15 06:17:57.000000 ork.build-0.0.55/modules/dep/ue5_cesium.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1669 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/unittestpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2361 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/usd.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1289 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/vhacd.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1316 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/vivado.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2962 2023-07-15 06:17:29.000000 ork.build-0.0.55/modules/dep/vpf.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1892 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/dep/vrx.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1972 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/vst3sdk.py
+-rw-r--r--   0 michael    (501) wheel        (0)     4325 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/vulkan.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2772 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/wt4.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2144 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/dep/xatlas.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1107 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/dep/yarl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1887 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/dep/yosys.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1922 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/dep/zephyr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1719 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/dep/zmq.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.141797 ork.build-0.0.55/modules/docker/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.264992 ork.build-0.0.55/modules/docker/amigadev/
+-rw-r--r--   0 michael    (501) wheel        (0)     1042 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/amigadev/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     2813 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/amigadev/amigadev.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.267868 ork.build-0.0.55/modules/docker/amigadev/test1/
+-rw-r--r--   0 michael    (501) wheel        (0)      280 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/amigadev/test1/Makefile
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.268376 ork.build-0.0.55/modules/docker/amigadev/test1/S/
+-rw-r--r--   0 michael    (501) wheel        (0)        8 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/amigadev/test1/S/Startup-Sequence
+-rwxr-xr-x   0 michael    (501) wheel        (0)      418 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/amigadev/test1/_build.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      527 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/amigadev/test1/build.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.269365 ork.build-0.0.55/modules/docker/amigadev/test1/libs/
+-rw-r--r--   0 michael    (501) wheel        (0)     4688 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/amigadev/test1/libs/mathieeedoubbas.library
+-rw-r--r--   0 michael    (501) wheel        (0)    15728 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library
+-rw-r--r--   0 michael    (501) wheel        (0)     5351 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/amigadev/test1/main.cpp
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1177 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/amigadev/test1/test_fsuae.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      391 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/amigadev/test1/test_vamos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.270401 ork.build-0.0.55/modules/docker/androiddev/
+-rw-r--r--   0 michael    (501) wheel        (0)     1679 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/androiddev/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     2071 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/androiddev/androiddev.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.274682 ork.build-0.0.55/modules/docker/cicd/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.278738 ork.build-0.0.55/modules/docker/cicd/bin/
+-rw-r--r--   0 michael    (501) wheel        (0)        1 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/bin/__init__.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      457 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/bin/build_master_image.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      276 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/bin/build_worker_android_image.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      271 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/bin/build_worker_ub20_image.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      271 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/bin/build_worker_ub22_image.py
+-rw-r--r--   0 michael    (501) wheel        (0)      644 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/bin/ci_common.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       66 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/bin/launch_attached.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       64 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/bin/launch_detached.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       83 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/bin/launch_testnossl.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       46 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/bin/terminate.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1188 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/bin/test_worker_android.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1235 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/bin/test_worker_ub20.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1255 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/bin/test_worker_ub22.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.288089 ork.build-0.0.55/modules/docker/cicd/ci_impl/
+-rw-r--r--   0 michael    (501) wheel        (0)      307 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/TODO.txt
+-rw-r--r--   0 michael    (501) wheel        (0)     9906 2023-07-15 05:59:09.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/_masterimpl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6829 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/_watcher.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1087 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/_workerimpl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3772 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/_zmqssh.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.289833 ork.build-0.0.55/modules/docker/cicd/ci_impl/assets/
+-rw-r--r--   0 michael    (501) wheel        (0)    71033 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/assets/OrkidLogo.png
+-rw-r--r--   0 michael    (501) wheel        (0)     1778 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/assets/index.template
+-rw-r--r--   0 michael    (501) wheel        (0)     3091 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/assets/variant.template
+-rw-r--r--   0 michael    (501) wheel        (0)     4134 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/badge.py
+-rw-r--r--   0 michael    (501) wheel        (0)      218 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/dummy.svg
+-rw-r--r--   0 michael    (501) wheel        (0)     2881 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/httphandler.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1768 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/master.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2597 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/orkbb.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1538 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/process_log.py
+-rw-r--r--   0 michael    (501) wheel        (0)     7766 2023-07-15 05:58:48.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/scheduler.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/spin.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/start-master.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/start-worker.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     7710 2023-07-15 05:58:58.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/worker.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     4005 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/worker_build_branch.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1335 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/ci_impl/worker_fetch_branch.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1708 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/cicd/cicd.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.290820 ork.build-0.0.55/modules/docker/cicd/conf/
+-rw-r--r--   0 michael    (501) wheel        (0)      420 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/conf/nginx_app.conf
+-rw-r--r--   0 michael    (501) wheel        (0)      898 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/conf/nginx_ssl.conf
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.294209 ork.build-0.0.55/modules/docker/cicd/container-scripts/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2542 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2626 2023-07-16 20:17:09.000000 ork.build-0.0.55/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py
+-rw-r--r--   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/container-scripts/spin.sh
+-rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/container-scripts/start-master.sh
+-rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/container-scripts/start-worker.sh
+-rw-r--r--   0 michael    (501) wheel        (0)       20 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/container-scripts/worker.bashrc
+-rw-r--r--   0 michael    (501) wheel        (0)      221 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/container-scripts/worker.test.sh
+-rw-r--r--   0 michael    (501) wheel        (0)     1126 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/docker-compose-nossl.yml
+-rw-r--r--   0 michael    (501) wheel        (0)     1222 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/docker-compose.yml
+-rw-r--r--   0 michael    (501) wheel        (0)     2043 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/master.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     1045 2023-07-15 07:01:02.000000 ork.build-0.0.55/modules/docker/cicd/master.json
+-rw-r--r--   0 michael    (501) wheel        (0)      228 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/readme.md
+-rw-r--r--   0 michael    (501) wheel        (0)     3551 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/worker-android.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/worker-ub20.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/worker-ub22.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/worker20.json
+-rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/cicd/worker22.json
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.297186 ork.build-0.0.55/modules/docker/ps1dev/
+-rw-r--r--   0 michael    (501) wheel        (0)     1019 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/ps1dev/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     2268 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/ps1dev/Makefile.cfg
+-rwxr-xr-x   0 michael    (501) wheel        (0)      223 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/ps1dev/fetch.sh
+-rw-r--r--   0 michael    (501) wheel        (0)     2750 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/ps1dev/ps1dev.py
+-rw-r--r--   0 michael    (501) wheel        (0)       71 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/ps1dev/readme.md
+-rwxr-xr-x   0 michael    (501) wheel        (0)      756 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/ps1dev/setup.sh
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.297685 ork.build-0.0.55/modules/docker/ps1dev/testprograms/
+-rw-r--r--   0 michael    (501) wheel        (0)      890 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/ps1dev/testprograms/project.mk
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.298762 ork.build-0.0.55/modules/docker/ps1dev/testprograms/test1/
+-rw-r--r--   0 michael    (501) wheel        (0)       86 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/ps1dev/testprograms/test1/Makefile
+-rw-r--r--   0 michael    (501) wheel        (0)     7821 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/ps1dev/testprograms/test1/test1.c
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.300130 ork.build-0.0.55/modules/docker/realsense2/
+-rw-r--r--   0 michael    (501) wheel        (0)     2325 2023-02-05 19:12:10.000000 ork.build-0.0.55/modules/docker/realsense2/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     3446 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/realsense2/realsense2.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.302577 ork.build-0.0.55/modules/docker/sagemath/
+-rw-r--r--   0 michael    (501) wheel        (0)     2646 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/sagemath/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)      347 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/sagemath/docker-compose.yml
+-rwxr-xr-x   0 michael    (501) wheel        (0)      100 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/sagemath/entrypoint.sh
+-rw-r--r--   0 michael    (501) wheel        (0)     2757 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/sagemath/sagemath.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.305072 ork.build-0.0.55/modules/docker/tflow2gpu/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2775 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/tflow2gpu/Dockerfile
+-rwxr-xr-x   0 michael    (501) wheel        (0)      519 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/tflow2gpu/test_mediapipe.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2533 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/tflow2gpu/test_multi_gpu.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1715 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/tflow2gpu/test_single_gpu.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2483 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/tflow2gpu/tflow2gpu.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.306057 ork.build-0.0.55/modules/docker/ub-focal/
+-rw-r--r--   0 michael    (501) wheel        (0)      517 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/docker/ub-focal/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     1702 2023-07-15 05:59:22.000000 ork.build-0.0.55/modules/docker/ub-focal/ub-focal.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.307972 ork.build-0.0.55/modules/host/
+-rw-r--r--   0 michael    (501) wheel        (0)     1181 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/host/aarch64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1629 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/host/aarch64-macos.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1409 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/host/x86_64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2159 2023-07-16 23:22:36.000000 ork.build-0.0.55/modules/host/x86_64-macos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.311018 ork.build-0.0.55/modules/sdk/
+-rw-r--r--   0 michael    (501) wheel        (0)     4088 2023-07-15 05:43:34.000000 ork.build-0.0.55/modules/sdk/aarch64-android.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1678 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/sdk/aarch64-ios.py
+-rw-r--r--   0 michael    (501) wheel        (0)      776 2023-07-16 23:12:45.000000 ork.build-0.0.55/modules/sdk/aarch64-macos.py
+-rw-r--r--   0 michael    (501) wheel        (0)      222 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/sdk/cuda.py
+-rw-r--r--   0 michael    (501) wheel        (0)      618 2023-07-15 05:42:23.000000 ork.build-0.0.55/modules/sdk/x86_64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)      619 2023-07-16 23:12:52.000000 ork.build-0.0.55/modules/sdk/x86_64-macos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.312975 ork.build-0.0.55/modules/subspace/
+-rw-r--r--   0 michael    (501) wheel        (0)     7785 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/subspace/conda.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1227 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/subspace/host.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.313459 ork.build-0.0.55/modules/subspace/nnsvs/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     3419 2023-07-15 05:41:15.000000 ork.build-0.0.55/modules/subspace/nnsvs/test.py
+-rw-r--r--   0 michael    (501) wheel        (0)     4513 2023-07-15 05:54:20.000000 ork.build-0.0.55/modules/subspace/nnsvs.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1187 2023-07-15 05:45:21.000000 ork.build-0.0.55/modules/subspace/yo.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.316480 ork.build-0.0.55/modules/target/
+-rw-r--r--   0 michael    (501) wheel        (0)      558 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/target/aarch64-android.py
+-rw-r--r--   0 michael    (501) wheel        (0)      551 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/target/aarch64-ios.py
+-rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/target/aarch64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/target/aarch64-macos.py
+-rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/target/x86_64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build-0.0.55/modules/target/x86_64-macos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.143592 ork.build-0.0.55/scripts/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.336737 ork.build-0.0.55/scripts/obt/
+-rw-r--r--   0 michael    (501) wheel        (0)       67 2023-02-05 19:12:10.000000 ork.build-0.0.55/scripts/obt/__init__.py
+-rw-r--r--   0 michael    (501) wheel        (0)    12350 2023-07-15 05:51:25.000000 ork.build-0.0.55/scripts/obt/_dep_build.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1460 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/_dep_dl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1619 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/_dep_enumerate.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8444 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/_dep_fetch.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2872 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/_dep_impl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     4734 2023-07-15 09:08:14.000000 ork.build-0.0.55/scripts/obt/_dep_node.py
+-rw-r--r--   0 michael    (501) wheel        (0)    13516 2023-07-15 05:54:20.000000 ork.build-0.0.55/scripts/obt/_dep_provider.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3450 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/_dep_x.py
+-rw-r--r--   0 michael    (501) wheel        (0)    13033 2023-07-15 08:10:41.000000 ork.build-0.0.55/scripts/obt/_envutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1925 2022-09-08 21:51:24.000000 ork.build-0.0.55/scripts/obt/_globals.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5607 2023-07-15 05:42:23.000000 ork.build-0.0.55/scripts/obt/buildtrace.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2975 2023-07-15 05:52:48.000000 ork.build-0.0.55/scripts/obt/cmake.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.337839 ork.build-0.0.55/scripts/obt/cnc/
+-rw-r--r--   0 michael    (501) wheel        (0)        2 2023-02-05 19:12:10.000000 ork.build-0.0.55/scripts/obt/cnc/__init__.py
+-rw-r--r--   0 michael    (501) wheel        (0)     7782 2023-02-05 19:12:10.000000 ork.build-0.0.55/scripts/obt/cnc/saf.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8668 2023-07-15 05:49:59.000000 ork.build-0.0.55/scripts/obt/command.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1486 2022-09-08 21:51:24.000000 ork.build-0.0.55/scripts/obt/common.py
+-rw-r--r--   0 michael    (501) wheel        (0)      803 2022-09-08 21:51:24.000000 ork.build-0.0.55/scripts/obt/config.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8068 2022-09-08 21:51:24.000000 ork.build-0.0.55/scripts/obt/deco.py
+-rw-r--r--   0 michael    (501) wheel        (0)      849 2023-07-15 05:37:57.000000 ork.build-0.0.55/scripts/obt/dep.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2756 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/docker.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1266 2023-07-15 08:33:20.000000 ork.build-0.0.55/scripts/obt/env.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1806 2023-07-15 05:43:34.000000 ork.build-0.0.55/scripts/obt/executors.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1241 2023-07-15 05:41:15.000000 ork.build-0.0.55/scripts/obt/gen_pkgconfig.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5172 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/git.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2876 2023-07-15 06:14:59.000000 ork.build-0.0.55/scripts/obt/host.py
+-rw-r--r--   0 michael    (501) wheel        (0)      268 2022-09-08 21:51:24.000000 ork.build-0.0.55/scripts/obt/libav.py
+-rw-r--r--   0 michael    (501) wheel        (0)      927 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/litex.py
+-rw-r--r--   0 michael    (501) wheel        (0)      285 2023-07-15 05:37:17.000000 ork.build-0.0.55/scripts/obt/log.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2849 2023-07-15 05:43:34.000000 ork.build-0.0.55/scripts/obt/macos.py
+-rw-r--r--   0 michael    (501) wheel        (0)      141 2023-07-15 05:41:15.000000 ork.build-0.0.55/scripts/obt/macos_homebrew.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1080 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/make.py
+-rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:24.000000 ork.build-0.0.55/scripts/obt/math.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2040 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/module.py
+-rw-r--r--   0 michael    (501) wheel        (0)      145 2022-09-08 21:51:24.000000 ork.build-0.0.55/scripts/obt/net.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1194 2023-07-15 05:41:15.000000 ork.build-0.0.55/scripts/obt/osrelease.py
+-rw-r--r--   0 michael    (501) wheel        (0)      983 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/patch.py
+-rw-r--r--   0 michael    (501) wheel        (0)     9592 2023-07-16 20:17:09.000000 ork.build-0.0.55/scripts/obt/path.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8544 2023-07-15 05:41:15.000000 ork.build-0.0.55/scripts/obt/pathtools.py
+-rw-r--r--   0 michael    (501) wheel        (0)      668 2023-07-15 05:43:34.000000 ork.build-0.0.55/scripts/obt/pip.py
+-rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:24.000000 ork.build-0.0.55/scripts/obt/pybind11.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1341 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/scp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1755 2023-07-15 06:15:14.000000 ork.build-0.0.55/scripts/obt/sdk.py
+-rw-r--r--   0 michael    (501) wheel        (0)     4538 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/search.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3241 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/subspace.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1342 2023-07-15 06:16:16.000000 ork.build-0.0.55/scripts/obt/target.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1559 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/template.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6511 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/utils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2080 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/wget.py
+-rw-r--r--   0 michael    (501) wheel        (0)      591 2023-07-15 05:45:21.000000 ork.build-0.0.55/scripts/obt/xcode.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.340538 ork.build-0.0.55/scripts/ork.build.egg-info/
+-rw-r--r--   0 michael    (501) wheel        (0)    16892 2023-07-16 23:23:06.000000 ork.build-0.0.55/scripts/ork.build.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) wheel        (0)    12158 2023-07-16 23:23:06.000000 ork.build-0.0.55/scripts/ork.build.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) wheel        (0)        1 2023-07-16 23:23:06.000000 ork.build-0.0.55/scripts/ork.build.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) wheel        (0)       14 2023-07-16 23:23:06.000000 ork.build-0.0.55/scripts/ork.build.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) wheel        (0)        4 2023-07-16 23:23:06.000000 ork.build-0.0.55/scripts/ork.build.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) wheel        (0)       38 2023-07-16 23:23:06.348101 ork.build-0.0.55/setup.cfg
+-rw-r--r--   0 michael    (501) wheel        (0)     1966 2023-07-16 23:22:49.000000 ork.build-0.0.55/setup.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.341529 ork.build-0.0.55/tests/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.343532 ork.build-0.0.55/tests/docker-gpu/
+-rw-r--r--   0 michael    (501) wheel        (0)      411 2022-09-08 21:51:24.000000 ork.build-0.0.55/tests/docker-gpu/Dockerfile
+-rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build-0.0.55/tests/docker-gpu/build.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      358 2022-09-08 21:51:24.000000 ork.build-0.0.55/tests/docker-gpu/launch_glmark.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      369 2022-09-08 21:51:24.000000 ork.build-0.0.55/tests/docker-gpu/launch_nvtopo.sh
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.345625 ork.build-0.0.55/tests/docker-gpu-tensorflow/
+-rw-r--r--   0 michael    (501) wheel        (0)      505 2022-09-08 21:51:24.000000 ork.build-0.0.55/tests/docker-gpu-tensorflow/Dockerfile
+-rwxr-xr-x   0 michael    (501) wheel        (0)       55 2022-09-08 21:51:24.000000 ork.build-0.0.55/tests/docker-gpu-tensorflow/build.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      379 2022-09-08 21:51:24.000000 ork.build-0.0.55/tests/docker-gpu-tensorflow/launch_nvtopo.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      391 2022-09-08 21:51:24.000000 ork.build-0.0.55/tests/docker-gpu-tensorflow/launch_tf.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1543 2023-07-15 05:41:15.000000 ork.build-0.0.55/tests/litex1_nx4.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      178 2023-07-15 05:45:21.000000 ork.build-0.0.55/tests/osx_rpaths.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-16 23:23:06.346629 ork.build-0.0.55/tests/pytorch/
+-rwxr-xr-x   0 michael    (501) wheel        (0)      916 2023-07-15 05:43:34.000000 ork.build-0.0.55/tests/pytorch/install.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1190 2023-07-15 06:00:28.000000 ork.build-0.0.55/tests/pytorch/training.py
```

### Comparing `ork.build-0.0.54/PKG-INFO` & `ork.build-0.0.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ork.build
-Version: 0.0.54
+Version: 0.0.55
 Summary: Orkid Build Tools
 Home-page: https://github.com/tweakoz/ork.build
 Author: Michael T. Mayers
 Author-email: michael@tweakoz.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ork.build-0.0.54/README.md` & `ork.build-0.0.55/README.md`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.dep.build.py` & `ork.build-0.0.55/bin_priv/obt.dep.build.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.dep.findtext.py` & `ork.build-0.0.55/bin_priv/obt.dep.findtext.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.dep.info.py` & `ork.build-0.0.55/bin_priv/obt.dep.info.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.dep.list.py` & `ork.build-0.0.55/bin_priv/obt.dep.list.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.dep.replacetext.py` & `ork.build-0.0.55/bin_priv/obt.dep.replacetext.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.dep.shell.py` & `ork.build-0.0.55/bin_priv/obt.dep.shell.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.dep.status.py` & `ork.build-0.0.55/bin_priv/obt.dep.status.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.docker.build.py` & `ork.build-0.0.55/bin_priv/obt.docker.build.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.docker.info.py` & `ork.build-0.0.55/bin_priv/obt.docker.info.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.docker.kill.py` & `ork.build-0.0.55/bin_priv/obt.docker.kill.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.docker.launch.py` & `ork.build-0.0.55/bin_priv/obt.docker.launch.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.docker.list.py` & `ork.build-0.0.55/bin_priv/obt.docker.list.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.docker.method.py` & `ork.build-0.0.55/bin_priv/obt.docker.method.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.ext.find.py` & `ork.build-0.0.55/bin_priv/obt.ext.find.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.find.in.dep.py` & `ork.build-0.0.55/bin_priv/obt.find.in.dep.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.find.py` & `ork.build-0.0.55/bin_priv/obt.find.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.host.info.py` & `ork.build-0.0.55/bin_priv/obt.host.info.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.installedacontainers.py` & `ork.build-0.0.55/bin_priv/obt.installedacontainers.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.litex.env.py` & `ork.build-0.0.55/bin_priv/obt.litex.env.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.litex.zephyrriscv-sample.py` & `ork.build-0.0.55/bin_priv/obt.litex.zephyrriscv-sample.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.lsusbx.py` & `ork.build-0.0.55/bin_priv/obt.lsusbx.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.osx.macho.fixup.libs.py` & `ork.build-0.0.55/bin_priv/obt.osx.macho.fixup.libs.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.replace.py` & `ork.build-0.0.55/bin_priv/obt.replace.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.sdk.info.py` & `ork.build-0.0.55/bin_priv/obt.sdk.info.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.sdk.install.py` & `ork.build-0.0.55/bin_priv/obt.sdk.install.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.subspace.build.py` & `ork.build-0.0.55/bin_priv/obt.subspace.build.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.subspace.launch.py` & `ork.build-0.0.55/bin_priv/obt.subspace.launch.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.subspace.list.py` & `ork.build-0.0.55/bin_priv/obt.subspace.list.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.target.info.py` & `ork.build-0.0.55/bin_priv/obt.target.info.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.vivado.getsites.py` & `ork.build-0.0.55/bin_priv/obt.vivado.getsites.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.vivado.launch.py` & `ork.build-0.0.55/bin_priv/obt.vivado.launch.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_priv/obt.vscode.create.debug.task.py` & `ork.build-0.0.55/bin_priv/obt.vscode.create.debug.task.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_pub/obt.create.env.py` & `ork.build-0.0.55/bin_pub/obt.create.env.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_pub/obt.init.env.py` & `ork.build-0.0.55/bin_pub/obt.init.env.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_pub/obt.ix.installdeps.linuxcnc.py` & `ork.build-0.0.55/bin_pub/obt.ix.installdeps.linuxcnc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py` & `ork.build-0.0.55/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py` & `ork.build-0.0.55/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/bin_pub/obt.versions.py` & `ork.build-0.0.55/bin_pub/obt.versions.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/examples/dep-overrides/orkid.py` & `ork.build-0.0.55/examples/dep-overrides/orkid.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/examples/litex1/arty.py` & `ork.build-0.0.55/examples/litex1/arty.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/examples/litex1/cmod_a7_platform.py` & `ork.build-0.0.55/examples/litex1/cmod_a7_platform.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/examples/litex1/cmod_a7_target.py` & `ork.build-0.0.55/examples/litex1/cmod_a7_target.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/examples/litex1/nexys_video.py` & `ork.build-0.0.55/examples/litex1/nexys_video.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/examples/litex1/nexysv.cfg` & `ork.build-0.0.55/examples/litex1/nexysv.cfg`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/examples/litex1/soc_nexysv.py` & `ork.build-0.0.55/examples/litex1/soc_nexysv.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/examples/litex_zephyrtest/LICENSE` & `ork.build-0.0.55/examples/litex_zephyrtest/LICENSE`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/examples/litex_zephyrtest/README.rst` & `ork.build-0.0.55/examples/litex_zephyrtest/README.rst`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/examples/litex_zephyrtest/sample.yaml` & `ork.build-0.0.55/examples/litex_zephyrtest/sample.yaml`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/examples/litex_zephyrtest/src/main.c` & `ork.build-0.0.55/examples/litex_zephyrtest/src/main.c`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/_binutils.py` & `ork.build-0.0.55/modules/dep/_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/_gcc.py` & `ork.build-0.0.55/modules/dep/_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/_nnsvs.py` & `ork.build-0.0.55/modules/dep/_nnsvs.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/apitrace.py` & `ork.build-0.0.55/modules/dep/apitrace.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/arachnepnr.py` & `ork.build-0.0.55/modules/dep/arachnepnr.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/arm64_binutils.py` & `ork.build-0.0.55/modules/dep/arm64_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/arm64_gcc.py` & `ork.build-0.0.55/modules/dep/arm64_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/assimp.py` & `ork.build-0.0.55/modules/dep/assimp.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/astcencoder.py` & `ork.build-0.0.55/modules/dep/astcencoder.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/audiofile.py` & `ork.build-0.0.55/modules/dep/audiofile.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/avr_binutils.py` & `ork.build-0.0.55/modules/dep/avr_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/avr_gcc.py` & `ork.build-0.0.55/modules/dep/avr_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/avr_libc.py` & `ork.build-0.0.55/modules/dep/avr_libc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/bazel.py` & `ork.build-0.0.55/modules/dep/bazel.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/blosc.py` & `ork.build-0.0.55/modules/dep/blosc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/boost.py` & `ork.build-0.0.55/modules/dep/boost.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/bullet.py` & `ork.build-0.0.55/modules/dep/bullet.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/calf.py` & `ork.build-0.0.55/modules/dep/calf.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/cgal.py` & `ork.build-0.0.55/modules/dep/cgal.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/clang.py` & `ork.build-0.0.55/modules/dep/clang.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/cmake.py` & `ork.build-0.0.55/modules/dep/cmake.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/cpppeglib.py` & `ork.build-0.0.55/modules/dep/cpppeglib.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/cppzmq.py` & `ork.build-0.0.55/modules/dep/cppzmq.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/csvparser.py` & `ork.build-0.0.55/modules/dep/csvparser.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/cuda.py` & `ork.build-0.0.55/modules/dep/cuda.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/curlpp.py` & `ork.build-0.0.55/modules/dep/curlpp.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/cycles.py` & `ork.build-0.0.55/modules/dep/cycles.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/depthaicore.py` & `ork.build-0.0.55/modules/dep/depthaicore.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/drawtext.py` & `ork.build-0.0.55/modules/dep/drawtext.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/easyprof.py` & `ork.build-0.0.55/modules/dep/easyprof.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/eigen.py` & `ork.build-0.0.55/modules/dep/eigen.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/embree.py` & `ork.build-0.0.55/modules/dep/embree.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/faust.py` & `ork.build-0.0.55/modules/dep/faust.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/fcollada.py` & `ork.build-0.0.55/modules/dep/fcollada.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/ffmpeg.py` & `ork.build-0.0.55/modules/dep/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/flatcam.py` & `ork.build-0.0.55/modules/dep/flatcam.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/fltk.py` & `ork.build-0.0.55/modules/dep/fltk.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/fluidsynth.py` & `ork.build-0.0.55/modules/dep/fluidsynth.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/frameretrace.py` & `ork.build-0.0.55/modules/dep/frameretrace.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/gcode_gpr.py` & `ork.build-0.0.55/modules/dep/gcode_gpr.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/giflib.py` & `ork.build-0.0.55/modules/dep/giflib.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/gitpython.py` & `ork.build-0.0.55/modules/dep/gitpython.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/glfw.py` & `ork.build-0.0.55/modules/dep/glfw.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/glm.py` & `ork.build-0.0.55/modules/dep/glm.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/gnutar.py` & `ork.build-0.0.55/modules/dep/gnutar.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/houdini.py` & `ork.build-0.0.55/modules/dep/houdini.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/icestorm.py` & `ork.build-0.0.55/modules/dep/icestorm.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/igl.py` & `ork.build-0.0.55/modules/dep/igl.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/irix65_binutils.py` & `ork.build-0.0.55/modules/dep/irix65_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/irix65_gcc.py` & `ork.build-0.0.55/modules/dep/irix65_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/irrlicht.py` & `ork.build-0.0.55/modules/dep/irrlicht.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/ispc.py` & `ork.build-0.0.55/modules/dep/ispc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/ispctexc.py` & `ork.build-0.0.55/modules/dep/ispctexc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/jpegturbo.py` & `ork.build-0.0.55/modules/dep/jpegturbo.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/klein.py` & `ork.build-0.0.55/modules/dep/klein.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/lapack.py` & `ork.build-0.0.55/modules/dep/lapack.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/lemongraph.py` & `ork.build-0.0.55/modules/dep/lemongraph.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/lexertl14.py` & `ork.build-0.0.55/modules/dep/lexertl14.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/libcurl.py` & `ork.build-0.0.55/modules/dep/libcurl.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/libfive.py` & `ork.build-0.0.55/modules/dep/libfive.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/libpqpp.py` & `ork.build-0.0.55/modules/dep/libpqpp.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/libsocket.py` & `ork.build-0.0.55/modules/dep/libsocket.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/libsurvive.py` & `ork.build-0.0.55/modules/dep/libsurvive.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/libtorch.py` & `ork.build-0.0.55/modules/dep/libtorch.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/linuxcnc.py` & `ork.build-0.0.55/modules/dep/linuxcnc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/litex.py` & `ork.build-0.0.55/modules/dep/litex.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/llvm.py` & `ork.build-0.0.55/modules/dep/llvm.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/lm32_binutils.py` & `ork.build-0.0.55/modules/dep/lm32_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/lm32_gcc.py` & `ork.build-0.0.55/modules/dep/lm32_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/lua.py` & `ork.build-0.0.55/modules/dep/lua.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/luajit.py` & `ork.build-0.0.55/modules/dep/luajit.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/m68k_amiga_binutils.py` & `ork.build-0.0.55/modules/dep/m68k_amiga_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/m68k_amiga_gcc.py` & `ork.build-0.0.55/modules/dep/m68k_amiga_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/minetest.py` & `ork.build-0.0.55/modules/dep/minetest.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/moltenvk.py` & `ork.build-0.0.55/modules/dep/moltenvk.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/nextpnr.py` & `ork.build-0.0.55/modules/dep/nextpnr.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/ngc.py` & `ork.build-0.0.55/modules/dep/ngc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/nlohmannjson.py` & `ork.build-0.0.55/modules/dep/nlohmannjson.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/nss.py` & `ork.build-0.0.55/modules/dep/nss.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/nsync_cpp.py` & `ork.build-0.0.55/modules/dep/nsync_cpp.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/nvtt.py` & `ork.build-0.0.55/modules/dep/nvtt.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/ocio.py` & `ork.build-0.0.55/modules/dep/ocio.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/oiio.py` & `ork.build-0.0.55/modules/dep/oiio.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/oneapimkl.py` & `ork.build-0.0.55/modules/dep/oneapimkl.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/openblas.py` & `ork.build-0.0.55/modules/dep/openblas.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/opencv.py` & `ork.build-0.0.55/modules/dep/opencv.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/opencv_contrib.py` & `ork.build-0.0.55/modules/dep/opencv_contrib.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/opendb.py` & `ork.build-0.0.55/modules/dep/opendb.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/openexr.py` & `ork.build-0.0.55/modules/dep/openexr.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/openjpeg.py` & `ork.build-0.0.55/modules/dep/openjpeg.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/openroad.py` & `ork.build-0.0.55/modules/dep/openroad.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/opensubdiv.py` & `ork.build-0.0.55/modules/dep/opensubdiv.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/openvdb.py` & `ork.build-0.0.55/modules/dep/openvdb.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/openvr.py` & `ork.build-0.0.55/modules/dep/openvr.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/orkid.py` & `ork.build-0.0.55/modules/dep/orkid.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/osgeolaszip.py` & `ork.build-0.0.55/modules/dep/osgeolaszip.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/osgeoliblas.py` & `ork.build-0.0.55/modules/dep/osgeoliblas.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/osgeoproj.py` & `ork.build-0.0.55/modules/dep/osgeoproj.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/osgeotiff.py` & `ork.build-0.0.55/modules/dep/osgeotiff.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/osl.py` & `ork.build-0.0.55/modules/dep/osl.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/ozzanim.py` & `ork.build-0.0.55/modules/dep/ozzanim.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/pangolin.py` & `ork.build-0.0.55/modules/dep/pangolin.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/parsertl14.py` & `ork.build-0.0.55/modules/dep/parsertl14.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/patches/boost/chg/darwin.jam` & `ork.build-0.0.55/modules/dep/patches/boost/chg/darwin.jam`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/patches/boost/chg/project-config.jam` & `ork.build-0.0.55/modules/dep/patches/boost/chg/project-config.jam`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/patches/boost/ori/darwin.jam` & `ork.build-0.0.55/modules/dep/patches/boost/ori/darwin.jam`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/patches/gcc/gcc.sgifixes.patch` & `ork.build-0.0.55/modules/dep/patches/gcc/gcc.sgifixes.patch`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch` & `ork.build-0.0.55/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/patches/gcc/newlib.sgifixes.patch` & `ork.build-0.0.55/modules/dep/patches/gcc/newlib.sgifixes.patch`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/patches/giflib/chg/Makefile` & `ork.build-0.0.55/modules/dep/patches/giflib/chg/Makefile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/patches/giflib/ori/Makefile` & `ork.build-0.0.55/modules/dep/patches/giflib/ori/Makefile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/patches/pillar/chg/markdown.py` & `ork.build-0.0.55/modules/dep/patches/pillar/chg/markdown.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/patches/pillar/ori/markdown.py` & `ork.build-0.0.55/modules/dep/patches/pillar/ori/markdown.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/pillar.py` & `ork.build-0.0.55/modules/dep/pillar.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/pkgconfig.py` & `ork.build-0.0.55/modules/dep/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/portaudio.py` & `ork.build-0.0.55/modules/dep/portaudio.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/postgresql.py` & `ork.build-0.0.55/modules/dep/postgresql.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/premake.py` & `ork.build-0.0.55/modules/dep/premake.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/ptex.py` & `ork.build-0.0.55/modules/dep/ptex.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/pugixml.py` & `ork.build-0.0.55/modules/dep/pugixml.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/pybind11.py` & `ork.build-0.0.55/modules/dep/pybind11.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/pydefaults.py` & `ork.build-0.0.55/modules/dep/pydefaults.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/pyopengl.py` & `ork.build-0.0.55/modules/dep/pyopengl.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/pyqt5.py` & `ork.build-0.0.55/modules/dep/pyqt5.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/pyside2.py` & `ork.build-0.0.55/modules/dep/pyside2.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/python.py` & `ork.build-0.0.55/modules/dep/python.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/qt5.py` & `ork.build-0.0.55/modules/dep/qt5.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/qt5ct.py` & `ork.build-0.0.55/modules/dep/qt5ct.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/qt5forpython.py` & `ork.build-0.0.55/modules/dep/qt5forpython.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/rapidjson.py` & `ork.build-0.0.55/modules/dep/rapidjson.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/realsense2.py` & `ork.build-0.0.55/modules/dep/realsense2.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/root.py` & `ork.build-0.0.55/modules/dep/root.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/rtmidi.py` & `ork.build-0.0.55/modules/dep/rtmidi.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/rv32_binutils.py` & `ork.build-0.0.55/modules/dep/rv32_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/rv32_gcc.py` & `ork.build-0.0.55/modules/dep/rv32_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/sigslot.py` & `ork.build-0.0.55/modules/dep/sigslot.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/simavr.py` & `ork.build-0.0.55/modules/dep/simavr.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/sse2neon.py` & `ork.build-0.0.55/modules/dep/sse2neon.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/tbb.py` & `ork.build-0.0.55/modules/dep/tbb.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/tflite.py` & `ork.build-0.0.55/modules/dep/tflite.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/ue5.py` & `ork.build-0.0.55/modules/dep/ue5.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/ue5_cesium.py` & `ork.build-0.0.55/modules/dep/ue5_cesium.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/unittestpp.py` & `ork.build-0.0.55/modules/dep/unittestpp.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/usd.py` & `ork.build-0.0.55/modules/dep/usd.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/vhacd.py` & `ork.build-0.0.55/modules/dep/vhacd.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/vivado.py` & `ork.build-0.0.55/modules/dep/vivado.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/vpf.py` & `ork.build-0.0.55/modules/dep/vpf.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/vrx.py` & `ork.build-0.0.55/modules/dep/vrx.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/vst3sdk.py` & `ork.build-0.0.55/modules/dep/vst3sdk.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/vulkan.py` & `ork.build-0.0.55/modules/dep/vulkan.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/wt4.py` & `ork.build-0.0.55/modules/dep/wt4.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/xatlas.py` & `ork.build-0.0.55/modules/dep/xatlas.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/yarl.py` & `ork.build-0.0.55/modules/dep/yarl.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/yosys.py` & `ork.build-0.0.55/modules/dep/yosys.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/zephyr.py` & `ork.build-0.0.55/modules/dep/zephyr.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/dep/zmq.py` & `ork.build-0.0.55/modules/dep/zmq.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/amigadev/Dockerfile` & `ork.build-0.0.55/modules/docker/amigadev/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/amigadev/amigadev.py` & `ork.build-0.0.55/modules/docker/amigadev/amigadev.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/amigadev/test1/build.py` & `ork.build-0.0.55/modules/docker/amigadev/test1/build.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/amigadev/test1/libs/mathieeedoubbas.library` & `ork.build-0.0.55/modules/docker/amigadev/test1/libs/mathieeedoubbas.library`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library` & `ork.build-0.0.55/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/amigadev/test1/main.cpp` & `ork.build-0.0.55/modules/docker/amigadev/test1/main.cpp`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/amigadev/test1/test_fsuae.py` & `ork.build-0.0.55/modules/docker/amigadev/test1/test_fsuae.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/androiddev/Dockerfile` & `ork.build-0.0.55/modules/docker/androiddev/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/androiddev/androiddev.py` & `ork.build-0.0.55/modules/docker/androiddev/androiddev.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/bin/ci_common.py` & `ork.build-0.0.55/modules/docker/cicd/bin/ci_common.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/bin/test_worker_android.py` & `ork.build-0.0.55/modules/docker/cicd/bin/test_worker_android.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/bin/test_worker_ub20.py` & `ork.build-0.0.55/modules/docker/cicd/bin/test_worker_ub20.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/bin/test_worker_ub22.py` & `ork.build-0.0.55/modules/docker/cicd/bin/test_worker_ub22.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/_masterimpl.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/_masterimpl.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/_watcher.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/_watcher.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/_workerimpl.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/_workerimpl.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/_zmqssh.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/_zmqssh.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/assets/OrkidLogo.png` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/assets/OrkidLogo.png`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/assets/index.template` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/assets/index.template`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/assets/variant.template` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/assets/variant.template`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/badge.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/badge.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/httphandler.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/httphandler.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/master.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/master.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/orkbb.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/orkbb.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/process_log.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/process_log.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/scheduler.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/scheduler.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/worker.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/worker.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/worker_build_branch.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/worker_build_branch.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/ci_impl/worker_fetch_branch.py` & `ork.build-0.0.55/modules/docker/cicd/ci_impl/worker_fetch_branch.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/cicd.py` & `ork.build-0.0.55/modules/docker/cicd/cicd.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/conf/nginx_ssl.conf` & `ork.build-0.0.55/modules/docker/cicd/conf/nginx_ssl.conf`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py` & `ork.build-0.0.55/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py` & `ork.build-0.0.55/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/docker-compose-nossl.yml` & `ork.build-0.0.55/modules/docker/cicd/docker-compose-nossl.yml`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/docker-compose.yml` & `ork.build-0.0.55/modules/docker/cicd/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/master.dockerfile` & `ork.build-0.0.55/modules/docker/cicd/master.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/master.json` & `ork.build-0.0.55/modules/docker/cicd/master.json`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/worker-android.dockerfile` & `ork.build-0.0.55/modules/docker/cicd/worker-android.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/worker-ub20.dockerfile` & `ork.build-0.0.55/modules/docker/cicd/worker-ub20.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/cicd/worker-ub22.dockerfile` & `ork.build-0.0.55/modules/docker/cicd/worker-ub22.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/ps1dev/Dockerfile` & `ork.build-0.0.55/modules/docker/ps1dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/ps1dev/Makefile.cfg` & `ork.build-0.0.55/modules/docker/ps1dev/Makefile.cfg`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/ps1dev/ps1dev.py` & `ork.build-0.0.55/modules/docker/ps1dev/ps1dev.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/ps1dev/setup.sh` & `ork.build-0.0.55/modules/docker/ps1dev/setup.sh`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/ps1dev/testprograms/project.mk` & `ork.build-0.0.55/modules/docker/ps1dev/testprograms/project.mk`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/ps1dev/testprograms/test1/test1.c` & `ork.build-0.0.55/modules/docker/ps1dev/testprograms/test1/test1.c`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/realsense2/Dockerfile` & `ork.build-0.0.55/modules/docker/realsense2/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/realsense2/realsense2.py` & `ork.build-0.0.55/modules/docker/realsense2/realsense2.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/sagemath/Dockerfile` & `ork.build-0.0.55/modules/docker/sagemath/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/sagemath/sagemath.py` & `ork.build-0.0.55/modules/docker/sagemath/sagemath.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/tflow2gpu/Dockerfile` & `ork.build-0.0.55/modules/docker/tflow2gpu/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/tflow2gpu/test_mediapipe.sh` & `ork.build-0.0.55/modules/docker/tflow2gpu/test_mediapipe.sh`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/tflow2gpu/test_multi_gpu.py` & `ork.build-0.0.55/modules/docker/tflow2gpu/test_multi_gpu.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/tflow2gpu/test_single_gpu.py` & `ork.build-0.0.55/modules/docker/tflow2gpu/test_single_gpu.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/tflow2gpu/tflow2gpu.py` & `ork.build-0.0.55/modules/docker/tflow2gpu/tflow2gpu.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/ub-focal/Dockerfile` & `ork.build-0.0.55/modules/docker/ub-focal/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/docker/ub-focal/ub-focal.py` & `ork.build-0.0.55/modules/docker/ub-focal/ub-focal.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/host/aarch64-linux.py` & `ork.build-0.0.55/modules/host/aarch64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/host/aarch64-macos.py` & `ork.build-0.0.55/modules/host/aarch64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/host/x86_64-linux.py` & `ork.build-0.0.55/modules/host/x86_64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/host/x86_64-macos.py` & `ork.build-0.0.55/modules/host/x86_64-macos.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,17 @@
     _xcodesdkstr = command.capture([
       "xcodebuild",
       "-version",
       "-sdk","macosx"]).splitlines()
     for l in _xcodesdkstr:
       x = l.split(": ")
       if x[0]=="Path":
-        env.append("OBT_MACOS_SDK_DIR",x[1])
+        env.set("OBT_MACOS_SDK_DIR",x[1])
       if x[0]=="PlatformVersion":
-        env.append("OBT_MACOS_PLATFORM_VERSION",x[1])
+        env.set("OBT_MACOS_PLATFORM_VERSION",x[1])
     print("MACOS-X86_64 Host Activated...")
   ###################################
   @property
   def num_cores(self):
     return multiprocessing.cpu_count()
   ###################################
   @property
```

### Comparing `ork.build-0.0.54/modules/sdk/aarch64-android.py` & `ork.build-0.0.55/modules/sdk/aarch64-android.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/sdk/aarch64-ios.py` & `ork.build-0.0.55/modules/sdk/aarch64-ios.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/sdk/aarch64-macos.py` & `ork.build-0.0.55/modules/sdk/aarch64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/sdk/x86_64-linux.py` & `ork.build-0.0.55/modules/sdk/x86_64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/sdk/x86_64-macos.py` & `ork.build-0.0.55/modules/sdk/x86_64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/subspace/conda.py` & `ork.build-0.0.55/modules/subspace/conda.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/subspace/host.py` & `ork.build-0.0.55/modules/subspace/host.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/subspace/nnsvs/test.py` & `ork.build-0.0.55/modules/subspace/nnsvs/test.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/subspace/nnsvs.py` & `ork.build-0.0.55/modules/subspace/nnsvs.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/subspace/yo.py` & `ork.build-0.0.55/modules/subspace/yo.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/target/aarch64-android.py` & `ork.build-0.0.55/modules/target/aarch64-android.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/target/aarch64-ios.py` & `ork.build-0.0.55/modules/target/aarch64-ios.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/target/aarch64-linux.py` & `ork.build-0.0.55/modules/target/aarch64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/target/aarch64-macos.py` & `ork.build-0.0.55/modules/target/aarch64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/target/x86_64-linux.py` & `ork.build-0.0.55/modules/target/x86_64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/modules/target/x86_64-macos.py` & `ork.build-0.0.55/modules/target/x86_64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/_dep_build.py` & `ork.build-0.0.55/scripts/obt/_dep_build.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/_dep_dl.py` & `ork.build-0.0.55/scripts/obt/_dep_dl.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/_dep_enumerate.py` & `ork.build-0.0.55/scripts/obt/_dep_enumerate.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/_dep_fetch.py` & `ork.build-0.0.55/scripts/obt/_dep_fetch.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/_dep_impl.py` & `ork.build-0.0.55/scripts/obt/_dep_impl.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/_dep_node.py` & `ork.build-0.0.55/scripts/obt/_dep_node.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/_dep_provider.py` & `ork.build-0.0.55/scripts/obt/_dep_provider.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/_dep_x.py` & `ork.build-0.0.55/scripts/obt/_dep_x.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/_envutils.py` & `ork.build-0.0.55/scripts/obt/_envutils.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/_globals.py` & `ork.build-0.0.55/scripts/obt/_globals.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/buildtrace.py` & `ork.build-0.0.55/scripts/obt/buildtrace.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/cmake.py` & `ork.build-0.0.55/scripts/obt/cmake.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/cnc/saf.py` & `ork.build-0.0.55/scripts/obt/cnc/saf.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/command.py` & `ork.build-0.0.55/scripts/obt/command.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/common.py` & `ork.build-0.0.55/scripts/obt/common.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/config.py` & `ork.build-0.0.55/scripts/obt/config.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/deco.py` & `ork.build-0.0.55/scripts/obt/deco.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/dep.py` & `ork.build-0.0.55/scripts/obt/dep.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/docker.py` & `ork.build-0.0.55/scripts/obt/docker.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/env.py` & `ork.build-0.0.55/scripts/obt/env.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/executors.py` & `ork.build-0.0.55/scripts/obt/executors.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/gen_pkgconfig.py` & `ork.build-0.0.55/scripts/obt/gen_pkgconfig.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/git.py` & `ork.build-0.0.55/scripts/obt/git.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/host.py` & `ork.build-0.0.55/scripts/obt/host.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/litex.py` & `ork.build-0.0.55/scripts/obt/litex.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/macos.py` & `ork.build-0.0.55/scripts/obt/macos.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/make.py` & `ork.build-0.0.55/scripts/obt/make.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/module.py` & `ork.build-0.0.55/scripts/obt/module.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/osrelease.py` & `ork.build-0.0.55/scripts/obt/osrelease.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/patch.py` & `ork.build-0.0.55/scripts/obt/patch.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/path.py` & `ork.build-0.0.55/scripts/obt/path.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/pathtools.py` & `ork.build-0.0.55/scripts/obt/pathtools.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/pip.py` & `ork.build-0.0.55/scripts/obt/pip.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/scp.py` & `ork.build-0.0.55/scripts/obt/scp.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/sdk.py` & `ork.build-0.0.55/scripts/obt/sdk.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/search.py` & `ork.build-0.0.55/scripts/obt/search.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/subspace.py` & `ork.build-0.0.55/scripts/obt/subspace.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/target.py` & `ork.build-0.0.55/scripts/obt/target.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/template.py` & `ork.build-0.0.55/scripts/obt/template.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/utils.py` & `ork.build-0.0.55/scripts/obt/utils.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/wget.py` & `ork.build-0.0.55/scripts/obt/wget.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/obt/xcode.py` & `ork.build-0.0.55/scripts/obt/xcode.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/scripts/ork.build.egg-info/PKG-INFO` & `ork.build-0.0.55/scripts/ork.build.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ork.build
-Version: 0.0.54
+Version: 0.0.55
 Summary: Orkid Build Tools
 Home-page: https://github.com/tweakoz/ork.build
 Author: Michael T. Mayers
 Author-email: michael@tweakoz.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ork.build-0.0.54/scripts/ork.build.egg-info/SOURCES.txt` & `ork.build-0.0.55/scripts/ork.build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/setup.py` & `ork.build-0.0.55/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import glob, os
 import platform
 
-version = "0.0.54"
+version = "0.0.55"
 
 ###############################################################################
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 ###############################################################################
```

### Comparing `ork.build-0.0.54/tests/litex1_nx4.py` & `ork.build-0.0.55/tests/litex1_nx4.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/tests/pytorch/install.py` & `ork.build-0.0.55/tests/pytorch/install.py`

 * *Files identical despite different names*

### Comparing `ork.build-0.0.54/tests/pytorch/training.py` & `ork.build-0.0.55/tests/pytorch/training.py`

 * *Files identical despite different names*

