# Comparing `tmp/gambaterm-0.9.8.tar.gz` & `tmp/gambaterm-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gambaterm-0.9.8.tar", last modified: Sun Aug 21 15:45:48 2022, max compression
+gzip compressed data, was "gambaterm-0.9.9.tar", last modified: Sun Aug 21 20:23:54 2022, max compression
```

## Comparing `gambaterm-0.9.8.tar` & `gambaterm-0.9.9.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.156344 gambaterm-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-08-21 15:45:42.000000 gambaterm-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-08-21 15:45:42.000000 gambaterm-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10832 2022-08-21 15:45:48.156344 gambaterm-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10103 2022-08-21 15:45:42.000000 gambaterm-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.144343 gambaterm-0.9.8/gambaterm/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2627 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/audio.py
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2547 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/controller_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/file_input.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7700 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/keyboard_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     5375 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/main.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5861 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     9264 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/ssh.py
--rw-r--r--   0 runner    (1001) docker     (121)     3515 2022-08-21 15:45:42.000000 gambaterm-0.9.8/gambaterm/ssh_app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.144343 gambaterm-0.9.8/gambaterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10832 2022-08-21 15:45:47.000000 gambaterm-0.9.8/gambaterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3283 2022-08-21 15:45:48.000000 gambaterm-0.9.8/gambaterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-21 15:45:47.000000 gambaterm-0.9.8/gambaterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-08-21 15:45:47.000000 gambaterm-0.9.8/gambaterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-08-21 15:45:47.000000 gambaterm-0.9.8/gambaterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-21 15:45:47.000000 gambaterm-0.9.8/gambaterm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.140343 gambaterm-0.9.8/libgambatte/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.144343 gambaterm-0.9.8/libgambatte/common/
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/common/array.h
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/common/defined_ptr.h
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/common/scoped_ptr.h
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/common/transfer_ptr.h
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/common/uncopyable.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.144343 gambaterm-0.9.8/libgambatte/include/
--rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/include/gambatte.h
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/include/gbint.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1193 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/include/inputgetter.h
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/include/loadres.h
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/include/pakinfo.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.148343 gambaterm-0.9.8/libgambatte/src/
--rw-r--r--   0 runner    (1001) docker     (121)    11368 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/bitmap_font.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/bitmap_font.h
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/counterdef.h
--rw-r--r--   0 runner    (1001) docker     (121)    45665 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/cpu.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.152344 gambaterm-0.9.8/libgambatte/src/file/
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/file/file.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/file/file.h
--rw-r--r--   0 runner    (1001) docker     (121)     5028 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/file/file_zip.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/file/stdfile.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.152344 gambaterm-0.9.8/libgambatte/src/file/unzip/
--rw-r--r--   0 runner    (1001) docker     (121)     4712 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/file/unzip/crypt.h
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/file/unzip/ioapi.h
--rw-r--r--   0 runner    (1001) docker     (121)    13009 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/file/unzip/unzip.h
--rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/gambatte.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    82449 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/initstate.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/initstate.h
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/insertion_sort.h
--rw-r--r--   0 runner    (1001) docker     (121)     2838 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/interrupter.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/interrupter.h
--rw-r--r--   0 runner    (1001) docker     (121)     3557 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/interruptrequester.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3611 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/interruptrequester.h
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/loadres.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.152344 gambaterm-0.9.8/libgambatte/src/mem/
--rw-r--r--   0 runner    (1001) docker     (121)    19458 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/mem/cartridge.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3553 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/mem/cartridge.h
--rw-r--r--   0 runner    (1001) docker     (121)     6181 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/mem/memptrs.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3937 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/mem/memptrs.h
--rw-r--r--   0 runner    (1001) docker     (121)     2533 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/mem/pakinfo.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/mem/pakinfo_internal.h
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/mem/rtc.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1998 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/mem/rtc.h
--rw-r--r--   0 runner    (1001) docker     (121)    29297 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/memory.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5244 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/memory.h
--rw-r--r--   0 runner    (1001) docker     (121)     4848 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/minkeeper.h
--rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/osd_element.h
--rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/savestate.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.156344 gambaterm-0.9.8/libgambatte/src/sound/
--rw-r--r--   0 runner    (1001) docker     (121)     6375 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/channel1.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/channel1.h
--rw-r--r--   0 runner    (1001) docker     (121)     4044 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/channel2.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/channel2.h
--rw-r--r--   0 runner    (1001) docker     (121)     5786 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/channel3.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2790 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/channel3.h
--rw-r--r--   0 runner    (1001) docker     (121)     6575 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/channel4.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3055 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/channel4.h
--rw-r--r--   0 runner    (1001) docker     (121)     4039 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/duty_unit.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/duty_unit.h
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/envelope_unit.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/envelope_unit.h
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/length_counter.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/length_counter.h
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/master_disabler.h
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/psgdef.h
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/sound_unit.h
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound/static_output_tester.h
--rw-r--r--   0 runner    (1001) docker     (121)     6336 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3361 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/sound.h
--rw-r--r--   0 runner    (1001) docker     (121)     5342 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/state_osd_elements.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/state_osd_elements.h
--rw-r--r--   0 runner    (1001) docker     (121)    18844 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/statesaver.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/statesaver.h
--rw-r--r--   0 runner    (1001) docker     (121)     5024 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/tima.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/tima.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.156344 gambaterm-0.9.8/libgambatte/src/video/
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/lcddef.h
--rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/ly_counter.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/ly_counter.h
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/lyc_irq.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/lyc_irq.h
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/mstat_irq.h
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/next_m0_time.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/next_m0_time.h
--rw-r--r--   0 runner    (1001) docker     (121)    61800 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/ppu.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/ppu.h
--rw-r--r--   0 runner    (1001) docker     (121)     5399 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/sprite_mapper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video/sprite_mapper.h
--rw-r--r--   0 runner    (1001) docker     (121)    28343 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8887 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte/src/video.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.156344 gambaterm-0.9.8/libgambatte_ext/
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-08-21 15:45:42.000000 gambaterm-0.9.8/libgambatte_ext/libgambatte.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-08-21 15:45:42.000000 gambaterm-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-21 15:45:48.156344 gambaterm-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2718 2022-08-21 15:45:42.000000 gambaterm-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 15:45:48.156344 gambaterm-0.9.8/termblit_ext/
--rw-r--r--   0 runner    (1001) docker     (121)     6492 2022-08-21 15:45:42.000000 gambaterm-0.9.8/termblit_ext/termblit.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.689976 gambaterm-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-08-21 20:23:34.000000 gambaterm-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-08-21 20:23:34.000000 gambaterm-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    10867 2022-08-21 20:23:54.689976 gambaterm-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10103 2022-08-21 20:23:34.000000 gambaterm-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.669975 gambaterm-0.9.9/gambaterm/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2627 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/audio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/colors.py
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/controller_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/file_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7700 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/keyboard_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5375 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5861 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9264 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3515 2022-08-21 20:23:34.000000 gambaterm-0.9.9/gambaterm/ssh_app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.669975 gambaterm-0.9.9/gambaterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10867 2022-08-21 20:23:54.000000 gambaterm-0.9.9/gambaterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3283 2022-08-21 20:23:54.000000 gambaterm-0.9.9/gambaterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-21 20:23:54.000000 gambaterm-0.9.9/gambaterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-08-21 20:23:54.000000 gambaterm-0.9.9/gambaterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-08-21 20:23:54.000000 gambaterm-0.9.9/gambaterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-21 20:23:54.000000 gambaterm-0.9.9/gambaterm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.669975 gambaterm-0.9.9/libgambatte/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.669975 gambaterm-0.9.9/libgambatte/common/
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/common/array.h
+-rw-r--r--   0 runner    (1001) docker     (121)      370 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/common/defined_ptr.h
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/common/scoped_ptr.h
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/common/transfer_ptr.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/common/uncopyable.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.673976 gambaterm-0.9.9/libgambatte/include/
+-rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/include/gambatte.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/include/gbint.h
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1193 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/include/inputgetter.h
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/include/loadres.h
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/include/pakinfo.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.677976 gambaterm-0.9.9/libgambatte/src/
+-rw-r--r--   0 runner    (1001) docker     (121)    11368 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/bitmap_font.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/bitmap_font.h
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/counterdef.h
+-rw-r--r--   0 runner    (1001) docker     (121)    45665 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/cpu.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.677976 gambaterm-0.9.9/libgambatte/src/file/
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/file/file.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/file/file.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5028 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/file/file_zip.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/file/stdfile.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.677976 gambaterm-0.9.9/libgambatte/src/file/unzip/
+-rw-r--r--   0 runner    (1001) docker     (121)     4712 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/file/unzip/crypt.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/file/unzip/ioapi.h
+-rw-r--r--   0 runner    (1001) docker     (121)    13009 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/file/unzip/unzip.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/gambatte.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    82449 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/initstate.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/initstate.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/insertion_sort.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2838 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/interrupter.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/interrupter.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3557 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/interruptrequester.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3611 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/interruptrequester.h
+-rw-r--r--   0 runner    (1001) docker     (121)      965 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/loadres.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.681976 gambaterm-0.9.9/libgambatte/src/mem/
+-rw-r--r--   0 runner    (1001) docker     (121)    19458 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/mem/cartridge.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3553 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/mem/cartridge.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6181 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/mem/memptrs.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3937 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/mem/memptrs.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2533 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/mem/pakinfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/mem/pakinfo_internal.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/mem/rtc.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1998 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/mem/rtc.h
+-rw-r--r--   0 runner    (1001) docker     (121)    29297 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/memory.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     5244 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/memory.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4848 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/minkeeper.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/osd_element.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/savestate.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.685976 gambaterm-0.9.9/libgambatte/src/sound/
+-rw-r--r--   0 runner    (1001) docker     (121)     6375 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/channel1.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2637 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/channel1.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4044 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/channel2.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/channel2.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5786 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/channel3.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2790 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/channel3.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6575 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/channel4.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3055 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/channel4.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4039 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/duty_unit.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/duty_unit.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/envelope_unit.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/envelope_unit.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/length_counter.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/length_counter.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/master_disabler.h
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/psgdef.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/sound_unit.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound/static_output_tester.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6336 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3361 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/sound.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5342 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/state_osd_elements.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/state_osd_elements.h
+-rw-r--r--   0 runner    (1001) docker     (121)    18844 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/statesaver.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/statesaver.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5024 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/tima.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/tima.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.685976 gambaterm-0.9.9/libgambatte/src/video/
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/lcddef.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1947 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/ly_counter.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/ly_counter.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/lyc_irq.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/lyc_irq.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/mstat_irq.h
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/next_m0_time.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/next_m0_time.h
+-rw-r--r--   0 runner    (1001) docker     (121)    61800 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/ppu.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/ppu.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5399 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/sprite_mapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4237 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video/sprite_mapper.h
+-rw-r--r--   0 runner    (1001) docker     (121)    28343 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8887 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte/src/video.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.689976 gambaterm-0.9.9/libgambatte_ext/
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-08-21 20:23:34.000000 gambaterm-0.9.9/libgambatte_ext/libgambatte.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-08-21 20:23:34.000000 gambaterm-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-21 20:23:54.689976 gambaterm-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-08-21 20:23:34.000000 gambaterm-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-21 20:23:54.689976 gambaterm-0.9.9/termblit_ext/
+-rw-r--r--   0 runner    (1001) docker     (121)     6492 2022-08-21 20:23:34.000000 gambaterm-0.9.9/termblit_ext/termblit.pyx
```

### Comparing `gambaterm-0.9.8/LICENSE` & `gambaterm-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/PKG-INFO` & `gambaterm-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gambaterm
-Version: 0.9.8
+Version: 0.9.9
 Summary: A terminal frontend for gambatte game boy color emulator 
 Home-page: https://github.com/vxgmichel/gambatte-terminal
 Author: Vincent Michel
 Author-email: vxgmichel@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: controller-support
 License-File: LICENSE
 
 gambatte-terminal
 -----------------
 
 [![](https://github.com/vxgmichel/gambatte-terminal/actions/workflows/build.yml/badge.svg)](https://github.com/vxgmichel/gambatte-terminal/actions/workflows/build.yml)
 [![](https://img.shields.io/pypi/v/gambaterm.svg)](https://pypi.python.org/pypi/gambaterm)
```

### Comparing `gambaterm-0.9.8/README.md` & `gambaterm-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/gambaterm/audio.py` & `gambaterm-0.9.9/gambaterm/audio.py`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/gambaterm/colors.py` & `gambaterm-0.9.9/gambaterm/colors.py`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/gambaterm/controller_input.py` & `gambaterm-0.9.9/gambaterm/controller_input.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,15 +27,25 @@
         "B6": GBInput.SELECT,
     }
 
 
 @contextmanager
 def pygame_button_pressed_context(deadzone=0.4):
     os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
-    import pygame
+
+    try:
+        import pygame
+    except ImportError:
+        raise SystemExit(
+            """\
+The pygame library is not available, which is required to get controller support.
+Please use the following command to install gambaterm with controller support:
+  pip3 install gambaterm[controller-support]
+"""
+        )
 
     pygame.init()
     pygame.joystick.init()
     joystick = None
 
     def get_pressed():
         nonlocal joystick
```

### Comparing `gambaterm-0.9.8/gambaterm/file_input.py` & `gambaterm-0.9.9/gambaterm/file_input.py`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/gambaterm/keyboard_input.py` & `gambaterm-0.9.9/gambaterm/keyboard_input.py`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/gambaterm/main.py` & `gambaterm-0.9.9/gambaterm/main.py`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/gambaterm/run.py` & `gambaterm-0.9.9/gambaterm/run.py`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/gambaterm/ssh.py` & `gambaterm-0.9.9/gambaterm/ssh.py`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/gambaterm/ssh_app_session.py` & `gambaterm-0.9.9/gambaterm/ssh_app_session.py`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/gambaterm.egg-info/PKG-INFO` & `gambaterm-0.9.9/gambaterm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gambaterm
-Version: 0.9.8
+Version: 0.9.9
 Summary: A terminal frontend for gambatte game boy color emulator 
 Home-page: https://github.com/vxgmichel/gambatte-terminal
 Author: Vincent Michel
 Author-email: vxgmichel@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: controller-support
 License-File: LICENSE
 
 gambatte-terminal
 -----------------
 
 [![](https://github.com/vxgmichel/gambatte-terminal/actions/workflows/build.yml/badge.svg)](https://github.com/vxgmichel/gambatte-terminal/actions/workflows/build.yml)
 [![](https://img.shields.io/pypi/v/gambaterm.svg)](https://pypi.python.org/pypi/gambaterm)
```

### Comparing `gambaterm-0.9.8/gambaterm.egg-info/SOURCES.txt` & `gambaterm-0.9.9/gambaterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/common/array.h` & `gambaterm-0.9.9/libgambatte/common/array.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/common/scoped_ptr.h` & `gambaterm-0.9.9/libgambatte/common/scoped_ptr.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/common/transfer_ptr.h` & `gambaterm-0.9.9/libgambatte/common/transfer_ptr.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/common/uncopyable.h` & `gambaterm-0.9.9/libgambatte/common/uncopyable.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/include/gambatte.h` & `gambaterm-0.9.9/libgambatte/include/gambatte.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/include/gbint.h` & `gambaterm-0.9.9/libgambatte/include/gbint.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/include/inputgetter.h` & `gambaterm-0.9.9/libgambatte/include/inputgetter.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/include/loadres.h` & `gambaterm-0.9.9/libgambatte/include/loadres.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/bitmap_font.cpp` & `gambaterm-0.9.9/libgambatte/src/bitmap_font.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/bitmap_font.h` & `gambaterm-0.9.9/libgambatte/src/bitmap_font.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/cpu.cpp` & `gambaterm-0.9.9/libgambatte/src/cpu.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/cpu.h` & `gambaterm-0.9.9/libgambatte/src/cpu.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/file/file.cpp` & `gambaterm-0.9.9/libgambatte/src/file/file.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/file/file.h` & `gambaterm-0.9.9/libgambatte/src/file/file.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/file/file_zip.cpp` & `gambaterm-0.9.9/libgambatte/src/file/file_zip.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/file/stdfile.h` & `gambaterm-0.9.9/libgambatte/src/file/stdfile.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/file/unzip/crypt.h` & `gambaterm-0.9.9/libgambatte/src/file/unzip/crypt.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/file/unzip/ioapi.h` & `gambaterm-0.9.9/libgambatte/src/file/unzip/ioapi.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/file/unzip/unzip.h` & `gambaterm-0.9.9/libgambatte/src/file/unzip/unzip.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/gambatte.cpp` & `gambaterm-0.9.9/libgambatte/src/gambatte.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/initstate.cpp` & `gambaterm-0.9.9/libgambatte/src/initstate.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/initstate.h` & `gambaterm-0.9.9/libgambatte/src/initstate.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/insertion_sort.h` & `gambaterm-0.9.9/libgambatte/src/insertion_sort.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/interrupter.cpp` & `gambaterm-0.9.9/libgambatte/src/interrupter.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/interrupter.h` & `gambaterm-0.9.9/libgambatte/src/interrupter.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/interruptrequester.cpp` & `gambaterm-0.9.9/libgambatte/src/interruptrequester.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/interruptrequester.h` & `gambaterm-0.9.9/libgambatte/src/interruptrequester.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/loadres.cpp` & `gambaterm-0.9.9/libgambatte/src/loadres.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/mem/cartridge.cpp` & `gambaterm-0.9.9/libgambatte/src/mem/cartridge.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/mem/cartridge.h` & `gambaterm-0.9.9/libgambatte/src/mem/cartridge.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/mem/memptrs.cpp` & `gambaterm-0.9.9/libgambatte/src/mem/memptrs.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/mem/memptrs.h` & `gambaterm-0.9.9/libgambatte/src/mem/memptrs.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/mem/pakinfo.cpp` & `gambaterm-0.9.9/libgambatte/src/mem/pakinfo.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/mem/rtc.cpp` & `gambaterm-0.9.9/libgambatte/src/mem/rtc.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/mem/rtc.h` & `gambaterm-0.9.9/libgambatte/src/mem/rtc.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/memory.cpp` & `gambaterm-0.9.9/libgambatte/src/memory.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/memory.h` & `gambaterm-0.9.9/libgambatte/src/memory.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/minkeeper.h` & `gambaterm-0.9.9/libgambatte/src/minkeeper.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/osd_element.h` & `gambaterm-0.9.9/libgambatte/src/osd_element.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/savestate.h` & `gambaterm-0.9.9/libgambatte/src/savestate.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/channel1.cpp` & `gambaterm-0.9.9/libgambatte/src/sound/channel1.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/channel1.h` & `gambaterm-0.9.9/libgambatte/src/sound/channel1.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/channel2.cpp` & `gambaterm-0.9.9/libgambatte/src/sound/channel2.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/channel2.h` & `gambaterm-0.9.9/libgambatte/src/sound/channel2.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/channel3.cpp` & `gambaterm-0.9.9/libgambatte/src/sound/channel3.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/channel3.h` & `gambaterm-0.9.9/libgambatte/src/sound/channel3.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/channel4.cpp` & `gambaterm-0.9.9/libgambatte/src/sound/channel4.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/channel4.h` & `gambaterm-0.9.9/libgambatte/src/sound/channel4.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/duty_unit.cpp` & `gambaterm-0.9.9/libgambatte/src/sound/duty_unit.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/duty_unit.h` & `gambaterm-0.9.9/libgambatte/src/sound/duty_unit.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/envelope_unit.cpp` & `gambaterm-0.9.9/libgambatte/src/sound/envelope_unit.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/envelope_unit.h` & `gambaterm-0.9.9/libgambatte/src/sound/envelope_unit.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/length_counter.cpp` & `gambaterm-0.9.9/libgambatte/src/sound/length_counter.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/length_counter.h` & `gambaterm-0.9.9/libgambatte/src/sound/length_counter.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/master_disabler.h` & `gambaterm-0.9.9/libgambatte/src/sound/master_disabler.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/sound_unit.h` & `gambaterm-0.9.9/libgambatte/src/sound/sound_unit.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound/static_output_tester.h` & `gambaterm-0.9.9/libgambatte/src/sound/static_output_tester.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound.cpp` & `gambaterm-0.9.9/libgambatte/src/sound.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/sound.h` & `gambaterm-0.9.9/libgambatte/src/sound.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/state_osd_elements.cpp` & `gambaterm-0.9.9/libgambatte/src/state_osd_elements.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/state_osd_elements.h` & `gambaterm-0.9.9/libgambatte/src/state_osd_elements.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/statesaver.cpp` & `gambaterm-0.9.9/libgambatte/src/statesaver.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/statesaver.h` & `gambaterm-0.9.9/libgambatte/src/statesaver.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/tima.cpp` & `gambaterm-0.9.9/libgambatte/src/tima.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/tima.h` & `gambaterm-0.9.9/libgambatte/src/tima.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video/lcddef.h` & `gambaterm-0.9.9/libgambatte/src/video/lcddef.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video/ly_counter.cpp` & `gambaterm-0.9.9/libgambatte/src/video/ly_counter.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video/ly_counter.h` & `gambaterm-0.9.9/libgambatte/src/video/ly_counter.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video/lyc_irq.cpp` & `gambaterm-0.9.9/libgambatte/src/video/lyc_irq.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video/lyc_irq.h` & `gambaterm-0.9.9/libgambatte/src/video/lyc_irq.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video/mstat_irq.h` & `gambaterm-0.9.9/libgambatte/src/video/mstat_irq.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video/ppu.cpp` & `gambaterm-0.9.9/libgambatte/src/video/ppu.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video/ppu.h` & `gambaterm-0.9.9/libgambatte/src/video/ppu.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video/sprite_mapper.cpp` & `gambaterm-0.9.9/libgambatte/src/video/sprite_mapper.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video/sprite_mapper.h` & `gambaterm-0.9.9/libgambatte/src/video/sprite_mapper.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video.cpp` & `gambaterm-0.9.9/libgambatte/src/video.cpp`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte/src/video.h` & `gambaterm-0.9.9/libgambatte/src/video.h`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/libgambatte_ext/libgambatte.pyx` & `gambaterm-0.9.9/libgambatte_ext/libgambatte.pyx`

 * *Files identical despite different names*

### Comparing `gambaterm-0.9.8/setup.py` & `gambaterm-0.9.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,28 +49,30 @@
     language="c",
     include_dirs=[NumpyIncludePath()],
     sources=["termblit_ext/termblit.pyx"],
 )
 
 setup(
     name="gambaterm",
-    version="0.9.8",
+    version="0.9.9",
     packages=["gambaterm"],
     setup_requires=["setuptools>=42", "Cython>=0.29.13", "numpy"],
     ext_modules=[gambatte_extension, termblit_extension],
     install_requires=[
         "numpy>=1",
         "asyncssh>=2",
         "prompt_toolkit>=3",
         "sounddevice",
         "samplerate",
         "python-xlib; sys_platform == 'linux'",
         "pynput; sys_platform != 'linux'",
-        "pygame>=1.9.5",
     ],
+    extras_require={
+        "controller-support": ["pygame>=1.9.5"],
+    },
     python_requires=">=3.6",
     entry_points={
         "console_scripts": [
             "gambaterm = gambaterm:main",
             "gambaterm-ssh = gambaterm.ssh:main",
         ],
     },
```

### Comparing `gambaterm-0.9.8/termblit_ext/termblit.pyx` & `gambaterm-0.9.9/termblit_ext/termblit.pyx`

 * *Files identical despite different names*

