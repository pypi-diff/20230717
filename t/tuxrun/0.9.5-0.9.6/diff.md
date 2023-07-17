# Comparing `tmp/tuxrun-0.9.5.tar.gz` & `tmp/tuxrun-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuxrun-0.9.5.tar", last modified: Thu Sep 23 11:42:13 2021, max compression
+gzip compressed data, was "tuxrun-0.9.6.tar", last modified: Thu Sep 23 16:03:40 2021, max compression
```

## Comparing `tuxrun-0.9.5.tar` & `tuxrun-0.9.6.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0       30 2021-09-23 11:42:11.235631 tuxrun-0.9.5/.flake8
--rw-r--r--   0        0        0       59 2021-09-23 11:42:11.236631 tuxrun-0.9.5/.gitignore
--rw-r--r--   0        0        0     2663 2021-09-23 11:42:11.236631 tuxrun-0.9.5/.gitlab-ci.yml
--rw-r--r--   0        0        0      414 2021-09-23 11:42:11.236631 tuxrun-0.9.5/Dockerfile.ci
--rw-r--r--   0        0        0      138 2021-09-23 11:42:11.236631 tuxrun-0.9.5/Dockerfile.ci-integration
--rw-r--r--   0        0        0     1054 2021-09-23 11:42:11.236631 tuxrun-0.9.5/LICENSE
--rw-r--r--   0        0        0      757 2021-09-23 11:42:11.236631 tuxrun-0.9.5/Makefile
--rw-r--r--   0        0        0     2523 2021-09-23 11:42:11.236631 tuxrun-0.9.5/README.md
--rw-r--r--   0        0        0     1729 2021-09-23 11:42:11.236631 tuxrun-0.9.5/docs/devices.md
--rw-r--r--   0        0        0      412 2021-09-23 11:42:11.236631 tuxrun-0.9.5/docs/install-pypi.md
--rw-r--r--   0        0        0     3664 2021-09-23 11:42:11.236631 tuxrun-0.9.5/docs/run-fvp.md
--rw-r--r--   0        0        0     1965 2021-09-23 11:42:11.237631 tuxrun-0.9.5/docs/run-qemu.md
--rw-r--r--   0        0        0      553 2021-09-23 11:42:11.237631 tuxrun-0.9.5/docs/run-uninstalled.md
--rw-r--r--   0        0        0      162 2021-09-23 11:42:11.237631 tuxrun-0.9.5/docs/style.css
--rw-r--r--   0        0        0     1829 2021-09-23 11:42:11.237631 tuxrun-0.9.5/docs/tests.md
--rw-r--r--   0        0        0     2001 2021-09-23 11:42:11.237631 tuxrun-0.9.5/docs/tuxrun.svg
--rw-r--r--   0        0        0     3060 2021-09-23 11:42:11.237631 tuxrun-0.9.5/docs/tuxrun_full.svg
--rw-r--r--   0        0        0     4404 2021-09-23 11:42:11.238631 tuxrun-0.9.5/docs/tuxrun_icon.svg
--rw-r--r--   0        0        0      791 2021-09-23 11:42:11.238631 tuxrun-0.9.5/mkdocs.yml
--rw-r--r--   0        0        0      459 2021-09-23 11:42:11.238631 tuxrun-0.9.5/pyproject.toml
--rwxr-xr-x   0        0        0      122 2021-09-23 11:42:11.238631 tuxrun-0.9.5/run
--rwxr-xr-x   0        0        0      166 2021-09-23 11:42:11.238631 tuxrun-0.9.5/scripts/readme2index.sh
--rwxr-xr-x   0        0        0     1665 2021-09-23 11:42:11.238631 tuxrun-0.9.5/scripts/release
--rw-r--r--   0        0        0      718 2021-09-23 11:42:11.238631 tuxrun-0.9.5/share/fvp/Dockerfile
--rw-r--r--   0        0        0      213 2021-09-23 11:42:11.238631 tuxrun-0.9.5/share/fvp/Makefile
--rwxr-xr-x   0        0        0       70 2021-09-23 11:42:11.239632 tuxrun-0.9.5/share/fvp/docker
--rw-r--r--   0        0        0      854 2021-09-23 11:42:11.239632 tuxrun-0.9.5/share/fvp/morello/Dockerfile
--rw-r--r--   0        0        0      383 2021-09-23 11:42:11.239632 tuxrun-0.9.5/test/conftest.py
--rwxr-xr-x   0        0        0     4074 2021-09-23 11:42:11.239632 tuxrun-0.9.5/test/integration.py
--rw-r--r--   0        0        0     2799 2021-09-23 11:42:11.239632 tuxrun-0.9.5/test/unit/test_assets.py
--rw-r--r--   0        0        0     9574 2021-09-23 11:42:11.239632 tuxrun-0.9.5/test/unit/test_main.py
--rw-r--r--   0        0        0     5025 2021-09-23 11:42:11.239632 tuxrun-0.9.5/test/unit/test_runtime.py
--rw-r--r--   0        0        0     2596 2021-09-23 11:42:11.239632 tuxrun-0.9.5/test/unit/test_tuxmake.py
--rw-r--r--   0        0        0     1305 2021-09-23 11:42:11.240631 tuxrun-0.9.5/test/unit/test_writer.py
--rw-r--r--   0        0        0      326 2021-09-23 11:42:11.240631 tuxrun-0.9.5/test/unit/test_xdg.py
--rw-r--r--   0        0        0      193 2021-09-23 11:42:11.240631 tuxrun-0.9.5/tuxrun/__init__.py
--rw-r--r--   0        0        0    17840 2021-09-23 11:42:11.240631 tuxrun-0.9.5/tuxrun/__main__.py
--rw-r--r--   0        0        0     4364 2021-09-23 11:42:11.240631 tuxrun-0.9.5/tuxrun/assets.py
--rw-r--r--   0        0        0      965 2021-09-23 11:42:11.240631 tuxrun-0.9.5/tuxrun/requests.py
--rw-r--r--   0        0        0     4852 2021-09-23 11:42:11.240631 tuxrun-0.9.5/tuxrun/runtimes.py
--rw-r--r--   0        0        0     1862 2021-09-23 11:42:11.240631 tuxrun-0.9.5/tuxrun/templates/__init__.py
--rw-r--r--   0        0        0    14336 2021-09-23 11:42:11.241632 tuxrun-0.9.5/tuxrun/templates/devices/base.yaml.jinja2
--rw-r--r--   0        0        0     1052 2021-09-23 11:42:11.241632 tuxrun-0.9.5/tuxrun/templates/devices/fvp.yaml.jinja2
--rw-r--r--   0        0        0     6914 2021-09-23 11:42:11.241632 tuxrun-0.9.5/tuxrun/templates/devices/qemu.yaml.jinja2
--rw-r--r--   0        0        0     1071 2021-09-23 11:42:11.241632 tuxrun-0.9.5/tuxrun/templates/dispatchers/dispatcher.yaml.jinja2
--rw-r--r--   0        0        0     2980 2021-09-23 11:42:11.241632 tuxrun-0.9.5/tuxrun/templates/jobs/base-fvp.yaml.jinja2
--rw-r--r--   0        0        0     1706 2021-09-23 11:42:11.241632 tuxrun-0.9.5/tuxrun/templates/jobs/base-qemu.yaml.jinja2
--rw-r--r--   0        0        0      104 2021-09-23 11:42:11.241632 tuxrun-0.9.5/tuxrun/templates/jobs/fvp-morello-android.yaml.jinja2
--rw-r--r--   0        0        0       99 2021-09-23 11:42:11.241632 tuxrun-0.9.5/tuxrun/templates/jobs/fvp-morello-busybox.yaml.jinja2
--rw-r--r--   0        0        0      114 2021-09-23 11:42:11.241632 tuxrun-0.9.5/tuxrun/templates/jobs/fvp-morello-oe.yaml.jinja2
--rw-r--r--   0        0        0      444 2021-09-23 11:42:11.242632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-arm64.yaml.jinja2
--rw-r--r--   0        0        0      461 2021-09-23 11:42:11.242632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-armv5.yaml.jinja2
--rw-r--r--   0        0        0      514 2021-09-23 11:42:11.242632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-armv7.yaml.jinja2
--rw-r--r--   0        0        0      348 2021-09-23 11:42:11.242632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-i386.yaml.jinja2
--rw-r--r--   0        0        0      330 2021-09-23 11:42:11.242632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-mips32.yaml.jinja2
--rw-r--r--   0        0        0      335 2021-09-23 11:42:11.242632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-mips32el.yaml.jinja2
--rw-r--r--   0        0        0      307 2021-09-23 11:42:11.242632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-mips64.yaml.jinja2
--rw-r--r--   0        0        0      311 2021-09-23 11:42:11.242632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-mips64el.yaml.jinja2
--rw-r--r--   0        0        0      351 2021-09-23 11:42:11.242632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-ppc32.yaml.jinja2
--rw-r--r--   0        0        0      395 2021-09-23 11:42:11.243632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-ppc64.yaml.jinja2
--rw-r--r--   0        0        0      399 2021-09-23 11:42:11.243632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-ppc64le.yaml.jinja2
--rw-r--r--   0        0        0      473 2021-09-23 11:42:11.243632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-riscv64.yaml.jinja2
--rw-r--r--   0        0        0      309 2021-09-23 11:42:11.243632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-sparc64.yaml.jinja2
--rw-r--r--   0        0        0      352 2021-09-23 11:42:11.243632 tuxrun-0.9.5/tuxrun/templates/jobs/qemu-x86_64.yaml.jinja2
--rw-r--r--   0        0        0      530 2021-09-23 11:42:11.243632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/base-ltp.yaml.jinja2
--rw-r--r--   0        0        0      486 2021-09-23 11:42:11.243632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/binder.yaml.jinja2
--rw-r--r--   0        0        0      703 2021-09-23 11:42:11.243632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/bionic.yaml.jinja2
--rw-r--r--   0        0        0      407 2021-09-23 11:42:11.243632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/command.yaml.jinja2
--rw-r--r--   0        0        0      501 2021-09-23 11:42:11.243632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/compartment.yaml.jinja2
--rw-r--r--   0        0        0      428 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/device-tree.yaml.jinja2
--rw-r--r--   0        0        0      414 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/dvfs.yaml.jinja2
--rw-r--r--   0        0        0      347 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/fwts.yaml.jinja2
--rw-r--r--   0        0        0      333 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/kunit.yaml.jinja2
--rw-r--r--   0        0        0      527 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/lldb.yaml.jinja2
--rw-r--r--   0        0        0      483 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/logd.yaml.jinja2
--rw-r--r--   0        0        0      100 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/ltp-fcntl-locktests.yaml.jinja2
--rw-r--r--   0        0        0       93 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/ltp-fs_bind.yaml.jinja2
--rw-r--r--   0        0        0      100 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/ltp-fs_perms_simple.yaml.jinja2
--rw-r--r--   0        0        0       88 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/ltp-fsx.yaml.jinja2
--rw-r--r--   0        0        0       90 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/ltp-nptl.yaml.jinja2
--rw-r--r--   0        0        0      122 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/ltp-smoke.yaml.jinja2
--rw-r--r--   0        0        0      429 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/templates/jobs/tests/multicore.yaml.jinja2
--rw-r--r--   0        0        0     1383 2021-09-23 11:42:11.244632 tuxrun-0.9.5/tuxrun/tuxmake.py
--rw-r--r--   0        0        0      892 2021-09-23 11:42:11.245632 tuxrun-0.9.5/tuxrun/utils.py
--rw-r--r--   0        0        0     1809 2021-09-23 11:42:11.245632 tuxrun-0.9.5/tuxrun/writer.py
--rw-r--r--   0        0        0      390 2021-09-23 11:42:11.245632 tuxrun-0.9.5/tuxrun/xdg.py
--rw-r--r--   0        0        0      470 2021-09-23 11:42:11.245632 tuxrun-0.9.5/tuxrun/yaml.py
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 tuxrun-0.9.5/setup.py
--rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 tuxrun-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0       30 2021-09-23 16:03:38.247157 tuxrun-0.9.6/.flake8
+-rw-r--r--   0        0        0       59 2021-09-23 16:03:38.247157 tuxrun-0.9.6/.gitignore
+-rw-r--r--   0        0        0     2663 2021-09-23 16:03:38.247157 tuxrun-0.9.6/.gitlab-ci.yml
+-rw-r--r--   0        0        0      414 2021-09-23 16:03:38.247157 tuxrun-0.9.6/Dockerfile.ci
+-rw-r--r--   0        0        0      138 2021-09-23 16:03:38.248157 tuxrun-0.9.6/Dockerfile.ci-integration
+-rw-r--r--   0        0        0     1054 2021-09-23 16:03:38.248157 tuxrun-0.9.6/LICENSE
+-rw-r--r--   0        0        0      757 2021-09-23 16:03:38.248157 tuxrun-0.9.6/Makefile
+-rw-r--r--   0        0        0     2523 2021-09-23 16:03:38.248157 tuxrun-0.9.6/README.md
+-rw-r--r--   0        0        0     1729 2021-09-23 16:03:38.248157 tuxrun-0.9.6/docs/devices.md
+-rw-r--r--   0        0        0      412 2021-09-23 16:03:38.248157 tuxrun-0.9.6/docs/install-pypi.md
+-rw-r--r--   0        0        0     3664 2021-09-23 16:03:38.248157 tuxrun-0.9.6/docs/run-fvp.md
+-rw-r--r--   0        0        0     1965 2021-09-23 16:03:38.248157 tuxrun-0.9.6/docs/run-qemu.md
+-rw-r--r--   0        0        0      553 2021-09-23 16:03:38.248157 tuxrun-0.9.6/docs/run-uninstalled.md
+-rw-r--r--   0        0        0      162 2021-09-23 16:03:38.248157 tuxrun-0.9.6/docs/style.css
+-rw-r--r--   0        0        0     1829 2021-09-23 16:03:38.249157 tuxrun-0.9.6/docs/tests.md
+-rw-r--r--   0        0        0     2001 2021-09-23 16:03:38.249157 tuxrun-0.9.6/docs/tuxrun.svg
+-rw-r--r--   0        0        0     3060 2021-09-23 16:03:38.249157 tuxrun-0.9.6/docs/tuxrun_full.svg
+-rw-r--r--   0        0        0     4404 2021-09-23 16:03:38.249157 tuxrun-0.9.6/docs/tuxrun_icon.svg
+-rw-r--r--   0        0        0      791 2021-09-23 16:03:38.249157 tuxrun-0.9.6/mkdocs.yml
+-rw-r--r--   0        0        0      459 2021-09-23 16:03:38.249157 tuxrun-0.9.6/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2021-09-23 16:03:38.249157 tuxrun-0.9.6/run
+-rwxr-xr-x   0        0        0      166 2021-09-23 16:03:38.250157 tuxrun-0.9.6/scripts/readme2index.sh
+-rwxr-xr-x   0        0        0     1665 2021-09-23 16:03:38.250157 tuxrun-0.9.6/scripts/release
+-rw-r--r--   0        0        0      718 2021-09-23 16:03:38.250157 tuxrun-0.9.6/share/fvp/Dockerfile
+-rw-r--r--   0        0        0      213 2021-09-23 16:03:38.250157 tuxrun-0.9.6/share/fvp/Makefile
+-rwxr-xr-x   0        0        0       70 2021-09-23 16:03:38.250157 tuxrun-0.9.6/share/fvp/docker
+-rw-r--r--   0        0        0      854 2021-09-23 16:03:38.250157 tuxrun-0.9.6/share/fvp/morello/Dockerfile
+-rw-r--r--   0        0        0      383 2021-09-23 16:03:38.250157 tuxrun-0.9.6/test/conftest.py
+-rwxr-xr-x   0        0        0     4074 2021-09-23 16:03:38.250157 tuxrun-0.9.6/test/integration.py
+-rw-r--r--   0        0        0     2799 2021-09-23 16:03:38.250157 tuxrun-0.9.6/test/unit/test_assets.py
+-rw-r--r--   0        0        0     9574 2021-09-23 16:03:38.251157 tuxrun-0.9.6/test/unit/test_main.py
+-rw-r--r--   0        0        0     5025 2021-09-23 16:03:38.251157 tuxrun-0.9.6/test/unit/test_runtime.py
+-rw-r--r--   0        0        0     2596 2021-09-23 16:03:38.251157 tuxrun-0.9.6/test/unit/test_tuxmake.py
+-rw-r--r--   0        0        0     1305 2021-09-23 16:03:38.251157 tuxrun-0.9.6/test/unit/test_writer.py
+-rw-r--r--   0        0        0      326 2021-09-23 16:03:38.251157 tuxrun-0.9.6/test/unit/test_xdg.py
+-rw-r--r--   0        0        0      193 2021-09-23 16:03:38.251157 tuxrun-0.9.6/tuxrun/__init__.py
+-rw-r--r--   0        0        0    17840 2021-09-23 16:03:38.251157 tuxrun-0.9.6/tuxrun/__main__.py
+-rw-r--r--   0        0        0     4364 2021-09-23 16:03:38.252157 tuxrun-0.9.6/tuxrun/assets.py
+-rw-r--r--   0        0        0      965 2021-09-23 16:03:38.252157 tuxrun-0.9.6/tuxrun/requests.py
+-rw-r--r--   0        0        0     4852 2021-09-23 16:03:38.252157 tuxrun-0.9.6/tuxrun/runtimes.py
+-rw-r--r--   0        0        0     1862 2021-09-23 16:03:38.252157 tuxrun-0.9.6/tuxrun/templates/__init__.py
+-rw-r--r--   0        0        0    14336 2021-09-23 16:03:38.252157 tuxrun-0.9.6/tuxrun/templates/devices/base.yaml.jinja2
+-rw-r--r--   0        0        0     1052 2021-09-23 16:03:38.252157 tuxrun-0.9.6/tuxrun/templates/devices/fvp.yaml.jinja2
+-rw-r--r--   0        0        0     6914 2021-09-23 16:03:38.252157 tuxrun-0.9.6/tuxrun/templates/devices/qemu.yaml.jinja2
+-rw-r--r--   0        0        0     1071 2021-09-23 16:03:38.253157 tuxrun-0.9.6/tuxrun/templates/dispatchers/dispatcher.yaml.jinja2
+-rw-r--r--   0        0        0     2978 2021-09-23 16:03:38.253157 tuxrun-0.9.6/tuxrun/templates/jobs/base-fvp.yaml.jinja2
+-rw-r--r--   0        0        0     1706 2021-09-23 16:03:38.253157 tuxrun-0.9.6/tuxrun/templates/jobs/base-qemu.yaml.jinja2
+-rw-r--r--   0        0        0      104 2021-09-23 16:03:38.253157 tuxrun-0.9.6/tuxrun/templates/jobs/fvp-morello-android.yaml.jinja2
+-rw-r--r--   0        0        0       99 2021-09-23 16:03:38.253157 tuxrun-0.9.6/tuxrun/templates/jobs/fvp-morello-busybox.yaml.jinja2
+-rw-r--r--   0        0        0      114 2021-09-23 16:03:38.253157 tuxrun-0.9.6/tuxrun/templates/jobs/fvp-morello-oe.yaml.jinja2
+-rw-r--r--   0        0        0      444 2021-09-23 16:03:38.253157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-arm64.yaml.jinja2
+-rw-r--r--   0        0        0      461 2021-09-23 16:03:38.253157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-armv5.yaml.jinja2
+-rw-r--r--   0        0        0      514 2021-09-23 16:03:38.253157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-armv7.yaml.jinja2
+-rw-r--r--   0        0        0      348 2021-09-23 16:03:38.254157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-i386.yaml.jinja2
+-rw-r--r--   0        0        0      330 2021-09-23 16:03:38.254157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-mips32.yaml.jinja2
+-rw-r--r--   0        0        0      335 2021-09-23 16:03:38.254157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-mips32el.yaml.jinja2
+-rw-r--r--   0        0        0      307 2021-09-23 16:03:38.254157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-mips64.yaml.jinja2
+-rw-r--r--   0        0        0      311 2021-09-23 16:03:38.254157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-mips64el.yaml.jinja2
+-rw-r--r--   0        0        0      351 2021-09-23 16:03:38.254157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-ppc32.yaml.jinja2
+-rw-r--r--   0        0        0      395 2021-09-23 16:03:38.254157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-ppc64.yaml.jinja2
+-rw-r--r--   0        0        0      399 2021-09-23 16:03:38.254157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-ppc64le.yaml.jinja2
+-rw-r--r--   0        0        0      473 2021-09-23 16:03:38.254157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-riscv64.yaml.jinja2
+-rw-r--r--   0        0        0      309 2021-09-23 16:03:38.254157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-sparc64.yaml.jinja2
+-rw-r--r--   0        0        0      352 2021-09-23 16:03:38.255157 tuxrun-0.9.6/tuxrun/templates/jobs/qemu-x86_64.yaml.jinja2
+-rw-r--r--   0        0        0      530 2021-09-23 16:03:38.255157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/base-ltp.yaml.jinja2
+-rw-r--r--   0        0        0      486 2021-09-23 16:03:38.255157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/binder.yaml.jinja2
+-rw-r--r--   0        0        0      703 2021-09-23 16:03:38.255157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/bionic.yaml.jinja2
+-rw-r--r--   0        0        0      407 2021-09-23 16:03:38.255157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/command.yaml.jinja2
+-rw-r--r--   0        0        0      501 2021-09-23 16:03:38.255157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/compartment.yaml.jinja2
+-rw-r--r--   0        0        0      428 2021-09-23 16:03:38.255157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/device-tree.yaml.jinja2
+-rw-r--r--   0        0        0      414 2021-09-23 16:03:38.255157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/dvfs.yaml.jinja2
+-rw-r--r--   0        0        0      347 2021-09-23 16:03:38.255157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/fwts.yaml.jinja2
+-rw-r--r--   0        0        0      334 2021-09-23 16:03:38.255157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/kunit.yaml.jinja2
+-rw-r--r--   0        0        0      527 2021-09-23 16:03:38.255157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/lldb.yaml.jinja2
+-rw-r--r--   0        0        0      483 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/logd.yaml.jinja2
+-rw-r--r--   0        0        0      100 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/ltp-fcntl-locktests.yaml.jinja2
+-rw-r--r--   0        0        0       93 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/ltp-fs_bind.yaml.jinja2
+-rw-r--r--   0        0        0      100 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/ltp-fs_perms_simple.yaml.jinja2
+-rw-r--r--   0        0        0       88 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/ltp-fsx.yaml.jinja2
+-rw-r--r--   0        0        0       90 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/ltp-nptl.yaml.jinja2
+-rw-r--r--   0        0        0      122 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/ltp-smoke.yaml.jinja2
+-rw-r--r--   0        0        0      429 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/templates/jobs/tests/multicore.yaml.jinja2
+-rw-r--r--   0        0        0     1383 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/tuxmake.py
+-rw-r--r--   0        0        0      892 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/utils.py
+-rw-r--r--   0        0        0     1809 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/writer.py
+-rw-r--r--   0        0        0      390 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/xdg.py
+-rw-r--r--   0        0        0      470 2021-09-23 16:03:38.256157 tuxrun-0.9.6/tuxrun/yaml.py
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 tuxrun-0.9.6/setup.py
+-rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 tuxrun-0.9.6/PKG-INFO
```

### Comparing `tuxrun-0.9.5/.gitlab-ci.yml` & `tuxrun-0.9.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/LICENSE` & `tuxrun-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/Makefile` & `tuxrun-0.9.6/Makefile`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/README.md` & `tuxrun-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/docs/devices.md` & `tuxrun-0.9.6/docs/devices.md`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/docs/run-fvp.md` & `tuxrun-0.9.6/docs/run-fvp.md`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/docs/run-qemu.md` & `tuxrun-0.9.6/docs/run-qemu.md`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/docs/run-uninstalled.md` & `tuxrun-0.9.6/docs/run-uninstalled.md`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/docs/tests.md` & `tuxrun-0.9.6/docs/tests.md`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/docs/tuxrun.svg` & `tuxrun-0.9.6/docs/tuxrun.svg`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/docs/tuxrun_full.svg` & `tuxrun-0.9.6/docs/tuxrun_full.svg`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/docs/tuxrun_icon.svg` & `tuxrun-0.9.6/docs/tuxrun_icon.svg`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/mkdocs.yml` & `tuxrun-0.9.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/scripts/release` & `tuxrun-0.9.6/scripts/release`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/share/fvp/Dockerfile` & `tuxrun-0.9.6/share/fvp/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/share/fvp/morello/Dockerfile` & `tuxrun-0.9.6/share/fvp/morello/Dockerfile`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/test/integration.py` & `tuxrun-0.9.6/test/integration.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/test/unit/test_assets.py` & `tuxrun-0.9.6/test/unit/test_assets.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/test/unit/test_main.py` & `tuxrun-0.9.6/test/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/test/unit/test_runtime.py` & `tuxrun-0.9.6/test/unit/test_runtime.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/test/unit/test_tuxmake.py` & `tuxrun-0.9.6/test/unit/test_tuxmake.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/test/unit/test_writer.py` & `tuxrun-0.9.6/test/unit/test_writer.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/__main__.py` & `tuxrun-0.9.6/tuxrun/__main__.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/assets.py` & `tuxrun-0.9.6/tuxrun/assets.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/requests.py` & `tuxrun-0.9.6/tuxrun/requests.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/runtimes.py` & `tuxrun-0.9.6/tuxrun/runtimes.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/templates/__init__.py` & `tuxrun-0.9.6/tuxrun/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/templates/devices/base.yaml.jinja2` & `tuxrun-0.9.6/tuxrun/templates/devices/base.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/templates/devices/fvp.yaml.jinja2` & `tuxrun-0.9.6/tuxrun/templates/devices/fvp.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/templates/devices/qemu.yaml.jinja2` & `tuxrun-0.9.6/tuxrun/templates/devices/qemu.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/templates/dispatchers/dispatcher.yaml.jinja2` & `tuxrun-0.9.6/tuxrun/templates/dispatchers/dispatcher.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/templates/jobs/base-fvp.yaml.jinja2` & `tuxrun-0.9.6/tuxrun/templates/jobs/base-fvp.yaml.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 job_name: "tuxrun@{{ device }}"
 priority: medium
 visibility: public
 
 {% block context %}{% endblock %}
 
-{%- set ns = namespace(timeout=10+20) %}
+{%- set ns = namespace(timeout=5+20) %}
 {%- for test in tests %}
   {%- set ns.timeout = ns.timeout + timeouts[test] %}
 {%- endfor %}
 
 timeouts:
   job:
     minutes: {{ ns.timeout }}
@@ -19,15 +19,15 @@
   connection:
     minutes: 10
 
 actions:
 - deploy:
     to: fvp
     timeout:
-      minutes: 10
+      minutes: 5
     images:
       scp_romfw:
         url: "{{ scp_romfw }}"
       scp_fw:
         url: "{{ scp_fw }}"
       mcp_romfw:
         url: "{{ mcp_romfw }}"
```

### Comparing `tuxrun-0.9.5/tuxrun/templates/jobs/base-qemu.yaml.jinja2` & `tuxrun-0.9.6/tuxrun/templates/jobs/base-qemu.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/templates/jobs/qemu-armv7.yaml.jinja2` & `tuxrun-0.9.6/tuxrun/templates/jobs/qemu-armv7.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/templates/jobs/tests/base-ltp.yaml.jinja2` & `tuxrun-0.9.6/tuxrun/templates/jobs/tests/base-ltp.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/templates/jobs/tests/bionic.yaml.jinja2` & `tuxrun-0.9.6/tuxrun/templates/jobs/tests/bionic.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/templates/jobs/tests/lldb.yaml.jinja2` & `tuxrun-0.9.6/tuxrun/templates/jobs/tests/lldb.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/tuxmake.py` & `tuxrun-0.9.6/tuxrun/tuxmake.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/utils.py` & `tuxrun-0.9.6/tuxrun/utils.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/tuxrun/writer.py` & `tuxrun-0.9.6/tuxrun/writer.py`

 * *Files identical despite different names*

### Comparing `tuxrun-0.9.5/setup.py` & `tuxrun-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = \
 ['jinja2', 'requests', 'PyYAML']
 
 entry_points = \
 {'console_scripts': ['tuxrun = tuxrun.__main__:main']}
 
 setup(name='tuxrun',
-      version='0.9.5',
+      version='0.9.6',
       description='Command line tool for testing Linux under QEMU',
       author='Antonio Terceiro',
       author_email='antonio.terceiro@linaro.org',
       url='https://tuxsuite.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

