# Comparing `tmp/siriuspy-2.77.0.tar.gz` & `tmp/siriuspy-2.78.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siriuspy-2.77.0.tar", last modified: Tue Jun 27 19:16:13 2023, max compression
+gzip compressed data, was "siriuspy-2.78.0.tar", last modified: Mon Jul 17 20:43:58 2023, max compression
```

## Comparing `siriuspy-2.77.0.tar` & `siriuspy-2.78.0.tar`

### file list

```diff
@@ -1,396 +1,396 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-06-27 19:16:04.000000 siriuspy-2.77.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-27 19:16:04.000000 siriuspy-2.77.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-27 19:16:13.604366 siriuspy-2.77.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-06-27 19:16:04.000000 siriuspy-2.77.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-27 19:16:04.000000 siriuspy-2.77.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 19:16:13.604366 siriuspy-2.77.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-06-27 19:16:04.000000 siriuspy-2.77.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.572365 siriuspy-2.77.0/siriuspy/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.572365 siriuspy-2.77.0/siriuspy/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.572365 siriuspy-2.77.0/siriuspy/clientarch/
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/pvarch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.576365 siriuspy-2.77.0/siriuspy/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/configdb_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/configdb_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/pvsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.576365 siriuspy-2.77.0/siriuspy/clientconfigdb/types/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_pwrstate.py
--rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)   123230 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/global_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_bbadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_bbbproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_idff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.576365 siriuspy-2.77.0/siriuspy/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientweb/implementation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.576365 siriuspy-2.77.0/siriuspy/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/currinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/currinfo/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.576365 siriuspy-2.77.0/siriuspy/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/currinfo/lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/currinfo/lifetime/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/currinfo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.580366 siriuspy-2.77.0/siriuspy/cycle/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/bo_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/fc_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/li_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/bbb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/blctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    41475 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/bpm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/currinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/dcct.py
--rw-r--r--   0 runner    (1001) docker     (122)    13949 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)    16525 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/dvf.py
--rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/egun.py
--rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/energy.py
--rw-r--r--   0 runner    (1001) docker     (122)    51622 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/ict.py
--rw-r--r--   0 runner    (1001) docker     (122)    10043 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/idff.py
--rw-r--r--   0 runner    (1001) docker     (122)    21328 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/ids.py
--rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/injctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/injsys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/lienergy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/lillrf.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/machshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/modltr.py
--rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/orbit_interlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/posang.py
--rw-r--r--   0 runner    (1001) docker     (122)    10195 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/psconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/pstesters.py
--rw-r--r--   0 runner    (1001) docker     (122)    30064 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/pwrsupply.py
--rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/screen.py
--rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/sofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/syncd.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/timing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/tune.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/bpm/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/bpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/bpm/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/dcct/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/dcct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/dcct/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/ict/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/ict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/ict/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/screen/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/screen/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/slit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/slit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/slit/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagsys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagsys/lidiag/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/lidiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/lidiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/lidiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/lidiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagsys/psdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/psdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/psdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/psdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/psdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagsys/pudiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/pudiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/pudiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/pudiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/pudiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagsys/rfdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/rfdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/rfdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/rfdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/rfdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/dvfimgproc/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/dvfimgproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/dvfimgproc/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    15295 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/dvfimgproc/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7082 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/dvfimgproc/meas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/envars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/epics/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/pv.py
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/pv_fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/pv_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/fofb/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/fofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20125 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/fofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    79363 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/fofb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/idff/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/idff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7475 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/idff/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/idff/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    14114 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/idff/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/injctrl/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/injctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15253 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/injctrl/bias_feedback.py
--rw-r--r--   0 runner    (1001) docker     (122)    24738 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/injctrl/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    70365 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/injctrl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/machshift/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/gensumm_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)    78928 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/macschedule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/savedata_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/excdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/meas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/meas/liemit/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/liemit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/liemit/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/liemit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/meas/lienergy/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/lienergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/lienergy/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/lienergy/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/namesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/namesys/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/optics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/optics/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/optics/lattice_survey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/chrom.py
--rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/oscilloscope/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/oscilloscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/oscilloscope/keysight.py
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/oscilloscope/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/posang/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/posang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/posang/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/posang/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/posang/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/beaglebone.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10629 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.596366 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/pru.py
--rw-r--r--   0 runner    (1001) docker     (122)    25723 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/prucontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/prucparms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/psdevstate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/udc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.596366 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscreaders.py
--rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscwriters.py
--rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/psmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    34142 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/siggen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.596366 siriuspy-2.77.0/siriuspy/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/magnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/test_reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/testwfm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.596366 siriuspy-2.77.0/siriuspy/search/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/bpms_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/hl_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/id_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/ioc_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/ll_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/ma_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/ps_search.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.596366 siriuspy-2.77.0/siriuspy/simul/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/simfactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/simps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/simpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/siriuspy/sofb/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/bpms.py
--rw-r--r--   0 runner    (1001) docker     (122)    32010 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/correctors.py
--rw-r--r--   0 runner    (1001) docker     (122)    47062 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    46398 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    11841 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    36357 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/siriuspy/stabinfo/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/stabinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/stabinfo/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/stabinfo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8598 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/siriuspy/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/hl_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/ll_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/plot_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/static_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.572365 siriuspy-2.77.0/siriuspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10133 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/test_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/test_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/test_serial.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/clientconfigdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/clientconfigdb/test_configdb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/clientweb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/clientweb/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/currinfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/currinfo/lifetime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/currinfo/lifetime/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/currinfo/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/currinfo/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/magnet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/magnet/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/magnet/tests_normalizer.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/mock_servweb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/namesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/namesys/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/test_chrom.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/test_opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/test_tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/posang/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/posang/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/posang/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/posang/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/db.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/pructrl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/pructrl/test_pru.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/psctrl/test_pscwriters.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/test_beaglebone.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/test_siggen.py
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/ramp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/ramp/test_magnet.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/ramp/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/search/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/test_hl_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/test_init.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/test_ll_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/test_ma_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/test_ps_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/test_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/test_envars.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/timesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/timesys/test_csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/timesys/test_plot_network.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-07-17 20:43:48.000000 siriuspy-2.78.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-17 20:43:48.000000 siriuspy-2.78.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-17 20:43:58.525197 siriuspy-2.78.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-07-17 20:43:48.000000 siriuspy-2.78.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-17 20:43:48.000000 siriuspy-2.78.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 20:43:58.525197 siriuspy-2.78.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-07-17 20:43:48.000000 siriuspy-2.78.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.497197 siriuspy-2.78.0/siriuspy/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.497197 siriuspy-2.78.0/siriuspy/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/bsmp/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/clientarch/
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/pvarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientarch/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/configdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/configdb_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/pvsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/clientconfigdb/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57620 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_pwrstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)   123005 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/global_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_bbadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_bbbproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/clientweb/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/currinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/currinfo/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.501197 siriuspy-2.78.0/siriuspy/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/currinfo/lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/currinfo/lifetime/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/currinfo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.505197 siriuspy-2.78.0/siriuspy/cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/bo_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/fc_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/li_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/cycle/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.505197 siriuspy-2.78.0/siriuspy/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/bbb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/blctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41475 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/bpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/currinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/dcct.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13949 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16525 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/dvf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/egun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/energy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51622 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/ict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10051 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21328 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20759 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/injctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38127 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/injsys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/lienergy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/lillrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/machshift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/modltr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/orbit_interlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/posang.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10195 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/psconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/pstesters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30064 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/pwrsupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/screen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/sofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/syncd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/timing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/devices/tune.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.505197 siriuspy-2.78.0/siriuspy/diagbeam/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.505197 siriuspy-2.78.0/siriuspy/diagbeam/bpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/bpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/bpm/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.505197 siriuspy-2.78.0/siriuspy/diagbeam/dcct/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/dcct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/dcct/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagbeam/ict/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/ict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/ict/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagbeam/screen/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/screen/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagbeam/slit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/slit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagbeam/slit/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagsys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagsys/lidiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/lidiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/lidiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/lidiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/lidiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagsys/psdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/psdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/psdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/psdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/psdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagsys/pudiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/pudiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/pudiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/pudiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/pudiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/diagsys/rfdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/rfdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/rfdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/rfdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/diagsys/rfdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/dvfimgproc/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/dvfimgproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/dvfimgproc/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15295 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/dvfimgproc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7082 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/dvfimgproc/meas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/envars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/epics/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/pv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/pv_fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/pv_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/epics/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/fofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/fofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/fofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77425 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/fofb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/idff/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/idff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7315 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/idff/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/idff/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14175 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/idff/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.509197 siriuspy-2.78.0/siriuspy/injctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/injctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15253 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/injctrl/bias_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24732 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/injctrl/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70114 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/injctrl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/machshift/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/gensumm_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)    78928 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/macschedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/savedata_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/machshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/excdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/magnet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/meas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/meas/liemit/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/liemit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/liemit/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/liemit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/meas/lienergy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/lienergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/lienergy/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/lienergy/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/meas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/namesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/namesys/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/optics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/optics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/optics/lattice_survey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/chrom.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/opticscorr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/oscilloscope/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/oscilloscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6974 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/oscilloscope/keysight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/oscilloscope/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.513197 siriuspy-2.78.0/siriuspy/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/posang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/posang/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/posang/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/posang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/beaglebone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)   150566 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10629 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/pru.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25723 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/prucontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/prucparms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/psdevstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/udc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscreaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscwriters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/psmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34142 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/pwrsupply/siggen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/test_reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/testwfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/ramp/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.517197 siriuspy-2.78.0/siriuspy/search/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/bpms_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6632 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/hl_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/id_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/ioc_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/ll_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/ma_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/search/ps_search.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/siriuspy/simul/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/simfactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/simps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/simpv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/simul/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/siriuspy/sofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/bpms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32010 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47062 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46398 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11841 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36357 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/sofb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/siriuspy/stabinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/stabinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/stabinfo/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/stabinfo/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8598 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/siriuspy/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/hl_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33264 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/ll_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/plot_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/timesys/static_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-07-17 20:43:48.000000 siriuspy-2.78.0/siriuspy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.497197 siriuspy-2.78.0/siriuspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10133 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-17 20:43:58.000000 siriuspy-2.78.0/siriuspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/test_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/test_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/test_serial.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/bsmp/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/clientconfigdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/clientconfigdb/test_configdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/clientweb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/clientweb/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/currinfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/currinfo/lifetime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/currinfo/lifetime/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/currinfo/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/currinfo/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/magnet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/magnet/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/magnet/tests_normalizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/mock_servweb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.521197 siriuspy-2.78.0/tests/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/namesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/namesys/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/test_chrom.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/test_opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/test_tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/opticscorr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/posang/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/posang/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/posang/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/db.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/pructrl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/pructrl/test_pru.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/psctrl/test_pscwriters.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/test_beaglebone.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/test_siggen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/pwrsupply/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/ramp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/ramp/test_magnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/ramp/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/test_hl_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/test_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/test_ll_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/test_ma_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/search/test_ps_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/test_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/test_envars.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:58.525197 siriuspy-2.78.0/tests/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/timesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/timesys/test_csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-07-17 20:43:48.000000 siriuspy-2.78.0/tests/timesys/test_plot_network.py
```

### Comparing `siriuspy-2.77.0/LICENSE` & `siriuspy-2.78.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/PKG-INFO` & `siriuspy-2.78.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.77.0
+Version: 2.78.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.77.0/README.md` & `siriuspy-2.78.0/README.md`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/setup.py` & `siriuspy-2.78.0/setup.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/__init__.py` & `siriuspy-2.78.0/siriuspy/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/bsmp/commands.py` & `siriuspy-2.78.0/siriuspy/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/bsmp/constants.py` & `siriuspy-2.78.0/siriuspy/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/bsmp/entities.py` & `siriuspy-2.78.0/siriuspy/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/bsmp/exceptions.py` & `siriuspy-2.78.0/siriuspy/bsmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/bsmp/serial.py` & `siriuspy-2.78.0/siriuspy/bsmp/serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/bsmp/types.py` & `siriuspy-2.78.0/siriuspy/bsmp/types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/callbacks.py` & `siriuspy-2.78.0/siriuspy/callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientarch/client.py` & `siriuspy-2.78.0/siriuspy/clientarch/client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientarch/devices.py` & `siriuspy-2.78.0/siriuspy/clientarch/devices.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientarch/exceptions.py` & `siriuspy-2.78.0/siriuspy/clientarch/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientarch/pvarch.py` & `siriuspy-2.78.0/siriuspy/clientarch/pvarch.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientarch/time.py` & `siriuspy-2.78.0/siriuspy/clientarch/time.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/_templates.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/_templates.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/configdb_client.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/configdb_document.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/configdb_document.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/pvsconfig.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/pvsconfig.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_corrloop_params.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_corrloop_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_diagnostics.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_diagnostics.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     'IA-16RaBPM:TI-AMCFPGAEVR:',
     'IA-17RaBPM:TI-AMCFPGAEVR:',
     'IA-18RaBPM:TI-AMCFPGAEVR:',
     'IA-19RaBPM:TI-AMCFPGAEVR:',
     'IA-20RaBPM:TI-AMCFPGAEVR:',
     'IA-20RaBPMTL:TI-AMCFPGAEVR:',
     ]
-_amcfpgaevr_amcs = ['AMC2', 'AMC3', 'AMC4', 'AMC5', 'AMC6', 'AMC7']
+_amcfpgaevr_amcs = ['AMC3', 'AMC4', 'AMC6', 'AMC7']
 _amcfpgaevr_propts = [
     ['State-Sel', 1, 0.0],
     ['Src-Sel', 3, 0.0],
     ['Dir-Sel', 0, 0.0],
     ['Evt-SP', 0, 0.0],
     ['WidthRaw-SP', 1, 0.0],
     ['Polarity-Sel', 0, 0.0],
```

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_pwrstate.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_pwrstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_rf.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/as_rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_normalized.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_orbit.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_ramp.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/global_config.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/global_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -616,14 +616,23 @@
     ['SI-Fam:TI-BPM:NrPulses-SP', 0, 0.0],
     ['SI-Fam:TI-BPM:Polarity-Sel', 0, 0.0],
     ['SI-Fam:TI-BPM:Src-Sel', 0, 0.0],
     ['SI-Fam:TI-BPM:State-Sel', 0, 0.0],
     ['SI-Fam:TI-BPM:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['SI-Fam:TI-BPM:LowLvlLock-Sel', 0, 0.0],
 
+    ['SI-Fam:TI-BPM-PsMtn:DelayRaw-SP', 0, 0],
+    ['SI-Fam:TI-BPM-PsMtn:WidthRaw-SP', 0, 0.0],
+    ['SI-Fam:TI-BPM-PsMtn:NrPulses-SP', 0, 0.0],
+    ['SI-Fam:TI-BPM-PsMtn:Polarity-Sel', 0, 0.0],
+    ['SI-Fam:TI-BPM-PsMtn:Src-Sel', 0, 0.0],
+    ['SI-Fam:TI-BPM-PsMtn:State-Sel', 0, 0.0],
+    ['SI-Fam:TI-BPM-PsMtn:DeltaDelayRaw-SP', 30*[0, ], 0],
+    ['SI-Fam:TI-BPM-PsMtn:LowLvlLock-Sel', 0, 0.0],
+
     ['SI-Fam:TI-FOFB:DelayRaw-SP', 0, 0],
     ['SI-Fam:TI-FOFB:WidthRaw-SP', 0, 0.0],
     ['SI-Fam:TI-FOFB:NrPulses-SP', 0, 0.0],
     ['SI-Fam:TI-FOFB:Polarity-Sel', 0, 0.0],
     ['SI-Fam:TI-FOFB:Src-Sel', 0, 0.0],
     ['SI-Fam:TI-FOFB:State-Sel', 0, 0.0],
     ['SI-Fam:TI-FOFB:DeltaDelayRaw-SP', 30*[0, ], 0],
@@ -2591,28 +2600,16 @@
     ['SI-01M1:PS-QFA:Current-SP', 0.0, 0.0],  # [A]
     ]
 
 
 _pvs_si_ps_ids = [
     ['SI-14SB:PS-CH-1:OpMode-Sel', _SLOWREF, 0.0],
     ['SI-14SB:PS-CH-2:OpMode-Sel', _SLOWREF, 0.0],
-    ['SI-10SB:PS-CH-1:OpMode-Sel', _SLOWREF, 0.0],
-    ['SI-10SB:PS-CH-2:OpMode-Sel', _SLOWREF, 0.0],
-    ['SI-10SB:PS-CV-1:OpMode-Sel', _SLOWREF, 0.0],
-    ['SI-10SB:PS-CV-2:OpMode-Sel', _SLOWREF, 0.0],
-    ['SI-10SB:PS-QS-1:OpMode-Sel', _SLOWREF, 0.0],
-    ['SI-10SB:PS-QS-2:OpMode-Sel', _SLOWREF, 0.0],
     ['SI-14SB:PS-CH-1:Current-SP', 0.0, 0.0],  # [A]
     ['SI-14SB:PS-CH-2:Current-SP', 0.0, 0.0],  # [A]
-    ['SI-10SB:PS-CH-1:Current-SP', 0.0, 0.0],  # [A]
-    ['SI-10SB:PS-CH-2:Current-SP', 0.0, 0.0],  # [A]
-    ['SI-10SB:PS-CV-1:Current-SP', 0.0, 0.0],  # [A]
-    ['SI-10SB:PS-CV-2:Current-SP', 0.0, 0.0],  # [A]
-    ['SI-10SB:PS-QS-1:Current-SP', 0.0, 0.0],  # [A]
-    ['SI-10SB:PS-QS-2:Current-SP', 0.0, 0.0],  # [A]
     ]
 
 
 _pvs_si_septff = [
     ['SI-01M1:PS-FFCH:OpMode-Sel', _SLOWREF, 0.0],
     ['SI-01M1:PS-FFCV:OpMode-Sel', _SLOWREF, 0.0],
     ['SI-01M2:PS-FFCH:OpMode-Sel', _SLOWREF, 0.0],
```

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_bbadata.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_bbadata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_bbbproc.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_bbbproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_fofb.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_id.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_id.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_idff.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_orbit.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_normalized.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_orbit.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_posang_respm.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/tb_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_orbit.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_posang_respm.py` & `siriuspy-2.78.0/siriuspy/clientconfigdb/types/ts_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/clientweb/implementation.py` & `siriuspy-2.78.0/siriuspy/clientweb/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/csdev.py` & `siriuspy-2.78.0/siriuspy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/currinfo/csdev.py` & `siriuspy-2.78.0/siriuspy/currinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/currinfo/lifetime/main.py` & `siriuspy-2.78.0/siriuspy/currinfo/lifetime/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/currinfo/main.py` & `siriuspy-2.78.0/siriuspy/currinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/cycle/__init__.py` & `siriuspy-2.78.0/siriuspy/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/cycle/bo_cycle_data.py` & `siriuspy-2.78.0/siriuspy/cycle/bo_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/cycle/conn.py` & `siriuspy-2.78.0/siriuspy/cycle/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/cycle/fc_cycle_data.py` & `siriuspy-2.78.0/siriuspy/cycle/fc_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/cycle/li_cycle_data.py` & `siriuspy-2.78.0/siriuspy/cycle/li_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/cycle/main.py` & `siriuspy-2.78.0/siriuspy/cycle/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/cycle/util.py` & `siriuspy-2.78.0/siriuspy/cycle/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/__init__.py` & `siriuspy-2.78.0/siriuspy/devices/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from .energy import Energy
 from .fofb import FOFBCtrlDCC, BPMDCC, FOFBCtrlRef, FamFOFBControllers, \
     FamFastCorrs, HLFOFB
 from .ict import ICT, TranspEff
 from .ids import APU, WIG, PAPU, EPU
 from .idff import IDFF, WIGIDFF, PAPUIDFF, EPUIDFF, APUIDFF
 from .injctrl import InjCtrl
-from .injsys import ASPUStandbyHandler, BOPSRampStandbyHandler, \
-    BORFRampStandbyHandler, InjBOStandbyHandler, InjSysStandbyHandler, \
-    LILLRFStandbyHandler, InjSysPUModeHandler
+from .injsys import PUMagsStandbyHandler, BOPSRampStandbyHandler, \
+    BORFRampStandbyHandler, InjSysStandbyHandler, LinacStandbyHandler, \
+    InjSysPUModeHandler
 from .lillrf import LILLRF, DevLILLRF
 from .machshift import MachShift
 from .modltr import LIModltr
 from .orbit_interlock import BPMOrbitIntlk, BaseOrbitIntlk, OrbitInterlock
 from .posang import PosAng
 from .psconv import PSProperty, StrengthConv
 from .pssofb import PSCorrSOFB, PSApplySOFB
```

### Comparing `siriuspy-2.77.0/siriuspy/devices/bbb.py` & `siriuspy-2.78.0/siriuspy/devices/bbb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/blctrl.py` & `siriuspy-2.78.0/siriuspy/devices/blctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/bpm.py` & `siriuspy-2.78.0/siriuspy/devices/bpm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/currinfo.py` & `siriuspy-2.78.0/siriuspy/devices/currinfo.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/dcct.py` & `siriuspy-2.78.0/siriuspy/devices/dcct.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/device.py` & `siriuspy-2.78.0/siriuspy/devices/device.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/dvf.py` & `siriuspy-2.78.0/siriuspy/devices/dvf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/egun.py` & `siriuspy-2.78.0/siriuspy/devices/egun.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/energy.py` & `siriuspy-2.78.0/siriuspy/devices/energy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/fofb.py` & `siriuspy-2.78.0/siriuspy/devices/fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/ict.py` & `siriuspy-2.78.0/siriuspy/devices/ict.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/idff.py` & `siriuspy-2.78.0/siriuspy/devices/idff.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     def get_polarization_state(
             self, pparameter_value=None, kparameter_value=None):
         """."""
         if self.pparametername is None:
             if kparameter_value is None:
                 kparameter_value = self.kparameter_mon
             return self.polarizations[0], pparameter_value, kparameter_value
-        if pparameter_value:
+        if pparameter_value is None:
             pparameter_value = self.pparameter_mon
         if kparameter_value is None:
             kparameter_value = self.kparameter_mon
         if None in (pparameter_value, kparameter_value):
             return None, pparameter_value, kparameter_value
         polarization = self.idffconfig.get_polarization_state(
             pparameter=pparameter_value, kparameter=kparameter_value)
```

### Comparing `siriuspy-2.77.0/siriuspy/devices/ids.py` & `siriuspy-2.78.0/siriuspy/devices/ids.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/injctrl.py` & `siriuspy-2.78.0/siriuspy/devices/injctrl.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,24 +93,24 @@
         # call base class constructor
         super().__init__(devname, properties=InjCtrl._properties)
 
     # ----- general injection properties -----
 
     @property
     def injmode(self):
-        """Injection mode (Decay or TopUp)."""
+        """Injection mode (Decay or TopUp or Accum)."""
         return self['Mode-Sts']
 
     @injmode.setter
     def injmode(self, value):
         self._enum_setter('Mode-Sel', value, self.InjMode)
 
     @property
     def injmode_str(self):
-        """Injection mode string (Decay or TopUp)."""
+        """Injection mode string (Decay or TopUp or Accum)."""
         return self.InjMode._fields[self['Mode-Sts']]
 
     @property
     def injtype(self):
         """Injection type (SingleBunch or MultiBunch)."""
         return self['Type-Sts']
```

### Comparing `siriuspy-2.77.0/siriuspy/devices/injsys.py` & `siriuspy-2.78.0/siriuspy/devices/injsys.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,45 @@
 from threading import Thread as _Thread, Event as _Flag
 import logging as _log
 
 from .device import Devices as _Devices, DeviceNC as _DeviceNC
 from .lillrf import DevLILLRF
 from .modltr import LIModltr
 from .pwrsupply import PowerSupply, PowerSupplyPU
-from .timing import EVG, Event, Trigger
+from .timing import HLTiming
 from .rf import ASLLRF
 from .posang import PosAng
 
 from ..search import PSSearch, HLTimeSearch
 from ..csdev import Const as _Const
 from ..timesys.csdev import Const as _TIConst
 from ..pwrsupply.csdev import Const as _PSConst
 from ..injctrl.csdev import Const as _InjConst
 from ..callbacks import Callback as _Callback
 
 
 class _BaseHandler(_Devices):
     """Base standby mode handler for injection procedure."""
 
+    def __init__(self, devname, devices, hltiming=None):
+        """."""
+        self._hltiming = hltiming or HLTiming()
+        devices = tuple(devices) + (self._hltiming, )
+        super().__init__(devname, devices)
+
+    @property
+    def hltiming(self):
+        """."""
+        return self._hltiming
+
+    @hltiming.setter
+    def hltiming(self, hltiming):
+        if isinstance(hltiming, HLTiming):
+            self._hltiming = hltiming
+
     @property
     def is_on(self):
         """Is on."""
         for dev, ppties in self._on_values.items():
             for ppty, val in ppties.items():
                 if not dev[ppty] == val:
                     return False
@@ -39,70 +55,46 @@
         vals = dict()
         for dev, ppties in self._on_values.items():
             for ppty, val in ppties.items():
                 vals[dev.pv_object(ppty).pvname] = val
         return vals
 
 
-class ASPUStandbyHandler(_BaseHandler):
+class PUMagsStandbyHandler(_BaseHandler):
     """Pulsed magnets standby mode handler for injection procedure."""
 
-    def __init__(self):
+    def __init__(self, hltiming=None):
         """Init."""
         self._punames = PSSearch.get_psnames(
             {'dis': 'PU', 'dev': '.*(Kckr|Sept)',
              'propty_name': '(?!:CCoil).*'})
         self._trignames = [
             dev.replace('PU', 'TI') for dev in self._punames]
-        self._modnames = LIModltr.DEVICES.ALL
 
         # pu devices
         self._pudevs = [PowerSupplyPU(pun) for pun in self._punames]
 
-        # trigger devices
-        self._trigdevs = [Trigger(trg) for trg in self._trignames]
-
-        # modulator devices
-        self._moddevs = [LIModltr(mod) for mod in self._modnames]
-        self._limps = _DeviceNC(
-            'LA-CN:H1MPS-1',
-            ('Mod1State_I', 'Mod1State_L', 'Mod1State_R',
-             'Mod2State_I', 'Mod2State_L', 'Mod2State_R'))
+        # call base class constructor
+        super().__init__('', self._pudevs, hltiming=hltiming)
 
-        alldevs = self._pudevs + self._trigdevs + self._moddevs
-        alldevs.append(self._limps)
-        alldevs = tuple(alldevs)
+        # trigger devices
+        self._trigdevs = [self._hltiming.triggers[t] for t in self._trignames]
 
         self._on_values = dict()
         for pudev in self._pudevs:
             if 'InjDpKckr' in pudev.devname:
                 continue
             self._on_values[pudev] = {
                 'Pulse-Sts': _PSConst.DsblEnbl.Enbl,
                 'PwrState-Sts': _PSConst.DsblEnbl.Enbl}
         for tdev in self._trigdevs:
             if 'InjDpKckr' in tdev.devname:
                 continue
             self._on_values[tdev] = {
                 'State-Sts': _TIConst.DsblEnbl.Enbl}
-        for mdev in self._moddevs:
-            self._on_values[mdev] = {
-                'CHARGE': _TIConst.DsblEnbl.Enbl,
-                'TRIGOUT': _TIConst.DsblEnbl.Enbl,
-                'CPS_ALL': 1,
-            }
-        self._on_values[self._limps] = {
-            'Mod1State_I': 0,
-            'Mod1State_L': 0,
-            'Mod2State_I': 0,
-            'Mod2State_L': 0,
-        }
-
-        # call base class constructor
-        super().__init__('', alldevs)
 
     @property
     def punames(self):
         """Power supply names."""
         return _dcopy(self._punames)
 
     @property
@@ -116,39 +108,16 @@
         return _dcopy(self._trignames)
 
     @property
     def trigdevices(self):
         """Trigger devices."""
         return self._trigdevs
 
-    @property
-    def modnames(self):
-        """Modulator names."""
-        return _dcopy(self._modnames)
-
-    @property
-    def moddevices(self):
-        """Modulator devices."""
-        return self._moddevs
-
     def cmd_turn_off(self):
         """Turn off."""
-        # turn modulator trigout off
-        self._set_devices_propty(
-            self._moddevs, 'TRIGOUT', _Const.DsblEnbl.Dsbl)
-
-        # wait for modulator trigout to turn off
-        retval = self._wait_devices_propty(
-            self._moddevs, 'TRIGOUT', _Const.DsblEnbl.Dsbl,
-            timeout=3, return_prob=True)
-        if not retval[0]:
-            text = 'Check for LI modulator TrigOut to be off timed '\
-                   'out without success! Verify LI Modulators!'
-            return [False, text, retval[1]]
-
         # set pulsed magnet pulse off
         self._set_devices_propty(
             self._pudevs, 'Pulse-Sel', _PSConst.DsblEnbl.Dsbl)
 
         # wait for pulsed magnet pulse to be off
         retval = self._wait_devices_propty(
             self._pudevs, 'Pulse-Sts', _PSConst.DsblEnbl.Dsbl,
@@ -167,164 +136,79 @@
             self._pudevs, 'PwrState-Sts', _PSConst.DsblEnbl.Dsbl,
             timeout=3, return_prob=True)
         if not retval[0]:
             text = 'Check for pulsed magnet PwrState to be off '\
                    'timed out without success! Verify pulsed magnets!'
             return [False, text, retval[1]]
 
-        # wait for modulators trig.out
-        _time.sleep(1)
-
-        # turn modulator charge off
-        self._set_devices_propty(
-            self._moddevs, 'CHARGE', _Const.DsblEnbl.Dsbl)
-
-        # wait for modulator charge to turn off
-        retval = self._wait_devices_propty(
-            self._moddevs, 'CHARGE', _Const.DsblEnbl.Dsbl,
-            timeout=3, return_prob=True)
-        if not retval[0]:
-            text = 'Check for LI modulator Charge to be off timed '\
-                   'out without success! Verify LI Modulators!'
-            return [False, text, retval[1]]
-
         return True, '', []
 
     def cmd_turn_on(self):
         """Turn on."""
-        # turn modulators charge on
-        self._set_devices_propty(
-            self._moddevs, 'CHARGE', _Const.DsblEnbl.Enbl)
-
-        # wait for modulators charge to turn on
-        retval = self._wait_devices_propty(
-            self._moddevs, 'CHARGE', _Const.DsblEnbl.Enbl,
-            timeout=3, return_prob=True)
-        if not retval[0]:
-            text = 'Check for LI modulator Charge to be on timed '\
-                   'out without success! Verify LI Modulators!'
-            return [False, text, retval[1]]
-
-        # reset modulator
-        for dev in self._moddevs:
-            if not dev.cmd_reset():
-                text = 'Could not reset LI modulator! Verify LI Modulators!'
-                return [False, text, [dev.devname+':RESET', ]]
-
         devs = [dev for dev in self._pudevs if 'InjDpKckr' not in dev.devname]
 
         # set pulsed magnet power state on
         self._set_devices_propty(devs, 'PwrState-Sel', _PSConst.DsblEnbl.Enbl)
 
         # wait for pulsed magnet power state to be on
         retval = self._wait_devices_propty(
             devs, 'PwrState-Sts', _PSConst.DsblEnbl.Enbl,
             timeout=3, return_prob=True)
         if not retval[0]:
             text = 'Check for pulsed magnet PwrState to be on '\
                    'timed out without success! Verify pulsed magnets!'
             return [False, text, retval[1]]
 
-        # wait a moment for the PU high voltage and modulators charge
+        # wait a moment for the PU high voltage
         _time.sleep(1)
 
         # set pulsed magnet pulse on
         self._set_devices_propty(devs, 'Pulse-Sel', _PSConst.DsblEnbl.Enbl)
 
         # wait for pulsed magnet pulse to be on
         retval = self._wait_devices_propty(
             devs, 'Pulse-Sts', _PSConst.DsblEnbl.Enbl,
             timeout=3, return_prob=True)
         if not retval[0]:
             text = 'Check for pulsed magnet Pulse to be enabled '\
-                   'timed out without success! Verify pulsed magnets!'
-            return [False, text, retval[1]]
-
-        # turn modulator trigout on
-        self._set_devices_propty(
-            self._moddevs, 'TRIGOUT', _Const.DsblEnbl.Enbl)
-
-        # wait for modulator trigout to turn on
-        retval = self._wait_devices_propty(
-            self._moddevs, 'TRIGOUT', _Const.DsblEnbl.Enbl,
-            timeout=3, return_prob=True)
-        if not retval[0]:
-            text = 'Check for LI modulator TrigOut to be on timed '\
-                   'out without success! Verify LI Modulators!'
+                'timed out without success! Verify pulsed magnets!'
             return [False, text, retval[1]]
 
-        # check if mps status is ok
-        _t0 = _time.time()
-        while _time.time() - _t0 < 5:
-            if not self._limps['Mod1State_I'] and \
-                    not self._limps['Mod2State_I']:
-                break
-        else:
-            problems = [
-                self._limps.pv_object('Mod'+i+'State_I').pvname for
-                i in ['1', '2'] if self._limps['Mod'+i+'State_I']]
-            text = 'Check for LI modulators MPS Status to be ok timed '\
-                   'out without success! Verify LI Modulators MPS!'
-            return [False, text, problems]
-
-        # reset linac mps modulator signal
-        self._limps['Mod1State_R'] = 1
-        self._limps['Mod2State_R'] = 1
-        _time.sleep(1)
-        self._limps['Mod1State_R'] = 0
-        self._limps['Mod2State_R'] = 0
-
-        # check if mps latch is ok
-        _t0 = _time.time()
-        while _time.time() - _t0 < 5:
-            if not self._limps['Mod1State_L'] and \
-                    not self._limps['Mod2State_L']:
-                break
-        else:
-            problems = [
-                self._limps.pv_object('Mod'+i+'State_L').pvname for
-                i in ['1', '2'] if self._limps['Mod'+i+'State_L']]
-            text = 'Check for LI modulators MPS Latch to be ok timed '\
-                   'out without success! Verify LI Modulators MPS!'
-            return [False, text, problems]
-
         return True, '', []
 
 
 class BOPSRampStandbyHandler(_BaseHandler):
     """BO PS Ramp standy mode handler for injection procedure."""
 
-    def __init__(self):
+    def __init__(self, hltiming=None):
         """Init."""
         self._psnames = PSSearch.get_psnames(
             {'sec': 'BO', 'dis': 'PS'})
         self._trignames = HLTimeSearch.get_hl_triggers(
             {'sec': 'BO', 'dev': 'Mags'})
 
         # ps devices
         self._psdevs = [PowerSupply(psn) for psn in self._psnames]
 
-        # trigger devices
-        self._trigdevs = [Trigger(trg) for trg in self._trignames]
+        # call base class constructor
+        super().__init__('', self._psdevs, hltiming=hltiming)
 
-        alldevs = tuple(self._psdevs + self._trigdevs)
+        # trigger devices
+        self._trigdevs = [self._hltiming.triggers[t] for t in self._trignames]
 
         self._on_values = dict()
         for psdev in self._psdevs:
             self._on_values[psdev] = {
                 'OpMode-Sts': _PSConst.States.RmpWfm,
                 'WfmUpdateAuto-Sts': _PSConst.DsblEnbl.Enbl}
         for tdev in self._trigdevs:
             self._on_values[tdev] = {
                 'State-Sts': _TIConst.DsblEnbl.Enbl,
                 'Src-Sts': tdev.source_options.index('RmpBO')}
 
-        # call base class constructor
-        super().__init__('', alldevs)
-
     @property
     def psnames(self):
         """Power supply names."""
         return _dcopy(self._psnames)
 
     @property
     def psdevices(self):
@@ -339,26 +223,17 @@
     @property
     def trigdevices(self):
         """Trigger devices."""
         return self._trigdevs
 
     def cmd_turn_off(self):
         """Turn off."""
-        # disable triggers
-        self._set_devices_propty(
-            self._trigdevs, 'State-Sel', _TIConst.DsblEnbl.Dsbl)
-
-        # wait for triggers to be disabled
-        retval = self._wait_devices_propty(
-            self._trigdevs, 'State-Sts', _TIConst.DsblEnbl.Dsbl,
-            timeout=3, return_prob=True)
+        retval = self.disable_triggers()
         if not retval[0]:
-            text = 'Check for BO Mags Triggers to be disabled timed '\
-                   'out without success! Verify BO Mags Triggers!'
-            return [False, text, retval[1]]
+            return retval
 
         # wait duration of a ramp for PS change opmode
         _time.sleep(0.5)
 
         # set slowref
         self._set_devices_propty(
             self._psdevs, 'OpMode-Sel', _PSConst.OpMode.SlowRef)
@@ -406,262 +281,420 @@
             self._psdevs, 'WfmUpdateAuto-Sel', _PSConst.DsblEnbl.Enbl)
 
         # wait for PS WfmUpdateAuto to be enabled
         retval = self._wait_devices_propty(
             self._psdevs, 'WfmUpdateAuto-Sts', _PSConst.DsblEnbl.Enbl,
             timeout=3, return_prob=True)
         if not retval[0]:
-            text = 'Check for BO PS WfmUpdateAuto to be enable '\
-                   'timed out without success! Verify BO PS!'
+            text = 'Check for BO PS WfmUpdateAuto to be enabled '\
+                'timed out without success! Verify BO PS!'
             return [False, text, retval[1]]
 
         # configure trigger source
         values = [dev.source_options.index('RmpBO') for dev in self._trigdevs]
         self._set_devices_propty(self._trigdevs, 'Src-Sel', values)
 
         # wait for trigger source to be configured
         retval = self._wait_devices_propty(
             self._trigdevs, 'Src-Sts', values, timeout=3, return_prob=True)
         if not retval[0]:
             text = 'Check for BO Mags Triggers to be in RmpBO event '\
                    'timed out without success! Verify BO Mags Triggers!'
             return [False, text, retval[1]]
 
+        retval = self.enable_triggers()
+        if not retval[0]:
+            return retval
+
+        return True, '', []
+
+    def disable_triggers(self):
+        """."""
+        # disable triggers
+        self._set_devices_propty(
+            self._trigdevs, 'State-Sel', _TIConst.DsblEnbl.Dsbl)
+
+        # wait for triggers to be disabled
+        retval = self._wait_devices_propty(
+            self._trigdevs, 'State-Sts', _TIConst.DsblEnbl.Dsbl,
+            timeout=3, return_prob=True)
+
+        if retval[0]:
+            return True, '', []
+        text = 'Check for BO Mags Triggers to be disabled timed '\
+               'out without success! Verify BO Mags Triggers!'
+        return [False, text, retval[1]]
+
+    def enable_triggers(self):
+        """."""
         # enable triggers
         self._set_devices_propty(
             self._trigdevs, 'State-Sel', _TIConst.DsblEnbl.Enbl)
 
-        # wait for triggers to be enable
+        # wait for triggers to be enabled
         retval = self._wait_devices_propty(
             self._trigdevs, 'State-Sts', _TIConst.DsblEnbl.Enbl,
             timeout=3, return_prob=True)
-        if not retval[0]:
-            text = 'Check for BO Mags Triggers to be enable timed '\
-                   'out without success! Verify BO Mags Triggers!'
-            return [False, text, retval[1]]
 
-        return True, '', []
+        if retval[0]:
+            return True, '', []
+        text = 'Check for BO Mags Triggers to be enabled timed '\
+            'out without success! Verify BO Mags Triggers!'
+        return [False, text, retval[1]]
 
 
 class BORFRampStandbyHandler(_BaseHandler):
     """BO RF Ramp standby mode handler for injection procedure."""
 
-    def __init__(self):
+    def __init__(self, hltiming=None):
+        """."""
         self.llrf = ASLLRF(ASLLRF.DEVICES.BO)
-        self.rmptrg = Trigger('BO-Glob:TI-LLRF-Rmp')
 
-        devices = (self.llrf, self.rmptrg)
+        # call base class constructor
+        super().__init__('', (self.llrf, ), hltiming=hltiming)
+
+        self.rmptrg = self._hltiming.triggers['BO-Glob:TI-LLRF-Rmp']
 
         self._on_values = dict()
         self._on_values[self.llrf] = {
             'RmpEnbl-Sts': _Const.DsblEnbl.Enbl,
             'RmpReady-Mon': _Const.DsblEnbl.Enbl}
         self._on_values[self.rmptrg] = {
             'State-Sts': _Const.DsblEnbl.Enbl}
 
-        # call base class constructor
-        super().__init__('', devices)
-
     def cmd_turn_off(self):
         """Turn off."""
         # set RF ramp to disable
         self.llrf.rmp_enable = _Const.DsblEnbl.Dsbl
 
         # wait for RF ramp to be disable
         retval = self._wait_devices_propty(
             self.llrf, 'RmpEnbl-Sts', _Const.DsblEnbl.Dsbl,
             timeout=3, return_prob=True)
         if not retval[0]:
             text = 'Check for BO RF Ramp to be disabled timed '\
                    'out without success! Verify BO RF Ramp!'
             return [False, text, retval[1]]
 
+        retval = self.disable_triggers()
+        if not retval[0]:
+            return retval
+
         return True, '', []
 
     def cmd_turn_on(self):
         """Turn on."""
+        retval = self.enable_triggers()
+        if not retval[0]:
+            return retval
+
         # set RF ramp to enabled
         self.llrf.rmp_enable = _Const.DsblEnbl.Enbl
 
         # wait for RF ramp to be enabled
         retval = self._wait_devices_propty(
             self.llrf, 'RmpEnbl-Sts', _Const.DsblEnbl.Enbl,
             timeout=3, return_prob=True)
         if not retval[0]:
             text = 'Check for BO RF Ramp to be enabled timed '\
-                   'out without success! Verify BO RF Ramp!'
+                'out without success! Verify BO RF Ramp!'
             return [False, text, retval[1]]
 
         return True, '', []
 
+    def disable_triggers(self):
+        """."""
+        # disable triggers
+        self._set_devices_propty(
+            self.rmptrg, 'State-Sel', _TIConst.DsblEnbl.Dsbl)
 
-class InjBOStandbyHandler(_BaseHandler):
-    """InjBO Event standby mode handler for injection procedure."""
-
-    def __init__(self):
-        self.evg = EVG()
-        self.injboevt = Event('InjBO')
-
-        devices = (self.evg, self.injboevt)
-
-        self._on_values = {
-            self.injboevt: {'Mode-Sts': Event.MODES.index('Continuous')}}
-
-        # call base class constructor
-        super().__init__('', devices)
-
-    def cmd_turn_off(self):
-        """Turn off."""
-        # disable injbo
-        self.injboevt.mode = 'Disable'
-
-        # wait for injbo to be disabled
+        # wait for triggers to be disabled
         retval = self._wait_devices_propty(
-            self.injboevt, 'Mode-Sts', Event.MODES.index('Disable'),
+            self.rmptrg, 'State-Sts', _TIConst.DsblEnbl.Dsbl,
             timeout=3, return_prob=True)
-        if not retval[0]:
-            text = 'Check for InjBO Event to be disabled timed '\
-                   'out without success! Verify InjBO Event!'
-            return [False, text, retval[1]]
 
-        # update events
-        _time.sleep(1)
-        self.evg.cmd_update_events()
-        _time.sleep(1)
-
-        return True, '', []
+        if retval[0]:
+            return True, '', []
+        text = 'Check for BO RF Triggers to be disabled timed '\
+            'out without success! Verify BO RF Triggers!'
+        return [False, text, retval[1]]
 
-    def cmd_turn_on(self):
-        """Turn on."""
-        # set injbo to Continuous table
-        self.injboevt.mode = 'Continuous'
+    def enable_triggers(self):
+        """."""
+        # enable triggers
+        self._set_devices_propty(
+            self.rmptrg, 'State-Sel', _TIConst.DsblEnbl.Enbl)
 
-        # wait for injbo to be in Continuous Table
+        # wait for triggers to be enabled
         retval = self._wait_devices_propty(
-            self.injboevt, 'Mode-Sts', Event.MODES.index('Continuous'),
+            self.rmptrg, 'State-Sts', _TIConst.DsblEnbl.Enbl,
             timeout=3, return_prob=True)
-        if not retval[0]:
-            text = 'Check for InjBO Event to be in Continuous table '\
-                   'timed out without success! Verify InjBO Event!'
-            return [False, text, retval[1]]
-
-        # update events
-        self.evg.cmd_update_events()
 
-        return True, '', []
+        if retval[0]:
+            return True, '', []
+        text = 'Check for BO RF Triggers to be enabled timed '\
+            'out without success! Verify BO RF Triggers!'
+        return [False, text, retval[1]]
 
 
-class LILLRFStandbyHandler(_BaseHandler):
+class LinacStandbyHandler(_BaseHandler):
     """LI LLRF standby mode handler for injection procedure."""
 
     WAIT_2_TURNON = 2  # [s]
 
-    def __init__(self):
+    def __init__(self, hltiming=None):
         """Init."""
 
         # create devices
-        devices = list()
+        self._llrf_devs = list()
         for dev in DevLILLRF.DEVICES.ALL:
-            devices.append(DevLILLRF(dev))
-        devices = tuple(devices)
+            self._llrf_devs.append(DevLILLRF(dev))
+
+        self._modnames = LIModltr.DEVICES.ALL
+
+        # modulator devices
+        self._moddevs = [LIModltr(mod) for mod in self._modnames]
+        self._limps = _DeviceNC(
+            'LA-CN:H1MPS-1',
+            ('Mod1State_I', 'Mod1State_L', 'Mod1State_R',
+             'Mod2State_I', 'Mod2State_L', 'Mod2State_R'))
+
+        devices = self._llrf_devs + self._moddevs
+        devices.append(self._limps)
+
+        # call base class constructor
+        super().__init__('', tuple(devices), hltiming=hltiming)
+
+        self._trig_names = HLTimeSearch.get_hl_triggers(
+            {'sec': 'LI', 'dev': '(Mod|LLRF|SSAmp|Osc)'})
 
         self._on_values = dict()
-        for dev in devices:
+        for dev in self._llrf_devs:
             self._on_values[dev] = {
                 'GET_INTEGRAL_ENABLE': _Const.DsblEnbl.Enbl,
                 'GET_FB_MODE': _Const.DsblEnbl.Enbl}
+        for mdev in self._moddevs:
+            self._on_values[mdev] = {
+                'CHARGE': _TIConst.DsblEnbl.Enbl,
+                'TRIGOUT': _TIConst.DsblEnbl.Enbl,
+                'CPS_ALL': 1}
+        self._on_values[self._limps] = {
+            'Mod1State_I': 0, 'Mod1State_L': 0,
+            'Mod2State_I': 0, 'Mod2State_L': 0}
 
-        # call base class constructor
-        super().__init__('', devices)
+    @property
+    def modnames(self):
+        """Modulator names."""
+        return _dcopy(self._modnames)
+
+    @property
+    def moddevices(self):
+        """Modulator devices."""
+        return self._moddevs
 
     def cmd_turn_off(self):
         """Turn off."""
         # turn feedback off
         self._set_devices_propty(
-            self.devices, 'SET_FB_MODE', _Const.DsblEnbl.Dsbl)
-
+            self._llrf_devs, 'SET_FB_MODE', _Const.DsblEnbl.Dsbl)
         # wait for feedback to turn off
         retval = self._wait_devices_propty(
-            self.devices, 'GET_FB_MODE', _Const.DsblEnbl.Dsbl,
+            self._llrf_devs, 'GET_FB_MODE', _Const.DsblEnbl.Dsbl,
             timeout=3, return_prob=True)
         if not retval[0]:
             text = 'Check for LI LLRF Feedback Mode to be off '\
                    'timed out without success! Verify LI LLRF!'
             return [False, text, retval[1]]
 
         # turn integral off
         self._set_devices_propty(
-            self.devices, 'SET_INTEGRAL_ENABLE', _Const.DsblEnbl.Dsbl)
-
+            self._llrf_devs, 'SET_INTEGRAL_ENABLE', _Const.DsblEnbl.Dsbl)
         # wait for integral to turn off
         retval = self._wait_devices_propty(
-            self.devices, 'GET_INTEGRAL_ENABLE', _Const.DsblEnbl.Dsbl,
+            self._llrf_devs, 'GET_INTEGRAL_ENABLE', _Const.DsblEnbl.Dsbl,
             timeout=3, return_prob=True)
         if not retval[0]:
             text = 'Check for LI LLRF Integral Mode to be off '\
                    'timed out without success! Verify LI LLRF!'
             return [False, text, retval[1]]
 
+        self.change_trigs_to_linac_evt()
+
+        # turn modulator trigout off
+        self._set_devices_propty(
+            self._moddevs, 'TRIGOUT', _Const.DsblEnbl.Dsbl)
+        # wait for modulator trigout to turn off
+        retval = self._wait_devices_propty(
+            self._moddevs, 'TRIGOUT', _Const.DsblEnbl.Dsbl,
+            timeout=3, return_prob=True)
+        if not retval[0]:
+            text = 'Check for LI modulator TrigOut to be off timed '\
+                   'out without success! Verify LI Modulators!'
+            return [False, text, retval[1]]
+
+        # wait for modulators trig.out
+        _time.sleep(1)
+
+        # turn modulator charge off
+        self._set_devices_propty(
+            self._moddevs, 'CHARGE', _Const.DsblEnbl.Dsbl)
+        # wait for modulator charge to turn off
+        retval = self._wait_devices_propty(
+            self._moddevs, 'CHARGE', _Const.DsblEnbl.Dsbl,
+            timeout=3, return_prob=True)
+        if not retval[0]:
+            text = 'Check for LI modulator Charge to be off timed '\
+                   'out without success! Verify LI Modulators!'
+            return [False, text, retval[1]]
+
         return True, '', []
 
     def cmd_turn_on(self):
         """Turn on."""
-        # wait for some InjBO pulses
-        _time.sleep(LILLRFStandbyHandler.WAIT_2_TURNON)
+        # turn modulators charge on
+        self._set_devices_propty(
+            self._moddevs, 'CHARGE', _Const.DsblEnbl.Enbl)
+        # wait for modulators charge to turn on
+        retval = self._wait_devices_propty(
+            self._moddevs, 'CHARGE', _Const.DsblEnbl.Enbl,
+            timeout=3, return_prob=True)
+        if not retval[0]:
+            text = 'Check for LI modulator Charge to be on timed '\
+                   'out without success! Verify LI Modulators!'
+            return [False, text, retval[1]]
 
-        # turn integral on
+        # reset modulator
+        for dev in self._moddevs:
+            if not dev.cmd_reset():
+                text = 'Could not reset LI modulator! Verify LI Modulators!'
+                return [False, text, [dev.devname+':RESET', ]]
+
+        # wait a moment for the modulators charge
+        _time.sleep(1)
+
+        # turn modulator trigout on
         self._set_devices_propty(
-            self.devices, 'SET_INTEGRAL_ENABLE', _Const.DsblEnbl.Enbl)
+            self._moddevs, 'TRIGOUT', _Const.DsblEnbl.Enbl)
+        # wait for modulator trigout to turn on
+        retval = self._wait_devices_propty(
+            self._moddevs, 'TRIGOUT', _Const.DsblEnbl.Enbl,
+            timeout=3, return_prob=True)
+        if not retval[0]:
+            text = 'Check for LI modulator TrigOut to be on timed '\
+                   'out without success! Verify LI Modulators!'
+            return [False, text, retval[1]]
+
+        retval = self.check_mps_status()
+        if not retval[0]:
+            return retval
+        retval = self.reset_mps_status()
+        if not retval[0]:
+            return retval
+
+        self.change_trigs_to_rmpbo_evt()
 
+        # wait for some pulses
+        _time.sleep(LinacStandbyHandler.WAIT_2_TURNON)
+
+        # turn integral on
+        self._set_devices_propty(
+            self._llrf_devs, 'SET_INTEGRAL_ENABLE', _Const.DsblEnbl.Enbl)
         # wait for integral to turn on
         retval = self._wait_devices_propty(
-            self.devices, 'GET_INTEGRAL_ENABLE', _Const.DsblEnbl.Enbl,
+            self._llrf_devs, 'GET_INTEGRAL_ENABLE', _Const.DsblEnbl.Enbl,
             timeout=3, return_prob=True)
         if not retval[0]:
             text = 'Check for LI LLRF Integral Mode to be on '\
                    'timed out without success! Verify LI LLRF!'
             return [False, text, retval[1]]
 
         # turn feedback on
         self._set_devices_propty(
-            self.devices, 'SET_FB_MODE', _Const.DsblEnbl.Enbl)
-
+            self._llrf_devs, 'SET_FB_MODE', _Const.DsblEnbl.Enbl)
         # wait for feedback to turn on
         retval = self._wait_devices_propty(
-            self.devices, 'GET_FB_MODE', _Const.DsblEnbl.Enbl,
+            self._llrf_devs, 'GET_FB_MODE', _Const.DsblEnbl.Enbl,
             timeout=3, return_prob=True)
         if not retval[0]:
             text = 'Check for LI LLRF Feedback Mode to be on '\
                    'timed out without success! Verify LI LLRF!'
             return [False, text, retval[1]]
 
         return True, '', []
 
+    def change_trigs_to_linac_evt(self):
+        """."""
+        return self.hltiming.change_triggers_source(
+            self._trig_names, new_src='Linac')
+
+    def change_trigs_to_rmpbo_evt(self):
+        """."""
+        return self.hltiming.change_triggers_source(
+            self._trig_names, new_src='RmpBO')
+
+    def check_mps_status(self):
+        """."""
+        # check if mps status is ok
+        _t0 = _time.time()
+        while _time.time() - _t0 < 5:
+            if not self._limps['Mod1State_I'] and \
+                    not self._limps['Mod2State_I']:
+                return True, '', []
+
+        problems = [
+            self._limps.pv_object('Mod'+i+'State_I').pvname for
+            i in ['1', '2'] if self._limps['Mod'+i+'State_I']]
+        text = 'Check for LI modulators MPS Status to be ok timed '\
+            'out without success! Verify LI Modulators MPS!'
+        return [False, text, problems]
+
+    def reset_mps_status(self):
+        """."""
+        # reset linac mps modulator signal
+        self._limps['Mod1State_R'] = 1
+        self._limps['Mod2State_R'] = 1
+        _time.sleep(1)
+        self._limps['Mod1State_R'] = 0
+        self._limps['Mod2State_R'] = 0
+
+        # check if mps latch is ok
+        _t0 = _time.time()
+        while _time.time() - _t0 < 5:
+            if not self._limps['Mod1State_L'] and \
+                    not self._limps['Mod2State_L']:
+                return True, '', []
+
+        problems = [
+            self._limps.pv_object('Mod'+i+'State_L').pvname for
+            i in ['1', '2'] if self._limps['Mod'+i+'State_L']]
+        text = 'Check for LI modulators MPS Latch to be ok timed '\
+            'out without success! Verify LI Modulators MPS!'
+        return [False, text, problems]
+
 
 class InjSysStandbyHandler(_Devices):
     """Injection system standy mode handler."""
 
     DEF_ON_ORDER = _InjConst.INJSYS_DEF_ON_ORDER
     DEF_OFF_ORDER = _InjConst.INJSYS_DEF_OFF_ORDER
     HANDLER_DESC = {
-        'as_pu': 'AS PU (Septa, Kickers and Modulators)',
+        'as_pu': 'AS PU (All Septa and Kickers)',
         'bo_ps': 'BO PS Ramp',
         'bo_rf': 'BO RF Ramp',
-        'injbo': 'TI InjBO Event',
-        'li_rf': 'LI LLRF (Klystrons Loop)',
+        'li_rf': 'LINAC (SHB, Klystrons and Modulators)',
     }
 
-    def __init__(self):
+    def __init__(self, hltiming=None):
         """Init."""
+        self._hltiming = hltiming or HLTiming()
         devs = {
-            'as_pu': ASPUStandbyHandler(),
-            'bo_ps': BOPSRampStandbyHandler(),
-            'bo_rf': BORFRampStandbyHandler(),
-            'injbo': InjBOStandbyHandler(),
-            'li_rf': LILLRFStandbyHandler(),
+            'as_pu': PUMagsStandbyHandler(hltiming=self._hltiming),
+            'bo_ps': BOPSRampStandbyHandler(hltiming=self._hltiming),
+            'bo_rf': BORFRampStandbyHandler(hltiming=self._hltiming),
+            'li_rf': LinacStandbyHandler(hltiming=self._hltiming),
         }
         self._dev_refs = devs
         self._on_order = InjSysStandbyHandler.DEF_ON_ORDER
         self._off_order = InjSysStandbyHandler.DEF_OFF_ORDER
         self._is_running = ''
         self._done = list()
         self._result = None
@@ -672,14 +705,30 @@
         for dev in devs.values():
             self._on_values.update(dev.on_values)
 
         # call super init
         super().__init__('', tuple(devs.values()))
 
     @property
+    def hltiming(self):
+        """."""
+        return self._hltiming
+
+    @hltiming.setter
+    def hltiming(self, hltiming):
+        """."""
+        if isinstance(hltiming, HLTiming):
+            self._hltiming = hltiming
+
+    @property
+    def handlers(self):
+        """."""
+        return self._dev_refs
+
+    @property
     def on_order(self):
         """On setpoints order."""
         return _dcopy(self._on_order)
 
     @on_order.setter
     def on_order(self, value):
         self._on_order = value
@@ -791,53 +840,66 @@
                 break
             handler = self._dev_refs[handler_name]
             func = getattr(handler, 'cmd_turn_'+cmdtype)
             retval = func()
             if retval[0]:
                 self._done.append(handler_name)
             else:
-                break
+                if self._result is None:
+                    self._result = retval
+                else:
+                    self._result[1] += '\n' + retval[1]
+                    self._result[2] += retval[2]
 
-        self._result = retval
+        if self._result is None:
+            self._result = [True, '', []]
 
         self._is_running = ''
 
 
 class InjSysPUModeHandler(_Devices, _Callback):
     """Device to control pulsed magnets configuration for injection."""
 
     _DEF_TIMEOUT = 10  # [s]
     _DEF_SLEEP = 0.1  # [s]
     SI_DPKCKR_DEFKICK = -6.7  # [mrad]
     TS_POSANG_DEFDELTA = 2.5  # [mrad]
     SI_DPKCKR_DLYREF = 36800000  # [count]
 
-    def __init__(self, print_log=True, callback=None):
+    def __init__(self, print_log=True, callback=None, hltiming=None):
         """Init."""
+        self._hltiming = hltiming or HLTiming()
         self.pudpk = PowerSupplyPU(PowerSupplyPU.DEVICES.SI_INJ_DPKCKR)
         self.punlk = PowerSupplyPU(PowerSupplyPU.DEVICES.SI_INJ_NLKCKR)
-        self.trigdpk = Trigger('SI-01SA:TI-InjDpKckr')
-        self.trignlk = Trigger('SI-01SA:TI-InjNLKckr')
+        self.trigdpk = self._hltiming.triggers['SI-01SA:TI-InjDpKckr']
+        self.trignlk = self._hltiming.triggers['SI-01SA:TI-InjNLKckr']
         self.posang = PosAng(PosAng.DEVICES.TS)
         self.delta_posang = self.TS_POSANG_DEFDELTA
         self.dpkckr_dlyref = self.SI_DPKCKR_DLYREF
         self.dpkckr_kick = self.SI_DPKCKR_DEFKICK
-        devices = (
-            self.pudpk, self.punlk,
-            self.trigdpk, self.trignlk,
-            self.posang,
-        )
+        devices = (self.pudpk, self.punlk, self._hltiming, self.posang)
         self._print_log = print_log
         self._abort = _Flag()
 
         # call super init
         _Devices.__init__(self, '', devices)
         _Callback.__init__(self, callback=callback)
 
     @property
+    def hltiming(self):
+        """."""
+        return self._hltiming
+
+    @hltiming.setter
+    def hltiming(self, hltiming):
+        """."""
+        if isinstance(hltiming, HLTiming):
+            self._hltiming = hltiming
+
+    @property
     def is_trigdpk_onaxis(self):
         """Whether DpK trigger delay raw is above dpkckr_dlyref."""
         return self.trigdpk.delay_raw > self.dpkckr_dlyref
 
     @property
     def is_accum(self):
         """If configuration is Accumulation."""
```

### Comparing `siriuspy-2.77.0/siriuspy/devices/lienergy.py` & `siriuspy-2.78.0/siriuspy/devices/lienergy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/lillrf.py` & `siriuspy-2.78.0/siriuspy/devices/lillrf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/machshift.py` & `siriuspy-2.78.0/siriuspy/devices/machshift.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/modltr.py` & `siriuspy-2.78.0/siriuspy/devices/modltr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/orbit_interlock.py` & `siriuspy-2.78.0/siriuspy/devices/orbit_interlock.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/posang.py` & `siriuspy-2.78.0/siriuspy/devices/posang.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/psconv.py` & `siriuspy-2.78.0/siriuspy/devices/psconv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/pssofb.py` & `siriuspy-2.78.0/siriuspy/devices/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/pstesters.py` & `siriuspy-2.78.0/siriuspy/devices/pstesters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/pwrsupply.py` & `siriuspy-2.78.0/siriuspy/devices/pwrsupply.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/rf.py` & `siriuspy-2.78.0/siriuspy/devices/rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/screen.py` & `siriuspy-2.78.0/siriuspy/devices/screen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/sofb.py` & `siriuspy-2.78.0/siriuspy/devices/sofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/syncd.py` & `siriuspy-2.78.0/siriuspy/devices/syncd.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/timing.py` & `siriuspy-2.78.0/siriuspy/devices/timing.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/devices/tune.py` & `siriuspy-2.78.0/siriuspy/devices/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagbeam/bpm/csdev.py` & `siriuspy-2.78.0/siriuspy/diagbeam/bpm/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagbeam/dcct/csdev.py` & `siriuspy-2.78.0/siriuspy/diagbeam/dcct/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagbeam/ict/csdev.py` & `siriuspy-2.78.0/siriuspy/diagbeam/ict/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagbeam/screen/csdev.py` & `siriuspy-2.78.0/siriuspy/diagbeam/screen/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagbeam/slit/csdev.py` & `siriuspy-2.78.0/siriuspy/diagbeam/slit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/app.py` & `siriuspy-2.78.0/siriuspy/diagsys/app.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/lidiag/csdev.py` & `siriuspy-2.78.0/siriuspy/diagsys/lidiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/lidiag/main.py` & `siriuspy-2.78.0/siriuspy/diagsys/lidiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/lidiag/pvs.py` & `siriuspy-2.78.0/siriuspy/diagsys/lidiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/psdiag/csdev.py` & `siriuspy-2.78.0/siriuspy/diagsys/psdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/psdiag/main.py` & `siriuspy-2.78.0/siriuspy/diagsys/psdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/psdiag/pvs.py` & `siriuspy-2.78.0/siriuspy/diagsys/psdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/pudiag/csdev.py` & `siriuspy-2.78.0/siriuspy/diagsys/pudiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/pudiag/main.py` & `siriuspy-2.78.0/siriuspy/diagsys/pudiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/pudiag/pvs.py` & `siriuspy-2.78.0/siriuspy/diagsys/pudiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/pvs.py` & `siriuspy-2.78.0/siriuspy/diagsys/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/rfdiag/csdev.py` & `siriuspy-2.78.0/siriuspy/diagsys/rfdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/rfdiag/main.py` & `siriuspy-2.78.0/siriuspy/diagsys/rfdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/diagsys/rfdiag/pvs.py` & `siriuspy-2.78.0/siriuspy/diagsys/rfdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/dvfimgproc/csdev.py` & `siriuspy-2.78.0/siriuspy/dvfimgproc/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/dvfimgproc/main.py` & `siriuspy-2.78.0/siriuspy/dvfimgproc/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/dvfimgproc/meas.py` & `siriuspy-2.78.0/siriuspy/dvfimgproc/meas.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/envars.py` & `siriuspy-2.78.0/siriuspy/envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/epics/multiproc.py` & `siriuspy-2.78.0/siriuspy/epics/multiproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/epics/properties.py` & `siriuspy-2.78.0/siriuspy/epics/properties.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/epics/pv_fake.py` & `siriuspy-2.78.0/siriuspy/epics/pv_fake.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/epics/pv_time_serie.py` & `siriuspy-2.78.0/siriuspy/epics/pv_time_serie.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/fofb/csdev.py` & `siriuspy-2.78.0/siriuspy/fofb/csdev.py`

 * *Files 10% similar despite different names*

```diff
@@ -240,45 +240,27 @@
             'CtrlrSyncTFrameLen-Cmd': {'type': 'int', 'value': 0},
             'CtrlrConfBPMLogTrg-Cmd': {'type': 'int', 'value': 0},
             'CtrlrSyncMaxOrbDist-Cmd': {'type': 'int', 'value': 0},
             'CtrlrSyncPacketLossDetec-Cmd': {'type': 'int', 'value': 0},
             'CtrlrReset-Cmd': {'type': 'int', 'value': 0},
             'CtrlrDsblSYSIDExc-Cmd': {'type': 'int', 'value': 0},
 
-            # Kicks and decimation configuration
+            # decimation configuration
             'FOFBAccDecimation-Sel': {
                 'type': 'enum', 'enums': _et.DEC_OPT,
                 'value': self.DecOpt.FOFB, 'unit': 'FOFB_Monit_Custom'},
             'FOFBAccDecimation-Sts': {
                 'type': 'enum', 'enums': _et.DEC_OPT,
                 'value': self.DecOpt.FOFB, 'unit': 'FOFB_Monit_Custom'},
             'FOFBAccDecimation-SP': {
                 'type': 'float', 'value': 1, 'prec': 0, 'lolim': 1,
                 'hilim': 8600, 'unit': 'count'},
             'FOFBAccDecimation-RB': {
                 'type': 'float', 'value': 1, 'prec': 0, 'lolim': 1,
                 'hilim': 8600, 'unit': 'count'},
-            'KickCHAcc-Mon': {
-                'type': 'float', 'unit': 'urad', 'count': self.nr_ch,
-                'value': self.nr_ch*[0]},
-            'KickCVAcc-Mon': {
-                'type': 'float', 'unit': 'urad', 'count': self.nr_cv,
-                'value': self.nr_cv*[0]},
-            'KickCHRef-Mon': {
-                'type': 'float', 'unit': 'urad', 'count': self.nr_ch,
-                'value': self.nr_ch*[0]},
-            'KickCVRef-Mon': {
-                'type': 'float', 'unit': 'urad', 'count': self.nr_cv,
-                'value': self.nr_cv*[0]},
-            'KickCH-Mon': {
-                'type': 'float', 'unit': 'urad', 'count': self.nr_ch,
-                'value': self.nr_ch*[0]},
-            'KickCV-Mon': {
-                'type': 'float', 'unit': 'urad', 'count': self.nr_cv,
-                'value': self.nr_cv*[0]},
 
             # Reference Orbit (same order of SOFB)
             'RefOrbX-SP': {
                 'type': 'float', 'unit': 'um', 'count': self.nr_bpms,
                 'value': self.nr_bpms*[0]},
             'RefOrbX-RB': {
                 'type': 'float', 'unit': 'um', 'count': self.nr_bpms,
```

### Comparing `siriuspy-2.77.0/siriuspy/fofb/main.py` & `siriuspy-2.78.0/siriuspy/fofb/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,30 +90,14 @@
 
         # devices and connections
         self._sisofb_dev = _SOFB(_SOFB.DEVICES.SI)
 
         corrnames = self._const.ch_names + self._const.cv_names
         self._corrs_dev = _FamFastCorrs(corrnames)
 
-        self._propty2kickpvs = {
-            'FOFBAcc-Mon': ['KickCHAcc-Mon', 'KickCVAcc-Mon'],
-            'CurrentRef-Mon': ['KickCHRef-Mon', 'KickCVRef-Mon'],
-            'Current-Mon': ['KickCH-Mon', 'KickCV-Mon'],
-        }
-        self._kick_mon = {}
-        size = len(self._corrs_dev.psdevs)
-        for propty in self._propty2kickpvs:
-            self._kick_mon[propty] = _np.zeros(size, dtype=float)
-            for idx, pso in enumerate(self._corrs_dev.psdevs):
-                pvo = pso.pv_object(propty)
-                pvo.set_auto_monitor(True)
-                pvo.add_callback(
-                    _part(self._update_kick_array, ps_index=idx),
-                    with_ctrlvars=False)
-
         self._rf_dev = _RFGen()
 
         self._llfofb_dev = _FamFOFBCtrls()
 
         self._intlk_pvs = list()
         self._intlk_values = dict()
         for dev in self._llfofb_dev.ctrlrefdevs.values():
@@ -194,16 +178,14 @@
         self.thread_check_corrs_configs.start()
         self.thread_check_ctrls_configs = _epics.ca.CAThread(
             target=self._check_ctrls_configs, daemon=True)
         self.thread_check_ctrls_configs.start()
 
     def init_database(self):
         """Set initial PV values."""
-        initkickch = _np.zeros(self._const.nr_ch, dtype=float)
-        initkickcv = _np.zeros(self._const.nr_cv, dtype=float)
         pvn2vals = {
             'LoopState-Sel': self._loop_state,
             'LoopState-Sts': self._loop_state,
             'LoopGainH-SP': self._loop_gain_h,
             'LoopGainH-RB': self._loop_gain_h,
             'LoopGainH-Mon': self._loop_gain_mon_h,
             'LoopGainV-SP': self._loop_gain_v,
@@ -244,20 +226,14 @@
             'CtrlrSyncPacketLossDetec-Cmd': 0,
             'CtrlrReset-Cmd': 0,
             'CtrlrDsblSYSIDExc-Cmd': 0,
             'FOFBAccDecimation-Sel': self._corr_accdec_enm,
             'FOFBAccDecimation-Sts': self._corr_accdec_enm,
             'FOFBAccDecimation-SP': self._corr_accdec_val,
             'FOFBAccDecimation-RB': self._corr_accdec_val,
-            'KickCHAcc-Mon': initkickch,
-            'KickCVAcc-Mon': initkickcv,
-            'KickCHRef-Mon': initkickch,
-            'KickCVRef-Mon': initkickcv,
-            'KickCH-Mon': initkickch,
-            'KickCV-Mon': initkickcv,
             'MinSingValue-SP': self._min_sing_val,
             'MinSingValue-RB': self._min_sing_val,
             'TikhonovRegConst-SP': self._tikhonov_reg_const,
             'TikhonovRegConst-RB': self._tikhonov_reg_const,
             'InvRespMatNormMode-Sel': self._invrespmat_normmode,
             'InvRespMatNormMode-Sts': self._invrespmat_normmode,
             'MeasRespMat-Cmd': 0,
@@ -305,20 +281,15 @@
     @property
     def pvs_database(self):
         """Return pvs_database."""
         return self._pvs_database
 
     def process(self, interval):
         """Sleep."""
-        t0_ = _time.time()
-        self._update_kicks()
-
-        dtime = interval - (_time.time()-t0_)
-        if dtime > 0:
-            _time.sleep(dtime)
+        _time.sleep(interval)
 
     def read(self, reason):
         """Read from IOC database."""
         value = None
         return value
 
     def write(self, reason, value):
@@ -962,37 +933,14 @@
         if not self._check_fofbctrl_connection():
             return False
         self._update_log('Disabling SYSID excitation...')
         self._llfofb_dev.cmd_dsbl_sysid_exc()
         self._update_log('...done!')
         return True
 
-    # --- kicks update ---
-
-    def _update_kick_array(self, pvname, value, ps_index, **kwargs):
-        _ = kwargs
-        if value is None:
-            return
-        val = self._corrs_dev.psconvs[ps_index].conv_current_2_strength(value)
-        if val is None:
-            return
-        propty = _PVName(pvname).propty
-        self._kick_mon[propty][ps_index] = val
-
-    def _update_kicks(self):
-        nrch, nrcv = self._const.nr_ch, self._const.nr_cv
-
-        for propty, kickpvs in self._propty2kickpvs.items():
-            kicks = self._kick_mon[propty]
-            kickch = kicks[:nrch]
-            kickcv = kicks[nrch:nrch+nrcv]
-
-            self.run_callbacks(kickpvs[0], kickch)
-            self.run_callbacks(kickpvs[1], kickcv)
-
     # --- reference orbit ---
 
     def set_reforbit(self, plane, value):
         """Set reference orbit."""
         self._update_log(f'Setting New RefOrb{plane.upper()}...')
 
         # check size
```

### Comparing `siriuspy-2.77.0/siriuspy/idff/config.py` & `siriuspy-2.78.0/siriuspy/idff/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,35 +7,28 @@
 from ..search import IDSearch as _IDSearch
 from ..clientconfigdb import ConfigDBDocument as _ConfigDBDocument
 
 
 class IDFFConfig(_ConfigDBDocument):
     """Insertion Device Feedforward Configuration."""
 
+    # NOTE: for EPU50 there is a large discrepancy
+    # between RB/SP/Mon phase values
+    PPARAM_TOL = 0.5  # [mm]
+    KPARAM_TOL = 0.1  # [mm]
     CONFIGDB_TYPE = 'si_idff'
 
     def __init__(self, name=None, url=None):
         """."""
         name_ = name or 'idff_' + self.generate_config_name()
         self._polarization_definitions = None
         super().__init__(
             config_type=IDFFConfig.CONFIGDB_TYPE, name=name_, url=url)
 
     @property
-    def name(self):
-        """Return configuration name."""
-        return self._name
-
-    @name.setter
-    def name(self, value):
-        """Set configuration name."""
-        if self.configdbclient.check_valid_configname(value):
-            self._name = value
-
-    @property
     def pparameter_pvname(self):
         """Return ID pparameter pvname."""
         config = self._value
         if config:
             kparm = config['pvnames']['pparameter']
             return kparm
         else:
@@ -171,25 +164,23 @@
     def load(self, discarded=False):
         """."""
         super().load(discarded=discarded)
         self._calc_polariz_defs()
 
     def get_polarization_state(self, pparameter, kparameter):
         """Return polarization state based on ID parameteres."""
-        PPARAM_TOL = 0.1
-        KPARAM_TOL = 0.1
         poldefs = self._polarization_definitions
         if poldefs is None:
             raise ValueError('No IDFF configuration defined.')
         for pol, val in poldefs.items():
             if pol == 'none':
                 continue
-            if val is None or abs(pparameter - val) < PPARAM_TOL:
+            if val is None or abs(pparameter - val) < IDFFConfig.PPARAM_TOL:
                 return pol
-        if abs(kparameter - poldefs['none']) < KPARAM_TOL:
+        if abs(kparameter - poldefs['none']) < IDFFConfig.KPARAM_TOL:
             return 'none'
         return 'not_defined'
 
     def check_valid_value(self, value):
         """."""
         if not super().check_valid_value(value):
             return False
```

### Comparing `siriuspy-2.77.0/siriuspy/idff/csdev.py` & `siriuspy-2.78.0/siriuspy/idff/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/idff/main.py` & `siriuspy-2.78.0/siriuspy/idff/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             'Polarization-Mon': self._polarization,
             'SOFBMode-Sel': self._pssofb_isused,
             'SOFBMode-Sts': self._pssofb_isused,
             'CorrConfig-Cmd': 0,
             'CorrStatus-Mon': 0b1111,
         }
         if self._const.has_qscorrs:
-            pvn2vals.ipdate({
+            pvn2vals.update({
                 'ControlQS-Sel': self._control_qs,
                 'ControlQS-Sts': self._control_qs,
                 })
         for pvn, val in pvn2vals.items():
             self.run_callbacks(pvn, val)
         self._update_log('Started.')
 
@@ -158,14 +158,15 @@
             self._update_log('ERR:Open loop before changing configuration.')
             return False
 
         if not self._load_config(value):
             return False
 
         self._config_name = value
+        self.update_autosave_file()
         self.run_callbacks('ConfigName-RB', value)
         return True
 
     def set_sofb_mode(self, value):
         """Set whether to use SOFBMode."""
         if not 0 <= value < len(_ETypes.DSBL_ENBL):
             return False
@@ -306,15 +307,16 @@
             # print()
             if self._pssofb_isused:
                 # calc setpoints
                 ret = self._idff.calculate_setpoints()
                 setpoints, *_ = ret
 
                 # built curr_sp vector
-                curr_sp = self._pssfob_current_setpoint(setpoints, corrdevs)
+                curr_sp = self._pssfob_get_current_setpoint(
+                    setpoints, corrdevs)
 
                 # apply curr_sp to pssofb
                 self._pssofb.bsmp_sofb_current_set_update((curr_sp, ))
             else:
                 # use PS IOCs (IDFF) to implement setpoints
                 self._idff.implement_setpoints(corrdevs=corrdevs)
```

### Comparing `siriuspy-2.77.0/siriuspy/injctrl/bias_feedback.py` & `siriuspy-2.78.0/siriuspy/injctrl/bias_feedback.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/injctrl/csdev.py` & `siriuspy-2.78.0/siriuspy/injctrl/csdev.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,16 @@
     MAX_INJTIMEOUT = 3*60  # [s]
 
     BIAS_SINGLE_BUNCH = -100.0  # [V]
     BIAS_MULTI_BUNCH = -56.0  # [V]
     FILACURR_OPVALUE = 1.39  # [A]
     HV_OPVALUE = 90.0  # [kV]
 
-    INJSYS_DEF_ON_ORDER = ['bo_rf', 'as_pu', 'bo_ps', 'injbo', 'li_rf']
-    INJSYS_DEF_OFF_ORDER = ['bo_rf', 'li_rf', 'injbo', 'as_pu', 'bo_ps']
+    INJSYS_DEF_ON_ORDER = ['bo_rf', 'as_pu', 'bo_ps', 'li_rf']
+    INJSYS_DEF_OFF_ORDER = ['bo_rf', 'li_rf', 'as_pu', 'bo_ps']
 
     BIASFB_AHEADSETIME = 10  # [s]
     BIASFB_MINIMUM_LIFETIME = 1800  # [s]
     BIASFB_PROPTY_PREFIX = 'BiasFB'
     BIASFB_MAX_DATA_SIZE = 1000
 
 
@@ -118,18 +118,18 @@
 
     dbase = {
         'Version-Cte': {'type': 'str', 'value': 'UNDEF'},
         'Log-Mon': {'type': 'str', 'value': 'Starting...'},
 
         'Mode-Sel': {
             'type': 'enum', 'value': _ct.InjMode.Decay,
-            'enums': _et.INJMODE, 'unit': 'Decay_Topup'},
+            'enums': _et.INJMODE, 'unit': 'Decay_Topup_Accum'},
         'Mode-Sts': {
             'type': 'enum', 'value': _ct.InjMode.Decay,
-            'enums': _et.INJMODE, 'unit': 'Decay_Topup'},
+            'enums': _et.INJMODE, 'unit': 'Decay_Topup_Accum'},
         'Type-Sel': {
             'type': 'enum', 'value': _ct.InjType.MultiBunch,
             'enums': _et.INJTYPE, 'unit': 'SB_MB'},
         'Type-Sts': {
             'type': 'enum', 'value': _ct.InjType.MultiBunch,
             'enums': _et.INJTYPE, 'unit': 'SB_MB'},
         'Type-Mon': {
```

### Comparing `siriuspy-2.77.0/siriuspy/injctrl/main.py` & `siriuspy-2.78.0/siriuspy/injctrl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from ..callbacks import Callback as _Callback
 from ..clientarch import Time as _Time
 
 from ..search import PSSearch as _PSSearch, HLTimeSearch as _HLTimeSearch
 from ..diagsys.lidiag.csdev import Const as _LIDiagConst, ETypes as _LIDiagEnum
 from ..diagsys.psdiag.csdev import ETypes as _PSDiagEnum
 from ..diagsys.rfdiag.csdev import Const as _RFDiagConst
-from ..devices import InjSysStandbyHandler, EVG, EGun, CurrInfoSI, \
-    PowerSupplyPU, RFKillBeam, InjSysPUModeHandler, Trigger, HLTiming
+from ..devices import InjSysStandbyHandler, EVG, EGun, CurrInfoSI, HLTiming, \
+    RFKillBeam, InjSysPUModeHandler
 
 from .csdev import Const as _Const, ETypes as _ETypes, \
     get_injctrl_propty_database as _get_database, \
     get_status_labels as _get_sts_lbls
 from .bias_feedback import BiasFeedback as _BiasFeedback
 
 
@@ -144,14 +144,17 @@
                     for n in _LIDiagConst.DEV_2_LINAME if 'EG' in n}
 
             if sec in ['BO', 'SI']:
                 self._pvs_diag[sec]['RF'] = {
                     n: _PV(n+':DiagStatus-Mon', connection_timeout=0.05)
                     for n in _RFDiagConst.ALL_DEVICES if n.startswith(sec)}
 
+        # Timing device
+        self._hlti_dev = HLTiming()
+
         # auxiliary injsys PVs
         self._pvs_injsys = dict()
         punames = _PSSearch.get_psnames({
             'sec': '(SI|TS)', 'dev': 'Inj(Sept.*|NLKckr)',
             'propty_name': '(?!:CCoil).*'})
         for pun in punames:
             pv_pulse = _PV(pun+':Pulse-Sts', connection_timeout=0.05)
@@ -166,58 +169,43 @@
         self.egun_dev = EGun(
             print_log=False, callback=self._update_dev_status)
         self._init_egun = False
         self.egun_dev.trigps.pv_object('enable').add_callback(
             self._callback_watch_eguntrig)
 
         self._pumode_dev = InjSysPUModeHandler(
-            print_log=False, callback=self._update_dev_status)
+            print_log=False, callback=self._update_dev_status,
+            hltiming=self._hlti_dev)
 
         self._evg_dev = EVG()
         self._init_injevt = False
         self._evg_dev.pv_object('InjectionEvt-Sel').add_callback(
             self._callback_watch_injectionevt)
         self._evg_dev.set_auto_monitor('TotalInjCount-Mon', True)
         self._evg_dev.pv_object('TotalInjCount-Mon').add_callback(
             self._callback_is_injecting)
 
-        self._injsys_dev = InjSysStandbyHandler()
+        self._injsys_dev = InjSysStandbyHandler(hltiming=self._hlti_dev)
 
         self.currinfo_dev = CurrInfoSI()
         self.currinfo_dev.set_auto_monitor('Current-Mon', True)
         curr_pvo = self.currinfo_dev.pv_object('Current-Mon')
         curr_pvo.add_callback(self._callback_autostop)
         curr_pvo.connection_callbacks.append(self._callback_conn_autostop)
 
-        self._pu_names = _PSSearch.get_psnames({
-            'dis': 'PU', 'dev': '.*(InjKckr|EjeKckr|InjNLKckr|Sept)',
-            'propty_name': '(?!:CCoil).*'})
-        self._pu_devs = [PowerSupplyPU(pun) for pun in self._pu_names]
+        self._pu_names = self._injsys_dev.handlers['as_pu'].punames
+        self._pu_devs = self._injsys_dev.handlers['as_pu'].pudevices
         self._pu_refvolt = list()
         for dev in self._pu_devs:
             pvo = dev.pv_object('Voltage-SP')
             self._pu_refvolt.append(pvo.value)
             pvo.add_callback(self._callback_update_pu_refvolt)
 
         self._rfkillbeam = RFKillBeam()
 
-        self._li_trig_names = _HLTimeSearch.get_hl_triggers(
-            {'sec': 'LI', 'dev': '(Mod|LLRF|SSAmp|Osc)'})
-        self._li_trig_devs = [Trigger(tin) for tin in self._li_trig_names]
-
-        self._bops_trig_names = _HLTimeSearch.get_hl_triggers(
-            {'sec': 'BO', 'dev': 'Mags'})
-        self._bops_trig_devs = [Trigger(tin) for tin in self._bops_trig_names]
-
-        self._borf_trig_names = _HLTimeSearch.get_hl_triggers(
-            {'sec': 'BO', 'dev': 'LLRF', 'idx': 'Rmp'})
-        self._borf_trig_devs = [Trigger(tin) for tin in self._borf_trig_names]
-
-        self._hlti_dev = HLTiming()
-
         # pvname to write method map
         self.map_pv2write = {
             'Mode-Sel': self.set_mode,
             'Type-Sel': self.set_type,
             'SglBunBiasVolt-SP': self.set_sglbunbiasvolt,
             'MultBunBiasVolt-SP': self.set_multbunbiasvolt,
             'FilaOpCurr-SP': self.set_filaopcurr,
@@ -451,14 +439,20 @@
         if self._accum_job and self._accum_job.is_alive():
             self._setting_mode = True
             self._stop_accum_job()
             self._setting_mode = False
 
         if value != _Const.InjMode.Decay:
             stg = 'top-up' if value == _Const.InjMode.TopUp else 'accumulation'
+
+            if self._pumode != _Const.PUMode.Accumulation:
+                self._update_log('ERR:Set PUMode to Accumulation before')
+                self._update_log('ERR:changing mode to {stg}')
+                return False
+
             self._update_log('Configuring EVG RepeatBucketList...')
             self._evg_dev['RepeatBucketList-SP'] = 1
             self._update_log(f'...done. Ready to start {stg:s}.')
 
         self._mode = value
         self.run_callbacks('Mode-Sts', self._mode)
         return True
@@ -572,16 +566,14 @@
         return True
 
     def set_pumode(self, value):
         """Set PU mode."""
         if not 0 <= value < len(_ETypes.PUMODE):
             return False
         if self._mode != _Const.InjMode.Decay:
-            topup = _Const.InjMode.TopUp
-            stg = 'top-up' if self._mode == topup else 'accumulation'
             self._update_log(
                 f'ERR:PUMode can only be changed in Decay mode.')
             return False
         if self._p2w['PUMode']['watcher'] is not None and \
                 self._p2w['PUMode']['watcher'].is_alive():
             self._update_log('WARN:Interrupting PUMode change command')
             self._pumode_dev.cmd_abort()
@@ -632,28 +624,28 @@
 
     def set_bucketlist_start(self, start):
         """Set bucketlist_start."""
         if not _Const.MIN_BKT <= start <= _Const.MAX_BKT:
             return False
         stop = self._bucketlist_stop
         step = self._bucketlist_step
-        if self._mode == _Const.InjMode.TopUp:
+        if self._mode == _Const.InjMode.Decay:
             if not self._cmd_bucketlist_fill(stop, start, step):
                 return False
         self._bucketlist_start = start
         self.run_callbacks('BucketListStart-RB', start)
         return True
 
     def set_bucketlist_stop(self, stop):
         """Set bucketlist_stop."""
         if not _Const.MIN_BKT <= stop <= _Const.MAX_BKT:
             return False
         start = self._bucketlist_start
         step = self._bucketlist_step
-        if self._mode == _Const.InjMode.TopUp:
+        if self._mode == _Const.InjMode.Decay:
             if not self._cmd_bucketlist_fill(stop, start, step):
                 return False
         self._bucketlist_stop = stop
         self.run_callbacks('BucketListStop-RB', stop)
         return True
 
     def set_bucketlist_step(self, step):
@@ -932,20 +924,24 @@
         while _time.time() - _t0 < timeout:
             if not self._injsys_dev.is_running:
                 break
             _time.sleep(0.1)
             self.run_callbacks(
                 'InjSysCmdDone-Mon', ','.join(self._injsys_dev.done))
         self.run_callbacks('InjSysCmdSts-Mon', _Const.InjSysCmdSts.Idle)
+
+        is_running = self._injsys_dev.is_running
         ret = self._injsys_dev.result
-        if ret is None:
-            msg = 'ERR:Timed out in turn '+cmd+' Inj.System.'
+        if is_running:
+            self._update_log('ERR:Timed out in turn '+cmd+' Inj.System.')
+            self._injsys_dev.cmd_abort()
         elif not ret[0]:
             self._update_log('ERR:Failed to turn '+cmd+' Inj.System.')
-            msgs = [ret[1][i:i+35] for i in range(0, len(ret[1]), 35)]
+            msgs = ret[1].split('\n')
+            msgs = [m[i:i+35] for m in msgs for i in range(0, len(m), 35)]
             for msg in msgs:
                 self._update_log('ERR:'+msg)
             self._update_log('ERR:Detail list: ')
             for item in ret[2]:
                 self._update_log('ERR:'+item)
         else:
             msg = 'Turned '+cmd+' Inj.System.'
@@ -1513,37 +1509,43 @@
         self._update_log('...done.')
 
     def _handle_liti_warmup_state(self, state):
         if self._liti_warmup_state == state:
             return
         self._liti_warmup_state = state
 
-        event = 'RmpBO' if state == _Const.StandbyInject.Inject else 'Linac'
-        self._hlti_dev.change_triggers_source(
-            self._li_trig_names, new_src=event, printlog=False)
+        lirf = self._injsys_dev.handlers['li_rf']
+        if state == _Const.StandbyInject.Inject:
+            lirf.change_trigs_to_rmpbo_evt()
+        else:
+            lirf.change_trigs_to_linac_evt()
         self._update_log('LI timing configured.')
 
     def _handle_bops_standby_state(self, state):
         if self._bops_standby_state == state:
             return
         self._bops_standby_state = state
 
-        trigstate = int(state == _Const.StandbyInject.Inject)
-        for trig in self._bops_trig_devs:
-            trig.state = trigstate
+        bops = self._injsys_dev.handlers['bo_ps']
+        if state == _Const.StandbyInject.Inject:
+            bops.enable_triggers()
+        else:
+            bops.disable_triggers()
         self._update_log('BO PS timing configured.')
 
     def _handle_borf_standby_state(self, state):
         if self._borf_standby_state == state:
             return
         self._borf_standby_state = state
 
-        trigstate = int(state == _Const.StandbyInject.Inject)
-        for trig in self._borf_trig_devs:
-            trig.state = trigstate
+        borf = self._injsys_dev.handlers['bo_rf']
+        if state == _Const.StandbyInject.Inject:
+            borf.enable_triggers()
+        else:
+            borf.disable_triggers()
         self._update_log('BO RF timing configured.')
 
     # --- auxiliary log methods ---
 
     def _launch_watch_dev_thread(self):
         if self._thread_watdev is None or not self._thread_watdev.is_alive():
             self._thread_watdev = _epics.ca.CAThread(
```

### Comparing `siriuspy-2.77.0/siriuspy/machshift/csdev.py` & `siriuspy-2.78.0/siriuspy/machshift/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/machshift/gensumm_macreport.py` & `siriuspy-2.78.0/siriuspy/machshift/gensumm_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/machshift/macreport.py` & `siriuspy-2.78.0/siriuspy/machshift/macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/machshift/macschedule.py` & `siriuspy-2.78.0/siriuspy/machshift/macschedule.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/machshift/main.py` & `siriuspy-2.78.0/siriuspy/machshift/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/machshift/savedata_macreport.py` & `siriuspy-2.78.0/siriuspy/machshift/savedata_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/machshift/utils.py` & `siriuspy-2.78.0/siriuspy/machshift/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/magnet/data.py` & `siriuspy-2.78.0/siriuspy/magnet/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/magnet/excdata.py` & `siriuspy-2.78.0/siriuspy/magnet/excdata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/magnet/factory.py` & `siriuspy-2.78.0/siriuspy/magnet/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/magnet/normalizer.py` & `siriuspy-2.78.0/siriuspy/magnet/normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/magnet/util.py` & `siriuspy-2.78.0/siriuspy/magnet/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/meas/csdev.py` & `siriuspy-2.78.0/siriuspy/meas/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/meas/liemit/csdev.py` & `siriuspy-2.78.0/siriuspy/meas/liemit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/meas/liemit/main.py` & `siriuspy-2.78.0/siriuspy/meas/liemit/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/meas/lienergy/csdev.py` & `siriuspy-2.78.0/siriuspy/meas/lienergy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/meas/lienergy/main.py` & `siriuspy-2.78.0/siriuspy/meas/lienergy/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/meas/util.py` & `siriuspy-2.78.0/siriuspy/meas/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/namesys/implementation.py` & `siriuspy-2.78.0/siriuspy/namesys/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/optics/lattice_survey.py` & `siriuspy-2.78.0/siriuspy/optics/lattice_survey.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/opticscorr/base.py` & `siriuspy-2.78.0/siriuspy/opticscorr/base.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/opticscorr/chrom.py` & `siriuspy-2.78.0/siriuspy/opticscorr/chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/opticscorr/csdev.py` & `siriuspy-2.78.0/siriuspy/opticscorr/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/opticscorr/opticscorr.py` & `siriuspy-2.78.0/siriuspy/opticscorr/opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/opticscorr/tune.py` & `siriuspy-2.78.0/siriuspy/opticscorr/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/opticscorr/utils.py` & `siriuspy-2.78.0/siriuspy/opticscorr/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/oscilloscope/keysight.py` & `siriuspy-2.78.0/siriuspy/oscilloscope/keysight.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     print(scope.scope_name)
     wavet, waved = scope.wfm_get_data()
     plt.plot(wavet, waved)
     plt.show()
 
     """
 
+    SOCKET_TIMEOUT = 10  # [s]
+
     def __init__(self, scope=None, scopesignal=None):
         """."""
         if scopesignal and isinstance(scopesignal, tuple):
             self.host = scopesignal[0]
             self.port = scopesignal[1]
             self.chan = scopesignal[2]
         elif scope and isinstance(scope, str):
@@ -52,34 +54,37 @@
         return _scopes.ScopeSignals.get_scope_name(self.host)
 
     def connect(self):
         """."""
         self._socket = _socket.socket(
             _socket.AF_INET,  # Internet
             _socket.SOCK_STREAM)  # TCP
-        self._socket.settimeout(10)
+        self._socket.settimeout(Keysight.SOCKET_TIMEOUT)
         self._socket.connect((self.host, self.port))
 
     def close(self):
         """."""
         self._socket.close()
 
     def wfm_enable(self):
         """Enable scope waveform acquisition."""
         return self.send_command(b'*IDN?\r\n')
 
-    def wfm_config(self):
+    def wfm_config(self, wait_trigger=False):
         """Set scope waveform format."""
         self.send_command(b":WAVeform:FORMat WORD\n", get_res=False)
         dataformat = self.send_command(b":WAVeform:FORMat?\n")
         print('Data format:', dataformat)
         # Set bit order to MSB First
         self.send_command(b":WAVeform:BYTeorder MSBF\n", get_res=False)
         # Acquire
-        self.send_command(b':DIG\n', get_res=False)
+        if wait_trigger:
+            self.send_command(b':DIG\n', get_res=False)
+        else:
+            self.send_command(b':RUN\n', get_res=False)
 
     def wfm_acquire(self, channel):
         """Acquire scope waveform."""
         if isinstance(channel, tuple):
             channel = channel[2]
 
         # Get the number of waveform points
@@ -98,17 +103,20 @@
         self.send_command(
             b":WAVeform:SOURce " + channel.encode('ascii')+b"\n",
             get_res=False)
         channel = self.send_command(b":WAVeform:SOURce?\n")
 
         # Get scales
         xinc = self.send_command(b":WAVeform:XINCrement?\n")
+        xinc = float(xinc)
         print('Horizontal Scale:', xinc)
         yinc = self.send_command(b":WAVeform:YINCrement?\n")
         yor = self.send_command(b":WAVeform:YORigin?\n")
+        yinc = float(yinc)
+        yor = float(yor)
         print('Vertical Scale:', xinc, yor)
 
         # Data aquisition
         self.send_command(b":WAVeform:STReaming OFF\n", get_res=False)
         self.send_command(b":WAVeform:DATA?\n", get_res=False)
         _ = self._socket.recv(1)  # ignore marker '#'
         num = int(self._socket.recv(1).decode('ascii'))
@@ -125,23 +133,23 @@
         va0 = _np.array(list(dataraw)[1::2])
 
         datay = ((va1 << 8) + va0 - 2**16*(va1 >> 7)) * yinc + yor
 
         datax = _np.arange(datay.size)*xinc
         return datax, datay, srate, bdw
 
-    def wfm_get_data(self, channel=None):
+    def wfm_get_data(self, channel=None, wait_trigger=False):
         """Enable and get sccope waveform data."""
         channel = channel or self.chan
         self.connect()
         wavet = None
         waved = None
         try:
             self.wfm_enable()
-            self.wfm_config()
+            self.wfm_config(wait_trigger)
             tini = _time.time()
             print('Acquiring ' + self.chan)
             wavet, waved, srate1, bdw1 = self.wfm_acquire(channel)
             print('Total acquisition time:', _time.time() - tini)
             # self.send_command(b":WAVeform:STReaming ON\n", get_res=False)
         except Exception:
             print('Close connection by exception')
```

### Comparing `siriuspy-2.77.0/siriuspy/oscilloscope/scopes.py` & `siriuspy-2.78.0/siriuspy/oscilloscope/scopes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/posang/csdev.py` & `siriuspy-2.78.0/siriuspy/posang/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/posang/main.py` & `siriuspy-2.78.0/siriuspy/posang/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/posang/utils.py` & `siriuspy-2.78.0/siriuspy/posang/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/beaglebone.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/beaglebone.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/commands.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/constants.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/entities.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/factory.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/bsmp/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/csdev.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/csdev.py`

 * *Files 0% similar despite different names*

```diff
@@ -877,15 +877,15 @@
 def get_ps_propty_database(psmodel=None, pstype=None, psname=None):
     """Return epics properties database for a power supply model and type."""
     # in case psname is given
     if psname is not None:
         psmodel = _PSSearch.conv_psname_2_psmodel(psname)
         pstype = _PSSearch.conv_psname_2_pstype(psname)
 
-    # get dbase for a psecific psmodel
+    # get dbase for a specific psmodel
     dbase = _get_model_db(psmodel)
 
     # insert corresponding strengths
     dbase = _insert_strengths(dbase, pstype)
 
     # update limits
     _set_limits(pstype, dbase)
@@ -3136,9 +3136,12 @@
     if pstype.startswith('li-'):
         if 'KickRef-Mon' in database:
             del database['KickRef-Mon']
         if 'KLRef-Mon' in database:
             del database['KLRef-Mon']
         if 'SLRef-Mon' in database:
             del database['SLRef-Mon']
+    elif '-fc' in pstype:
+        database['KickAcc-Mon'] = {
+            'type': 'float', 'value': 0.0, 'prec': prec_kick, 'unit': 'urad'}
 
     return database
```

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/data.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/factory.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/__init__.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/pru.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/prucontroller.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/prucontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/prucparms.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/prucparms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/psdevstate.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/psdevstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/udc.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/pructrl/udc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/__init__.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscontroller.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscreaders.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscreaders.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscstatus.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscstatus.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscwriters.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/psmodel.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/psctrl/psmodel.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/pssofb.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/pwrsupply/siggen.py` & `siriuspy-2.78.0/siriuspy/pwrsupply/siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/ramp/conn.py` & `siriuspy-2.78.0/siriuspy/ramp/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/ramp/magnet.py` & `siriuspy-2.78.0/siriuspy/ramp/magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/ramp/ramp.py` & `siriuspy-2.78.0/siriuspy/ramp/ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/ramp/reconst_factory.py` & `siriuspy-2.78.0/siriuspy/ramp/reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/ramp/test_reconst_factory.py` & `siriuspy-2.78.0/siriuspy/ramp/test_reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/ramp/testwfm.py` & `siriuspy-2.78.0/siriuspy/ramp/testwfm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/ramp/util.py` & `siriuspy-2.78.0/siriuspy/ramp/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/ramp/waveform.py` & `siriuspy-2.78.0/siriuspy/ramp/waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/search/bpms_search.py` & `siriuspy-2.78.0/siriuspy/search/bpms_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/search/hl_time_search.py` & `siriuspy-2.78.0/siriuspy/search/hl_time_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     def get_ll_trigger_names(cls, hl_trigger):
         """Get Low Level trigger object names."""
         cls._init()
         return sorted(cls._hl2ll_trigs.get(hl_trigger, list()))
 
     @classmethod
     def get_hl_from_ll_triggers(cls, channel):
+        cls._init()
         # channel = _LLSearch.get_channel_output_port_pvname(channel)
         prpt = channel.propty
         if prpt.startswith('OTP'):
             val = int(prpt[3:]) - 12
             newprpt = 'OUT'+str(val) if 0 <= val < 8 else 'OTP'+str(val+12)
             channel = channel.substitute(propty=newprpt)
         return cls._ll2hl_trigs.get(channel, '')
```

### Comparing `siriuspy-2.77.0/siriuspy/search/id_search.py` & `siriuspy-2.78.0/siriuspy/search/id_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/search/ioc_search.py` & `siriuspy-2.78.0/siriuspy/search/ioc_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/search/ll_time_search.py` & `siriuspy-2.78.0/siriuspy/search/ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/search/ma_search.py` & `siriuspy-2.78.0/siriuspy/search/ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/search/ps_search.py` & `siriuspy-2.78.0/siriuspy/search/ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/simul/simfactory.py` & `siriuspy-2.78.0/siriuspy/simul/simfactory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/simul/simps.py` & `siriuspy-2.78.0/siriuspy/simul/simps.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/simul/simpv.py` & `siriuspy-2.78.0/siriuspy/simul/simpv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/simul/simulation.py` & `siriuspy-2.78.0/siriuspy/simul/simulation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/simul/simulator.py` & `siriuspy-2.78.0/siriuspy/simul/simulator.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/sofb/base_class.py` & `siriuspy-2.78.0/siriuspy/sofb/base_class.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/sofb/bpms.py` & `siriuspy-2.78.0/siriuspy/sofb/bpms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/sofb/correctors.py` & `siriuspy-2.78.0/siriuspy/sofb/correctors.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/sofb/csdev.py` & `siriuspy-2.78.0/siriuspy/sofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/sofb/main.py` & `siriuspy-2.78.0/siriuspy/sofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/sofb/matrix.py` & `siriuspy-2.78.0/siriuspy/sofb/matrix.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/sofb/orbit.py` & `siriuspy-2.78.0/siriuspy/sofb/orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/sofb/utils.py` & `siriuspy-2.78.0/siriuspy/sofb/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/stabinfo/csdev.py` & `siriuspy-2.78.0/siriuspy/stabinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/stabinfo/main.py` & `siriuspy-2.78.0/siriuspy/stabinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/thread.py` & `siriuspy-2.78.0/siriuspy/thread.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/timesys/csdev.py` & `siriuspy-2.78.0/siriuspy/timesys/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/timesys/hl_classes.py` & `siriuspy-2.78.0/siriuspy/timesys/hl_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/timesys/ll_classes.py` & `siriuspy-2.78.0/siriuspy/timesys/ll_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -674,15 +674,15 @@
             dic_ = {'Src': n, 'Evt': _TIConst.EvtLL.Evt00}
         if pname.startswith('Clock'):
             n = _TIConst.TrigSrcLL._fields.index(pname)
             n -= offset
             dic_ = {'Src': n}
         else:
             n -= offset
-            evt = int(_TIConst.EvtHL2LLMap[pname][-2:])
+            evt = int(_TIConst.EvtHL2LLMap[pname].strip('Evt'))
             dic_ = {'Src': n, 'Evt': evt}
         if 'SrcTrig' in self._dict_convert_prop2pv.keys():
             intrg = _LLSearch.get_channel_internal_trigger_pvname(
                 self.channel)
             intrg = int(intrg[-2:])  # get internal trigger number for EVR
             dic_['SrcTrig'] = intrg
         return dic_
```

### Comparing `siriuspy-2.77.0/siriuspy/timesys/plot_network.py` & `siriuspy-2.78.0/siriuspy/timesys/plot_network.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/timesys/static_table.py` & `siriuspy-2.78.0/siriuspy/timesys/static_table.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy/util.py` & `siriuspy-2.78.0/siriuspy/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/siriuspy.egg-info/PKG-INFO` & `siriuspy-2.78.0/siriuspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.77.0
+Version: 2.78.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.77.0/siriuspy.egg-info/SOURCES.txt` & `siriuspy-2.78.0/siriuspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/bsmp/test_bsmp.py` & `siriuspy-2.78.0/tests/bsmp/test_bsmp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/bsmp/test_commands.py` & `siriuspy-2.78.0/tests/bsmp/test_commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/bsmp/test_entities.py` & `siriuspy-2.78.0/tests/bsmp/test_entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/bsmp/test_serial.py` & `siriuspy-2.78.0/tests/bsmp/test_serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/bsmp/test_types.py` & `siriuspy-2.78.0/tests/bsmp/test_types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/clientconfigdb/test_configdb_client.py` & `siriuspy-2.78.0/tests/clientconfigdb/test_configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/clientweb/test_implementation.py` & `siriuspy-2.78.0/tests/clientweb/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/currinfo/lifetime/test_main.py` & `siriuspy-2.78.0/tests/currinfo/lifetime/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/currinfo/test_csdev.py` & `siriuspy-2.78.0/tests/currinfo/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/currinfo/test_main.py` & `siriuspy-2.78.0/tests/currinfo/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/magnet/test_factory.py` & `siriuspy-2.78.0/tests/magnet/test_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/magnet/tests_normalizer.py` & `siriuspy-2.78.0/tests/magnet/tests_normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/mock_servweb.py` & `siriuspy-2.78.0/tests/mock_servweb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/namesys/test_implementation.py` & `siriuspy-2.78.0/tests/namesys/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/opticscorr/test_chrom.py` & `siriuspy-2.78.0/tests/opticscorr/test_chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/opticscorr/test_csdev.py` & `siriuspy-2.78.0/tests/opticscorr/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/opticscorr/test_opticscorr.py` & `siriuspy-2.78.0/tests/opticscorr/test_opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/opticscorr/test_tune.py` & `siriuspy-2.78.0/tests/opticscorr/test_tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/opticscorr/test_utils.py` & `siriuspy-2.78.0/tests/opticscorr/test_utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/posang/test_csdev.py` & `siriuspy-2.78.0/tests/posang/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/posang/test_main.py` & `siriuspy-2.78.0/tests/posang/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/pwrsupply/db.py` & `siriuspy-2.78.0/tests/pwrsupply/db.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/pwrsupply/pructrl/test_pru.py` & `siriuspy-2.78.0/tests/pwrsupply/pructrl/test_pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/pwrsupply/psctrl/test_pscwriters.py` & `siriuspy-2.78.0/tests/pwrsupply/psctrl/test_pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/pwrsupply/test_csdev.py` & `siriuspy-2.78.0/tests/pwrsupply/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/pwrsupply/test_data.py` & `siriuspy-2.78.0/tests/pwrsupply/test_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/pwrsupply/test_siggen.py` & `siriuspy-2.78.0/tests/pwrsupply/test_siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/pwrsupply/variables.py` & `siriuspy-2.78.0/tests/pwrsupply/variables.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/ramp/test_magnet.py` & `siriuspy-2.78.0/tests/ramp/test_magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/ramp/test_waveform.py` & `siriuspy-2.78.0/tests/ramp/test_waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/search/test_hl_time_search.py` & `siriuspy-2.78.0/tests/search/test_hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/search/test_init.py` & `siriuspy-2.78.0/tests/search/test_init.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/search/test_ll_time_search.py` & `siriuspy-2.78.0/tests/search/test_ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/search/test_ma_search.py` & `siriuspy-2.78.0/tests/search/test_ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/search/test_ps_search.py` & `siriuspy-2.78.0/tests/search/test_ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/test_callbacks.py` & `siriuspy-2.78.0/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/test_csdev.py` & `siriuspy-2.78.0/tests/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/test_envars.py` & `siriuspy-2.78.0/tests/test_envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/test_util.py` & `siriuspy-2.78.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/timesys/test_csdev.py` & `siriuspy-2.78.0/tests/timesys/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.77.0/tests/timesys/test_plot_network.py` & `siriuspy-2.78.0/tests/timesys/test_plot_network.py`

 * *Files identical despite different names*

