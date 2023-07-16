# Comparing `tmp/zcmds_win32-1.2.0.tar.gz` & `tmp/zcmds_win32-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcmds_win32-1.2.0.tar", last modified: Sun Jul 16 22:54:31 2023, max compression
+gzip compressed data, was "zcmds_win32-1.2.1.tar", last modified: Sun Jul 16 23:04:47 2023, max compression
```

## Comparing `zcmds_win32-1.2.0.tar` & `zcmds_win32-1.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.969883 zcmds_win32-1.2.0/
-drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.894231 zcmds_win32-1.2.0/.github/
-drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.910215 zcmds_win32-1.2.0/.github/workflows/
--rw-rw-rw-   0        0        0      880 2023-03-24 01:40:21.000000 zcmds_win32-1.2.0/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      858 2023-03-24 01:34:49.000000 zcmds_win32-1.2.0/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     1844 2023-07-16 22:43:59.000000 zcmds_win32-1.2.0/.gitignore
-drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.911179 zcmds_win32-1.2.0/.vscode/
--rw-rw-rw-   0        0        0      833 2023-03-06 04:33:48.000000 zcmds_win32-1.2.0/.vscode/settings.json
--rw-rw-rw-   0        0        0     2541 2023-07-16 22:54:31.968885 zcmds_win32-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2099 2023-07-16 22:53:12.000000 zcmds_win32-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.915179 zcmds_win32-1.2.0/assets/
--rw-rw-rw-   0        0        0  1932219 2023-07-16 22:10:40.000000 zcmds_win32-1.2.0/assets/dig-for-windows-9.9.5-W1.zip
--rw-rw-rw-   0        0        0  3280133 2023-05-08 19:20:06.000000 zcmds_win32-1.2.0/assets/git-bash-bin.zip
--rw-rw-rw-   0        0        0      350 2023-07-16 22:44:44.000000 zcmds_win32-1.2.0/lint.sh
--rw-rw-rw-   0        0        0     1620 2023-07-16 22:52:10.000000 zcmds_win32-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       28 2022-02-21 03:22:36.000000 zcmds_win32-1.2.0/requirements.testing.txt
--rw-rw-rw-   0        0        0        0 2022-10-15 20:56:38.000000 zcmds_win32-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 22:54:31.969883 zcmds_win32-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      163 2023-03-24 00:34:00.000000 zcmds_win32-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.922180 zcmds_win32-1.2.0/tests/
--rw-rw-rw-   0        0        0      369 2023-07-16 22:48:29.000000 zcmds_win32-1.2.0/tests/test_dig.py
--rw-rw-rw-   0        0        0      478 2023-03-24 02:08:04.000000 zcmds_win32-1.2.0/tests/test_git_bin_install.py
--rw-rw-rw-   0        0        0      485 2023-03-24 02:22:33.000000 zcmds_win32-1.2.0/tests/test_main.py
--rw-rw-rw-   0        0        0      544 2023-03-24 02:24:34.000000 zcmds_win32-1.2.0/tox.ini
--rw-rw-rw-   0        0        0      275 2023-07-03 05:37:10.000000 zcmds_win32-1.2.0/upload_package.sh
-drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.929776 zcmds_win32-1.2.0/zcmds_win32/
--rw-rw-rw-   0        0        0        0 2022-02-21 10:38:44.000000 zcmds_win32-1.2.0/zcmds_win32/__init__.py
--rw-rw-rw-   0        0        0      343 2023-02-22 21:00:08.000000 zcmds_win32-1.2.0/zcmds_win32/_exec.py
-drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.967940 zcmds_win32-1.2.0/zcmds_win32/cmds/
--rw-rw-rw-   0        0        0      131 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/cat.py
--rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/cp.py
--rw-rw-rw-   0        0        0      620 2023-07-16 22:45:51.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/dig.py
--rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/du.py
--rw-rw-rw-   0        0        0      282 2023-03-24 00:47:30.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/fixvmmem.py
--rw-rw-rw-   0        0        0      322 2022-08-06 19:05:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/git_bash.py
--rw-rw-rw-   0        0        0      132 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/grep.py
--rw-rw-rw-   0        0        0      168 2022-10-15 22:21:22.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/home.py
--rw-rw-rw-   0        0        0      170 2023-03-24 01:49:26.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/id.py
--rw-rw-rw-   0        0        0      170 2023-03-24 00:49:32.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/ls.py
--rw-rw-rw-   0        0        0      174 2023-03-24 01:55:14.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/md5sum.py
--rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/mv.py
--rw-rw-rw-   0        0        0      132 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/nano.py
--rw-rw-rw-   0        0        0     2521 2023-07-13 20:05:10.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/open.py
--rw-rw-rw-   0        0        0      132 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/pico.py
--rw-rw-rw-   0        0        0      170 2023-03-24 01:49:36.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/ps.py
--rw-rw-rw-   0        0        0      171 2023-03-24 01:58:49.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/pwd.py
--rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/rm.py
--rw-rw-rw-   0        0        0      131 2023-07-03 08:49:13.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/sed.py
--rw-rw-rw-   0        0        0      171 2023-03-24 01:52:42.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/tee.py
--rw-rw-rw-   0        0        0      142 2023-03-24 00:42:29.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/touch.py
--rw-rw-rw-   0        0        0      132 2023-05-08 19:20:55.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/uname.py
--rw-rw-rw-   0        0        0      132 2023-05-08 19:20:40.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/uniq.py
--rw-rw-rw-   0        0        0      133 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/unzip.py
--rw-rw-rw-   0        0        0      170 2023-03-24 01:53:28.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/wc.py
--rw-rw-rw-   0        0        0       99 2022-10-15 22:21:22.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/which.py
--rw-rw-rw-   0        0        0      173 2023-03-24 01:49:52.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/xargs.py
--rw-rw-rw-   0        0        0      131 2023-03-24 00:45:58.000000 zcmds_win32-1.2.0/zcmds_win32/cmds/yes.py
--rw-rw-rw-   0        0        0     1582 2023-07-16 22:45:26.000000 zcmds_win32-1.2.0/zcmds_win32/install_tool.py
--rw-rw-rw-   0        0        0       96 2023-03-24 02:08:51.000000 zcmds_win32-1.2.0/zcmds_win32/settings.py
--rw-rw-rw-   0        0        0     1501 2023-07-16 22:45:09.000000 zcmds_win32-1.2.0/zcmds_win32/unix_tool_path.py
--rw-rw-rw-   0        0        0      111 2023-07-16 22:52:05.000000 zcmds_win32-1.2.0/zcmds_win32/version.py
-drwxrwxrwx   0        0        0        0 2023-07-16 22:54:31.939863 zcmds_win32-1.2.0/zcmds_win32.egg-info/
--rw-rw-rw-   0        0        0     2541 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1382 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      886 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-16 22:54:31.000000 zcmds_win32-1.2.0/zcmds_win32.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 23:04:47.199479 zcmds_win32-1.2.1/
+drwxrwxrwx   0        0        0        0 2023-07-16 23:04:47.089104 zcmds_win32-1.2.1/.github/
+drwxrwxrwx   0        0        0        0 2023-07-16 23:04:47.105939 zcmds_win32-1.2.1/.github/workflows/
+-rw-rw-rw-   0        0        0      880 2023-03-24 01:40:21.000000 zcmds_win32-1.2.1/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      858 2023-03-24 01:34:49.000000 zcmds_win32-1.2.1/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     1844 2023-07-16 23:01:43.000000 zcmds_win32-1.2.1/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-16 23:04:47.106937 zcmds_win32-1.2.1/.vscode/
+-rw-rw-rw-   0        0        0      833 2023-03-06 04:33:48.000000 zcmds_win32-1.2.1/.vscode/settings.json
+-rw-rw-rw-   0        0        0     2532 2023-07-16 23:04:47.198478 zcmds_win32-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2091 2023-07-16 23:02:30.000000 zcmds_win32-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 23:04:47.111938 zcmds_win32-1.2.1/assets/
+-rw-rw-rw-   0        0        0  1932219 2023-07-16 22:10:40.000000 zcmds_win32-1.2.1/assets/dig-for-windows-9.9.5-W1.zip
+-rw-rw-rw-   0        0        0  3280133 2023-05-08 19:20:06.000000 zcmds_win32-1.2.1/assets/git-bash-bin.zip
+-rw-rw-rw-   0        0        0      350 2023-07-16 23:01:43.000000 zcmds_win32-1.2.1/lint.sh
+-rw-rw-rw-   0        0        0     1620 2023-07-16 23:02:23.000000 zcmds_win32-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       28 2022-02-21 03:22:36.000000 zcmds_win32-1.2.1/requirements.testing.txt
+-rw-rw-rw-   0        0        0        0 2022-10-15 20:56:38.000000 zcmds_win32-1.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 23:04:47.199479 zcmds_win32-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      163 2023-03-24 00:34:00.000000 zcmds_win32-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:04:47.120056 zcmds_win32-1.2.1/tests/
+-rw-rw-rw-   0        0        0      369 2023-07-16 23:01:43.000000 zcmds_win32-1.2.1/tests/test_dig.py
+-rw-rw-rw-   0        0        0      478 2023-03-24 02:08:04.000000 zcmds_win32-1.2.1/tests/test_git_bin_install.py
+-rw-rw-rw-   0        0        0      485 2023-03-24 02:22:33.000000 zcmds_win32-1.2.1/tests/test_main.py
+-rw-rw-rw-   0        0        0      544 2023-03-24 02:24:34.000000 zcmds_win32-1.2.1/tox.ini
+-rw-rw-rw-   0        0        0      275 2023-07-03 05:37:10.000000 zcmds_win32-1.2.1/upload_package.sh
+drwxrwxrwx   0        0        0        0 2023-07-16 23:04:47.130982 zcmds_win32-1.2.1/zcmds_win32/
+-rw-rw-rw-   0        0        0        0 2022-02-21 10:38:44.000000 zcmds_win32-1.2.1/zcmds_win32/__init__.py
+-rw-rw-rw-   0        0        0      343 2023-02-22 21:00:08.000000 zcmds_win32-1.2.1/zcmds_win32/_exec.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:04:47.197574 zcmds_win32-1.2.1/zcmds_win32/cmds/
+-rw-rw-rw-   0        0        0      131 2023-03-24 00:45:58.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/cat.py
+-rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/cp.py
+-rw-rw-rw-   0        0        0      620 2023-07-16 23:01:43.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/dig.py
+-rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/du.py
+-rw-rw-rw-   0        0        0      282 2023-03-24 00:47:30.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/fixvmmem.py
+-rw-rw-rw-   0        0        0      322 2022-08-06 19:05:58.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/git_bash.py
+-rw-rw-rw-   0        0        0      132 2023-03-24 00:45:58.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/grep.py
+-rw-rw-rw-   0        0        0      168 2022-10-15 22:21:22.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/home.py
+-rw-rw-rw-   0        0        0      170 2023-03-24 01:49:26.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/id.py
+-rw-rw-rw-   0        0        0      170 2023-03-24 00:49:32.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/ls.py
+-rw-rw-rw-   0        0        0      174 2023-03-24 01:55:14.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/md5sum.py
+-rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/mv.py
+-rw-rw-rw-   0        0        0      132 2023-03-24 00:45:58.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/nano.py
+-rw-rw-rw-   0        0        0     2521 2023-07-13 20:05:10.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/open.py
+-rw-rw-rw-   0        0        0      132 2023-03-24 00:45:58.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/pico.py
+-rw-rw-rw-   0        0        0      170 2023-03-24 01:49:36.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/ps.py
+-rw-rw-rw-   0        0        0      171 2023-03-24 01:58:49.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/pwd.py
+-rw-rw-rw-   0        0        0      130 2023-03-24 00:45:58.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/rm.py
+-rw-rw-rw-   0        0        0      131 2023-07-03 08:49:13.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/sed.py
+-rw-rw-rw-   0        0        0      171 2023-03-24 01:52:42.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/tee.py
+-rw-rw-rw-   0        0        0      142 2023-03-24 00:42:29.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/touch.py
+-rw-rw-rw-   0        0        0      132 2023-05-08 19:20:55.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/uname.py
+-rw-rw-rw-   0        0        0      132 2023-05-08 19:20:40.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/uniq.py
+-rw-rw-rw-   0        0        0      133 2023-03-24 00:45:58.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/unzip.py
+-rw-rw-rw-   0        0        0      170 2023-03-24 01:53:28.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/wc.py
+-rw-rw-rw-   0        0        0       99 2022-10-15 22:21:22.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/which.py
+-rw-rw-rw-   0        0        0      173 2023-03-24 01:49:52.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/xargs.py
+-rw-rw-rw-   0        0        0      131 2023-03-24 00:45:58.000000 zcmds_win32-1.2.1/zcmds_win32/cmds/yes.py
+-rw-rw-rw-   0        0        0     1582 2023-07-16 23:01:43.000000 zcmds_win32-1.2.1/zcmds_win32/install_tool.py
+-rw-rw-rw-   0        0        0       96 2023-03-24 02:08:51.000000 zcmds_win32-1.2.1/zcmds_win32/settings.py
+-rw-rw-rw-   0        0        0     2114 2023-07-16 23:01:45.000000 zcmds_win32-1.2.1/zcmds_win32/unix_tool_path.py
+-rw-rw-rw-   0        0        0      107 2023-07-16 23:02:26.000000 zcmds_win32-1.2.1/zcmds_win32/version.py
+drwxrwxrwx   0        0        0        0 2023-07-16 23:04:47.159868 zcmds_win32-1.2.1/zcmds_win32.egg-info/
+-rw-rw-rw-   0        0        0     2532 2023-07-16 23:04:46.000000 zcmds_win32-1.2.1/zcmds_win32.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1382 2023-07-16 23:04:47.000000 zcmds_win32-1.2.1/zcmds_win32.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 23:04:46.000000 zcmds_win32-1.2.1/zcmds_win32.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      886 2023-07-16 23:04:46.000000 zcmds_win32-1.2.1/zcmds_win32.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-07-16 23:04:46.000000 zcmds_win32-1.2.1/zcmds_win32.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 23:04:46.000000 zcmds_win32-1.2.1/zcmds_win32.egg-info/top_level.txt
```

### Comparing `zcmds_win32-1.2.0/.github/workflows/lint.yml` & `zcmds_win32-1.2.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.2.0/.github/workflows/push_win.yml` & `zcmds_win32-1.2.1/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.2.0/.gitignore` & `zcmds_win32-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.2.0/.vscode/settings.json` & `zcmds_win32-1.2.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.2.0/PKG-INFO` & `zcmds_win32-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcmds_win32
-Version: 1.2.0
+Version: 1.2.1
 Summary: Cross platform(ish) productivity commands written in python.
 License: BSD 3-Clause License
 Keywords: zcmds,win32,zcmds_win32,zcmds-win32,cli,command line,command line interface
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -16,15 +16,14 @@
 Optional zcmds package for win32 to make it feel more like a linux distribution. This is a great package to use if you want to
 use things like `tee`, `grep` and unix commands and have it work on windows.
 
 # Commands
 
   * cat
   * cp
-  * dig
   * du
   * git-bash
   * grep
   * home
   * false
   * id
   * ls
@@ -59,15 +58,15 @@
   * `git clone https://github.com/zackees/zcmds_win32`
   * `cd zcmds_win32`
   * `python -pip install -e .`
 
 
 # Release Notes
 
-  * 1.2.0: Adds tool `dig`
+  * 1.2.1: Adds tool `dig`
   * 1.0.26: When sublime is opened via `open` it now opens in it's own window.
   * 1.0.25: Fix `open` for python 3.9
   * 1.0.24: Add `sed`
   * 1.0.23: Yank 1.0.21/22
   * 1.0.20: Adds `uniq` and `uname`
   * 1.0.19: Change default text editor to sublime over textpad
   * 1.0.18: Adds `true` and `false` and `timeout`
```

### Comparing `zcmds_win32-1.2.0/README.md` & `zcmds_win32-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 Optional zcmds package for win32 to make it feel more like a linux distribution. This is a great package to use if you want to
 use things like `tee`, `grep` and unix commands and have it work on windows.
 
 # Commands
 
   * cat
   * cp
-  * dig
   * du
   * git-bash
   * grep
   * home
   * false
   * id
   * ls
@@ -49,15 +48,15 @@
   * `git clone https://github.com/zackees/zcmds_win32`
   * `cd zcmds_win32`
   * `python -pip install -e .`
 
 
 # Release Notes
 
-  * 1.2.0: Adds tool `dig`
+  * 1.2.1: Adds tool `dig`
   * 1.0.26: When sublime is opened via `open` it now opens in it's own window.
   * 1.0.25: Fix `open` for python 3.9
   * 1.0.24: Add `sed`
   * 1.0.23: Yank 1.0.21/22
   * 1.0.20: Adds `uniq` and `uname`
   * 1.0.19: Change default text editor to sublime over textpad
   * 1.0.18: Adds `true` and `false` and `timeout`
```

### Comparing `zcmds_win32-1.2.0/assets/dig-for-windows-9.9.5-W1.zip` & `zcmds_win32-1.2.1/assets/dig-for-windows-9.9.5-W1.zip`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.2.0/assets/git-bash-bin.zip` & `zcmds_win32-1.2.1/assets/git-bash-bin.zip`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.2.0/pyproject.toml` & `zcmds_win32-1.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "sudo_win32[sudo]",
     "download",
 ]
 # Change this with the version number bump.
-version = "1.2.0"
+version = "1.2.1"
 
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = "missing-module-docstring,missing-function-docstring"
 
 [project.scripts]
 cat = "zcmds_win32.cmds.cat:main"
```

### Comparing `zcmds_win32-1.2.0/tox.ini` & `zcmds_win32-1.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.2.0/zcmds_win32/cmds/dig.py` & `zcmds_win32-1.2.1/zcmds_win32/cmds/dig.py`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.2.0/zcmds_win32/cmds/open.py` & `zcmds_win32-1.2.1/zcmds_win32/cmds/open.py`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.2.0/zcmds_win32/install_tool.py` & `zcmds_win32-1.2.1/zcmds_win32/install_tool.py`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.2.0/zcmds_win32/unix_tool_path.py` & `zcmds_win32-1.2.1/zcmds_win32/unix_tool_path.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 """
 Resolves the unix tool, either by finding it in PATH or by downloading it.
 """
 
 import os
 import shutil
+from tempfile import TemporaryDirectory
 from typing import Optional
 
+from download import download  # type: ignore
+
 from zcmds_win32._exec import os_exec
-from zcmds_win32.install_tool import install as install_tool
 
 GIT_BIN = r"C:\Program Files\Git\usr\bin"
 GIT_BIN_TOOL_URL = (
     "https://github.com/zackees/zcmds_win32/raw/main/assets/git-bash-bin.zip"
 )
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 DOWNLOADED_GIT_BIN = os.path.join(HERE, "git-bash-bin")
 
 
 def install() -> None:
     """Installs the Unix tools."""
-    install_tool(GIT_BIN_TOOL_URL, DOWNLOADED_GIT_BIN)
+    with TemporaryDirectory() as tmpdir:
+        download(GIT_BIN_TOOL_URL, tmpdir, replace=True, kind="zip")
+        dst = os.path.join(HERE, "git-bash-bin")
+        os.makedirs(dst, exist_ok=True)
+        files = os.listdir(os.path.join(tmpdir, "git-bash-bin"))
+        # Sort dll's so that they are first
+        files.sort(key=lambda x: not x.endswith(".dll"))
+        files = [os.path.join(tmpdir, "git-bash-bin", f) for f in files]
+        for src in files:
+            filename = os.path.basename(src)
+            try:
+                shutil.move(src, os.path.join(dst, filename))
+            except shutil.Error:
+                pass
 
 
 def get_or_fetch_unix_tool_path(name: str) -> Optional[str]:
     """Attempts to find the given Unix tool."""
     path = shutil.which(name)
     if path and os.path.basename(os.path.dirname(path)).lower() != "scripts":
         return path
```

### Comparing `zcmds_win32-1.2.0/zcmds_win32.egg-info/PKG-INFO` & `zcmds_win32-1.2.1/zcmds_win32.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcmds-win32
-Version: 1.2.0
+Version: 1.2.1
 Summary: Cross platform(ish) productivity commands written in python.
 License: BSD 3-Clause License
 Keywords: zcmds,win32,zcmds_win32,zcmds-win32,cli,command line,command line interface
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -16,15 +16,14 @@
 Optional zcmds package for win32 to make it feel more like a linux distribution. This is a great package to use if you want to
 use things like `tee`, `grep` and unix commands and have it work on windows.
 
 # Commands
 
   * cat
   * cp
-  * dig
   * du
   * git-bash
   * grep
   * home
   * false
   * id
   * ls
@@ -59,15 +58,15 @@
   * `git clone https://github.com/zackees/zcmds_win32`
   * `cd zcmds_win32`
   * `python -pip install -e .`
 
 
 # Release Notes
 
-  * 1.2.0: Adds tool `dig`
+  * 1.2.1: Adds tool `dig`
   * 1.0.26: When sublime is opened via `open` it now opens in it's own window.
   * 1.0.25: Fix `open` for python 3.9
   * 1.0.24: Add `sed`
   * 1.0.23: Yank 1.0.21/22
   * 1.0.20: Adds `uniq` and `uname`
   * 1.0.19: Change default text editor to sublime over textpad
   * 1.0.18: Adds `true` and `false` and `timeout`
```

### Comparing `zcmds_win32-1.2.0/zcmds_win32.egg-info/SOURCES.txt` & `zcmds_win32-1.2.1/zcmds_win32.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.2.0/zcmds_win32.egg-info/entry_points.txt` & `zcmds_win32-1.2.1/zcmds_win32.egg-info/entry_points.txt`

 * *Files identical despite different names*

