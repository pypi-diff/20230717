# Comparing `tmp/zcmds_win32-1.0.9.tar.gz` & `tmp/zcmds_win32-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcmds_win32-1.0.9.tar", last modified: Mon Mar 13 07:48:06 2023, max compression
+gzip compressed data, was "zcmds_win32-1.2.0.tar", last modified: Sun Jul 16 22:54:31 2023, max compression
```

## Comparing `zcmds_win32-1.0.9.tar` & `zcmds_win32-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 07:48:06.673760 zcmds_win32-1.0.9/
--rw-rw-rw-   0        0        0     1799 2022-10-15 22:06:33.000000 zcmds_win32-1.0.9/.gitignore
-drwxrwxrwx   0        0        0        0 2023-03-13 07:48:06.635761 zcmds_win32-1.0.9/.vscode/
--rw-rw-rw-   0        0        0      833 2023-03-06 04:33:48.000000 zcmds_win32-1.0.9/.vscode/settings.json
--rw-rw-rw-   0        0        0     1311 2023-03-13 07:48:06.673760 zcmds_win32-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      901 2023-03-13 07:47:32.000000 zcmds_win32-1.0.9/README.md
--rw-rw-rw-   0        0        0     1058 2023-03-13 07:47:18.000000 zcmds_win32-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       28 2022-02-21 03:22:36.000000 zcmds_win32-1.0.9/requirements.testing.txt
--rw-rw-rw-   0        0        0        0 2022-10-15 20:56:38.000000 zcmds_win32-1.0.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-13 07:48:06.674762 zcmds_win32-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0       77 2023-01-03 07:29:58.000000 zcmds_win32-1.0.9/setup.py
--rw-rw-rw-   0        0        0      465 2022-11-28 03:18:18.000000 zcmds_win32-1.0.9/tox.ini
--rw-rw-rw-   0        0        0      249 2023-03-06 08:05:13.000000 zcmds_win32-1.0.9/upload_package.sh
-drwxrwxrwx   0        0        0        0 2023-03-13 07:48:06.658762 zcmds_win32-1.0.9/zcmds_win32/
--rw-rw-rw-   0        0        0        0 2022-02-21 10:38:44.000000 zcmds_win32-1.0.9/zcmds_win32/__init__.py
--rw-rw-rw-   0        0        0      343 2023-02-22 21:00:08.000000 zcmds_win32-1.0.9/zcmds_win32/_exec.py
--rw-rw-rw-   0        0        0      130 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/cat.py
--rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/cp.py
--rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/du.py
--rw-rw-rw-   0        0        0      292 2023-03-06 08:05:13.000000 zcmds_win32-1.0.9/zcmds_win32/fixvmmem.py
--rw-rw-rw-   0        0        0      322 2022-08-06 19:05:58.000000 zcmds_win32-1.0.9/zcmds_win32/git_bash.py
--rw-rw-rw-   0        0        0      131 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/grep.py
--rw-rw-rw-   0        0        0      168 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/home.py
--rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/ls.py
--rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/mv.py
--rw-rw-rw-   0        0        0      131 2023-01-03 07:29:12.000000 zcmds_win32-1.0.9/zcmds_win32/nano.py
--rw-rw-rw-   0        0        0      349 2023-03-13 07:47:07.000000 zcmds_win32-1.0.9/zcmds_win32/open.py
--rw-rw-rw-   0        0        0      131 2023-01-03 07:29:03.000000 zcmds_win32-1.0.9/zcmds_win32/pico.py
--rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/rm.py
--rw-rw-rw-   0        0        0      142 2022-08-09 06:13:38.000000 zcmds_win32-1.0.9/zcmds_win32/touch.py
--rw-rw-rw-   0        0        0      132 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/unzip.py
--rw-rw-rw-   0        0        0      112 2022-10-15 21:20:31.000000 zcmds_win32-1.0.9/zcmds_win32/version.py
--rw-rw-rw-   0        0        0       99 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/which.py
-drwxrwxrwx   0        0        0        0 2023-03-13 07:48:06.672761 zcmds_win32-1.0.9/zcmds_win32.egg-info/
--rw-rw-rw-   0        0        0     1311 2023-03-13 07:48:06.000000 zcmds_win32-1.0.9/zcmds_win32.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      700 2023-03-13 07:48:06.000000 zcmds_win32-1.0.9/zcmds_win32.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 07:48:06.000000 zcmds_win32-1.0.9/zcmds_win32.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      482 2023-03-13 07:48:06.000000 zcmds_win32-1.0.9/zcmds_win32.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2023-03-13 07:48:06.000000 zcmds_win32-1.0.9/zcmds_win32.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.969883 zcmds_win32-1.2.0/
+drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.894231 zcmds_win32-1.2.0/.github/
+drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.910215 zcmds_win32-1.2.0/.github/workflows/
+-rw-rw-rw-   0        0        0      880 2023-03-24 01:40:21.000000 zcmds_win32-1.2.0/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      858 2023-03-24 01:34:49.000000 zcmds_win32-1.2.0/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     1844 2023-07-16 22:43:59.000000 zcmds_win32-1.2.0/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.911179 zcmds_win32-1.2.0/.vscode/
+-rw-rw-rw-   0        0        0      833 2023-03-06 04:33:48.000000 zcmds_win32-1.2.0/.vscode/settings.json
+-rw-rw-rw-   0        0        0     2541 2023-07-16 22:54:31.968885 zcmds_win32-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2099 2023-07-16 22:53:12.000000 zcmds_win32-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.915179 zcmds_win32-1.2.0/assets/
+-rw-rw-rw-   0        0        0  1932219 2023-07-16 22:10:40.000000 zcmds_win32-1.2.0/assets/dig-for-windows-9.9.5-W1.zip
+-rw-rw-rw-   0        0        0  3280133 2023-05-08 19:20:06.000000 zcmds_win32-1.2.0/assets/git-bash-bin.zip
+-rw-rw-rw-   0        0        0      350 2023-07-16 22:44:44.000000 zcmds_win32-1.2.0/lint.sh
+-rw-rw-rw-   0        0        0     1620 2023-07-16 22:52:10.000000 zcmds_win32-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       28 2022-02-21 03:22:36.000000 zcmds_win32-1.2.0/requirements.testing.txt
+-rw-rw-rw-   0        0        0        0 2022-10-15 20:56:38.000000 zcmds_win32-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 22:54:31.969883 zcmds_win32-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      163 2023-03-24 00:34:00.000000 zcmds_win32-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.922180 zcmds_win32-1.2.0/tests/
+-rw-rw-rw-   0        0        0      369 2023-07-16 22:48:29.000000 zcmds_win32-1.2.0/tests/test_dig.py
+-rw-rw-rw-   0        0        0      478 2023-03-24 02:08:04.000000 zcmds_win32-1.2.0/tests/test_git_bin_install.py
+-rw-rw-rw-   0        0        0      485 2023-03-24 02:22:33.000000 zcmds_win32-1.2.0/tests/test_main.py
+-rw-rw-rw-   0        0        0      544 2023-03-24 02:24:34.000000 zcmds_win32-1.2.0/tox.ini
+-rw-rw-rw-   0        0        0      275 2023-07-03 05:37:10.000000 zcmds_win32-1.2.0/upload_package.sh
+drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.929776 zcmds_win32-1.2.0/zcmds_win32/
+-rw-rw-rw-   0        0        0        0 2022-02-21 10:38:44.000000 zcmds_win32-1.2.0/zcmds_win32/__init__.py
+-rw-rw-rw-   0        0        0      343 2023-02-22 21:00:08.000000 zcmds_win32-1.2.0/zcmds_win32/_exec.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.967940 zcmds_win32-1.2.0/zcmds_win32/cmds/
+-rw-rw-rw-   0        0        0      131 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/cat.py
+-rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/cp.py
+-rw-rw-rw-   0        0        0      620 2023-07-16 22:45:51.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/dig.py
+-rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/du.py
+-rw-rw-rw-   0        0        0      282 2023-03-24 00:47:30.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/fixvmmem.py
+-rw-rw-rw-   0        0        0      322 2022-08-06 19:05:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/git_bash.py
+-rw-rw-rw-   0        0        0      132 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/grep.py
+-rw-rw-rw-   0        0        0      168 2022-10-15 22:21:22.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/home.py
+-rw-rw-rw-   0        0        0      170 2023-03-24 01:49:26.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/id.py
+-rw-rw-rw-   0        0        0      170 2023-03-24 00:49:32.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/ls.py
+-rw-rw-rw-   0        0        0      174 2023-03-24 01:55:14.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/md5sum.py
+-rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/mv.py
+-rw-rw-rw-   0        0        0      132 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/nano.py
+-rw-rw-rw-   0        0        0     2521 2023-07-13 20:05:10.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/open.py
+-rw-rw-rw-   0        0        0      132 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/pico.py
+-rw-rw-rw-   0        0        0      170 2023-03-24 01:49:36.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/ps.py
+-rw-rw-rw-   0        0        0      171 2023-03-24 01:58:49.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/pwd.py
+-rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/rm.py
+-rw-rw-rw-   0        0        0      131 2023-07-03 08:49:13.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/sed.py
+-rw-rw-rw-   0        0        0      171 2023-03-24 01:52:42.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/tee.py
+-rw-rw-rw-   0        0        0      142 2023-03-24 00:42:29.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/touch.py
+-rw-rw-rw-   0        0        0      132 2023-05-08 19:20:55.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/uname.py
+-rw-rw-rw-   0        0        0      132 2023-05-08 19:20:40.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/uniq.py
+-rw-rw-rw-   0        0        0      133 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/unzip.py
+-rw-rw-rw-   0        0        0      170 2023-03-24 01:53:28.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/wc.py
+-rw-rw-rw-   0        0        0       99 2022-10-15 22:21:22.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/which.py
+-rw-rw-rw-   0        0        0      173 2023-03-24 01:49:52.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/xargs.py
+-rw-rw-rw-   0        0        0      131 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/yes.py
+-rw-rw-rw-   0        0        0     1582 2023-07-16 22:45:26.000000 zcmds_win32-1.2.0/zcmds_win32/install_tool.py
+-rw-rw-rw-   0        0        0       96 2023-03-24 02:08:51.000000 zcmds_win32-1.2.0/zcmds_win32/settings.py
+-rw-rw-rw-   0        0        0     1501 2023-07-16 22:45:09.000000 zcmds_win32-1.2.0/zcmds_win32/unix_tool_path.py
+-rw-rw-rw-   0        0        0      111 2023-07-16 22:52:05.000000 zcmds_win32-1.2.0/zcmds_win32/version.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.939863 zcmds_win32-1.2.0/zcmds_win32.egg-info/
+-rw-rw-rw-   0        0        0     2541 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1382 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      886 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/top_level.txt
```

### Comparing `zcmds_win32-1.0.9/.gitignore` & `zcmds_win32-1.2.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -123,7 +123,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+zcmds_win32/git-bash-bin/
+zcmds_win32/tools/
```

### Comparing `zcmds_win32-1.0.9/.vscode/settings.json` & `zcmds_win32-1.2.0/.vscode/settings.json`

 * *Files identical despite different names*

