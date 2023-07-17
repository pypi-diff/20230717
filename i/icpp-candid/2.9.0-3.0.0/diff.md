# Comparing `tmp/icpp-candid-2.9.0.tar.gz` & `tmp/icpp-candid-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icpp-candid-2.9.0.tar", last modified: Mon Jul 10 13:53:24 2023, max compression
+gzip compressed data, was "icpp-candid-3.0.0.tar", last modified: Mon Jul 17 01:01:59 2023, max compression
```

## Comparing `icpp-candid-2.9.0.tar` & `icpp-candid-3.0.0.tar`

### file list

```diff
@@ -1,177 +1,181 @@
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-10 13:53:24.940784 icpp-candid-2.9.0/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1066 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/LICENSE
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2940 2023-07-10 13:53:24.940784 icpp-candid-2.9.0/PKG-INFO
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2185 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/README.md
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      453 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/pyproject.toml
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       38 2023-07-10 13:53:24.940784 icpp-candid-2.9.0/setup.cfg
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     9759 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/setup.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-10 13:53:24.900784 icpp-candid-2.9.0/src/
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-10 13:53:24.904784 icpp-candid-2.9.0/src/icpp_candid/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      652 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/__init__.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-10 13:53:24.932784 icpp-candid-2.9.0/src/icpp_candid/candid/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     6153 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      986 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_assert.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      335 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_assert.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    13930 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_deserialize.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1392 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_deserialize.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7021 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_opcode.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2878 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_opcode.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4328 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_serialize.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1000 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_serialize.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1761 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_base.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1976 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_base.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2048 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_bool.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      626 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_bool.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1120 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_empty.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      420 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_empty.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2187 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_float32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      657 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_float32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2195 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_float64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      664 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_float64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1966 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      661 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2016 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      655 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2016 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      655 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2016 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      655 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1990 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      640 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1988 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      667 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2008 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      662 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2008 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      662 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2008 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      662 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1982 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      647 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      786 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_null.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      339 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_null.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1819 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_base.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      412 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_base.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2679 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_bool.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      804 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_bool.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2696 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_float32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      826 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_float32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2702 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_float64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      833 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_float64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2688 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      841 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2678 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      830 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2678 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      832 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2678 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      830 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2655 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      818 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2694 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      848 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2684 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      837 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2684 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      837 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2684 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      837 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2661 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      825 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2926 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_principal.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      880 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_principal.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2925 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_text.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      853 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_text.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      148 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_prim.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      484 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_prim.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     9795 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_principal.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1842 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_principal.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    10646 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_record.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1206 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_record.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1045 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_reserved.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      434 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_reserved.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2579 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_table.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      676 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_table.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2861 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_text.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      728 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_text.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    12406 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_variant.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1673 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_variant.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1819 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_base.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      412 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_base.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2485 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_bool.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      678 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_bool.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2485 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_float32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      700 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_float32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2492 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_float64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      707 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_float64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2457 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      715 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2502 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      704 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2502 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      704 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2502 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      704 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2479 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      692 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2504 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      722 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2517 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat16.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      711 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat16.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2517 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      711 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2517 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat64.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      711 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat64.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2493 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat8.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      699 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat8.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2661 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_principal.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      752 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_principal.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2724 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_text.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      727 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_text.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    15454 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/vec_bytes.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7790 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/candid/vec_bytes.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)       98 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/py.typed
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-10 13:53:24.904784 icpp-candid-2.9.0/src/icpp_candid/vendors/
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-10 13:53:24.936784 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1155 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/LICENSE
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3933 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1366 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1342 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3090 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_hex.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3143 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1336 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1381 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3070 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3201 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_url.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1805 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-10 13:53:24.936784 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/data/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    12087 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/data/access.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2352 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-10 13:53:24.940784 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7970 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/base32.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5676 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/base64.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    11905 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/codec.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1606 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/config.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4533 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/hex.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    19640 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3009 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/hex_lower.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2994 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/hex_upper.hpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3283 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/parse_error.hpp
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-10 13:53:24.940784 icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      861 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/LICENSE
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    31026 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/crc32.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1736 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/crc32.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1758 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/readme.md
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)    15133 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/sha256.cpp
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1968 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/sha256.h
--rw-r--r--   0 arjaan    (1000) arjaan    (1000)      322 2023-07-10 11:15:35.000000 icpp-candid-2.9.0/src/icpp_candid/version.py
-drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-10 13:53:24.904784 icpp-candid-2.9.0/src/icpp_candid.egg-info/
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2940 2023-07-10 13:53:24.000000 icpp-candid-2.9.0/src/icpp_candid.egg-info/PKG-INFO
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     7512 2023-07-10 13:53:24.000000 icpp-candid-2.9.0/src/icpp_candid.egg-info/SOURCES.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        1 2023-07-10 13:53:24.000000 icpp-candid-2.9.0/src/icpp_candid.egg-info/dependency_links.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       45 2023-07-10 13:53:24.000000 icpp-candid-2.9.0/src/icpp_candid.egg-info/requires.txt
--rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       12 2023-07-10 13:53:24.000000 icpp-candid-2.9.0/src/icpp_candid.egg-info/top_level.txt
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 01:01:59.835740 icpp-candid-3.0.0/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1066 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/LICENSE
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2940 2023-07-17 01:01:59.835740 icpp-candid-3.0.0/PKG-INFO
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2185 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/README.md
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      453 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/pyproject.toml
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       38 2023-07-17 01:01:59.835740 icpp-candid-3.0.0/setup.cfg
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     9863 2023-07-17 01:01:37.000000 icpp-candid-3.0.0/setup.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 01:01:59.799740 icpp-candid-3.0.0/src/
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 01:01:59.803740 icpp-candid-3.0.0/src/icpp_candid/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      652 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/__init__.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 01:01:59.827740 icpp-candid-3.0.0/src/icpp_candid/candid/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      381 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_args.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      362 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_args.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1699 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_assert.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      613 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_assert.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    14245 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_deserialize.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1071 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_deserialize.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7115 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_opcode.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2856 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_opcode.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4243 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_serialize.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      989 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_serialize.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3546 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2290 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_all_includes.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1820 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_base.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1955 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_base.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2062 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_bool.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      869 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_bool.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1163 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_empty.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      663 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_empty.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2232 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_float32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      900 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_float32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2239 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_float64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      907 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_float64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1979 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      904 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2031 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2031 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2031 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2004 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      883 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2001 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      910 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2023 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2023 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2023 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1996 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      890 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      816 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_null.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      559 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_null.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1861 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_base.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      445 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_base.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2743 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_bool.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      871 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_bool.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2763 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_float32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      896 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_float32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2769 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_float64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      903 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_float64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2751 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      907 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2744 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2743 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      900 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2743 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      898 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2719 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      885 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2757 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      914 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2749 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2749 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2749 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      905 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2725 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      892 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3030 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_principal.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      952 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_principal.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3019 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_text.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      920 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_text.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     9802 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_principal.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2032 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_principal.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    11268 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_record.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1253 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_record.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1059 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_reserved.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      677 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_reserved.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2660 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_table.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      618 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_table.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2832 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_text.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      971 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_text.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    13313 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_variant.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1720 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_variant.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1861 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_base.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      445 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_base.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2552 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_bool.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      745 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_bool.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2525 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_float32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      770 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_float32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2532 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_float64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      777 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_float64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2493 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      781 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      772 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      772 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      772 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2516 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      759 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2540 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      788 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2555 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat16.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      779 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat16.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2555 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      779 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2555 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat64.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      779 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat64.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2530 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat8.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      766 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat8.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2738 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_principal.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      824 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_principal.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2791 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_text.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      795 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_text.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    20524 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/vec_bytes.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5038 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/candid/vec_bytes.h
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 01:01:59.827740 icpp-candid-3.0.0/src/icpp_candid/hooks/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3481 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/hooks/icpp_hooks.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1192 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/hooks/icpp_hooks.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)       98 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/py.typed
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 01:01:59.803740 icpp-candid-3.0.0/src/icpp_candid/vendors/
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 01:01:59.831740 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1155 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/LICENSE
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3933 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1366 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1342 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3090 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_hex.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3143 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1356 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1336 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1381 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3070 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3201 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_url.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1805 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 01:01:59.831740 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/data/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    12087 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/data/access.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2352 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 01:01:59.835740 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     7994 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/base32.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     5692 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/base64.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    11905 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/codec.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1606 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/config.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     4545 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/hex.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    19664 2023-07-16 22:17:57.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1328 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3009 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/hex_lower.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     2994 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/hex_upper.hpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     3283 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/parse_error.hpp
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 01:01:59.835740 icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      861 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/LICENSE
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    31026 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/crc32.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1736 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/crc32.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1758 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/readme.md
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)    15133 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/sha256.cpp
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)     1968 2023-07-10 11:15:35.000000 icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/sha256.h
+-rw-r--r--   0 arjaan    (1000) arjaan    (1000)      322 2023-07-16 23:21:23.000000 icpp-candid-3.0.0/src/icpp_candid/version.py
+drwxrwxr-x   0 arjaan    (1000) arjaan    (1000)        0 2023-07-17 01:01:59.803740 icpp-candid-3.0.0/src/icpp_candid.egg-info/
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     2940 2023-07-17 01:01:59.000000 icpp-candid-3.0.0/src/icpp_candid.egg-info/PKG-INFO
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)     7629 2023-07-17 01:01:59.000000 icpp-candid-3.0.0/src/icpp_candid.egg-info/SOURCES.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)        1 2023-07-17 01:01:59.000000 icpp-candid-3.0.0/src/icpp_candid.egg-info/dependency_links.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       45 2023-07-17 01:01:59.000000 icpp-candid-3.0.0/src/icpp_candid.egg-info/requires.txt
+-rw-rw-r--   0 arjaan    (1000) arjaan    (1000)       12 2023-07-17 01:01:59.000000 icpp-candid-3.0.0/src/icpp_candid.egg-info/top_level.txt
```

### Comparing `icpp-candid-2.9.0/LICENSE` & `icpp-candid-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/PKG-INFO` & `icpp-candid-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpp-candid
-Version: 2.9.0
+Version: 3.0.0
 Summary: C++ Candid Library
 Home-page: https://docs.icpp.world/
 Author: icppWorld
 Author-email: icpp@icpp.world
 License: MIT
 Keywords: C++ Candid Library,Internet Computer,C++,Candid,blockchain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `icpp-candid-2.9.0/README.md` & `icpp-candid-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/setup.py` & `icpp-candid-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,18 @@
     #
     package_data={  # Optional
         "icpp_candid": [
             "candid/*.c",
             "candid/*.cpp",
             "candid/*.h",
             "candid/*.hpp",
+            "hooks/*.c",
+            "hooks/*.cpp",
+            "hooks/*.h",
+            "hooks/*.hpp",
             "vendors/cppcodec/*",
             "vendors/cppcodec/data/*",
             "vendors/cppcodec/detail/*",
             "vendors/hash-library/*",
             "vendors/hash-library/tests/*",
             "py.typed",
         ],
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/__init__.py` & `icpp-candid-3.0.0/src/icpp_candid/__init__.py`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_deserialize.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_deserialize.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 // Candid deserialization class
 // https://github.com/dfinity/candid/blob/master/spec/Candid.md#parameters-and-results
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_all_includes.h"
+#include "candid_deserialize.h"
 #include "candid_assert.h"
 #include "candid_opcode.h"
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidDeserialize::CandidDeserialize() { deserialize(); }
 CandidDeserialize::CandidDeserialize(const VecBytes &B,
-                                     std::vector<CandidType> A) {
+                                     CandidArgs A) {
   m_A = A;
   m_B = B;
   m_hex_string = ""; // TOdo
   deserialize();
 }
 CandidDeserialize::CandidDeserialize(const std::string hex_string,
-                                     std::vector<CandidType> A) {
+                                     CandidArgs A) {
   m_A = A;
   m_hex_string = hex_string;
   m_B.store_hex_string(hex_string);
   deserialize();
 }
 CandidDeserialize::~CandidDeserialize() {}
 
@@ -63,15 +65,15 @@
   {
     __uint128_t B_offset_start = B_offset;
     std::string parse_error;
     __uint128_t numbytes;
     if (m_B.parse_uleb128(B_offset, num_typetables, numbytes, parse_error)) {
       std::string to_be_parsed =
           "Number of unique type tables, T*(<comptype>*)";
-      trap_with_parse_error(B_offset_start, B_offset, to_be_parsed,
+      CandidAssert::trap_with_parse_error(B_offset_start, B_offset, to_be_parsed,
                             parse_error);
     }
   }
 
   // Parse the unique type tables
   for (size_t i = 0; i < num_typetables; ++i) {
     CandidTypeTable type_table = CandidTypeTable(m_B, B_offset);
@@ -93,37 +95,37 @@
 
   {
     __uint128_t B_offset_start = B_offset;
     std::string parse_error;
     __uint128_t numbytes;
     if (m_B.parse_uleb128(B_offset, num_args, numbytes, parse_error)) {
       std::string to_be_parsed = "Number of arguments, I*(<datatype>*)";
-      trap_with_parse_error(B_offset_start, B_offset, to_be_parsed,
+      CandidAssert::trap_with_parse_error(B_offset_start, B_offset, to_be_parsed,
                             parse_error);
     }
   }
 
-  if (num_args != m_A.size()) {
+  if (num_args != m_A.m_args_ptrs.size()) {
     std::string msg;
     msg.append("ERROR: wrong number of arguments on wire.\n");
     msg.append("       Expected number of arguments:" +
-               std::to_string(m_A.size()) + "\n");
+               std::to_string(m_A.m_args_ptrs.size()) + "\n");
     msg.append("       Number of arguments on wire :" +
-               IC_API::to_string_128(num_args));
-    IC_API::trap(msg);
+               ICPP_HOOKS::to_string_128(num_args));
+    ICPP_HOOKS::trap(msg);
   }
 
   for (size_t i = 0; i < num_args; ++i) {
     __uint128_t B_offset_start = B_offset;
     std::string parse_error;
     __uint128_t numbytes;
     __int128_t datatype;
     if (m_B.parse_sleb128(B_offset, datatype, numbytes, parse_error)) {
       std::string to_be_parsed = "datatype, I*(<datatype>*)";
-      trap_with_parse_error(B_offset_start, B_offset, to_be_parsed,
+      CandidAssert::trap_with_parse_error(B_offset_start, B_offset, to_be_parsed,
                             parse_error);
     }
     m_args_datatypes.push_back(int(datatype));
     m_args_datatypes_offset_start.push_back(B_offset_start);
     m_args_datatypes_offset_end.push_back(B_offset);
   }
 
@@ -148,73 +150,85 @@
       size_t type_table_index = m_args_datatypes[i];
       CandidTypeTable type_table = m_typetables[type_table_index];
 
       // Verify that the type_table found on the wire is the same as the expected type_table
       int opcode_found = type_table.get_opcode();
       v_opcode_found.push_back(opcode_found);
 
-      int opcode_expected =
-          std::visit([](auto &&c) { return c.get_datatype_opcode(); }, m_A[i]);
+      int opcode_expected = m_A.m_args_ptrs[i]->get_datatype_opcode();
 
       if (opcode_found != opcode_expected) {
         if (opcode_expected < 0) {
           std::string msg;
           msg.append(
               "ERROR: expecting an Opcode, but a type table reference was found on wire instead.\n");
           msg.append("       Argument index    : " + std::to_string(i) + "\n");
           msg.append("       Bytes offset start: " +
-                     IC_API::to_string_128(m_args_datatypes_offset_start[i]) +
+                     ICPP_HOOKS::to_string_128(m_args_datatypes_offset_start[i]) +
                      "\n");
           msg.append("       Bytes offset end  : " +
-                     IC_API::to_string_128(m_args_datatypes_offset_end[i]) +
+                     ICPP_HOOKS::to_string_128(m_args_datatypes_offset_end[i]) +
                      "\n");
           msg.append(
               "       Expecting opcode  :" + std::to_string(opcode_expected) +
               " (" + CandidOpcode().name_from_opcode(opcode_expected) + ")" +
               "\n");
           msg.append("       Found type table    :" +
                      std::to_string(opcode_found));
-          IC_API::trap(msg);
+          ICPP_HOOKS::trap(msg);
         } else {
           std::string msg;
           msg.append("ERROR: wrong type table reference found on wire.\n");
           msg.append("       Argument index: " + std::to_string(i) + "\n");
           msg.append("       Bytes offset start: " +
-                     IC_API::to_string_128(m_args_datatypes_offset_start[i]) +
+                     ICPP_HOOKS::to_string_128(m_args_datatypes_offset_start[i]) +
                      "\n");
           msg.append("       Bytes offset end  : " +
-                     IC_API::to_string_128(m_args_datatypes_offset_end[i]) +
+                     ICPP_HOOKS::to_string_128(m_args_datatypes_offset_end[i]) +
                      "\n");
           msg.append("       Expecting type table:" +
                      std::to_string(opcode_expected) + "\n");
           msg.append("       Found type table    :" +
                      std::to_string(opcode_found));
-          IC_API::trap(msg);
+          ICPP_HOOKS::trap(msg);
         }
       }
       if (opcode_found == CandidOpcode().Record) {
         CandidTypeRecord *p_wire =
             get_if<CandidTypeRecord>(type_table.get_candidType_ptr());
-        CandidTypeRecord *p_expected = get_if<CandidTypeRecord>(&m_A[i]);
-
-        // Trap if type table does not match the wire
-        p_expected->check_type_table(p_wire);
+        // CandidTypeRecord *p_expected = get_if<CandidTypeRecord>(&m_A[i]);
+        std::shared_ptr<CandidTypeRecord> p_expected = std::dynamic_pointer_cast<CandidTypeRecord>(m_A.m_args_ptrs[i]);
+        if (!p_expected) {
+            ICPP_HOOKS::trap("ERROR: Expecting a CandidTypeRecord during deserialization.");
+        } else if(p_wire) {
+          // Traps if type table of Record does not match the wire
+          p_expected->check_type_table(p_wire);  
+        } else {
+          ICPP_HOOKS::trap("ERROR: Logic error during deserialization of a CandidTypeRecord.");
+        }
       } else if (opcode_found == CandidOpcode().Variant) {
         CandidTypeVariant *p_wire =
             get_if<CandidTypeVariant>(type_table.get_candidType_ptr());
-        CandidTypeVariant *p_expected = get_if<CandidTypeVariant>(&m_A[i]);
-        p_expected->check_type_table(p_wire);
+        // CandidTypeVariant *p_expected = get_if<CandidTypeVariant>(&m_A[i]);
+        std::shared_ptr<CandidTypeVariant> p_expected = std::dynamic_pointer_cast<CandidTypeVariant>(m_A.m_args_ptrs[i]);
+        if (!p_expected) {
+            ICPP_HOOKS::trap("ERROR: Expecting a CandidTypeVariant during deserialization.");
+        } else if(p_wire) {
+          // Traps if type table of Variant does not match the wire
+          p_expected->check_type_table(p_wire);  
+        } else {
+          ICPP_HOOKS::trap("ERROR: Logic error during deserialization of a CandidTypeVariant.");
+        }
       } else if (opcode_found == CandidOpcode().Vec ||
                  opcode_found == CandidOpcode().Opt) {
 
         int content_opcode_found =
             std::visit([](auto &&c) { return c.get_content_type_opcode(); },
                        *type_table.get_candidType_ptr());
-        int content_opcode_expected = std::visit(
-            [](auto &&c) { return c.get_content_type_opcode(); }, m_A[i]);
+        int content_opcode_expected = m_A.m_args_ptrs[i]->get_content_type_opcode();
 
         if (content_opcode_found != content_opcode_expected) {
           std::string msg;
           if (opcode_found == CandidOpcode().Vec) {
             msg.append(
                 "ERROR: Vector with wrong content opcode found on wire.\n");
           } else if (opcode_found == CandidOpcode().Opt) {
@@ -222,67 +236,66 @@
           } else {
             msg.append(
                 "ERROR: const of unknown type with wrong content opcode found on wire.\n");
           }
 
           msg.append("       Argument index: " + std::to_string(i) + "\n");
           msg.append("       Bytes offset start: " +
-                     IC_API::to_string_128(m_args_datatypes_offset_start[i]) +
+                     ICPP_HOOKS::to_string_128(m_args_datatypes_offset_start[i]) +
                      "\n");
           msg.append("       Bytes offset end  : " +
-                     IC_API::to_string_128(m_args_datatypes_offset_end[i]) +
+                     ICPP_HOOKS::to_string_128(m_args_datatypes_offset_end[i]) +
                      "\n");
           msg.append("       Expecting content opcode:" +
                      std::to_string(content_opcode_expected) + " (" +
                      CandidOpcode().name_from_opcode(content_opcode_expected) +
                      ")" + "\n");
           msg.append("       Found content opcode    :" +
                      std::to_string(content_opcode_found) + " (" +
                      CandidOpcode().name_from_opcode(content_opcode_found) +
                      ")" + "\n");
-          IC_API::trap(msg);
+          ICPP_HOOKS::trap(msg);
         }
       } else {
-        IC_API::trap(
+        ICPP_HOOKS::trap(
             "ERROR: Deserialization not yet implemented for this constype");
       }
 
     } else {
       // <primptype>
 
       // There is no type-table. The datatype is an Opcode
       int opcode_found = m_args_datatypes[i];
       v_opcode_found.push_back(opcode_found);
 
-      int opcode_expected =
-          std::visit([](auto &&c) { return c.get_datatype_opcode(); }, m_A[i]);
+      int opcode_expected = m_A.m_args_ptrs[i]->get_datatype_opcode();
 
       if (opcode_found != opcode_expected) {
         if (opcode_found == CandidOpcode().Null &&
             opcode_expected == CandidOpcode().Opt) {
           // This is ok. A null is passed for an Opt
         } else {
           // TODO:  IMPLEMENT CHECK ON COVARIANCE/CONTRAVARIANCE
           std::string msg;
           msg.append("ERROR: wrong opcode found on wire.\n");
           msg.append("       Argument index: " + std::to_string(i) + "\n");
           msg.append("       Bytes offset start: " +
-                     IC_API::to_string_128(m_args_datatypes_offset_start[i]) +
+                     ICPP_HOOKS::to_string_128(m_args_datatypes_offset_start[i]) +
                      "\n");
           msg.append("       Bytes offset end  : " +
-                     IC_API::to_string_128(m_args_datatypes_offset_end[i]) +
+                     ICPP_HOOKS::to_string_128(m_args_datatypes_offset_end[i]) +
                      "\n");
           msg.append(
               "       Expecting opcode:" + std::to_string(opcode_expected) +
               " (" + CandidOpcode().name_from_opcode(opcode_expected) + ")" +
               "\n");
           msg.append("       Found opcode    :" + std::to_string(opcode_found) +
                      " (" + CandidOpcode().name_from_opcode(opcode_found) +
                      ")");
-          IC_API::trap(msg);
+          ICPP_HOOKS::trap(msg);
         }
       }
     }
   }
   // (4) using the inverse of the M function, indexed by (<t>,*), to decode the values (<v>,*)
   //
   // (5) use the coercion function C[(<t>,*) <: (<t'>,*)]((<v>,*)) to understand the decoded values at the expected type.
@@ -293,20 +306,18 @@
       // There is no value to decode
       continue;
     }
     __uint128_t B_offset_start = B_offset;
     std::string parse_error = "";
     __uint128_t numbytes;
 
-    if (std::visit(
-            [&](auto &&c) { return c.decode_M(m_B, B_offset, parse_error); },
-            m_A[i])) {
+    if (m_A.m_args_ptrs[i]->decode_M(m_B, B_offset, parse_error)) {
       std::string to_be_parsed =
           "Values (decoding M) for argument at index " + std::to_string(i);
-      CandidDeserialize::trap_with_parse_error(B_offset_start, B_offset,
+      CandidAssert::trap_with_parse_error(B_offset_start, B_offset,
                                                to_be_parsed, parse_error);
     }
   }
 
   // Append R
   // Was never implemented int Candid, although it is still in the spec
   // https://www.joachim-breitner.de/blog/786-A_Candid_explainer__Quirks
@@ -314,20 +325,9 @@
 
 // Assert candid VecBytes against a string in "hex" format (didc encode)
 int CandidDeserialize::assert_candid(const std::string &candid_expected,
                                      const bool &assert_value) {
   return CandidAssert::assert_candid(m_B, candid_expected, assert_value);
 }
 
-// Trap with parse error message
-void CandidDeserialize::trap_with_parse_error(const __uint128_t &B_offset_start,
-                                              const __uint128_t &B_offset,
-                                              const std::string &to_be_parsed,
-                                              const std::string &parse_error) {
-  std::string msg;
-  msg.append("ERROR: decoding of Candid byte stream failed.\n");
-  msg.append("       trying to extract: " + to_be_parsed + "\n");
-  msg.append("       parsing error:" + parse_error + "\n");
-  msg.append("       byte offset:" + IC_API::to_string_128(B_offset_start) +
-             "\n");
-  IC_API::trap(msg);
-}
+CandidArgs CandidDeserialize::get_A() { return m_A; }
+VecBytes CandidDeserialize::get_B() { return m_B; }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_deserialize.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_deserialize.h`

 * *Files 18% similar despite different names*

```diff
@@ -2,39 +2,35 @@
 // https://github.com/dfinity/candid/blob/master/spec/Candid.md#parameters-and-results
 
 #pragma once
 
 #include <string>
 #include <vector>
 
-#include "candid.h"
+#include "candid_args.h"
+#include "candid_type_table.h"
 
 class CandidDeserialize {
 public:
   CandidDeserialize();
-  CandidDeserialize(const VecBytes &B, std::vector<CandidType> A);
-  CandidDeserialize(const std::string hex_string, std::vector<CandidType> A);
+  CandidDeserialize(const VecBytes &B, CandidArgs A);
+  CandidDeserialize(const std::string hex_string, CandidArgs A);
   ~CandidDeserialize();
 
-  std::vector<CandidType> get_A() { return m_A; }
-  VecBytes get_B() { return m_B; }
+  CandidArgs get_A();
+  VecBytes get_B();
 
   int assert_candid(const std::string &candid_expected,
                     const bool &assert_value);
 
-  static void trap_with_parse_error(const __uint128_t &B_offset_start,
-                                    const __uint128_t &B_offset,
-                                    const std::string &to_be_parsed,
-                                    const std::string &parse_error);
-
 private:
   void deserialize();
 
   // The vector with placeholders for the expected arguments of the byte stream coming in
-  std::vector<CandidType> m_A;
+  CandidArgs m_A;
 
   // The deserialized type tables
   std::vector<CandidTypeTable> m_typetables;
 
   // The deserialized argument list
   std::vector<int> m_args_datatypes;
   std::vector<__uint128_t> m_args_datatypes_offset_start;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_opcode.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_opcode.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The Candid type Opcodes and helper methods
 
 #include <string>
 #include <unordered_map>
 
-#include "candid.h"
-#include "ic_api.h"
+#include "candid_type.h"
+#include "candid_type_all_includes.h"
+#include "candid_opcode.h"
+#include "icpp_hooks.h"
 
 CandidOpcode::CandidOpcode() {}
 
 CandidOpcode::~CandidOpcode() {}
 
 bool CandidOpcode::is_primtype(const int &t) {
   if (t == -1 || t == -2 || t == -3 || t == -4 || t == -5 || t == -6 ||
@@ -88,32 +90,32 @@
     c = CandidTypePrincipal();
   } else if (opcode == Vec) {
     std::string msg;
     msg.append(
         "ERROR: NOT SUPPORTED FOR VEC. (use candid_vec_type_from_opcode)");
     msg.append("       datatype = " + std::to_string(opcode));
     msg.append("      " + std::string(__func__));
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   } else if (opcode == Opt) {
     std::string msg;
     msg.append(
         "ERROR: NOT SUPPORTED FOR OPT. (use candid_opt_type_from_opcode)");
     msg.append("       datatype = " + std::to_string(opcode));
     msg.append("      " + std::string(__func__));
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   } else if (opcode == Record) {
     c = CandidTypeRecord();
   } else if (opcode == Variant) {
     c = CandidTypeVariant();
   } else {
     std::string msg;
     msg.append("ERROR: NOT YET IMPLEMENTED FOR THIS OPCODE.");
     msg.append("       datatype = " + std::to_string(opcode));
     msg.append("      " + std::string(__func__));
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   }
 }
 
 void CandidOpcode::candid_type_vec_from_opcode(CandidType &c, int opcode) {
   // if (opcode == Null) {
   //   c = CandidTypeVecNull();
   // } else if (opcode == Empty) {
@@ -156,15 +158,15 @@
     // } else if (opcode == Record) {
     //   c = CandidTypeVecRecord();
   } else {
     std::string msg;
     msg.append("ERROR: NOT YET IMPLEMENTED CandidTypeVecXXX.");
     msg.append("       for content type = " + std::to_string(opcode));
     msg.append("      " + std::string(__func__));
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   }
 }
 
 void CandidOpcode::candid_type_opt_from_opcode(CandidType &c, int opcode) {
   // if (opcode == Null) {
   //   c = CandidTypeOptNull();
   // } else if (opcode == Empty) {
@@ -208,10 +210,10 @@
     // } else if (opcode == Record) {
     //   c = CandidTypeOptRecord();
   } else {
     std::string msg;
     msg.append("ERROR: NOT YET IMPLEMENTED CandidTypeOptXXX.");
     msg.append("       for content type = " + std::to_string(opcode));
     msg.append("      " + std::string(__func__));
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   }
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_opcode.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_opcode.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 // The Candid type Opcodes and helper methods
 //
 //     https://github.com/dfinity/candid/blob/master/spec/Candid.md#types
 
 #pragma once
 
 #include <string>
-
-#include "candid.h"
-#include "ic_api.h"
+#include <cstdint>
 
 class CandidOpcode {
 public:
   CandidOpcode();
   ~CandidOpcode();
 
   bool is_primtype(const int &t);
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_serialize.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_serialize.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 // Candid serialization class
 // https://github.com/dfinity/candid/blob/master/spec/Candid.md#parameters-and-results
 
-#include "candid.h"
-#include "candid_assert.h"
+#include <variant>
 
-#include "ic_api.h"
+#include "candid_type.h"
+#include "candid_type_all_includes.h"
+#include "candid_serialize.h"
+#include "candid_assert.h"
 
 // Default constructor handles nullary input '()'
 CandidSerialize::CandidSerialize() { serialize(); }
 CandidSerialize::CandidSerialize(const CandidType &a) {
-  m_A.push_back(a);
+  m_A.append(a);
   serialize();
 }
-CandidSerialize::CandidSerialize(const std::vector<CandidType> &A) : m_A{A} {
+CandidSerialize::CandidSerialize(const CandidArgs &A) : m_A{A} {
   serialize();
 }
 
 CandidSerialize::~CandidSerialize() {}
 
 void CandidSerialize::serialize() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#parameters-and-results
@@ -40,27 +42,23 @@
   // (-) Constructed Types (opt, vec, record, variant)
   // (-) Reference Types (func, service)
 
   // Check how many unique typetables we have and set the index
   const __uint128_t NO_TYPE_TABLE = -9999999999999999;
   __uint128_t typetable_i = 0;
 
-  for (size_t i = 0; i < m_A.size(); ++i) {
+  for (size_t i = 0; i < m_A.m_args_ptrs.size(); ++i) {
     m_type_table_A_index.push_back(NO_TYPE_TABLE);
     m_type_table_index.push_back(NO_TYPE_TABLE);
-
-    CandidType c = m_A[i];
-
-    VecBytes T = std::visit([](auto &&c) { return c.get_T(); }, c);
+    VecBytes T = m_A.m_args_ptrs[i]->get_T();
 
     if (T.size() > 0) {
       bool new_type_table = true;
       for (size_t i1 = 0; i1 < i; ++i1) {
-        CandidType c1 = m_A[i1];
-        VecBytes T1 = std::visit([](auto &&c) { return c.get_T(); }, c1);
+        VecBytes T1 = m_A.m_args_ptrs[i1]->get_T();
         if (T == T1) {
           m_type_table_A_index[i] = m_type_table_A_index[i1];
           m_type_table_index[i] = m_type_table_index[i1];
           new_type_table = false;
           break;
         }
       }
@@ -72,45 +70,45 @@
     }
   }
 
   // Append the number of unique type tables
   m_B.append_uleb128(m_num_typetables);
 
   // Now write the unique type tables
-  for (size_t i = 0; i < m_A.size(); ++i) {
+  for (size_t i = 0; i < m_A.m_args_ptrs.size(); ++i) {
     if (m_type_table_A_index[i] == i) {
-      VecBytes T = std::visit([](auto &&c) { return c.get_T(); }, m_A[i]);
+      VecBytes T = m_A.m_args_ptrs[i]->get_T();
       for (std::byte b : T.vec()) {
         m_B.append_byte(b);
       }
     }
   }
 
   // -------------------------------------------------------------------------------------
   // I*(<datatype>*)                      types of the argument list
-  m_B.append_uleb128(__uint128_t(m_A.size()));
+  m_B.append_uleb128(__uint128_t(m_A.m_args_ptrs.size()));
 
-  for (size_t i = 0; i < m_A.size(); ++i) {
-    VecBytes T = std::visit([](auto &&c) { return c.get_T(); }, m_A[i]);
+  for (size_t i = 0; i < m_A.m_args_ptrs.size(); ++i) {
+    VecBytes T = m_A.m_args_ptrs[i]->get_T();
     if (T.size() > 0) {
       // For <comptypes>, we use the index into the type table we defined above
       m_B.append_uleb128(m_type_table_index[i]);
     } else {
       // For <primtypes>, use the Opcode, already stored
-      VecBytes I = std::visit([](auto &&c) { return c.get_I(); }, m_A[i]);
+      VecBytes I = m_A.m_args_ptrs[i]->get_I();
       for (std::byte b : I.vec()) {
         m_B.append_byte(b);
       }
     }
   }
 
   // -------------------------------------------------------------------------------------
   // M(kv* : <datatype>*)                 values of argument list
-  for (CandidType c : m_A) {
-    VecBytes M = std::visit([](auto &&c) { return c.get_M(); }, c);
+  for (std::shared_ptr<CandidTypeBase> p_c : m_A.m_args_ptrs) {
+    VecBytes M = p_c->get_M();
     for (std::byte b : M.vec()) {
       m_B.append_byte(b);
     }
   }
 
   // Append R
   // Was never implemented in Candid, although it is still in the spec
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_serialize.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_serialize.h`

 * *Files 22% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 // https://github.com/dfinity/candid/blob/master/spec/Candid.md#parameters-and-results
 
 #pragma once
 
 #include <string>
 #include <vector>
 
-#include "candid.h"
+#include "candid_args.h"
+#include "vec_bytes.h"
 
 class CandidSerialize {
 public:
   CandidSerialize(const CandidType &a);
-  CandidSerialize(const std::vector<CandidType> &A);
+  CandidSerialize(const CandidArgs &A);
   CandidSerialize();
   ~CandidSerialize();
 
-  std::vector<CandidType> get_A() { return m_A; }
+  CandidArgs get_A() { return m_A; }
   VecBytes get_B() { return m_B; }
   __uint128_t get_num_typetables() { return m_num_typetables; }
 
   int assert_candid(const std::string &candid_expected,
                     const bool &assert_value);
 
 private:
   void serialize();
 
   // The argument list to be serialized
-  std::vector<CandidType> m_A;
+  CandidArgs m_A;
 
   // The serialized byte stream
   VecBytes m_B;
 
   // For the <comptype> arguments with a unique type table
   __uint128_t m_num_typetables;
   std::vector<__uint128_t> m_type_table_A_index; // Index into m_A
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_base.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_base.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 // The base class for all Candid Types
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_base.h"
 
 #include <charconv>
 #include <cmath>
 #include <system_error>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidTypeBase::CandidTypeBase() {}
 
 CandidTypeBase::~CandidTypeBase() {}
 
 void CandidTypeBase::trap_if_wrong_type_on_wire(
     const std::string &type_on_wire) {
   if (type_on_wire != m_datatype_textual) {
     std::string msg;
     msg.append("ERROR: wrong Candid type on wire.\n");
     msg.append("       Candid type on wire  = " + type_on_wire + "\n");
     msg.append("       Expected Candid type = " + m_datatype_textual);
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   };
 }
 
 // Virtual method to be implemented by the <comptype> CandidTypes
 // Non <comptype> should not call this method.
 bool CandidTypeBase::decode_T(const VecBytes B, __uint128_t &offset,
                               std::string &parse_error) {
-  IC_API::trap("ERROR: decode_T not implemented...");
+  ICPP_HOOKS::trap("ERROR: decode_T not implemented...");
   return true;
 }
 void CandidTypeBase::set_content_type() {
-  IC_API::trap("ERROR: set_content_type not implemented...");
+  ICPP_HOOKS::trap("ERROR: set_content_type not implemented...");
 }
 
 // Virtual method to be implemented by all CandidTypes to support deserialization
 bool CandidTypeBase::decode_M(const VecBytes B, __uint128_t &offset,
                               std::string &parse_error) {
-  IC_API::trap("ERROR: decode_M not implemented...");
+  ICPP_HOOKS::trap("ERROR: decode_M not implemented...");
   return true;
 }
 void CandidTypeBase::encode_M() {
-  IC_API::trap("ERROR: encode_M not implemented...");
+  ICPP_HOOKS::trap("ERROR: encode_M not implemented...");
 }
 
 // https://github.com/dfinity/candid/blob/master/spec/Candid.md#records
 uint32_t CandidTypeBase::idl_hash(const std::string &s) {
   uint32_t hash{};
 
   // hash(id) = ( Sum_(i=0..k) utf8(id)[i] * 223^(k-i) ) mod 2^32 where k = |utf8(id)|-1
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_base.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_base.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 // The base class for all Candid Types
 
 #pragma once
 
 #include <string>
 #include <vector>
 
-#include "candid.h"
-
 #include "candid_opcode.h"
 #include "vec_bytes.h"
 
 class CandidTypeBase {
 public:
   CandidTypeBase();
   ~CandidTypeBase();
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_bool.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_bool.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 // The class for the Primitive Candid Type: bool
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_bool.h"
+#include "candid_assert.h"
 
 #include "candid_opcode.h"
 
-CandidTypeBool::CandidTypeBool() : CandidTypePrim() { initialize(true); }
+CandidTypeBool::CandidTypeBool() { initialize(true); }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeBool::CandidTypeBool(bool *p_v) : CandidTypePrim() {
+CandidTypeBool::CandidTypeBool(bool *p_v) {
   set_pv(p_v);
 
   const bool v = const_cast<bool &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeBool::CandidTypeBool(const bool v) : CandidTypePrim() {
+CandidTypeBool::CandidTypeBool(const bool v) {
   initialize(v);
 }
 
 CandidTypeBool::~CandidTypeBool() {}
 
 // Initialize things
 void CandidTypeBool::initialize(const bool &v) {
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
 void CandidTypeBool::set_pv(bool *v) { m_pv = v; }
 
@@ -55,15 +58,15 @@
                               std::string &parse_error) {
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t iv{0};
   if (B.parse_uleb128(offset, iv, numbytes, parse_error)) {
     std::string to_be_parsed = "Value for CandidTypeBool";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (iv == 0) {
     m_v = false;
   } else {
     m_v = true;
   }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_empty.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_empty.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 // The class for the Primitive Candid Type: empty
 
-#include "candid.h"
-#include "ic_api.h"
+#include "candid_type.h"
+#include "candid_type_empty.h"
+#include "icpp_hooks.h"
 
 #include "candid_opcode.h"
 
-CandidTypeEmpty::CandidTypeEmpty() : CandidTypePrim() {
+CandidTypeEmpty::CandidTypeEmpty() {
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 CandidTypeEmpty::~CandidTypeEmpty() {}
 
 void CandidTypeEmpty::set_datatype() {
@@ -24,16 +26,16 @@
   // For <primtype>: the negative Opcode
   m_I.append_byte((std::byte)m_datatype_hex);
 }
 
 void CandidTypeEmpty::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // NB: M(_ : empty) just ignore
-  // IC_API::trap("ERROR - CandidTypeEmpty cannot have a value to encode.");
+  // ICPP_HOOKS::trap("ERROR - CandidTypeEmpty cannot have a value to encode.");
 }
 
 // Decode the values, starting at & updating offset
 bool CandidTypeEmpty::decode_M(VecBytes B, __uint128_t &offset,
                                std::string &parse_error) {
-  IC_API::trap("ERROR - CandidTypeEmpty cannot have a value to decode.");
+  ICPP_HOOKS::trap("ERROR - CandidTypeEmpty cannot have a value to decode.");
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_float32.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_float32.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 // The class for the Primitive Candid Type: float32
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_float32.h"
+#include "icpp_hooks.h"
+#include "candid_assert.h"
 
 #include "candid_opcode.h"
 #include "pro.h"
 
-CandidTypeFloat32::CandidTypeFloat32() : CandidTypePrim() {
+CandidTypeFloat32::CandidTypeFloat32() {
 
   float v = 0.0;
   initialize(v);
 }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeFloat32::CandidTypeFloat32(float *p_v) : CandidTypePrim() {
+CandidTypeFloat32::CandidTypeFloat32(float *p_v) {
 
   set_pv(p_v);
 
   const float v = const_cast<float &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeFloat32::CandidTypeFloat32(const float v) : CandidTypePrim() {
+CandidTypeFloat32::CandidTypeFloat32(const float v) {
 
   initialize(v);
 }
 
 CandidTypeFloat32::~CandidTypeFloat32() {}
 
 // Initialize things
 void CandidTypeFloat32::initialize(const float &v) {
   if (sizeof(v) != 4) {
-    IC_API::trap(
+    ICPP_HOOKS::trap(
         "ERROR: The type float is not 4 bytes. \nThis is not yet supported.\n" +
         std::string(__func__));
   }
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
 void CandidTypeFloat32::set_pv(float *v) { m_pv = v; }
 
@@ -65,15 +69,15 @@
 // Decode the values, starting at & updating offset
 bool CandidTypeFloat32::decode_M(VecBytes B, __uint128_t &offset,
                                  std::string &parse_error) {
   __uint128_t offset_start = offset;
   parse_error = "";
   if (B.parse_float_ieee754(offset, m_v, parse_error)) {
     std::string to_be_parsed = "Value for CandidTypeFloat32";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_float64.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_float64.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 // The class for the Primitive Candid Type: float64
 
-#include "candid.h"
-
+#include "candid_type.h"
+#include "candid_type_float64.h"
+#include "icpp_hooks.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 #include "pro.h"
 
-CandidTypeFloat64::CandidTypeFloat64() : CandidTypePrim() {
+CandidTypeFloat64::CandidTypeFloat64() {
 
   double v = 0.0;
   initialize(v);
 }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeFloat64::CandidTypeFloat64(double *p_v) : CandidTypePrim() {
+CandidTypeFloat64::CandidTypeFloat64(double *p_v) {
 
   set_pv(p_v);
 
   const double v = const_cast<double &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeFloat64::CandidTypeFloat64(const double v) : CandidTypePrim() {
+CandidTypeFloat64::CandidTypeFloat64(const double v) {
 
   initialize(v);
 }
 
 CandidTypeFloat64::~CandidTypeFloat64() {}
 
 // Initialize things
 void CandidTypeFloat64::initialize(const double &v) {
   if (sizeof(v) != 8) {
-    IC_API::trap(
+    ICPP_HOOKS::trap(
         "ERROR: The type double is not 8 bytes. \nThis is not yet supported.\n" +
         std::string(__func__));
   }
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
 void CandidTypeFloat64::set_pv(double *v) { m_pv = v; }
 
@@ -65,15 +68,15 @@
 // Decode the values, starting at & updating offset
 bool CandidTypeFloat64::decode_M(VecBytes B, __uint128_t &offset,
                                  std::string &parse_error) {
   __uint128_t offset_start = offset;
   parse_error = "";
   if (B.parse_float_ieee754(offset, m_v, parse_error)) {
     std::string to_be_parsed = "Value for CandidTypeFloat64";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_float64.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_float32.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-// The class for the Primitive Candid Type: float64
+// The class for the Primitive Candid Type: float32
 
 #pragma once
 
-#include "candid.h"
+#include "candid_type_base.h"
+#include "vec_bytes.h"
 
-class CandidTypeFloat64 : public CandidTypePrim {
+class CandidTypeFloat32 : public CandidTypeBase {
 public:
   // Constructors
-  CandidTypeFloat64();
-  // docs start: demo_candid_type_float64
-  CandidTypeFloat64(double *v);
-  CandidTypeFloat64(const double v); // docs end: demo_candid_type_float64
+  CandidTypeFloat32();
+  // docs start: demo_candid_type_float32
+  CandidTypeFloat32(float *v);
+  CandidTypeFloat32(const float v); // docs end: demo_candid_type_float32
 
   // Destructor
-  ~CandidTypeFloat64();
+  ~CandidTypeFloat32();
 
+  bool decode_T(VecBytes B, __uint128_t &offset, std::string &parse_error) {
+    return false; // type table for Primitives is empty
+  }
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  double get_v() { return m_v; }
+  float get_v() { return m_v; }
 
 protected:
-  void set_pv(double *v);
-  void initialize(const double &v);
+  void set_pv(float *v);
+  void initialize(const float &v);
   void set_datatype();
+  void encode_T() { m_T.clear(); } // type table for Primitives is empty
   void encode_I();
   void encode_M();
 
-  double m_v;
-  double *m_pv{nullptr};
+  float m_v;
+  float *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 // The class for the Primitive Candid Type: int
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_int.h"
+#include "candid_assert.h"
 
 #include "candid_opcode.h"
 
-CandidTypeInt::CandidTypeInt() : CandidTypePrim() { initialize(0); }
+CandidTypeInt::CandidTypeInt() { initialize(0); }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeInt::CandidTypeInt(__int128_t *p_v) : CandidTypePrim() {
+CandidTypeInt::CandidTypeInt(__int128_t *p_v) {
   set_pv(p_v);
 
   const __int128_t v = const_cast<__int128_t &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeInt::CandidTypeInt(const __int128_t &v) : CandidTypePrim() {
+CandidTypeInt::CandidTypeInt(const __int128_t &v) {
   initialize(v);
 }
 
 CandidTypeInt::~CandidTypeInt() {}
 
 // Initialize things
 void CandidTypeInt::initialize(const __int128_t &v) {
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
 void CandidTypeInt::set_pv(__int128_t *v) { m_pv = v; }
 
@@ -54,15 +57,15 @@
 bool CandidTypeInt::decode_M(VecBytes B, __uint128_t &offset,
                              std::string &parse_error) {
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   if (B.parse_sleb128(offset, m_v, numbytes, parse_error)) {
     std::string to_be_parsed = "Value for CandidTypeInt";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int16.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int16.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 // The class for the Primitive Candid Type: int16
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_int16.h"
+#include "candid_assert.h"
 
 #include "candid_opcode.h"
 #include "pro.h"
 
-CandidTypeInt16::CandidTypeInt16() : CandidTypePrim() { initialize(0); }
+CandidTypeInt16::CandidTypeInt16() { initialize(0); }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeInt16::CandidTypeInt16(int16_t *p_v) : CandidTypePrim() {
+CandidTypeInt16::CandidTypeInt16(int16_t *p_v) {
 
   set_pv(p_v);
 
   const int16_t v = const_cast<int16_t &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeInt16::CandidTypeInt16(const int16_t v) : CandidTypePrim() {
+CandidTypeInt16::CandidTypeInt16(const int16_t v) {
 
   initialize(v);
 }
 
 CandidTypeInt16::~CandidTypeInt16() {}
 
 // Initialize things
 void CandidTypeInt16::initialize(const int16_t &v) {
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
 void CandidTypeInt16::set_pv(int16_t *v) { m_pv = v; }
 
@@ -57,15 +60,15 @@
 bool CandidTypeInt16::decode_M(VecBytes B, __uint128_t &offset,
                                std::string &parse_error) {
 
   __uint128_t offset_start = offset;
   parse_error = "";
   if (B.parse_int_fixed_width(offset, m_v, parse_error)) {
     std::string to_be_parsed = "Value for CandidTypeInt16";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int32.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int32.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 // The class for the Primitive Candid Type: int32
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_int32.h"
+#include "candid_assert.h"
 
 #include "candid_opcode.h"
 #include "pro.h"
 
-CandidTypeInt32::CandidTypeInt32() : CandidTypePrim() { initialize(0); }
+CandidTypeInt32::CandidTypeInt32() { initialize(0); }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeInt32::CandidTypeInt32(int32_t *p_v) : CandidTypePrim() {
+CandidTypeInt32::CandidTypeInt32(int32_t *p_v) {
 
   set_pv(p_v);
 
   const int32_t v = const_cast<int32_t &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeInt32::CandidTypeInt32(const int32_t v) : CandidTypePrim() {
+CandidTypeInt32::CandidTypeInt32(const int32_t v) {
 
   initialize(v);
 }
 
 CandidTypeInt32::~CandidTypeInt32() {}
 
 // Initialize things
 void CandidTypeInt32::initialize(const int32_t &v) {
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
 void CandidTypeInt32::set_pv(int32_t *v) { m_pv = v; }
 
@@ -57,15 +60,15 @@
 bool CandidTypeInt32::decode_M(VecBytes B, __uint128_t &offset,
                                std::string &parse_error) {
 
   __uint128_t offset_start = offset;
   parse_error = "";
   if (B.parse_int_fixed_width(offset, m_v, parse_error)) {
     std::string to_be_parsed = "Value for CandidTypeInt32";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int64.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int64.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 // The class for the Primitive Candid Type: int64
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_int64.h"
+#include "candid_assert.h"
 
 #include "candid_opcode.h"
 #include "pro.h"
 
-CandidTypeInt64::CandidTypeInt64() : CandidTypePrim() { initialize(0); }
+CandidTypeInt64::CandidTypeInt64() { initialize(0); }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeInt64::CandidTypeInt64(int64_t *p_v) : CandidTypePrim() {
+CandidTypeInt64::CandidTypeInt64(int64_t *p_v) {
 
   set_pv(p_v);
 
   const int64_t v = const_cast<int64_t &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeInt64::CandidTypeInt64(const int64_t v) : CandidTypePrim() {
+CandidTypeInt64::CandidTypeInt64(const int64_t v) {
 
   initialize(v);
 }
 
 CandidTypeInt64::~CandidTypeInt64() {}
 
 // Initialize things
 void CandidTypeInt64::initialize(const int64_t &v) {
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
 void CandidTypeInt64::set_pv(int64_t *v) { m_pv = v; }
 
@@ -57,15 +60,15 @@
 bool CandidTypeInt64::decode_M(VecBytes B, __uint128_t &offset,
                                std::string &parse_error) {
 
   __uint128_t offset_start = offset;
   parse_error = "";
   if (B.parse_int_fixed_width(offset, m_v, parse_error)) {
     std::string to_be_parsed = "Value for CandidTypeInt64";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int64.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat64.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-// The class for the Primitive Candid Type: int64
+// The class for the Candid Type: vec
 
 #pragma once
 
-#include "candid.h"
+#include <cstring>
 
-class CandidTypeInt64 : public CandidTypePrim {
+#include "candid_type_vec_base.h"
+#include "candid_type_nat64.h"
+#include "vec_bytes.h"
+
+class CandidTypeVecNat64 : public CandidTypeVecBase {
 public:
   // Constructors
-  CandidTypeInt64();
-  // docs start: demo_candid_type_int64
-  CandidTypeInt64(int64_t *v);
-  CandidTypeInt64(const int64_t v); // docs end: demo_candid_type_int64
+  CandidTypeVecNat64();
+  CandidTypeVecNat64(const std::vector<uint64_t> v);
+
+  CandidTypeVecNat64(std::vector<uint64_t> *p_v);
 
   // Destructor
-  ~CandidTypeInt64();
+  ~CandidTypeVecNat64();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  int64_t get_v() { return m_v; }
+  std::vector<uint64_t> get_v() { return m_v; }
 
 protected:
-  void set_pv(int64_t *v);
-  void initialize(const int64_t &v);
-  void set_datatype();
-  void encode_I();
+  void set_pv(std::vector<uint64_t> *v) { m_pv = v; }
+  void set_v(const std::vector<uint64_t> &v) { m_v = v; }
+  void set_content_type();
   void encode_M();
 
-  int64_t m_v;
-  int64_t *m_pv{nullptr};
+  std::vector<uint64_t> m_v;
+  std::vector<uint64_t> *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int8.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int8.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 // The class for the Primitive Candid Type: int8
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_int8.h"
+#include "candid_assert.h"
 
 #include "candid_opcode.h"
 #include "pro.h"
 
-CandidTypeInt8::CandidTypeInt8() : CandidTypePrim() { initialize(0); }
+CandidTypeInt8::CandidTypeInt8() { initialize(0); }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeInt8::CandidTypeInt8(int8_t *p_v) : CandidTypePrim() {
+CandidTypeInt8::CandidTypeInt8(int8_t *p_v) {
 
   set_pv(p_v);
 
   const int8_t v = const_cast<int8_t &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeInt8::CandidTypeInt8(const int8_t v) : CandidTypePrim() {
+CandidTypeInt8::CandidTypeInt8(const int8_t v) {
 
   initialize(v);
 }
 
 CandidTypeInt8::~CandidTypeInt8() {}
 
 // Initialize things
 void CandidTypeInt8::initialize(const int8_t &v) {
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
 void CandidTypeInt8::set_pv(int8_t *v) { m_pv = v; }
 
@@ -57,15 +60,15 @@
 bool CandidTypeInt8::decode_M(VecBytes B, __uint128_t &offset,
                               std::string &parse_error) {
 
   __uint128_t offset_start = offset;
   parse_error = "";
   if (B.parse_int_fixed_width(offset, m_v, parse_error)) {
     std::string to_be_parsed = "Value for CandidTypeInt8";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_int8.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_int8.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 // The class for the Primitive Candid Type: int8
 
 #pragma once
 
-#include "candid.h"
+#include "candid_type_base.h"
+#include "vec_bytes.h"
 
-class CandidTypeInt8 : public CandidTypePrim {
+class CandidTypeInt8 : public CandidTypeBase {
 public:
   // Constructors
   CandidTypeInt8();
   // docs start: demo_candid_type_int8
   CandidTypeInt8(int8_t *v);
   CandidTypeInt8(const int8_t v); // docs end: demo_candid_type_int8
 
   // Destructor
   ~CandidTypeInt8();
 
+  bool decode_T(VecBytes B, __uint128_t &offset, std::string &parse_error) {
+    return false; // type table for Primitives is empty
+  }
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
   int8_t get_v() { return m_v; }
 
 protected:
   void set_pv(int8_t *v);
   void initialize(const int8_t &v);
   void set_datatype();
+  void encode_T() { m_T.clear(); } // type table for Primitives is empty
   void encode_I();
   void encode_M();
 
   int8_t m_v;
   int8_t *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 // The class for the Primitive Candid Type: nat
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_nat.h"
+#include "candid_assert.h"
 
 #include "candid_opcode.h"
 #include "pro.h"
 
-CandidTypeNat::CandidTypeNat() : CandidTypePrim() { initialize(0); }
+CandidTypeNat::CandidTypeNat() { initialize(0); }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeNat::CandidTypeNat(__uint128_t *p_v) : CandidTypePrim() {
+CandidTypeNat::CandidTypeNat(__uint128_t *p_v) {
 
   set_pv(p_v);
 
   const __uint128_t v = const_cast<__uint128_t &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeNat::CandidTypeNat(const __uint128_t v) : CandidTypePrim() {
+CandidTypeNat::CandidTypeNat(const __uint128_t v) {
 
   initialize(v);
 }
 
 CandidTypeNat::~CandidTypeNat() {}
 
 // Initialize things
 void CandidTypeNat::initialize(const __uint128_t &v) {
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
 void CandidTypeNat::set_pv(__uint128_t *v) { m_pv = v; }
 
@@ -57,15 +60,15 @@
 bool CandidTypeNat::decode_M(VecBytes B, __uint128_t &offset,
                              std::string &parse_error) {
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   if (B.parse_uleb128(offset, m_v, numbytes, parse_error)) {
     std::string to_be_parsed = "Value for CandidTypeNat";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat32.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-// The class for the Primitive Candid Type: nat
+// The class for the Primitive Candid Type: nat32
 
 #pragma once
 
-#include "candid.h"
+#include "candid_type_base.h"
+#include "vec_bytes.h"
 
-class CandidTypeNat : public CandidTypePrim {
+class CandidTypeNat32 : public CandidTypeBase {
 public:
   // Constructors
-  CandidTypeNat();
-  // docs start: demo_candid_type_nat
-  CandidTypeNat(__uint128_t *v);
-  CandidTypeNat(const __uint128_t v); // docs end: demo_candid_type_nat
+  CandidTypeNat32();
+  // docs start: demo_candid_type_nat32
+  CandidTypeNat32(uint32_t *v);
+  CandidTypeNat32(const uint32_t v); // docs end: demo_candid_type_nat32
 
   // Destructor
-  ~CandidTypeNat();
+  ~CandidTypeNat32();
 
+  bool decode_T(VecBytes B, __uint128_t &offset, std::string &parse_error) {
+    return false; // type table for Primitives is empty
+  }
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  __uint128_t get_v() { return m_v; }
+  uint32_t get_v() { return m_v; }
 
 protected:
-  void set_pv(__uint128_t *v);
-  void initialize(const __uint128_t &v);
+  void set_pv(uint32_t *v);
+  void initialize(const uint32_t &v);
   void set_datatype();
+  void encode_T() { m_T.clear(); } // type table for Primitives is empty
   void encode_I();
   void encode_M();
 
-  __uint128_t m_v;
-  __uint128_t *m_pv{nullptr};
+  uint32_t m_v;
+  uint32_t *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat16.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat32.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,73 @@
-// The class for the Primitive Candid Type: nat16
+// The class for the Primitive Candid Type: nat32
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_nat32.h"
+#include "candid_assert.h"
 
 #include "candid_opcode.h"
 #include "pro.h"
 
-CandidTypeNat16::CandidTypeNat16() : CandidTypePrim() { initialize(0); }
+CandidTypeNat32::CandidTypeNat32() { initialize(0); }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeNat16::CandidTypeNat16(uint16_t *p_v) : CandidTypePrim() {
+CandidTypeNat32::CandidTypeNat32(uint32_t *p_v) {
 
   set_pv(p_v);
 
-  const uint16_t v = const_cast<uint16_t &>(*p_v);
+  const uint32_t v = const_cast<uint32_t &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeNat16::CandidTypeNat16(const uint16_t v) : CandidTypePrim() {
+CandidTypeNat32::CandidTypeNat32(const uint32_t v) {
 
   initialize(v);
 }
 
-CandidTypeNat16::~CandidTypeNat16() {}
+CandidTypeNat32::~CandidTypeNat32() {}
 
 // Initialize things
-void CandidTypeNat16::initialize(const uint16_t &v) {
+void CandidTypeNat32::initialize(const uint32_t &v) {
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
-void CandidTypeNat16::set_pv(uint16_t *v) { m_pv = v; }
+void CandidTypeNat32::set_pv(uint32_t *v) { m_pv = v; }
 
-void CandidTypeNat16::set_datatype() {
-  m_datatype_opcode = CandidOpcode().Nat16;
-  m_datatype_hex = OpcodeHex().Nat16;
-  m_datatype_textual = OpcodeTextual().Nat16;
+void CandidTypeNat32::set_datatype() {
+  m_datatype_opcode = CandidOpcode().Nat32;
+  m_datatype_hex = OpcodeHex().Nat32;
+  m_datatype_textual = OpcodeTextual().Nat32;
 }
 
-void CandidTypeNat16::encode_I() {
+void CandidTypeNat32::encode_I() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#types
   // For <primtype>: the negative Opcode
   m_I.append_byte((std::byte)m_datatype_hex);
 }
 
-void CandidTypeNat16::encode_M() {
+void CandidTypeNat32::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(n : nat<N>)   = i<N>(n)    (Litte Endian)
   m_M.append_int_fixed_width(m_v);
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeNat16::decode_M(VecBytes B, __uint128_t &offset,
+bool CandidTypeNat32::decode_M(VecBytes B, __uint128_t &offset,
                                std::string &parse_error) {
   __uint128_t offset_start = offset;
   parse_error = "";
   if (B.parse_int_fixed_width(offset, m_v, parse_error)) {
-    std::string to_be_parsed = "Value for CandidTypeNat16";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    std::string to_be_parsed = "Value for CandidTypeNat32";
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat16.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat16.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 // The class for the Primitive Candid Type: nat16
 
 #pragma once
 
-#include "candid.h"
+#include "candid_type_base.h"
+#include "vec_bytes.h"
 
-class CandidTypeNat16 : public CandidTypePrim {
+class CandidTypeNat16 : public CandidTypeBase {
 public:
   // Constructors
   CandidTypeNat16();
   // docs start: demo_candid_type_nat16
   CandidTypeNat16(uint16_t *v);
   CandidTypeNat16(const uint16_t v); // docs end: demo_candid_type_nat16
 
   // Destructor
   ~CandidTypeNat16();
 
+  bool decode_T(VecBytes B, __uint128_t &offset, std::string &parse_error) {
+    return false; // type table for Primitives is empty
+  }
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
   uint16_t get_v() { return m_v; }
 
 protected:
   void set_pv(uint16_t *v);
   void initialize(const uint16_t &v);
   void set_datatype();
+  void encode_T() { m_T.clear(); } // type table for Primitives is empty
   void encode_I();
   void encode_M();
 
   uint16_t m_v;
   uint16_t *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat32.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat64.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,73 @@
-// The class for the Primitive Candid Type: nat32
+// The class for the Primitive Candid Type: nat64
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_nat64.h"
+#include "candid_assert.h"
 
 #include "candid_opcode.h"
 #include "pro.h"
 
-CandidTypeNat32::CandidTypeNat32() : CandidTypePrim() { initialize(0); }
+CandidTypeNat64::CandidTypeNat64() { initialize(0); }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeNat32::CandidTypeNat32(uint32_t *p_v) : CandidTypePrim() {
+CandidTypeNat64::CandidTypeNat64(uint64_t *p_v) {
 
   set_pv(p_v);
 
-  const uint32_t v = const_cast<uint32_t &>(*p_v);
+  const uint64_t v = const_cast<uint64_t &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeNat32::CandidTypeNat32(const uint32_t v) : CandidTypePrim() {
+CandidTypeNat64::CandidTypeNat64(const uint64_t v) {
 
   initialize(v);
 }
 
-CandidTypeNat32::~CandidTypeNat32() {}
+CandidTypeNat64::~CandidTypeNat64() {}
 
 // Initialize things
-void CandidTypeNat32::initialize(const uint32_t &v) {
+void CandidTypeNat64::initialize(const uint64_t &v) {
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
-void CandidTypeNat32::set_pv(uint32_t *v) { m_pv = v; }
+void CandidTypeNat64::set_pv(uint64_t *v) { m_pv = v; }
 
-void CandidTypeNat32::set_datatype() {
-  m_datatype_opcode = CandidOpcode().Nat32;
-  m_datatype_hex = OpcodeHex().Nat32;
-  m_datatype_textual = OpcodeTextual().Nat32;
+void CandidTypeNat64::set_datatype() {
+  m_datatype_opcode = CandidOpcode().Nat64;
+  m_datatype_hex = OpcodeHex().Nat64;
+  m_datatype_textual = OpcodeTextual().Nat64;
 }
 
-void CandidTypeNat32::encode_I() {
+void CandidTypeNat64::encode_I() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#types
   // For <primtype>: the negative Opcode
   m_I.append_byte((std::byte)m_datatype_hex);
 }
 
-void CandidTypeNat32::encode_M() {
+void CandidTypeNat64::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(n : nat<N>)   = i<N>(n)    (Litte Endian)
   m_M.append_int_fixed_width(m_v);
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeNat32::decode_M(VecBytes B, __uint128_t &offset,
+bool CandidTypeNat64::decode_M(VecBytes B, __uint128_t &offset,
                                std::string &parse_error) {
   __uint128_t offset_start = offset;
   parse_error = "";
   if (B.parse_int_fixed_width(offset, m_v, parse_error)) {
-    std::string to_be_parsed = "Value for CandidTypeNat32";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    std::string to_be_parsed = "Value for CandidTypeNat64";
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat64.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_float64.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,88 @@
-// The class for the Primitive Candid Type: nat64
-
-#include "candid.h"
+// The class for the Candid Type: vec
 
+#include "candid_type.h"
+#include "candid_type_vec_float64.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
-#include "pro.h"
 
-CandidTypeNat64::CandidTypeNat64() : CandidTypePrim() { initialize(0); }
+#include <cassert>
 
-// This constructor allows for setting the value during Deserialization
-CandidTypeNat64::CandidTypeNat64(uint64_t *p_v) : CandidTypePrim() {
 
-  set_pv(p_v);
 
-  const uint64_t v = const_cast<uint64_t &>(*p_v);
-  initialize(v);
+CandidTypeVecFloat64::CandidTypeVecFloat64() : CandidTypeVecBase() {
+  std::vector<double> v;
+  set_v(v);
+  initialize();
 }
 
-// This constructor is only for encoding
-CandidTypeNat64::CandidTypeNat64(const uint64_t v) : CandidTypePrim() {
+// These constructors allows for setting the value during Deserialization
+CandidTypeVecFloat64::CandidTypeVecFloat64(std::vector<double> *p_v)
+    : CandidTypeVecBase() {
+  set_pv(p_v);
 
-  initialize(v);
+  const std::vector<double> v = const_cast<std::vector<double> &>(*p_v);
+  set_v(v);
+  initialize();
 }
 
-CandidTypeNat64::~CandidTypeNat64() {}
-
-// Initialize things
-void CandidTypeNat64::initialize(const uint64_t &v) {
-  m_v = v;
-  set_datatype();
-  encode_I();
-  encode_M();
+// These constructors are only for encoding
+CandidTypeVecFloat64::CandidTypeVecFloat64(const std::vector<double> v)
+    : CandidTypeVecBase() {
+  set_v(v);
+  initialize();
 }
 
-// pointer to data in caller, for storing decoded value
-void CandidTypeNat64::set_pv(uint64_t *v) { m_pv = v; }
-
-void CandidTypeNat64::set_datatype() {
-  m_datatype_opcode = CandidOpcode().Nat64;
-  m_datatype_hex = OpcodeHex().Nat64;
-  m_datatype_textual = OpcodeTextual().Nat64;
-}
+CandidTypeVecFloat64::~CandidTypeVecFloat64() {}
 
-void CandidTypeNat64::encode_I() {
-  // https://github.com/dfinity/candid/blob/master/spec/Candid.md#types
-  // For <primtype>: the negative Opcode
-  m_I.append_byte((std::byte)m_datatype_hex);
+void CandidTypeVecFloat64::set_content_type() {
+  m_content_type_opcode = CandidOpcode().Float64;
+  m_content_type_hex = OpcodeHex().Float64;
+  m_content_type_textual = OpcodeTextual().Float64;
 }
 
-void CandidTypeNat64::encode_M() {
+void CandidTypeVecFloat64::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
-  // M(n : nat<N>)   = i<N>(n)    (Litte Endian)
-  m_M.append_int_fixed_width(m_v);
+  // M(v^N  : vec <datatype>) = leb128(N) M(v : <datatype>)^N
+
+  // encoded size of vec - leb128(N)
+  m_M.append_uleb128(__uint128_t(m_v.size()));
+
+  // encoded vec values - M(v : <datatype>)^N
+  // M(z : float<N>) = f<N>(z)
+  for (double const &c : m_v) {
+    m_M.append_float_ieee754(c);
+  }
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeNat64::decode_M(VecBytes B, __uint128_t &offset,
-                               std::string &parse_error) {
+bool CandidTypeVecFloat64::decode_M(VecBytes B, __uint128_t &offset,
+                                    std::string &parse_error) {
+  // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
+  __uint128_t numbytes;
   parse_error = "";
-  if (B.parse_int_fixed_width(offset, m_v, parse_error)) {
-    std::string to_be_parsed = "Value for CandidTypeNat64";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+  __uint128_t size_vec;
+  if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
+    std::string to_be_parsed = "Size of vec- leb128(N)";
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
+  m_v.clear();
+  double v;
+  offset_start = offset;
+  parse_error = "";
+  for (size_t i = 0; i < size_vec; ++i) {
+    if (B.parse_float_ieee754(offset, v, parse_error)) {
+      std::string to_be_parsed = "Vec: Value for CandidTypeFloat64";
+      CandidAssert::trap_with_parse_error(offset_start, offset,
+                                               to_be_parsed, parse_error);
+    }
+    m_v.push_back(v);
+  }
+
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat64.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-// The class for the Primitive Candid Type: nat64
+// The class for the Candid Type: vec
 
 #pragma once
 
-#include "candid.h"
+#include <cstring>
 
-class CandidTypeNat64 : public CandidTypePrim {
+#include "candid_type_vec_base.h"
+#include "candid_type_nat.h"
+#include "vec_bytes.h"
+
+class CandidTypeVecNat : public CandidTypeVecBase {
 public:
   // Constructors
-  CandidTypeNat64();
-  // docs start: demo_candid_type_nat64
-  CandidTypeNat64(uint64_t *v);
-  CandidTypeNat64(const uint64_t v); // docs end: demo_candid_type_nat64
+  CandidTypeVecNat();
+  CandidTypeVecNat(const std::vector<__uint128_t> v);
+
+  CandidTypeVecNat(std::vector<__uint128_t> *p_v);
 
   // Destructor
-  ~CandidTypeNat64();
+  ~CandidTypeVecNat();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  uint64_t get_v() { return m_v; }
+  std::vector<__uint128_t> get_v() { return m_v; }
 
 protected:
-  void set_pv(uint64_t *v);
-  void initialize(const uint64_t &v);
-  void set_datatype();
-  void encode_I();
+  void set_pv(std::vector<__uint128_t> *v) { m_pv = v; }
+  void set_v(const std::vector<__uint128_t> &v) { m_v = v; }
+  void set_content_type();
   void encode_M();
 
-  uint64_t m_v;
-  uint64_t *m_pv{nullptr};
+  std::vector<__uint128_t> m_v;
+  std::vector<__uint128_t> *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_nat8.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_nat16.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,73 @@
-// The class for the Primitive Candid Type: nat8
+// The class for the Primitive Candid Type: nat16
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_nat16.h"
+#include "candid_assert.h"
 
 #include "candid_opcode.h"
 #include "pro.h"
 
-CandidTypeNat8::CandidTypeNat8() : CandidTypePrim() { initialize(0); }
+CandidTypeNat16::CandidTypeNat16() { initialize(0); }
 
 // This constructor allows for setting the value during Deserialization
-CandidTypeNat8::CandidTypeNat8(uint8_t *p_v) : CandidTypePrim() {
+CandidTypeNat16::CandidTypeNat16(uint16_t *p_v) {
 
   set_pv(p_v);
 
-  const uint8_t v = const_cast<uint8_t &>(*p_v);
+  const uint16_t v = const_cast<uint16_t &>(*p_v);
   initialize(v);
 }
 
 // This constructor is only for encoding
-CandidTypeNat8::CandidTypeNat8(const uint8_t v) : CandidTypePrim() {
+CandidTypeNat16::CandidTypeNat16(const uint16_t v) {
 
   initialize(v);
 }
 
-CandidTypeNat8::~CandidTypeNat8() {}
+CandidTypeNat16::~CandidTypeNat16() {}
 
 // Initialize things
-void CandidTypeNat8::initialize(const uint8_t &v) {
+void CandidTypeNat16::initialize(const uint16_t &v) {
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
-void CandidTypeNat8::set_pv(uint8_t *v) { m_pv = v; }
+void CandidTypeNat16::set_pv(uint16_t *v) { m_pv = v; }
 
-void CandidTypeNat8::set_datatype() {
-  m_datatype_opcode = CandidOpcode().Nat8;
-  m_datatype_hex = OpcodeHex().Nat8;
-  m_datatype_textual = OpcodeTextual().Nat8;
+void CandidTypeNat16::set_datatype() {
+  m_datatype_opcode = CandidOpcode().Nat16;
+  m_datatype_hex = OpcodeHex().Nat16;
+  m_datatype_textual = OpcodeTextual().Nat16;
 }
 
-void CandidTypeNat8::encode_I() {
+void CandidTypeNat16::encode_I() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#types
   // For <primtype>: the negative Opcode
   m_I.append_byte((std::byte)m_datatype_hex);
 }
 
-void CandidTypeNat8::encode_M() {
+void CandidTypeNat16::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(n : nat<N>)   = i<N>(n)    (Litte Endian)
   m_M.append_int_fixed_width(m_v);
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeNat8::decode_M(VecBytes B, __uint128_t &offset,
-                              std::string &parse_error) {
+bool CandidTypeNat16::decode_M(VecBytes B, __uint128_t &offset,
+                               std::string &parse_error) {
   __uint128_t offset_start = offset;
   parse_error = "";
   if (B.parse_int_fixed_width(offset, m_v, parse_error)) {
-    std::string to_be_parsed = "Value for CandidTypeNat8";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    std::string to_be_parsed = "Value for CandidTypeNat16";
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_null.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_null.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Primitive Candid Type: null
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_null.h"
 
 #include "candid_opcode.h"
 
-CandidTypeNull::CandidTypeNull() : CandidTypePrim() {
+CandidTypeNull::CandidTypeNull() {
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 CandidTypeNull::~CandidTypeNull() {}
 
 void CandidTypeNull::set_datatype() {
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_base.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_base.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The base class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_base.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+
 #include "pro.h"
 
 CandidTypeOptBase::CandidTypeOptBase() : CandidTypeBase() {}
 
 CandidTypeOptBase::~CandidTypeOptBase() {}
 
 // Initialize things
@@ -41,15 +43,15 @@
   // The opcode for content type
   __uint128_t offset_start = offset;
   parse_error = "";
   __int128_t content_type;
   __uint128_t numbytes;
   if (B.parse_sleb128(offset, content_type, numbytes, parse_error)) {
     std::string to_be_parsed = "Type table: a Opt's content type";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_content_type_opcode = int(content_type);
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_bool.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_bool.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_bool.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidTypeOptBool::CandidTypeOptBool() : CandidTypeOptBase() {
   std::optional<bool> v;
   set_v(v);
   initialize();
 }
 
@@ -61,30 +63,30 @@
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
     offset_start = offset;
     parse_error = "";
     CandidTypeBool c{}; // dummy so we can use it's decode_M
     if (c.decode_M(B, offset, parse_error)) {
       std::string to_be_parsed = "Opt: Value for CandidTypeBool";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = c.get_v();
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt bool coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt bool coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_bool.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_bool.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_bool.h"
+#include "vec_bytes.h"
 
 class CandidTypeOptBool : public CandidTypeOptBase {
 public:
   // Constructors
   CandidTypeOptBool();
   // clang-format off
   // docs start: demo_candid_type_opt
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_float32.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_float32.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_float32.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidTypeOptFloat32::CandidTypeOptFloat32() : CandidTypeOptBase() {
   std::optional<float> v;
   set_v(v);
   initialize();
 }
 
@@ -61,30 +63,30 @@
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
     float v;
     offset_start = offset;
     parse_error = "";
     if (B.parse_float_ieee754(offset, v, parse_error)) {
       std::string to_be_parsed = "Opt: Value for CandidTypeFloat32";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt float32 coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt float32 coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_float32.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_float32.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_float32.h"
+#include "vec_bytes.h"
 
 class CandidTypeOptFloat32 : public CandidTypeOptBase {
 public:
   // Constructors
   CandidTypeOptFloat32();
   // clang-format off
   // docs start: demo_candid_type_opt
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_float64.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_float64.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_float64.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidTypeOptFloat64::CandidTypeOptFloat64() : CandidTypeOptBase() {
   std::optional<double> v;
   set_v(v);
   initialize();
 }
 
@@ -61,30 +63,30 @@
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
     double v;
     offset_start = offset;
     parse_error = "";
     if (B.parse_float_ieee754(offset, v, parse_error)) {
       std::string to_be_parsed = "Opt: Value for CandidTypeFloat64";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt float64 coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt float64 coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_float64.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_float64.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_float64.h"
+#include "vec_bytes.h"
 
 class CandidTypeOptFloat64 : public CandidTypeOptBase {
 public:
   // Constructors
   CandidTypeOptFloat64();
   // clang-format off
   // docs start: demo_candid_type_opt
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_int.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidTypeOptInt::CandidTypeOptInt() : CandidTypeOptBase() {
   std::optional<__int128_t> v;
   set_v(v);
   initialize();
 }
 
@@ -62,31 +64,31 @@
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
     __int128_t v;
     offset_start = offset;
     __uint128_t numbytes;
     parse_error = "";
     if (B.parse_sleb128(offset, v, numbytes, parse_error)) {
       std::string to_be_parsed = "Opt: Value for CandidTypeInt";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt int coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt int coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_int.h"
+#include "vec_bytes.h"
 
 class CandidTypeOptInt : public CandidTypeOptBase {
 public:
   // Constructors
   CandidTypeOptInt();
   // clang-format off
   // docs start: demo_candid_type_opt
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int16.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int16.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_int16.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
+#include "icpp_hooks.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+
 
 CandidTypeOptInt16::CandidTypeOptInt16() : CandidTypeOptBase() {
   std::optional<int16_t> v;
   set_v(v);
   initialize();
 }
 
@@ -61,30 +64,30 @@
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
     int16_t v;
     offset_start = offset;
     parse_error = "";
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
       std::string to_be_parsed = "Opt: Value for CandidTypeInt16";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt int16 coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt int16 coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int16.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int8.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_int8.h"
+#include "vec_bytes.h"
 
-class CandidTypeOptInt16 : public CandidTypeOptBase {
+class CandidTypeOptInt8 : public CandidTypeOptBase {
 public:
   // Constructors
-  CandidTypeOptInt16();
+  CandidTypeOptInt8();
   // clang-format off
   // docs start: demo_candid_type_opt
-  CandidTypeOptInt16(std::optional<int16_t> *v);
-  CandidTypeOptInt16(const std::optional<int16_t> v); // docs end: demo_candid_type_opt
+  CandidTypeOptInt8(std::optional<int8_t> *v);
+  CandidTypeOptInt8(const std::optional<int8_t> v); // docs end: demo_candid_type_opt
   // clang-format on
 
   // Destructor
-  ~CandidTypeOptInt16();
+  ~CandidTypeOptInt8();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  std::optional<int16_t> get_v() { return m_v; }
+  std::optional<int8_t> get_v() { return m_v; }
 
 protected:
-  void set_pv(std::optional<int16_t> *v) { m_pv = v; }
-  void set_v(const std::optional<int16_t> &v) { m_v = v; }
+  void set_pv(std::optional<int8_t> *v) { m_pv = v; }
+  void set_v(const std::optional<int8_t> &v) { m_v = v; }
   void set_content_type();
   void encode_M();
 
-  std::optional<int16_t> m_v;
-  std::optional<int16_t> *m_pv{nullptr};
+  std::optional<int8_t> m_v;
+  std::optional<int8_t> *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int32.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int32.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_int32.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidTypeOptInt32::CandidTypeOptInt32() : CandidTypeOptBase() {
   std::optional<int32_t> v;
   set_v(v);
   initialize();
 }
 
@@ -61,30 +63,30 @@
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
     int32_t v;
     offset_start = offset;
     parse_error = "";
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
       std::string to_be_parsed = "Opt: Value for CandidTypeInt32";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt int32 coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt int32 coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int32.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int32.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_int32.h"
+#include "vec_bytes.h"
 
 class CandidTypeOptInt32 : public CandidTypeOptBase {
 public:
   // Constructors
   CandidTypeOptInt32();
   // clang-format off
   // docs start: demo_candid_type_opt
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int64.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int64.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_int64.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidTypeOptInt64::CandidTypeOptInt64() : CandidTypeOptBase() {
   std::optional<int64_t> v;
   set_v(v);
   initialize();
 }
 
@@ -61,30 +63,30 @@
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
     int64_t v;
     offset_start = offset;
     parse_error = "";
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
       std::string to_be_parsed = "Opt: Value for CandidTypeInt64";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt int64 coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt int64 coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int64.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_nat.h"
+#include "vec_bytes.h"
 
-class CandidTypeOptInt64 : public CandidTypeOptBase {
+class CandidTypeOptNat : public CandidTypeOptBase {
 public:
   // Constructors
-  CandidTypeOptInt64();
+  CandidTypeOptNat();
   // clang-format off
   // docs start: demo_candid_type_opt
-  CandidTypeOptInt64(std::optional<int64_t> *v);
-  CandidTypeOptInt64(const std::optional<int64_t> v); // docs end: demo_candid_type_opt
+  CandidTypeOptNat(std::optional<__uint128_t> *v);
+  CandidTypeOptNat(const std::optional<__uint128_t> v); // docs end: demo_candid_type_opt
   // clang-format on
 
   // Destructor
-  ~CandidTypeOptInt64();
+  ~CandidTypeOptNat();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  std::optional<int64_t> get_v() { return m_v; }
+  std::optional<__uint128_t> get_v() { return m_v; }
 
 protected:
-  void set_pv(std::optional<int64_t> *v) { m_pv = v; }
-  void set_v(const std::optional<int64_t> &v) { m_v = v; }
+  void set_pv(std::optional<__uint128_t> *v) { m_pv = v; }
+  void set_v(const std::optional<__uint128_t> &v) { m_v = v; }
   void set_content_type();
   void encode_M();
 
-  std::optional<int64_t> m_v;
-  std::optional<int64_t> *m_pv{nullptr};
+  std::optional<__uint128_t> m_v;
+  std::optional<__uint128_t> *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int8.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int8.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_int8.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidTypeOptInt8::CandidTypeOptInt8() : CandidTypeOptBase() {
   std::optional<int8_t> v;
   set_v(v);
   initialize();
 }
 
@@ -61,30 +63,30 @@
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
     int8_t v;
     offset_start = offset;
     parse_error = "";
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
       std::string to_be_parsed = "Opt: Value for CandidTypeInt8";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt int8 coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt int8 coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_int8.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat64.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_nat64.h"
+#include "vec_bytes.h"
 
-class CandidTypeOptInt8 : public CandidTypeOptBase {
+class CandidTypeOptNat64 : public CandidTypeOptBase {
 public:
   // Constructors
-  CandidTypeOptInt8();
+  CandidTypeOptNat64();
   // clang-format off
   // docs start: demo_candid_type_opt
-  CandidTypeOptInt8(std::optional<int8_t> *v);
-  CandidTypeOptInt8(const std::optional<int8_t> v); // docs end: demo_candid_type_opt
+  CandidTypeOptNat64(std::optional<uint64_t> *v);
+  CandidTypeOptNat64(const std::optional<uint64_t> v); // docs end: demo_candid_type_opt
   // clang-format on
 
   // Destructor
-  ~CandidTypeOptInt8();
+  ~CandidTypeOptNat64();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  std::optional<int8_t> get_v() { return m_v; }
+  std::optional<uint64_t> get_v() { return m_v; }
 
 protected:
-  void set_pv(std::optional<int8_t> *v) { m_pv = v; }
-  void set_v(const std::optional<int8_t> &v) { m_v = v; }
+  void set_pv(std::optional<uint64_t> *v) { m_pv = v; }
+  void set_v(const std::optional<uint64_t> &v) { m_v = v; }
   void set_content_type();
   void encode_M();
 
-  std::optional<int8_t> m_v;
-  std::optional<int8_t> *m_pv{nullptr};
+  std::optional<uint64_t> m_v;
+  std::optional<uint64_t> *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_nat.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidTypeOptNat::CandidTypeOptNat() : CandidTypeOptBase() {
   std::optional<__uint128_t> v;
   set_v(v);
   initialize();
 }
 
@@ -62,31 +64,31 @@
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
     __uint128_t v;
     offset_start = offset;
     __uint128_t numbytes;
     parse_error = "";
     if (B.parse_uleb128(offset, v, numbytes, parse_error)) {
       std::string to_be_parsed = "Opt: Value for CandidTypeNat";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt nat coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt nat coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat8.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_nat8.h"
+#include "vec_bytes.h"
 
-class CandidTypeOptNat : public CandidTypeOptBase {
+class CandidTypeOptNat8 : public CandidTypeOptBase {
 public:
   // Constructors
-  CandidTypeOptNat();
+  CandidTypeOptNat8();
   // clang-format off
   // docs start: demo_candid_type_opt
-  CandidTypeOptNat(std::optional<__uint128_t> *v);
-  CandidTypeOptNat(const std::optional<__uint128_t> v); // docs end: demo_candid_type_opt
+  CandidTypeOptNat8(std::optional<uint8_t> *v);
+  CandidTypeOptNat8(const std::optional<uint8_t> v); // docs end: demo_candid_type_opt
   // clang-format on
 
   // Destructor
-  ~CandidTypeOptNat();
+  ~CandidTypeOptNat8();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  std::optional<__uint128_t> get_v() { return m_v; }
+  std::optional<uint8_t> get_v() { return m_v; }
 
 protected:
-  void set_pv(std::optional<__uint128_t> *v) { m_pv = v; }
-  void set_v(const std::optional<__uint128_t> &v) { m_v = v; }
+  void set_pv(std::optional<uint8_t> *v) { m_pv = v; }
+  void set_v(const std::optional<uint8_t> &v) { m_v = v; }
   void set_content_type();
   void encode_M();
 
-  std::optional<__uint128_t> m_v;
-  std::optional<__uint128_t> *m_pv{nullptr};
+  std::optional<uint8_t> m_v;
+  std::optional<uint8_t> *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat16.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat32.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_nat32.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
-CandidTypeOptNat16::CandidTypeOptNat16() : CandidTypeOptBase() {
-  std::optional<uint16_t> v;
+CandidTypeOptNat32::CandidTypeOptNat32() : CandidTypeOptBase() {
+  std::optional<uint32_t> v;
   set_v(v);
   initialize();
 }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypeOptNat16::CandidTypeOptNat16(std::optional<uint16_t> *p_v)
+CandidTypeOptNat32::CandidTypeOptNat32(std::optional<uint32_t> *p_v)
     : CandidTypeOptBase() {
   set_pv(p_v);
 
-  const std::optional<uint16_t> v = const_cast<std::optional<uint16_t> &>(*p_v);
+  const std::optional<uint32_t> v = const_cast<std::optional<uint32_t> &>(*p_v);
   set_v(v);
   initialize();
 }
 
 // These constructors are only for encoding
-CandidTypeOptNat16::CandidTypeOptNat16(const std::optional<uint16_t> v)
+CandidTypeOptNat32::CandidTypeOptNat32(const std::optional<uint32_t> v)
     : CandidTypeOptBase() {
   set_v(v);
   initialize();
 }
 
-CandidTypeOptNat16::~CandidTypeOptNat16() {}
+CandidTypeOptNat32::~CandidTypeOptNat32() {}
 
-void CandidTypeOptNat16::set_content_type() {
-  m_content_type_opcode = CandidOpcode().Nat16;
-  m_content_type_hex = OpcodeHex().Nat16;
-  m_content_type_textual = OpcodeTextual().Nat16;
+void CandidTypeOptNat32::set_content_type() {
+  m_content_type_opcode = CandidOpcode().Nat32;
+  m_content_type_hex = OpcodeHex().Nat32;
+  m_content_type_textual = OpcodeTextual().Nat32;
 }
 
-void CandidTypeOptNat16::encode_M() {
+void CandidTypeOptNat32::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(null : opt <datatype>) = i8(0)
   // M(?v   : opt <datatype>) = i8(1) M(v : <datatype>)
 
   if (!m_v.has_value()) {
     m_M.append_int_fixed_width(uint8_t{0});
   } else {
     m_M.append_int_fixed_width(uint8_t{1});
     m_M.append_int_fixed_width(m_v.value());
   }
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeOptNat16::decode_M(VecBytes B, __uint128_t &offset,
+bool CandidTypeOptNat32::decode_M(VecBytes B, __uint128_t &offset,
                                   std::string &parse_error) {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(null : opt <datatype>) = i8(0)
   // M(?v   : opt <datatype>) = i8(1) M(v : <datatype>)
 
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
-    uint16_t v;
+    uint32_t v;
     offset_start = offset;
     parse_error = "";
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
-      std::string to_be_parsed = "Opt: Value for CandidTypeNat16";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      std::string to_be_parsed = "Opt: Value for CandidTypeNat32";
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt nat16 coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt nat32 coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat16.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat16.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_nat16.h"
+#include "vec_bytes.h"
 
 class CandidTypeOptNat16 : public CandidTypeOptBase {
 public:
   // Constructors
   CandidTypeOptNat16();
   // clang-format off
   // docs start: demo_candid_type_opt
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat32.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat8.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_nat8.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
-CandidTypeOptNat32::CandidTypeOptNat32() : CandidTypeOptBase() {
-  std::optional<uint32_t> v;
+CandidTypeOptNat8::CandidTypeOptNat8() : CandidTypeOptBase() {
+  std::optional<uint8_t> v;
   set_v(v);
   initialize();
 }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypeOptNat32::CandidTypeOptNat32(std::optional<uint32_t> *p_v)
+CandidTypeOptNat8::CandidTypeOptNat8(std::optional<uint8_t> *p_v)
     : CandidTypeOptBase() {
   set_pv(p_v);
 
-  const std::optional<uint32_t> v = const_cast<std::optional<uint32_t> &>(*p_v);
+  const std::optional<uint8_t> v = const_cast<std::optional<uint8_t> &>(*p_v);
   set_v(v);
   initialize();
 }
 
 // These constructors are only for encoding
-CandidTypeOptNat32::CandidTypeOptNat32(const std::optional<uint32_t> v)
+CandidTypeOptNat8::CandidTypeOptNat8(const std::optional<uint8_t> v)
     : CandidTypeOptBase() {
   set_v(v);
   initialize();
 }
 
-CandidTypeOptNat32::~CandidTypeOptNat32() {}
+CandidTypeOptNat8::~CandidTypeOptNat8() {}
 
-void CandidTypeOptNat32::set_content_type() {
-  m_content_type_opcode = CandidOpcode().Nat32;
-  m_content_type_hex = OpcodeHex().Nat32;
-  m_content_type_textual = OpcodeTextual().Nat32;
+void CandidTypeOptNat8::set_content_type() {
+  m_content_type_opcode = CandidOpcode().Nat8;
+  m_content_type_hex = OpcodeHex().Nat8;
+  m_content_type_textual = OpcodeTextual().Nat8;
 }
 
-void CandidTypeOptNat32::encode_M() {
+void CandidTypeOptNat8::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(null : opt <datatype>) = i8(0)
   // M(?v   : opt <datatype>) = i8(1) M(v : <datatype>)
 
   if (!m_v.has_value()) {
     m_M.append_int_fixed_width(uint8_t{0});
   } else {
     m_M.append_int_fixed_width(uint8_t{1});
     m_M.append_int_fixed_width(m_v.value());
   }
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeOptNat32::decode_M(VecBytes B, __uint128_t &offset,
-                                  std::string &parse_error) {
+bool CandidTypeOptNat8::decode_M(VecBytes B, __uint128_t &offset,
+                                 std::string &parse_error) {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(null : opt <datatype>) = i8(0)
   // M(?v   : opt <datatype>) = i8(1) M(v : <datatype>)
 
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
-    uint32_t v;
+    uint8_t v;
     offset_start = offset;
     parse_error = "";
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
-      std::string to_be_parsed = "Opt: Value for CandidTypeNat32";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      std::string to_be_parsed = "Opt: Value for CandidTypeNat8";
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt nat32 coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt nat8 coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat32.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat32.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_nat32.h"
+#include "vec_bytes.h"
 
 class CandidTypeOptNat32 : public CandidTypeOptBase {
 public:
   // Constructors
   CandidTypeOptNat32();
   // clang-format off
   // docs start: demo_candid_type_opt
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat64.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat16.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_nat16.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
-CandidTypeOptNat64::CandidTypeOptNat64() : CandidTypeOptBase() {
-  std::optional<uint64_t> v;
+CandidTypeOptNat16::CandidTypeOptNat16() : CandidTypeOptBase() {
+  std::optional<uint16_t> v;
   set_v(v);
   initialize();
 }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypeOptNat64::CandidTypeOptNat64(std::optional<uint64_t> *p_v)
+CandidTypeOptNat16::CandidTypeOptNat16(std::optional<uint16_t> *p_v)
     : CandidTypeOptBase() {
   set_pv(p_v);
 
-  const std::optional<uint64_t> v = const_cast<std::optional<uint64_t> &>(*p_v);
+  const std::optional<uint16_t> v = const_cast<std::optional<uint16_t> &>(*p_v);
   set_v(v);
   initialize();
 }
 
 // These constructors are only for encoding
-CandidTypeOptNat64::CandidTypeOptNat64(const std::optional<uint64_t> v)
+CandidTypeOptNat16::CandidTypeOptNat16(const std::optional<uint16_t> v)
     : CandidTypeOptBase() {
   set_v(v);
   initialize();
 }
 
-CandidTypeOptNat64::~CandidTypeOptNat64() {}
+CandidTypeOptNat16::~CandidTypeOptNat16() {}
 
-void CandidTypeOptNat64::set_content_type() {
-  m_content_type_opcode = CandidOpcode().Nat64;
-  m_content_type_hex = OpcodeHex().Nat64;
-  m_content_type_textual = OpcodeTextual().Nat64;
+void CandidTypeOptNat16::set_content_type() {
+  m_content_type_opcode = CandidOpcode().Nat16;
+  m_content_type_hex = OpcodeHex().Nat16;
+  m_content_type_textual = OpcodeTextual().Nat16;
 }
 
-void CandidTypeOptNat64::encode_M() {
+void CandidTypeOptNat16::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(null : opt <datatype>) = i8(0)
   // M(?v   : opt <datatype>) = i8(1) M(v : <datatype>)
 
   if (!m_v.has_value()) {
     m_M.append_int_fixed_width(uint8_t{0});
   } else {
     m_M.append_int_fixed_width(uint8_t{1});
     m_M.append_int_fixed_width(m_v.value());
   }
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeOptNat64::decode_M(VecBytes B, __uint128_t &offset,
+bool CandidTypeOptNat16::decode_M(VecBytes B, __uint128_t &offset,
                                   std::string &parse_error) {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(null : opt <datatype>) = i8(0)
   // M(?v   : opt <datatype>) = i8(1) M(v : <datatype>)
 
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
-    uint64_t v;
+    uint16_t v;
     offset_start = offset;
     parse_error = "";
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
-      std::string to_be_parsed = "Opt: Value for CandidTypeNat64";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      std::string to_be_parsed = "Opt: Value for CandidTypeNat16";
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt nat64 coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt nat16 coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat64.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int64.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_int64.h"
+#include "vec_bytes.h"
 
-class CandidTypeOptNat64 : public CandidTypeOptBase {
+class CandidTypeOptInt64 : public CandidTypeOptBase {
 public:
   // Constructors
-  CandidTypeOptNat64();
+  CandidTypeOptInt64();
   // clang-format off
   // docs start: demo_candid_type_opt
-  CandidTypeOptNat64(std::optional<uint64_t> *v);
-  CandidTypeOptNat64(const std::optional<uint64_t> v); // docs end: demo_candid_type_opt
+  CandidTypeOptInt64(std::optional<int64_t> *v);
+  CandidTypeOptInt64(const std::optional<int64_t> v); // docs end: demo_candid_type_opt
   // clang-format on
 
   // Destructor
-  ~CandidTypeOptNat64();
+  ~CandidTypeOptInt64();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  std::optional<uint64_t> get_v() { return m_v; }
+  std::optional<int64_t> get_v() { return m_v; }
 
 protected:
-  void set_pv(std::optional<uint64_t> *v) { m_pv = v; }
-  void set_v(const std::optional<uint64_t> &v) { m_v = v; }
+  void set_pv(std::optional<int64_t> *v) { m_pv = v; }
+  void set_v(const std::optional<int64_t> &v) { m_v = v; }
   void set_content_type();
   void encode_M();
 
-  std::optional<uint64_t> m_v;
-  std::optional<uint64_t> *m_pv{nullptr};
+  std::optional<int64_t> m_v;
+  std::optional<int64_t> *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat8.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_nat64.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_nat64.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
-CandidTypeOptNat8::CandidTypeOptNat8() : CandidTypeOptBase() {
-  std::optional<uint8_t> v;
+CandidTypeOptNat64::CandidTypeOptNat64() : CandidTypeOptBase() {
+  std::optional<uint64_t> v;
   set_v(v);
   initialize();
 }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypeOptNat8::CandidTypeOptNat8(std::optional<uint8_t> *p_v)
+CandidTypeOptNat64::CandidTypeOptNat64(std::optional<uint64_t> *p_v)
     : CandidTypeOptBase() {
   set_pv(p_v);
 
-  const std::optional<uint8_t> v = const_cast<std::optional<uint8_t> &>(*p_v);
+  const std::optional<uint64_t> v = const_cast<std::optional<uint64_t> &>(*p_v);
   set_v(v);
   initialize();
 }
 
 // These constructors are only for encoding
-CandidTypeOptNat8::CandidTypeOptNat8(const std::optional<uint8_t> v)
+CandidTypeOptNat64::CandidTypeOptNat64(const std::optional<uint64_t> v)
     : CandidTypeOptBase() {
   set_v(v);
   initialize();
 }
 
-CandidTypeOptNat8::~CandidTypeOptNat8() {}
+CandidTypeOptNat64::~CandidTypeOptNat64() {}
 
-void CandidTypeOptNat8::set_content_type() {
-  m_content_type_opcode = CandidOpcode().Nat8;
-  m_content_type_hex = OpcodeHex().Nat8;
-  m_content_type_textual = OpcodeTextual().Nat8;
+void CandidTypeOptNat64::set_content_type() {
+  m_content_type_opcode = CandidOpcode().Nat64;
+  m_content_type_hex = OpcodeHex().Nat64;
+  m_content_type_textual = OpcodeTextual().Nat64;
 }
 
-void CandidTypeOptNat8::encode_M() {
+void CandidTypeOptNat64::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(null : opt <datatype>) = i8(0)
   // M(?v   : opt <datatype>) = i8(1) M(v : <datatype>)
 
   if (!m_v.has_value()) {
     m_M.append_int_fixed_width(uint8_t{0});
   } else {
     m_M.append_int_fixed_width(uint8_t{1});
     m_M.append_int_fixed_width(m_v.value());
   }
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeOptNat8::decode_M(VecBytes B, __uint128_t &offset,
-                                 std::string &parse_error) {
+bool CandidTypeOptNat64::decode_M(VecBytes B, __uint128_t &offset,
+                                  std::string &parse_error) {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(null : opt <datatype>) = i8(0)
   // M(?v   : opt <datatype>) = i8(1) M(v : <datatype>)
 
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
-    uint8_t v;
+    uint64_t v;
     offset_start = offset;
     parse_error = "";
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
-      std::string to_be_parsed = "Opt: Value for CandidTypeNat8";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      std::string to_be_parsed = "Opt: Value for CandidTypeNat64";
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = v;
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt nat8 coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt nat64 coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_nat8.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_int16.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_int16.h"
+#include "vec_bytes.h"
 
-class CandidTypeOptNat8 : public CandidTypeOptBase {
+class CandidTypeOptInt16 : public CandidTypeOptBase {
 public:
   // Constructors
-  CandidTypeOptNat8();
+  CandidTypeOptInt16();
   // clang-format off
   // docs start: demo_candid_type_opt
-  CandidTypeOptNat8(std::optional<uint8_t> *v);
-  CandidTypeOptNat8(const std::optional<uint8_t> v); // docs end: demo_candid_type_opt
+  CandidTypeOptInt16(std::optional<int16_t> *v);
+  CandidTypeOptInt16(const std::optional<int16_t> v); // docs end: demo_candid_type_opt
   // clang-format on
 
   // Destructor
-  ~CandidTypeOptNat8();
+  ~CandidTypeOptInt16();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  std::optional<uint8_t> get_v() { return m_v; }
+  std::optional<int16_t> get_v() { return m_v; }
 
 protected:
-  void set_pv(std::optional<uint8_t> *v) { m_pv = v; }
-  void set_v(const std::optional<uint8_t> &v) { m_v = v; }
+  void set_pv(std::optional<int16_t> *v) { m_pv = v; }
+  void set_v(const std::optional<int16_t> &v) { m_v = v; }
   void set_content_type();
   void encode_M();
 
-  std::optional<uint8_t> m_v;
-  std::optional<uint8_t> *m_pv{nullptr};
+  std::optional<int16_t> m_v;
+  std::optional<int16_t> *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_principal.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_principal.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_principal.h"
+#include "candid_type_principal.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidTypeOptPrincipal::CandidTypeOptPrincipal() : CandidTypeOptBase() {
   std::optional<std::string> v;
   set_v(v);
   initialize();
 }
 
@@ -67,30 +70,30 @@
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
     offset_start = offset;
     parse_error = "";
     CandidTypePrincipal c{}; // dummy so we can use it's decode_M
     if (c.decode_M(B, offset, parse_error)) {
       std::string to_be_parsed = "Opt: Value for CandidTypePrincipal";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = c.get_v();
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt principal coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt principal coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_principal.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_principal.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_principal.h"
+#include "vec_bytes.h"
 
 class CandidTypeOptPrincipal : public CandidTypeOptBase {
 public:
   // Constructors
   CandidTypeOptPrincipal();
   // clang-format off
   // docs start: demo_candid_type_opt
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_text.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_text.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 // The class for the Candid Type: opt
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_opt_text.h"
+#include "candid_type_text.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 CandidTypeOptText::CandidTypeOptText() : CandidTypeOptBase() {
   std::optional<std::string> v;
   set_v(v);
   initialize();
 }
 
@@ -70,30 +73,30 @@
   // get tag of opt - i8(0)
   // this will also work if there is a null on the wire.
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t tag;
   if (B.parse_int_fixed_width(offset, tag, parse_error)) {
     std::string to_be_parsed = "Opt tag.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (tag == 1) {
     offset_start = offset;
     parse_error = "";
     CandidTypeText c{}; // dummy so we can use it's decode_M
     if (c.decode_M(B, offset, parse_error)) {
       std::string to_be_parsed = "Opt: Value for CandidTypeText";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v = c.get_v();
 
   } else if (tag != 0) {
-    IC_API::trap("ERROR: tag in opt text coming from wire is not 0 or 1");
+    ICPP_HOOKS::trap("ERROR: tag in opt text coming from wire is not 0 or 1");
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_opt_text.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_opt_text.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: opt
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_opt_base.h"
+#include "candid_type_text.h"
+#include "vec_bytes.h"
 
 class CandidTypeOptText : public CandidTypeOptBase {
 public:
   // Constructors
   CandidTypeOptText();
   // clang-format off
   // docs start: demo_candid_type_opt
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_principal.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_principal.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 // The class for the Primitive Candid Type: text
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_principal.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 #include "pro.h"
 
 #include <cassert>
 
 #include "cppcodec/base32_rfc4648.hpp"
 #include "hash-library/crc32.h"
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 // DON'T PUT DATA IN GLOBAL/STATIC MEMORY. IT BREAKS ALL UPDATE CALLS
 //                                                               data_bytes
 // const std::string PRINCIPAL_ID_ANONYMOUS = "2vxsx-fae";          // 1 byte: x04
 // const std::string PRINCIPAL_ID_MANAGEMENT_CANISTER = "aaaaa-aa"; // no bytes
 
 // const uint32_t MAX_LENGTH_IN_BYTES = 29;
@@ -32,38 +34,38 @@
 // const std::string PRINCIPAL_ERROR_CHECK_SEQUENCE_NOT_MATCH =
 //     "Principal Error: CRC32 checksum doesn't match.";
 // const std::string PRINCIPAL_ERROR_ABNORMAL_GROUPED =
 //     "Principal Error: Text should be separated by - (dash) every 5 characters";
 // const std::string PRINCIPAL_ERROR_INVALID_BASE32_ENCODING =
 //     "Principal Error: Text must be in valid Base32 encoding. Decoding/Encoding roundtrip fails.";
 
-CandidTypePrincipal::CandidTypePrincipal() : CandidTypePrim() {
+CandidTypePrincipal::CandidTypePrincipal() {
   initialize("");
 }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypePrincipal::CandidTypePrincipal(std::string *p_v) : CandidTypePrim() {
+CandidTypePrincipal::CandidTypePrincipal(std::string *p_v) {
   set_pv(p_v);
 
   const std::string v = const_cast<std::string &>(*p_v);
   initialize(v);
 }
 
 // These constructors are only for encoding
-CandidTypePrincipal::CandidTypePrincipal(const char *c) : CandidTypePrim() {
+CandidTypePrincipal::CandidTypePrincipal(const char *c) {
   std::string v(c);
   initialize(v);
 }
 CandidTypePrincipal::CandidTypePrincipal(const std::string v)
-    : CandidTypePrim() {
+    {
   initialize(v);
 }
-// Constructor used by IC_API::from_wire to store caller
+// Constructor used by ICPP_HOOKS::from_wire to store caller
 CandidTypePrincipal::CandidTypePrincipal(const std::vector<uint8_t> &bytes)
-    : CandidTypePrim() {
+    {
   std::string v = string_from_bytes(bytes);
   initialize(v);
 }
 
 CandidTypePrincipal::~CandidTypePrincipal() {}
 
 // Initialize things
@@ -71,14 +73,15 @@
   if (v == "") {
     m_v = "2vxsx-fae";
     // Fill the user's data placeholder, if a pointer was provided
     if (m_pv) *m_pv = m_v;
   } else m_v = v;
   bytes_from_string();
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
 void CandidTypePrincipal::set_pv(std::string *v) { m_pv = v; }
 
@@ -119,38 +122,38 @@
   // Get the unused opaque reference: i8(0)
   // Verify that the value is 1. This is the convention
   __uint128_t offset_start = offset;
   parse_error = "";
   uint8_t ref_r;
   if (B.parse_int_fixed_width(offset, ref_r, parse_error)) {
     std::string to_be_parsed = "Unused opaque reference.";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (ref_r != 1) {
-    IC_API::trap(
+    ICPP_HOOKS::trap(
         "Principal Error: Found a value different that 1 for the reference. Opaque reference not supported.");
   }
 
   // Get the length
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t numBytes_principal;
   if (B.parse_uleb128(offset, numBytes_principal, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of data bytes for principal";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // Get the encoded principal bytes as uint8_t
   std::vector<uint8_t> data_bytes;
   if (B.parse_bytes(offset, data_bytes, numBytes_principal, numbytes,
                     parse_error)) {
     std::string to_be_parsed = "Data bytes for principal";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v = string_from_bytes(data_bytes);
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
@@ -165,54 +168,54 @@
 
   std::string s = m_v;
   ungroup(s);
   make_ascii_uppercase(s);
   std::vector<uint8_t> bytes = base32_decode(s);
 
   if (bytes.size() < 4) {
-    IC_API::trap("Principal Error: Text is too short.");
+    ICPP_HOOKS::trap("Principal Error: Text is too short.");
   }
 
   // First 4 bytes are a CRC32 checksum of the data that follows. The data bytes are the principal ID
   std::vector<uint8_t> crc_bytes(bytes.begin(), bytes.begin() + 4);
   std::vector<uint8_t> data_bytes(bytes.begin() + 4, bytes.end());
 
   if (data_bytes.size() > 29) {
-    IC_API::trap("Principal Error: Text is too long.");
+    ICPP_HOOKS::trap("Principal Error: Text is too long.");
   }
 
   // Verify the CRC32 checksum of the data bytes
   std::array<uint8_t, 4> crc_data = crc32(data_bytes);
   if (!std::equal(crc_bytes.begin(), crc_bytes.end(), crc_data.begin())) {
-    IC_API::trap("Principal Error: CRC32 checksum doesn't match.");
+    ICPP_HOOKS::trap("Principal Error: CRC32 checksum doesn't match.");
   }
 
   // from https://internetcomputer.org/docs/current/references/id-encoding-spec
   //   w3gef-eqbai -> 0102 -> w3gef-eqbai
   //   w3gef-eqbaj -> 0102 -> w3gef-eqbai ==> Error due to non-zero padding bits
   //
   // Verify that roundtrip back to string gives same result
   std::string s_roundtrip = string_from_bytes(data_bytes);
   if (s_roundtrip != m_v) {
-    IC_API::trap(
+    ICPP_HOOKS::trap(
         "Principal Error: Text must be in valid Base32 encoding. Decoding/Encoding roundtrip fails.");
   }
 
   // All is OK, store the bytes of the Principal ID
   m_v_bytes.append_bytes(data_bytes.data(), data_bytes.size());
 }
 
 // convert bytes of principal into string representation
 std::string
 CandidTypePrincipal::string_from_bytes(const std::vector<uint8_t> &data_bytes) {
   // spec: https://internetcomputer.org/docs/current/references/id-encoding-spec
   // m_v = Encode(data) := Group(LowerCase(Base32(CRC32(data) || data)))
 
   if (data_bytes.size() > 29) {
-    IC_API::trap("Principal Error: Text is too long.");
+    ICPP_HOOKS::trap("Principal Error: Text is too long.");
   }
 
   // CRC32(data) - checksum of the data bytes
   std::array<uint8_t, 4> crc_bytes = crc32(data_bytes);
 
   // Base32(CRC32(data) || data)
   std::vector<uint8_t> bytes(crc_bytes.begin(), crc_bytes.end());
@@ -225,15 +228,15 @@
 
   return s;
 }
 
 void CandidTypePrincipal::ungroup(std::string &s) {
   for (size_t i = 5; i < s.size(); i += 6) {
     if (s[i] != '-') {
-      IC_API::trap(
+      ICPP_HOOKS::trap(
           "Principal Error: Text should be separated by - (dash) every 5 characters");
     }
   }
   s.erase(std::remove(s.begin(), s.end(), '-'), s.end());
 }
 
 void CandidTypePrincipal::group(std::string &s) {
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_principal.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_principal.h`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 #include <algorithm>
 #include <array>
 #include <cassert>
 #include <cmath>
 #include <cstring>
 
-#include "candid.h"
-#include "candid_type_prim.h"
+#include "candid_type_base.h"
 #include "vec_bytes.h"
 
-class CandidTypePrincipal : public CandidTypePrim {
+class CandidTypePrincipal : public CandidTypeBase {
 public:
   // Constructors
   CandidTypePrincipal();
   CandidTypePrincipal(const char *c);
   // clang-format off
   // docs start: demo_candid_type_principal
   CandidTypePrincipal(const std::string v); // docs end: demo_candid_type_principal
@@ -25,24 +24,28 @@
   CandidTypePrincipal(std::string *v);
 
   CandidTypePrincipal(const std::vector<uint8_t> &bytes);
 
   // Destructor
   ~CandidTypePrincipal();
 
+  bool decode_T(VecBytes B, __uint128_t &offset, std::string &parse_error) {
+    return false; // type table for Primitives is empty
+  }
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
   std::string get_v() { return m_v; }
   std::string get_text() { return m_v; }
   const VecBytes &get_v_bytes() const { return m_v_bytes; }
   bool is_anonymous();
 
 protected:
   void set_pv(std::string *v);
   void initialize(const std::string &v);
   void set_datatype();
+  void encode_T() { m_T.clear(); } // type table for Primitives is empty
   void encode_I();
   void encode_M();
   void bytes_from_string();
   std::string string_from_bytes(const std::vector<uint8_t> &data_bytes);
 
   void make_ascii_uppercase(std::string &s) {
     std::transform(s.begin(), s.end(), s.begin(), ::toupper);
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_record.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_record.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 // The class for the Candid Type: Record
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_all_includes.h"
+#include "candid_type_record.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 #include "pro.h"
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 #include <algorithm>
 #include <cassert>
 #include <utility>
 
 CandidTypeRecord::CandidTypeRecord() : CandidTypeBase() {
 
@@ -36,70 +39,73 @@
 void CandidTypeRecord::append(std::string field_name, CandidType field) {
   uint32_t field_id = idl_hash(field_name);
   _append(field_id, field_name, field);
 }
 
 // Tuple notation without field_id -> generate sequential uint32_t field_id
 void CandidTypeRecord::append(CandidType field) {
-  if (m_fields.size() == 0) {
+  if (m_fields_ptrs.size() == 0) {
     uint32_t field_id = 0;
     append(field_id, field);
   }
 
   if (std::in_range<std::uint32_t>(m_field_ids.back() + 1)) {
     uint32_t field_id = m_field_ids.back() + 1;
     append(field_id, field);
   } else {
     std::string msg;
     msg.append("ERROR: field_id outside range of uint32_t\n");
     msg.append("       id of previous field in record: " +
                std::to_string(m_field_ids.back()) + "\n");
     msg.append(
         "       because no field_id was specified for current field, we want to increase it by 1");
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   }
 }
 
 void CandidTypeRecord::_append(uint32_t field_id, std::string field_name,
                                CandidType field) {
   // Check if field with identical hash already exists
   auto iter = std::find(begin(m_field_ids), end(m_field_ids), field_id);
   if (iter != end(m_field_ids)) {
     auto i = std::distance(begin(m_field_ids), iter);
     std::string msg;
     msg.append("ERROR: record already has a field with the same field_id.\n");
     msg.append("       field id (hash): " + std::to_string(field_id) + "\n");
     msg.append("       field name 1   : " + m_field_names[i] + "\n");
     msg.append("       field name 2   : " + field_name + "\n");
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   }
 
   // Add the field
   m_field_ids.push_back(field_id);
   m_field_names.push_back(field_name);
   int datatype =
       std::visit([](auto &&c) { return c.get_datatype_opcode(); }, field);
   m_field_datatypes.push_back(datatype);
-  m_fields.push_back(field);
+  // Store the shared pointer to a CandidTypeBase class
+  m_fields_ptrs.push_back(std::visit([](auto&& arg) -> std::shared_ptr<CandidTypeBase> {
+    return std::make_shared<std::decay_t<decltype(arg)>>(arg);
+  }, field));
 
   // Sort by field_id (hash)
   for (std::size_t i = 0; i < m_field_ids.size(); ++i) {
     for (std::size_t j = i + 1; j < m_field_ids.size(); ++j) {
       if (m_field_ids[i] > m_field_ids[j]) {
         auto temp_field_id = std::move(m_field_ids[i]);
         m_field_ids[i] = std::move(m_field_ids[j]);
         m_field_ids[j] = std::move(temp_field_id);
 
         auto temp_field_name = std::move(m_field_names[i]);
         m_field_names[i] = std::move(m_field_names[j]);
         m_field_names[j] = std::move(temp_field_name);
 
-        auto temp_field = std::move(m_fields[i]);
-        m_fields[i] = std::move(m_fields[j]);
-        m_fields[j] = std::move(temp_field);
+        auto temp_field = std::move(m_fields_ptrs[i]);
+        m_fields_ptrs[i] = std::move(m_fields_ptrs[j]);
+        m_fields_ptrs[j] = std::move(temp_field);
 
         auto temp_field_datatype = std::move(m_field_datatypes[i]);
         m_field_datatypes[i] = std::move(m_field_datatypes[j]);
         m_field_datatypes[j] = std::move(temp_field_datatype);
       }
     }
   }
@@ -109,33 +115,36 @@
 }
 
 // (re-)build the type table encoding
 void CandidTypeRecord::encode_T() {
   m_T.clear();
 
   m_T.append_byte((std::byte)m_datatype_hex);
-  m_T.append_uleb128(__uint128_t(m_fields.size()));
-  for (size_t i = 0; i < m_fields.size(); ++i) {
+  m_T.append_uleb128(__uint128_t(m_fields_ptrs.size()));
+  for (size_t i = 0; i < m_fields_ptrs.size(); ++i) {
     // id or hash of the record field, append without packing into a fixed width
     m_T.append_uleb128(__uint128_t(m_field_ids[i]));
 
     // data type of the record field
-    VecBytes I = std::visit([](auto &&c) { return c.get_I(); }, m_fields[i]);
-    for (std::byte b : I.vec()) {
-      m_T.append_byte(b);
+    // The get_I method is in the CandidTypeBase class.
+    if(m_fields_ptrs[i]) {
+      VecBytes I = m_fields_ptrs[i]->get_I();
+      for (std::byte b : I.vec()) {
+        m_T.append_byte(b);
+      }
     }
   }
 }
 
 // Decode the type table, starting at & updating offset
 bool CandidTypeRecord::decode_T(VecBytes B, __uint128_t &offset,
                                 std::string &parse_error) {
   m_field_ids.clear();
   m_field_names.clear();
-  m_fields.clear();
+  m_fields_ptrs.clear();
   m_field_datatypes.clear();
 
   __uint128_t num_fields;
   __uint128_t numbytes;
   if (B.parse_uleb128(offset, num_fields, numbytes, parse_error)) {
     return true;
   }
@@ -153,59 +162,61 @@
     // Get the datatype of the type table
     __uint128_t offset_start = offset;
     std::string parse_error;
     __int128_t datatype;
     numbytes = 0;
     if (B.parse_sleb128(offset, datatype, numbytes, parse_error)) {
       std::string to_be_parsed = "Type table: datatype";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_field_datatypes.push_back(int(datatype));
 
     // Create a CandidType instance for the field
     CandidType c;
     if (int(datatype) == CandidOpcode().Vec) {
       // for a Vec, the typetable is simple the datatype of it's content
       offset_start = offset;
       parse_error = "";
       __int128_t content_opcode;
       if (B.parse_sleb128(offset, content_opcode, numbytes, parse_error)) {
         std::string to_be_parsed =
             "Type table: a record field of type Vec -> the Vec's content type";
-        CandidDeserialize::trap_with_parse_error(offset_start, offset,
+        CandidAssert::trap_with_parse_error(offset_start, offset,
                                                  to_be_parsed, parse_error);
       }
       CandidOpcode().candid_type_vec_from_opcode(c, content_opcode);
     } else if (int(datatype) == CandidOpcode().Opt) {
       // for an Opt, the typetable is simple the datatype of it's content
       offset_start = offset;
       parse_error = "";
       __int128_t content_opcode;
       if (B.parse_sleb128(offset, content_opcode, numbytes, parse_error)) {
         std::string to_be_parsed =
             "Type table: a record field of type Opt -> the Opt's content type";
-        CandidDeserialize::trap_with_parse_error(offset_start, offset,
+        CandidAssert::trap_with_parse_error(offset_start, offset,
                                                  to_be_parsed, parse_error);
       }
       CandidOpcode().candid_type_opt_from_opcode(c, content_opcode);
     } else {
       // Decode type table using the CandidType variant's decode_T method.
       CandidOpcode().candid_type_from_opcode(c, datatype);
       parse_error = "";
       if (std::visit(
               [&](auto &&c) { return c.decode_T(B, offset, parse_error); },
               c)) {
         std::string to_be_parsed = "Type table: record field";
-        CandidDeserialize::trap_with_parse_error(offset_start, offset,
+        CandidAssert::trap_with_parse_error(offset_start, offset,
                                                  to_be_parsed, parse_error);
       }
     }
-    // Store the CandidType in m_fields vector
-    m_fields.push_back(c);
+    // Store a shared pointer to the CandidTypeBase class
+    m_fields_ptrs.push_back(std::visit([](auto&& arg) -> std::shared_ptr<CandidTypeBase> {
+        return std::make_shared<std::decay_t<decltype(arg)>>(arg);
+    }, c));
   }
   return false;
 }
 
 // For records, we set the Opcode, but note that it is not used during serialization.
 // At serialization time, we use the index in the overall type table.
 //
@@ -216,66 +227,69 @@
   m_I.append_byte((std::byte)m_datatype_hex);
 }
 
 // (re-)build the value encoding
 void CandidTypeRecord::encode_M() {
   m_M.clear();
 
-  for (CandidType field : m_fields) {
-    VecBytes M = std::visit([](auto &&c) { return c.get_M(); }, field);
-    for (std::byte b : M.vec()) {
-      m_M.append_byte(b);
+  for (auto p_field : m_fields_ptrs) {
+    // The get_M method is in the CandidTypeBase class
+    if(p_field) {
+      VecBytes M = p_field->get_M();
+      for (std::byte b : M.vec()) {
+        m_M.append_byte(b);
+      }
     }
   }
 }
 
 // Decode the values, starting at & updating offset
 bool CandidTypeRecord::decode_M(VecBytes B, __uint128_t &offset,
                                 std::string &parse_error) {
-  for (size_t i = 0; i < m_fields.size(); ++i) {
+  for (size_t i = 0; i < m_fields_ptrs.size(); ++i) {
     if (m_field_datatypes_wire[i] == CandidOpcode().Null) {
       // There is no value to decode
       continue;
     }
     int datatype = m_field_datatypes[i];
     if (CandidOpcode().is_primtype(datatype)) {
       parse_error = "";
       __uint128_t offset_start = offset;
-      if (std::visit(
-              [&](auto &&c) { return c.decode_M(B, offset, parse_error); },
-              m_fields[i])) {
-        std::string to_be_parsed = "Value for a Record field";
-        CandidDeserialize::trap_with_parse_error(offset_start, offset,
-                                                 to_be_parsed, parse_error);
+      if(m_fields_ptrs[i]) {
+        if(m_fields_ptrs[i]->decode_M(B, offset, parse_error)){
+          std::string to_be_parsed = "Value for a Record field at index " + std::to_string(i);
+          CandidAssert::trap_with_parse_error(offset_start, offset,
+                                                  to_be_parsed, parse_error);
+        }
       }
     } else {
-      IC_API::trap(
+      ICPP_HOOKS::trap(
           "TODO: Implement decode for non primitive type as a record field, using recursion " +
           std::to_string(datatype) + std::string(__func__));
     }
   }
 
   return false;
 }
 
 // Traps if the type table does not match the type table on the wire
 void CandidTypeRecord::check_type_table(const CandidTypeRecord *p_from_wire) {
   m_field_datatypes_wire.clear();
-  for (size_t i = 0; i < m_fields.size(); ++i) {
+  for (size_t i = 0; i < m_fields_ptrs.size(); ++i) {
     // id or hash of the record field
     uint32_t id = m_field_ids[i];
     uint32_t id_wire = p_from_wire->m_field_ids[i];
     if (id != id_wire) {
       std::string msg;
       msg.append("ERROR: the hashed id for the Record field at index " +
                  std::to_string(i) + " is wrong on the wire.\n");
       msg.append("       expected value of the hashed id: " +
                  std::to_string(id) + " (" + m_field_names[i] + ")" + "\n");
       msg.append("       found on wire  : " + std::to_string(id_wire) + "\n");
-      IC_API::trap(msg);
+      ICPP_HOOKS::trap(msg);
     }
 
     int datatype = m_field_datatypes[i];
     int datatype_wire = p_from_wire->m_field_datatypes[i];
     m_field_datatypes_wire.push_back(
         datatype_wire); // save it for use in decode_M
 
@@ -289,12 +303,12 @@
                    std::to_string(i) + " is wrong on the wire.\n");
         msg.append("       expected datatype: " + std::to_string(datatype) +
                    " (" + CandidOpcode().name_from_opcode(datatype) + ")" +
                    "\n");
         msg.append("       type on wire : " + std::to_string(datatype_wire) +
                    " (" + CandidOpcode().name_from_opcode(datatype_wire) + ")" +
                    "\n");
-        IC_API::trap(msg);
+        ICPP_HOOKS::trap(msg);
       }
     }
   }
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_record.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_record.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 // The class for the Candid Type: record
 
 #pragma once
 
 #include <cstring>
+#include <memory>
 
-#include "candid.h"
+#include "vec_bytes.h"
 
 class CandidTypeRecord : public CandidTypeBase {
 public:
   // Constructors
   CandidTypeRecord();
 
   // Destructor
@@ -33,12 +34,12 @@
   void encode_T();
   void encode_I();
   void encode_M();
 
   std::vector<uint32_t> m_field_ids; // id | hash
   std::vector<std::string> m_field_names;
   std::vector<int> m_field_datatypes;
-  std::vector<CandidType> m_fields;
+  std::vector<std::shared_ptr<CandidTypeBase>> m_fields_ptrs;
 
   // To help with decoding checks
   std::vector<int> m_field_datatypes_wire;
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_reserved.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_reserved.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 // The class for the Primitive Candid Type: reserved
 
-#include "candid.h"
-#include "ic_api.h"
+#include "candid_type.h"
+#include "candid_type_reserved.h"
 
 #include "candid_opcode.h"
 #include "pro.h"
 
-CandidTypeReserved::CandidTypeReserved() : CandidTypePrim() {
+CandidTypeReserved::CandidTypeReserved() {
 
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 CandidTypeReserved::~CandidTypeReserved() {}
 
 void CandidTypeReserved::set_datatype() {
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_table.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_table.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 // Candid type table
 // https://github.com/dfinity/candid/blob/master/spec/Candid.md#parameters-and-results
 
-#include "candid.h"
+#include <string>
+
+#include "candid_type.h"
+#include "candid_type_all_includes.h"
+#include "candid_type_table.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
-#include "ic_api.h"
+
 
 #include <cassert>
 #include <utility>
 
 CandidTypeTable::CandidTypeTable() {}
 
 CandidTypeTable::CandidTypeTable(const VecBytes &B, __uint128_t &B_offset) {
@@ -22,49 +27,49 @@
   // Get the datatype for the type table
   __uint128_t B_offset_start = B_offset;
   std::string parse_error;
   __int128_t datatype;
   __uint128_t numbytes;
   if (m_B.parse_sleb128(B_offset, datatype, numbytes, parse_error)) {
     std::string to_be_parsed = "Type table: opcode";
-    CandidDeserialize::trap_with_parse_error(B_offset_start, B_offset,
+    CandidAssert::trap_with_parse_error(B_offset_start, B_offset,
                                              to_be_parsed, parse_error);
   }
   m_opcode = int(datatype);
 
   // Deserialize the type-table
 
   if (m_opcode == CandidOpcode().Vec) {
     // for a Vec, the typetable is simple the datatype of it's content
     B_offset_start = B_offset;
     parse_error = "";
     __int128_t content_opcode;
     if (m_B.parse_sleb128(B_offset, content_opcode, numbytes, parse_error)) {
       std::string to_be_parsed = "Type table: a Vec's content type";
-      CandidDeserialize::trap_with_parse_error(B_offset_start, B_offset,
+      CandidAssert::trap_with_parse_error(B_offset_start, B_offset,
                                                to_be_parsed, parse_error);
     }
     CandidOpcode().candid_type_vec_from_opcode(m_c, content_opcode);
   } else if (m_opcode == CandidOpcode().Opt) {
     // for a Opt, the typetable is simple the datatype of it's content
     B_offset_start = B_offset;
     parse_error = "";
     __int128_t content_opcode;
     if (m_B.parse_sleb128(B_offset, content_opcode, numbytes, parse_error)) {
       std::string to_be_parsed = "Type table: an Opt's content type";
-      CandidDeserialize::trap_with_parse_error(B_offset_start, B_offset,
+      CandidAssert::trap_with_parse_error(B_offset_start, B_offset,
                                                to_be_parsed, parse_error);
     }
     CandidOpcode().candid_type_opt_from_opcode(m_c, content_opcode);
   } else {
     // using the decoder of the datatype
     CandidOpcode().candid_type_from_opcode(m_c, m_opcode);
     parse_error = "";
     if (std::visit(
             [&](auto &&c) { return c.decode_T(m_B, B_offset, parse_error); },
             m_c)) {
       std::string to_be_parsed = "Type table";
-      CandidDeserialize::trap_with_parse_error(B_offset_start, B_offset,
+      CandidAssert::trap_with_parse_error(B_offset_start, B_offset,
                                                to_be_parsed, parse_error);
     }
   }
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_table.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_table.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 // The candid type table of a Candid variable
 // https://github.com/dfinity/candid/blob/master/spec/Candid.md#parameters-and-results
 
 #pragma once
 
-#include <string>
-#include <vector>
-
-#include "candid.h"
-
 class CandidTypeTable {
 public:
   CandidTypeTable();
   CandidTypeTable(const VecBytes &B, __uint128_t &B_offset);
   ~CandidTypeTable();
 
   VecBytes get_B() { return m_B; }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_text.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_text.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 // The class for the Primitive Candid Type: text
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_text.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
 
-CandidTypeText::CandidTypeText() : CandidTypePrim() { initialize(""); }
+
+CandidTypeText::CandidTypeText() { initialize(""); }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypeText::CandidTypeText(std::string *p_v) : CandidTypePrim() {
+CandidTypeText::CandidTypeText(std::string *p_v) {
   set_pv(p_v);
 
   const std::string v = const_cast<std::string &>(*p_v);
   initialize(v);
 }
 
 // These constructors are only for encoding
-CandidTypeText::CandidTypeText(const char *c) : CandidTypePrim() {
+CandidTypeText::CandidTypeText(const char *c) {
   std::string v(c);
   initialize(v);
 }
-CandidTypeText::CandidTypeText(const std::string v) : CandidTypePrim() {
+CandidTypeText::CandidTypeText(const std::string v) {
   initialize(v);
 }
 
 CandidTypeText::~CandidTypeText() {}
 
 // Initialize things
 void CandidTypeText::initialize(const std::string &v) {
   m_v = v;
   set_datatype();
+  encode_T();
   encode_I();
   encode_M();
 }
 
 // pointer to data in caller, for storing decoded value
 void CandidTypeText::set_pv(std::string *v) { m_pv = v; }
 
@@ -71,22 +74,22 @@
   // get size of text - leb128(|utf8(t)|)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t numBytes_text;
   if (B.parse_uleb128(offset, numBytes_text, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of text- leb128(|utf8(t)|)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   std::vector<std::byte> data_bytes;
   if (B.parse_bytes(offset, data_bytes, numBytes_text, numbytes, parse_error)) {
     std::string to_be_parsed = "Data bytes for Text";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v = "";
   for (size_t i = 0; i < numBytes_text; ++i) {
     m_v.append(VecBytes::byte_to_char(data_bytes[i]));
   }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_text.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_text.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 // The class for the Primitive Candid Type: text
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_base.h"
+#include "vec_bytes.h"
 
-class CandidTypeText : public CandidTypePrim {
+class CandidTypeText : public CandidTypeBase {
 public:
   // Constructors
   CandidTypeText();
   CandidTypeText(const char *c);
   // docs start: demo_candid_type_text
   CandidTypeText(std::string *v);
   CandidTypeText(const std::string v); // docs end: demo_candid_type_text
 
   // Destructor
   ~CandidTypeText();
 
+  bool decode_T(VecBytes B, __uint128_t &offset, std::string &parse_error) {
+    return false; // type table for Primitives is empty
+  }
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
   std::string get_v() { return m_v; }
 
 protected:
   void set_pv(std::string *v);
   void initialize(const std::string &v);
   void set_datatype();
+  void encode_T() { m_T.clear(); } // type table for Primitives is empty
   void encode_I();
   void encode_M();
 
   std::string m_v;
   std::string *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_variant.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_variant.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 // The class for the Candid Type: variant
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_all_includes.h"
+#include "candid_type_variant.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 #include "pro.h"
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 #include <algorithm>
 #include <cassert>
 #include <utility>
 
 CandidTypeVariant::CandidTypeVariant() : CandidTypeBase() { initialize(); }
 
@@ -62,99 +65,106 @@
 void CandidTypeVariant::append(std::string field_name, CandidType field) {
   uint32_t field_id = idl_hash(field_name);
   _append(field_id, field_name, field);
 }
 
 // Tuple notation without field_id -> generate sequential uint32_t field_id
 void CandidTypeVariant::append(CandidType field) {
-  if (m_fields.size() == 0) {
+  if (m_fields_ptrs.size() == 0) {
     uint32_t field_id = 0;
     append(field_id, field);
   }
 
   if (std::in_range<std::uint32_t>(m_field_ids.back() + 1)) {
     uint32_t field_id = m_field_ids.back() + 1;
     append(field_id, field);
   } else {
     std::string msg;
     msg.append("ERROR: field_id outside range of uint32_t\n");
     msg.append("       id of previous field in variant: " +
                std::to_string(m_field_ids.back()) + "\n");
     msg.append(
         "       because no field_id was specified for current field, we want to increase it by 1");
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   }
 }
 
 void CandidTypeVariant::_append(uint32_t field_id, std::string field_name,
                                 CandidType field) {
 
   auto iter = std::find(begin(m_field_ids), end(m_field_ids), field_id);
 
   if (iter != end(m_field_ids) && field_name == m_label && !m_label_value_set) {
     // Erase the entry of the label, because it was not yet set by user
     auto i = std::distance(begin(m_field_ids), iter);
     m_field_ids.erase(m_field_ids.begin() + i);
     m_field_names.erase(m_field_names.begin() + i);
     m_field_datatypes.erase(m_field_datatypes.begin() + i);
-    m_fields.erase(m_fields.begin() + i);
+    m_fields_ptrs.erase(m_fields_ptrs.begin() + i);
 
     // Check again
     iter = std::find(begin(m_field_ids), end(m_field_ids), field_id);
   }
 
   if (iter != end(m_field_ids)) {
     auto i = std::distance(begin(m_field_ids), iter);
     std::string msg;
     msg.append("ERROR: variant already has a field with the same field_id.\n");
     msg.append("       field id (hash): " + std::to_string(field_id) + "\n");
     msg.append("       field name 1   : " + m_field_names[i] + "\n");
     msg.append("       field name 2   : " + field_name + "\n");
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   }
   // Add the field
   m_field_ids.push_back(field_id);
   m_field_names.push_back(field_name);
   int datatype =
       std::visit([](auto &&c) { return c.get_datatype_opcode(); }, field);
   m_field_datatypes.push_back(datatype);
-  m_fields.push_back(field);
+  // Store the shared pointer to a CandidTypeBase class
+  m_fields_ptrs.push_back(std::visit([](auto&& arg) -> std::shared_ptr<CandidTypeBase> {
+    return std::make_shared<std::decay_t<decltype(arg)>>(arg);
+  }, field));
+
 
   if (field_name == m_label) {
     m_label_value_set = true;
   }
 
   encode_T();
   encode_M();
 }
 
 // (re-)build the type table encoding
 void CandidTypeVariant::encode_T() {
   m_T.clear();
 
   m_T.append_byte((std::byte)m_datatype_hex);
-  m_T.append_uleb128(__uint128_t(m_fields.size()));
-  for (size_t i = 0; i < m_fields.size(); ++i) {
+  m_T.append_uleb128(__uint128_t(m_fields_ptrs.size()));
+  for (size_t i = 0; i < m_fields_ptrs.size(); ++i) {
     // id or hash of the variant field, append without packing into a fixed width
     m_T.append_uleb128(__uint128_t(m_field_ids[i]));
 
     // data type of the variant field
-    VecBytes I = std::visit([](auto &&c) { return c.get_I(); }, m_fields[i]);
-    for (std::byte b : I.vec()) {
-      m_T.append_byte(b);
+    // The get_I method is in the CandidTypeBase class.
+    if(m_fields_ptrs[i]) {
+      VecBytes I = m_fields_ptrs[i]->get_I();
+      for (std::byte b : I.vec()) {
+        m_T.append_byte(b);
+      }
     }
   }
 }
 
 // Decode the type table, starting at & updating offset
 bool CandidTypeVariant::decode_T(VecBytes B, __uint128_t &offset,
                                  std::string &parse_error) {
   m_field_ids.clear();
   m_field_names.clear();
-  m_fields.clear();
+  m_fields_ptrs.clear();
   m_field_datatypes.clear();
 
   __uint128_t num_fields;
   __uint128_t numbytes;
   if (B.parse_uleb128(offset, num_fields, numbytes, parse_error)) {
     return true;
   }
@@ -172,59 +182,61 @@
     // Get the datatype of the type table
     __uint128_t offset_start = offset;
     std::string parse_error;
     __int128_t datatype;
     numbytes = 0;
     if (B.parse_sleb128(offset, datatype, numbytes, parse_error)) {
       std::string to_be_parsed = "Type table: datatype";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_field_datatypes.push_back(int(datatype));
 
     // Create a CandidType instance for the field
     CandidType c;
     if (int(datatype) == CandidOpcode().Vec) {
       // for a Vec, the typetable is simple the datatype of it's content
       offset_start = offset;
       parse_error = "";
       __int128_t content_opcode;
       if (B.parse_sleb128(offset, content_opcode, numbytes, parse_error)) {
         std::string to_be_parsed =
             "Type table: a variant field of type Vec -> the Vec's content type";
-        CandidDeserialize::trap_with_parse_error(offset_start, offset,
+        CandidAssert::trap_with_parse_error(offset_start, offset,
                                                  to_be_parsed, parse_error);
       }
       CandidOpcode().candid_type_vec_from_opcode(c, content_opcode);
     } else if (int(datatype) == CandidOpcode().Opt) {
       // for an Opt, the typetable is simple the datatype of it's content
       offset_start = offset;
       parse_error = "";
       __int128_t content_opcode;
       if (B.parse_sleb128(offset, content_opcode, numbytes, parse_error)) {
         std::string to_be_parsed =
             "Type table: a variant field of type Opt -> the Opt's content type";
-        CandidDeserialize::trap_with_parse_error(offset_start, offset,
+        CandidAssert::trap_with_parse_error(offset_start, offset,
                                                  to_be_parsed, parse_error);
       }
       CandidOpcode().candid_type_opt_from_opcode(c, content_opcode);
     } else {
       // Decode type table using the CandidType variant's decode_T method.
       CandidOpcode().candid_type_from_opcode(c, datatype);
       parse_error = "";
       if (std::visit(
               [&](auto &&c) { return c.decode_T(B, offset, parse_error); },
               c)) {
         std::string to_be_parsed = "Type table: variant field";
-        CandidDeserialize::trap_with_parse_error(offset_start, offset,
+        CandidAssert::trap_with_parse_error(offset_start, offset,
                                                  to_be_parsed, parse_error);
       }
     }
-    // Store the CandidType in m_fields vector
-    m_fields.push_back(c);
+    // Store a shared pointer to the CandidTypeBase class
+    m_fields_ptrs.push_back(std::visit([](auto&& arg) -> std::shared_ptr<CandidTypeBase> {
+        return std::make_shared<std::decay_t<decltype(arg)>>(arg);
+    }, c));
   }
   return false;
 }
 
 // For variants, we set the Opcode, but note that it is not used during serialization.
 // At serialization time, we use the index in the overall type table.
 //
@@ -243,17 +255,20 @@
 
   for (size_t i = 0; i < m_field_names.size(); ++i) {
     if (m_field_names[i] == m_label) {
       // encode index of variant options - leb128(i)
       m_M.append_uleb128(__uint128_t(i));
 
       // encode the variant's value
-      VecBytes M = std::visit([](auto &&c) { return c.get_M(); }, m_fields[i]);
-      for (std::byte b : M.vec()) {
-        m_M.append_byte(b);
+      // The get_M method is in the CandidTypeBase class
+      if(m_fields_ptrs[i]) {
+        VecBytes M = m_fields_ptrs[i]->get_M();
+        for (std::byte b : M.vec()) {
+          m_M.append_byte(b);
+        }
       }
 
       break;
     }
   }
 }
 
@@ -266,21 +281,21 @@
   //       We have to check on the variant label-hash, not on the full variant index.
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t j;
   if (B.parse_uleb128(offset, j, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   // match the variant's id (hash) of wire with passed in variant fields
   bool found_match{false};
-  for (size_t i = 0; i < m_fields.size(); ++i) {
+  for (size_t i = 0; i < m_fields_ptrs.size(); ++i) {
     if (m_field_ids_wire[j] == m_field_ids[i]) {
       found_match = true;
       m_label = m_field_names[i];
       m_variant_index = i;
       m_variant_index_wire = j;
       break;
     }
@@ -288,19 +303,19 @@
   if (!found_match) {
     std::string msg;
     msg.append(
         "ERROR: The id (hash) of the Variant's value on the wire does not match any of the expected Variant ids.\n");
     msg.append("       The id (hash) on wire: " +
                std::to_string(m_field_ids_wire[j]) + "\n");
     msg.append("       Expecting one of the following ids:\n");
-    for (size_t i = 0; i < m_fields.size(); ++i) {
+    for (size_t i = 0; i < m_fields_ptrs.size(); ++i) {
       msg.append("       - " + std::to_string(m_field_ids[i]) + " (" +
                  m_field_names[i] + ")" + "\n");
     }
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   }
   // verify that the types match
   int datatype = m_field_datatypes[m_variant_index];
   int datatype_wire = m_field_datatypes_wire[m_variant_index_wire];
   if (datatype != datatype_wire) {
     std::string msg;
     msg.append(
@@ -310,43 +325,51 @@
                m_label + ")" + "\n");
     msg.append("       expected datatype for this id (hash): " +
                std::to_string(datatype) + " (" +
                CandidOpcode().name_from_opcode(datatype) + ")" + "\n");
     msg.append("       datatype on wire                    : " +
                std::to_string(datatype_wire) + " (" +
                CandidOpcode().name_from_opcode(datatype_wire) + ")" + "\n");
-    IC_API::trap(msg);
+    ICPP_HOOKS::trap(msg);
   }
 
   // decode the value
   if (datatype_wire == CandidOpcode().Null) {
     // There is no value to decode
-  } else if (CandidOpcode().is_primtype(datatype_wire)) {
+    // TODO: REMOVE THIS LINE.
+  // } else if (CandidOpcode().is_primtype(datatype_wire)) {
+  } else {
+    // We can just call the decode_M method on the base class, use runtime polymorphism
+    // (-) The method decode_M is declared as a virtual function the base class
+    // (-) It is implemented for ALL derived classes
     parse_error = "";
     __uint128_t offset_start = offset;
-    if (std::visit([&](auto &&c) { return c.decode_M(B, offset, parse_error); },
-                   m_fields[m_variant_index])) {
-      std::string to_be_parsed = "Value for a Variant";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
-                                               to_be_parsed, parse_error);
+
+    if(m_fields_ptrs[m_variant_index]) {
+      if (m_fields_ptrs[m_variant_index]->decode_M(B, offset, parse_error)){
+        std::string to_be_parsed = "Value for a Variant";
+        CandidAssert::trap_with_parse_error(offset_start, offset,
+                                                to_be_parsed, parse_error);
+      }
     }
-  } else {
-    IC_API::trap(
-        "TODO: Implement decode for non primitive type as a variant field, using recursion " +
-        std::to_string(datatype) + std::string(__func__));
-  }
+  } 
+  // else {
+  //   ICPP_HOOKS::trap(
+  //       "TODO: Implement decode for non primitive type as a variant field, using recursion " +
+  //       std::to_string(datatype) + std::string(__func__));
+  // }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_p_label) *m_p_label = m_label;
 
   return false;
 }
 
 void CandidTypeVariant::check_type_table(const CandidTypeVariant *p_from_wire) {
   // Save type table data on wire for use in decode_M
   m_field_ids_wire.clear();
   m_field_datatypes_wire.clear();
-  for (size_t i = 0; i < p_from_wire->m_fields.size(); ++i) {
+  for (size_t i = 0; i < p_from_wire->m_fields_ptrs.size(); ++i) {
     m_field_ids_wire.push_back(p_from_wire->m_field_ids[i]);
     m_field_datatypes_wire.push_back(p_from_wire->m_field_datatypes[i]);
   }
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_variant.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_variant.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 // The class for the Candid Type: variant
 
 #pragma once
 
 #include <cstring>
+#include <memory>
 
-#include "candid.h"
+#include "vec_bytes.h"
 
 class CandidTypeVariant : public CandidTypeBase {
 public:
   // Constructors
   CandidTypeVariant();
   CandidTypeVariant(std::string *p_label);
   CandidTypeVariant(const std::string label);
@@ -37,15 +38,15 @@
   void encode_T();
   void encode_I();
   void encode_M();
 
   std::vector<uint32_t> m_field_ids; // id | hash
   std::vector<std::string> m_field_names;
   std::vector<int> m_field_datatypes;
-  std::vector<CandidType> m_fields;
+  std::vector<std::shared_ptr<CandidTypeBase>> m_fields_ptrs;
 
   // Label & id (hash) of the field that contains the Variant's data
   std::string m_label{""};
   __uint128_t m_variant_index{0};
   bool m_label_value_set{false};
 
   // Pointer to the label passed in by caller during deserialization
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_base.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_base.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 // The base class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_base.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 #include "pro.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+
 
 CandidTypeVecBase::CandidTypeVecBase() : CandidTypeBase() {}
 
 CandidTypeVecBase::~CandidTypeVecBase() {}
 
 // Initialize things
 void CandidTypeVecBase::initialize() {
@@ -41,15 +43,15 @@
   // The opcode for content type
   __uint128_t offset_start = offset;
   parse_error = "";
   __int128_t content_type;
   __uint128_t numbytes;
   if (B.parse_sleb128(offset, content_type, numbytes, parse_error)) {
     std::string to_be_parsed = "Type table: a Vec's content type";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_content_type_opcode = int(content_type);
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_bool.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_bool.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_bool.h"
+#include "candid_type_bool.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+
 
 CandidTypeVecBool::CandidTypeVecBool() : CandidTypeVecBase() {
   std::vector<bool> v;
   set_v(v);
   initialize();
 }
 
@@ -58,26 +61,26 @@
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
   offset_start = offset;
   parse_error = "";
   CandidTypeBool c{}; // dummy so we can use it's decode_M
   for (size_t i = 0; i < size_vec; ++i) {
     if (c.decode_M(B, offset, parse_error)) {
       std::string to_be_parsed = "Vec: Value for CandidTypeBool";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(c.get_v());
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_bool.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_bool.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: vec
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_vec_base.h"
+#include "candid_type_bool.h"
+#include "vec_bytes.h"
 
 class CandidTypeVecBool : public CandidTypeVecBase {
 public:
   // Constructors
   CandidTypeVecBool();
   CandidTypeVecBool(const std::vector<bool> v);
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_float32.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_float32.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_float32.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+
 
 CandidTypeVecFloat32::CandidTypeVecFloat32() : CandidTypeVecBase() {
   std::vector<float> v;
   set_v(v);
   initialize();
 }
 
@@ -58,26 +60,26 @@
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
   float v;
   offset_start = offset;
   parse_error = "";
   for (size_t i = 0; i < size_vec; ++i) {
     if (B.parse_float_ieee754(offset, v, parse_error)) {
       std::string to_be_parsed = "Vec: Value for CandidTypeFloat32";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(v);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_float32.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_float32.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: vec
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_vec_base.h"
+#include "candid_type_float32.h"
+#include "vec_bytes.h"
 
 class CandidTypeVecFloat32 : public CandidTypeVecBase {
 public:
   // Constructors
   CandidTypeVecFloat32();
   CandidTypeVecFloat32(const std::vector<float> v);
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_float64.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,85 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_int.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
 
-CandidTypeVecFloat64::CandidTypeVecFloat64() : CandidTypeVecBase() {
-  std::vector<double> v;
+
+CandidTypeVecInt::CandidTypeVecInt() : CandidTypeVecBase() {
+  std::vector<__int128_t> v;
   set_v(v);
   initialize();
 }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypeVecFloat64::CandidTypeVecFloat64(std::vector<double> *p_v)
+CandidTypeVecInt::CandidTypeVecInt(std::vector<__int128_t> *p_v)
     : CandidTypeVecBase() {
   set_pv(p_v);
 
-  const std::vector<double> v = const_cast<std::vector<double> &>(*p_v);
+  const std::vector<__int128_t> v = const_cast<std::vector<__int128_t> &>(*p_v);
   set_v(v);
   initialize();
 }
 
 // These constructors are only for encoding
-CandidTypeVecFloat64::CandidTypeVecFloat64(const std::vector<double> v)
+CandidTypeVecInt::CandidTypeVecInt(const std::vector<__int128_t> v)
     : CandidTypeVecBase() {
   set_v(v);
   initialize();
 }
 
-CandidTypeVecFloat64::~CandidTypeVecFloat64() {}
+CandidTypeVecInt::~CandidTypeVecInt() {}
 
-void CandidTypeVecFloat64::set_content_type() {
-  m_content_type_opcode = CandidOpcode().Float64;
-  m_content_type_hex = OpcodeHex().Float64;
-  m_content_type_textual = OpcodeTextual().Float64;
+void CandidTypeVecInt::set_content_type() {
+  m_content_type_opcode = CandidOpcode().Int;
+  m_content_type_hex = OpcodeHex().Int;
+  m_content_type_textual = OpcodeTextual().Int;
 }
 
-void CandidTypeVecFloat64::encode_M() {
+void CandidTypeVecInt::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(v^N  : vec <datatype>) = leb128(N) M(v : <datatype>)^N
 
   // encoded size of vec - leb128(N)
   m_M.append_uleb128(__uint128_t(m_v.size()));
 
   // encoded vec values - M(v : <datatype>)^N
-  // M(z : float<N>) = f<N>(z)
-  for (double const &c : m_v) {
-    m_M.append_float_ieee754(c);
+  // M(i : int)      = sleb128(i)
+  for (__int128_t const &c : m_v) {
+    m_M.append_sleb128(c);
   }
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeVecFloat64::decode_M(VecBytes B, __uint128_t &offset,
-                                    std::string &parse_error) {
+bool CandidTypeVecInt::decode_M(VecBytes B, __uint128_t &offset,
+                                std::string &parse_error) {
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
-  double v;
+  __int128_t v;
   offset_start = offset;
   parse_error = "";
   for (size_t i = 0; i < size_vec; ++i) {
-    if (B.parse_float_ieee754(offset, v, parse_error)) {
-      std::string to_be_parsed = "Vec: Value for CandidTypeFloat64";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+    if (B.parse_sleb128(offset, v, numbytes, parse_error)) {
+      std::string to_be_parsed = "Vec: Value for CandidTypeInt";
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(v);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_float64.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_float64.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: vec
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_vec_base.h"
+#include "candid_type_float64.h"
+#include "vec_bytes.h"
 
 class CandidTypeVecFloat64 : public CandidTypeVecBase {
 public:
   // Constructors
   CandidTypeVecFloat64();
   CandidTypeVecFloat64(const std::vector<double> v);
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int32.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,85 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_int32.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
 
-CandidTypeVecInt::CandidTypeVecInt() : CandidTypeVecBase() {
-  std::vector<__int128_t> v;
+
+CandidTypeVecInt32::CandidTypeVecInt32() : CandidTypeVecBase() {
+  std::vector<int32_t> v;
   set_v(v);
   initialize();
 }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypeVecInt::CandidTypeVecInt(std::vector<__int128_t> *p_v)
+CandidTypeVecInt32::CandidTypeVecInt32(std::vector<int32_t> *p_v)
     : CandidTypeVecBase() {
   set_pv(p_v);
 
-  const std::vector<__int128_t> v = const_cast<std::vector<__int128_t> &>(*p_v);
+  const std::vector<int32_t> v = const_cast<std::vector<int32_t> &>(*p_v);
   set_v(v);
   initialize();
 }
 
 // These constructors are only for encoding
-CandidTypeVecInt::CandidTypeVecInt(const std::vector<__int128_t> v)
+CandidTypeVecInt32::CandidTypeVecInt32(const std::vector<int32_t> v)
     : CandidTypeVecBase() {
   set_v(v);
   initialize();
 }
 
-CandidTypeVecInt::~CandidTypeVecInt() {}
+CandidTypeVecInt32::~CandidTypeVecInt32() {}
 
-void CandidTypeVecInt::set_content_type() {
-  m_content_type_opcode = CandidOpcode().Int;
-  m_content_type_hex = OpcodeHex().Int;
-  m_content_type_textual = OpcodeTextual().Int;
+void CandidTypeVecInt32::set_content_type() {
+  m_content_type_opcode = CandidOpcode().Int32;
+  m_content_type_hex = OpcodeHex().Int32;
+  m_content_type_textual = OpcodeTextual().Int32;
 }
 
-void CandidTypeVecInt::encode_M() {
+void CandidTypeVecInt32::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(v^N  : vec <datatype>) = leb128(N) M(v : <datatype>)^N
 
   // encoded size of vec - leb128(N)
   m_M.append_uleb128(__uint128_t(m_v.size()));
 
   // encoded vec values - M(v : <datatype>)^N
-  // M(i : int)      = sleb128(i)
-  for (__int128_t const &c : m_v) {
-    m_M.append_sleb128(c);
+  // M(n : int<N>)   = i<N>(signed_N^-1(i))    (Litte Endian)
+  for (int32_t const &c : m_v) {
+    m_M.append_int_fixed_width(c);
   }
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeVecInt::decode_M(VecBytes B, __uint128_t &offset,
-                                std::string &parse_error) {
+bool CandidTypeVecInt32::decode_M(VecBytes B, __uint128_t &offset,
+                                  std::string &parse_error) {
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
-  __int128_t v;
+  int32_t v;
   offset_start = offset;
   parse_error = "";
   for (size_t i = 0; i < size_vec; ++i) {
-    if (B.parse_sleb128(offset, v, numbytes, parse_error)) {
-      std::string to_be_parsed = "Vec: Value for CandidTypeInt";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+    if (B.parse_int_fixed_width(offset, v, parse_error)) {
+      std::string to_be_parsed = "Vec: Value for CandidTypeInt32";
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(v);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int32.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 // The class for the Candid Type: vec
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_vec_base.h"
+#include "candid_type_int32.h"
+#include "vec_bytes.h"
 
-class CandidTypeVecInt : public CandidTypeVecBase {
+class CandidTypeVecInt32 : public CandidTypeVecBase {
 public:
   // Constructors
-  CandidTypeVecInt();
-  CandidTypeVecInt(const std::vector<__int128_t> v);
+  CandidTypeVecInt32();
+  CandidTypeVecInt32(const std::vector<int32_t> v);
 
-  CandidTypeVecInt(std::vector<__int128_t> *p_v);
+  CandidTypeVecInt32(std::vector<int32_t> *p_v);
 
   // Destructor
-  ~CandidTypeVecInt();
+  ~CandidTypeVecInt32();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  std::vector<__int128_t> get_v() { return m_v; }
+  std::vector<int32_t> get_v() { return m_v; }
 
 protected:
-  void set_pv(std::vector<__int128_t> *v) { m_pv = v; }
-  void set_v(const std::vector<__int128_t> &v) { m_v = v; }
+  void set_pv(std::vector<int32_t> *v) { m_pv = v; }
+  void set_v(const std::vector<int32_t> &v) { m_v = v; }
   void set_content_type();
   void encode_M();
 
-  std::vector<__int128_t> m_v;
-  std::vector<__int128_t> *m_pv{nullptr};
+  std::vector<int32_t> m_v;
+  std::vector<int32_t> *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int16.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int16.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_int16.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+
 
 CandidTypeVecInt16::CandidTypeVecInt16() : CandidTypeVecBase() {
   std::vector<int16_t> v;
   set_v(v);
   initialize();
 }
 
@@ -58,26 +60,26 @@
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
   int16_t v;
   offset_start = offset;
   parse_error = "";
   for (size_t i = 0; i < size_vec; ++i) {
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
       std::string to_be_parsed = "Vec: Value for CandidTypeInt16";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(v);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int16.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 // The class for the Candid Type: vec
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_vec_base.h"
+#include "candid_type_int.h"
+#include "vec_bytes.h"
 
-class CandidTypeVecInt16 : public CandidTypeVecBase {
+class CandidTypeVecInt : public CandidTypeVecBase {
 public:
   // Constructors
-  CandidTypeVecInt16();
-  CandidTypeVecInt16(const std::vector<int16_t> v);
+  CandidTypeVecInt();
+  CandidTypeVecInt(const std::vector<__int128_t> v);
 
-  CandidTypeVecInt16(std::vector<int16_t> *p_v);
+  CandidTypeVecInt(std::vector<__int128_t> *p_v);
 
   // Destructor
-  ~CandidTypeVecInt16();
+  ~CandidTypeVecInt();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  std::vector<int16_t> get_v() { return m_v; }
+  std::vector<__int128_t> get_v() { return m_v; }
 
 protected:
-  void set_pv(std::vector<int16_t> *v) { m_pv = v; }
-  void set_v(const std::vector<int16_t> &v) { m_v = v; }
+  void set_pv(std::vector<__int128_t> *v) { m_pv = v; }
+  void set_v(const std::vector<__int128_t> &v) { m_v = v; }
   void set_content_type();
   void encode_M();
 
-  std::vector<int16_t> m_v;
-  std::vector<int16_t> *m_pv{nullptr};
+  std::vector<__int128_t> m_v;
+  std::vector<__int128_t> *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int32.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int8.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,85 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_int8.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
 
-CandidTypeVecInt32::CandidTypeVecInt32() : CandidTypeVecBase() {
-  std::vector<int32_t> v;
+
+CandidTypeVecInt8::CandidTypeVecInt8() : CandidTypeVecBase() {
+  std::vector<int8_t> v;
   set_v(v);
   initialize();
 }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypeVecInt32::CandidTypeVecInt32(std::vector<int32_t> *p_v)
+CandidTypeVecInt8::CandidTypeVecInt8(std::vector<int8_t> *p_v)
     : CandidTypeVecBase() {
   set_pv(p_v);
 
-  const std::vector<int32_t> v = const_cast<std::vector<int32_t> &>(*p_v);
+  const std::vector<int8_t> v = const_cast<std::vector<int8_t> &>(*p_v);
   set_v(v);
   initialize();
 }
 
 // These constructors are only for encoding
-CandidTypeVecInt32::CandidTypeVecInt32(const std::vector<int32_t> v)
+CandidTypeVecInt8::CandidTypeVecInt8(const std::vector<int8_t> v)
     : CandidTypeVecBase() {
   set_v(v);
   initialize();
 }
 
-CandidTypeVecInt32::~CandidTypeVecInt32() {}
+CandidTypeVecInt8::~CandidTypeVecInt8() {}
 
-void CandidTypeVecInt32::set_content_type() {
-  m_content_type_opcode = CandidOpcode().Int32;
-  m_content_type_hex = OpcodeHex().Int32;
-  m_content_type_textual = OpcodeTextual().Int32;
+void CandidTypeVecInt8::set_content_type() {
+  m_content_type_opcode = CandidOpcode().Int8;
+  m_content_type_hex = OpcodeHex().Int8;
+  m_content_type_textual = OpcodeTextual().Int8;
 }
 
-void CandidTypeVecInt32::encode_M() {
+void CandidTypeVecInt8::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(v^N  : vec <datatype>) = leb128(N) M(v : <datatype>)^N
 
   // encoded size of vec - leb128(N)
   m_M.append_uleb128(__uint128_t(m_v.size()));
 
   // encoded vec values - M(v : <datatype>)^N
   // M(n : int<N>)   = i<N>(signed_N^-1(i))    (Litte Endian)
-  for (int32_t const &c : m_v) {
+  for (int8_t const &c : m_v) {
     m_M.append_int_fixed_width(c);
   }
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeVecInt32::decode_M(VecBytes B, __uint128_t &offset,
-                                  std::string &parse_error) {
+bool CandidTypeVecInt8::decode_M(VecBytes B, __uint128_t &offset,
+                                 std::string &parse_error) {
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
-  int32_t v;
+  int8_t v;
   offset_start = offset;
   parse_error = "";
   for (size_t i = 0; i < size_vec; ++i) {
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
-      std::string to_be_parsed = "Vec: Value for CandidTypeInt32";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      std::string to_be_parsed = "Vec: Value for CandidTypeInt8";
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(v);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int64.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int64.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_int64.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+
 
 CandidTypeVecInt64::CandidTypeVecInt64() : CandidTypeVecBase() {
   std::vector<int64_t> v;
   set_v(v);
   initialize();
 }
 
@@ -58,26 +60,26 @@
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
   int64_t v;
   offset_start = offset;
   parse_error = "";
   for (size_t i = 0; i < size_vec; ++i) {
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
       std::string to_be_parsed = "Vec: Value for CandidTypeInt64";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(v);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int64.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int64.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: vec
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_vec_base.h"
+#include "candid_type_int64.h"
+#include "vec_bytes.h"
 
 class CandidTypeVecInt64 : public CandidTypeVecBase {
 public:
   // Constructors
   CandidTypeVecInt64();
   CandidTypeVecInt64(const std::vector<int64_t> v);
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int8.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat64.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,83 +1,85 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_nat64.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
 
-CandidTypeVecInt8::CandidTypeVecInt8() : CandidTypeVecBase() {
-  std::vector<int8_t> v;
+
+CandidTypeVecNat64::CandidTypeVecNat64() : CandidTypeVecBase() {
+  std::vector<uint64_t> v;
   set_v(v);
   initialize();
 }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypeVecInt8::CandidTypeVecInt8(std::vector<int8_t> *p_v)
+CandidTypeVecNat64::CandidTypeVecNat64(std::vector<uint64_t> *p_v)
     : CandidTypeVecBase() {
   set_pv(p_v);
 
-  const std::vector<int8_t> v = const_cast<std::vector<int8_t> &>(*p_v);
+  const std::vector<uint64_t> v = const_cast<std::vector<uint64_t> &>(*p_v);
   set_v(v);
   initialize();
 }
 
 // These constructors are only for encoding
-CandidTypeVecInt8::CandidTypeVecInt8(const std::vector<int8_t> v)
+CandidTypeVecNat64::CandidTypeVecNat64(const std::vector<uint64_t> v)
     : CandidTypeVecBase() {
   set_v(v);
   initialize();
 }
 
-CandidTypeVecInt8::~CandidTypeVecInt8() {}
+CandidTypeVecNat64::~CandidTypeVecNat64() {}
 
-void CandidTypeVecInt8::set_content_type() {
-  m_content_type_opcode = CandidOpcode().Int8;
-  m_content_type_hex = OpcodeHex().Int8;
-  m_content_type_textual = OpcodeTextual().Int8;
+void CandidTypeVecNat64::set_content_type() {
+  m_content_type_opcode = CandidOpcode().Nat64;
+  m_content_type_hex = OpcodeHex().Nat64;
+  m_content_type_textual = OpcodeTextual().Nat64;
 }
 
-void CandidTypeVecInt8::encode_M() {
+void CandidTypeVecNat64::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(v^N  : vec <datatype>) = leb128(N) M(v : <datatype>)^N
 
   // encoded size of vec - leb128(N)
   m_M.append_uleb128(__uint128_t(m_v.size()));
 
   // encoded vec values - M(v : <datatype>)^N
-  // M(n : int<N>)   = i<N>(signed_N^-1(i))    (Litte Endian)
-  for (int8_t const &c : m_v) {
+  // Nat64:             - M(n : nat<N>)   = i<N>(n)    (Litte Endian)
+  for (uint64_t const &c : m_v) {
     m_M.append_int_fixed_width(c);
   }
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeVecInt8::decode_M(VecBytes B, __uint128_t &offset,
-                                 std::string &parse_error) {
+bool CandidTypeVecNat64::decode_M(VecBytes B, __uint128_t &offset,
+                                  std::string &parse_error) {
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
-  int8_t v;
+  uint64_t v;
   offset_start = offset;
   parse_error = "";
   for (size_t i = 0; i < size_vec; ++i) {
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
-      std::string to_be_parsed = "Vec: Value for CandidTypeInt8";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      std::string to_be_parsed = "Vec: Value for CandidTypeNat64";
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(v);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_int8.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_int8.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: vec
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_vec_base.h"
+#include "candid_type_int8.h"
+#include "vec_bytes.h"
 
 class CandidTypeVecInt8 : public CandidTypeVecBase {
 public:
   // Constructors
   CandidTypeVecInt8();
   CandidTypeVecInt8(const std::vector<int8_t> v);
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_nat.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+
 
 CandidTypeVecNat::CandidTypeVecNat() : CandidTypeVecBase() {
   std::vector<__uint128_t> v;
   set_v(v);
   initialize();
 }
 
@@ -59,26 +61,26 @@
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
   __uint128_t v;
   offset_start = offset;
   parse_error = "";
   for (size_t i = 0; i < size_vec; ++i) {
     if (B.parse_uleb128(offset, v, numbytes, parse_error)) {
       std::string to_be_parsed = "Vec: Value for CandidTypeNat";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(v);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat16.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 // The class for the Candid Type: vec
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_vec_base.h"
+#include "candid_type_nat16.h"
+#include "vec_bytes.h"
 
-class CandidTypeVecNat : public CandidTypeVecBase {
+class CandidTypeVecNat16 : public CandidTypeVecBase {
 public:
   // Constructors
-  CandidTypeVecNat();
-  CandidTypeVecNat(const std::vector<__uint128_t> v);
+  CandidTypeVecNat16();
+  CandidTypeVecNat16(const std::vector<uint16_t> v);
 
-  CandidTypeVecNat(std::vector<__uint128_t> *p_v);
+  CandidTypeVecNat16(std::vector<uint16_t> *p_v);
 
   // Destructor
-  ~CandidTypeVecNat();
+  ~CandidTypeVecNat16();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
-  std::vector<__uint128_t> get_v() { return m_v; }
+  std::vector<uint16_t> get_v() { return m_v; }
 
 protected:
-  void set_pv(std::vector<__uint128_t> *v) { m_pv = v; }
-  void set_v(const std::vector<__uint128_t> &v) { m_v = v; }
+  void set_pv(std::vector<uint16_t> *v) { m_pv = v; }
+  void set_v(const std::vector<uint16_t> &v) { m_v = v; }
   void set_content_type();
   void encode_M();
 
-  std::vector<__uint128_t> m_v;
-  std::vector<__uint128_t> *m_pv{nullptr};
+  std::vector<uint16_t> m_v;
+  std::vector<uint16_t> *m_pv{nullptr};
 };
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat16.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_text.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,96 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_text.h"
+#include "candid_type_text.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
 
-CandidTypeVecNat16::CandidTypeVecNat16() : CandidTypeVecBase() {
-  std::vector<uint16_t> v;
+
+CandidTypeVecText::CandidTypeVecText() : CandidTypeVecBase() {
+  std::vector<std::string> v;
   set_v(v);
   initialize();
 }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypeVecNat16::CandidTypeVecNat16(std::vector<uint16_t> *p_v)
+CandidTypeVecText::CandidTypeVecText(std::vector<std::string> *p_v)
     : CandidTypeVecBase() {
   set_pv(p_v);
 
-  const std::vector<uint16_t> v = const_cast<std::vector<uint16_t> &>(*p_v);
+  const std::vector<std::string> v =
+      const_cast<std::vector<std::string> &>(*p_v);
   set_v(v);
   initialize();
 }
 
 // These constructors are only for encoding
-CandidTypeVecNat16::CandidTypeVecNat16(const std::vector<uint16_t> v)
+CandidTypeVecText::CandidTypeVecText(const std::vector<std::string> v)
     : CandidTypeVecBase() {
   set_v(v);
   initialize();
 }
 
-CandidTypeVecNat16::~CandidTypeVecNat16() {}
+CandidTypeVecText::~CandidTypeVecText() {}
 
-void CandidTypeVecNat16::set_content_type() {
-  m_content_type_opcode = CandidOpcode().Nat16;
-  m_content_type_hex = OpcodeHex().Nat16;
-  m_content_type_textual = OpcodeTextual().Nat16;
+void CandidTypeVecText::set_content_type() {
+  m_content_type_opcode = CandidOpcode().Text;
+  m_content_type_hex = OpcodeHex().Text;
+  m_content_type_textual = OpcodeTextual().Text;
 }
 
-void CandidTypeVecNat16::encode_M() {
+void CandidTypeVecText::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(v^N  : vec <datatype>) = leb128(N) M(v : <datatype>)^N
 
   // encoded size of vec - leb128(N)
   m_M.append_uleb128(__uint128_t(m_v.size()));
 
   // encoded vec values - M(v : <datatype>)^N
-  // Nat16:             - M(n : nat<N>)   = i<N>(n)    (Litte Endian)
-  for (uint16_t const &c : m_v) {
-    m_M.append_int_fixed_width(c);
+  // M(t : text)     = leb128(|utf8(t)|) i8*(utf8(t))
+  for (std::string const &s : m_v) {
+    // encoded size of string - leb128(|utf8(t)|)
+    m_M.append_uleb128(__uint128_t(s.size()));
+
+    // encoded string - i8*(utf8(t))
+    for (char const &c : s) {
+      m_M.append_byte((std::byte)c);
+    }
   }
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeVecNat16::decode_M(VecBytes B, __uint128_t &offset,
-                                  std::string &parse_error) {
+bool CandidTypeVecText::decode_M(VecBytes B, __uint128_t &offset,
+                                 std::string &parse_error) {
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
-  uint16_t v;
   offset_start = offset;
   parse_error = "";
+  CandidTypeText c{""}; // dummy so we can use it's decode_M
   for (size_t i = 0; i < size_vec; ++i) {
-    if (B.parse_int_fixed_width(offset, v, parse_error)) {
-      std::string to_be_parsed = "Vec: Value for CandidTypeNat16";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+    if (c.decode_M(B, offset, parse_error)) {
+      std::string to_be_parsed = "Vec: Value for CandidTypeText";
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
-    m_v.push_back(v);
+    m_v.push_back(c.get_v());
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
 
   return false;
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat32.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat32.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_nat32.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+
 
 CandidTypeVecNat32::CandidTypeVecNat32() : CandidTypeVecBase() {
   std::vector<uint32_t> v;
   set_v(v);
   initialize();
 }
 
@@ -58,26 +60,26 @@
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
   uint32_t v;
   offset_start = offset;
   parse_error = "";
   for (size_t i = 0; i < size_vec; ++i) {
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
       std::string to_be_parsed = "Vec: Value for CandidTypeNat32";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(v);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat32.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat32.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: vec
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_vec_base.h"
+#include "candid_type_nat32.h"
+#include "vec_bytes.h"
 
 class CandidTypeVecNat32 : public CandidTypeVecBase {
 public:
   // Constructors
   CandidTypeVecNat32();
   CandidTypeVecNat32(const std::vector<uint32_t> v);
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat64.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat16.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,85 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_nat16.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
 
-CandidTypeVecNat64::CandidTypeVecNat64() : CandidTypeVecBase() {
-  std::vector<uint64_t> v;
+
+CandidTypeVecNat16::CandidTypeVecNat16() : CandidTypeVecBase() {
+  std::vector<uint16_t> v;
   set_v(v);
   initialize();
 }
 
 // These constructors allows for setting the value during Deserialization
-CandidTypeVecNat64::CandidTypeVecNat64(std::vector<uint64_t> *p_v)
+CandidTypeVecNat16::CandidTypeVecNat16(std::vector<uint16_t> *p_v)
     : CandidTypeVecBase() {
   set_pv(p_v);
 
-  const std::vector<uint64_t> v = const_cast<std::vector<uint64_t> &>(*p_v);
+  const std::vector<uint16_t> v = const_cast<std::vector<uint16_t> &>(*p_v);
   set_v(v);
   initialize();
 }
 
 // These constructors are only for encoding
-CandidTypeVecNat64::CandidTypeVecNat64(const std::vector<uint64_t> v)
+CandidTypeVecNat16::CandidTypeVecNat16(const std::vector<uint16_t> v)
     : CandidTypeVecBase() {
   set_v(v);
   initialize();
 }
 
-CandidTypeVecNat64::~CandidTypeVecNat64() {}
+CandidTypeVecNat16::~CandidTypeVecNat16() {}
 
-void CandidTypeVecNat64::set_content_type() {
-  m_content_type_opcode = CandidOpcode().Nat64;
-  m_content_type_hex = OpcodeHex().Nat64;
-  m_content_type_textual = OpcodeTextual().Nat64;
+void CandidTypeVecNat16::set_content_type() {
+  m_content_type_opcode = CandidOpcode().Nat16;
+  m_content_type_hex = OpcodeHex().Nat16;
+  m_content_type_textual = OpcodeTextual().Nat16;
 }
 
-void CandidTypeVecNat64::encode_M() {
+void CandidTypeVecNat16::encode_M() {
   // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
   // M(v^N  : vec <datatype>) = leb128(N) M(v : <datatype>)^N
 
   // encoded size of vec - leb128(N)
   m_M.append_uleb128(__uint128_t(m_v.size()));
 
   // encoded vec values - M(v : <datatype>)^N
-  // Nat64:             - M(n : nat<N>)   = i<N>(n)    (Litte Endian)
-  for (uint64_t const &c : m_v) {
+  // Nat16:             - M(n : nat<N>)   = i<N>(n)    (Litte Endian)
+  for (uint16_t const &c : m_v) {
     m_M.append_int_fixed_width(c);
   }
 }
 
 // Decode the values, starting at & updating offset
-bool CandidTypeVecNat64::decode_M(VecBytes B, __uint128_t &offset,
+bool CandidTypeVecNat16::decode_M(VecBytes B, __uint128_t &offset,
                                   std::string &parse_error) {
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
-  uint64_t v;
+  uint16_t v;
   offset_start = offset;
   parse_error = "";
   for (size_t i = 0; i < size_vec; ++i) {
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
-      std::string to_be_parsed = "Vec: Value for CandidTypeNat64";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      std::string to_be_parsed = "Vec: Value for CandidTypeNat16";
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(v);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat8.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat8.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_nat8.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+
 
 CandidTypeVecNat8::CandidTypeVecNat8() : CandidTypeVecBase() {
   std::vector<uint8_t> v;
   set_v(v);
   initialize();
 }
 
@@ -58,26 +60,26 @@
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
   uint8_t v;
   offset_start = offset;
   parse_error = "";
   for (size_t i = 0; i < size_vec; ++i) {
     if (B.parse_int_fixed_width(offset, v, parse_error)) {
       std::string to_be_parsed = "Vec: Value for CandidTypeNat8";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(v);
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_nat8.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_nat8.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // The class for the Candid Type: vec
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_vec_base.h"
+#include "candid_type_nat8.h"
+#include "vec_bytes.h"
 
 class CandidTypeVecNat8 : public CandidTypeVecBase {
 public:
   // Constructors
   CandidTypeVecNat8();
   CandidTypeVecNat8(const std::vector<uint8_t> v);
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_principal.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_principal.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 // The class for the Candid Type: vec
 
-#include "candid.h"
+#include "candid_type.h"
+#include "candid_type_vec_principal.h"
+#include "candid_type_principal.h"
+#include "candid_assert.h"
 #include "candid_opcode.h"
 
 #include <cassert>
 
-#include "ic_api.h"
+
 
 CandidTypeVecPrincipal::CandidTypeVecPrincipal() : CandidTypeVecBase() {
   std::vector<std::string> v;
   set_v(v);
   initialize();
 }
 
@@ -60,26 +63,26 @@
   // get size of vec - leb128(N)
   __uint128_t offset_start = offset;
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t size_vec;
   if (B.parse_uleb128(offset, size_vec, numbytes, parse_error)) {
     std::string to_be_parsed = "Size of vec- leb128(N)";
-    CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
+    CandidAssert::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
 
   m_v.clear();
   offset_start = offset;
   parse_error = "";
   CandidTypePrincipal c{""}; // dummy so we can use it's decode_M
   for (size_t i = 0; i < size_vec; ++i) {
     if (c.decode_M(B, offset, parse_error)) {
       std::string to_be_parsed = "Vec: Value for CandidTypePrincipal";
-      CandidDeserialize::trap_with_parse_error(offset_start, offset,
+      CandidAssert::trap_with_parse_error(offset_start, offset,
                                                to_be_parsed, parse_error);
     }
     m_v.push_back(c.get_v());
   }
 
   // Fill the user's data placeholder, if a pointer was provided
   if (m_pv) *m_pv = m_v;
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/candid_type_vec_principal.h` & `icpp-candid-3.0.0/src/icpp_candid/candid/candid_type_vec_text.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-// The class for the Candid Type: vec
+// The class for the Candid Type: text
 
 #pragma once
 
 #include <cstring>
 
-#include "candid.h"
+#include "candid_type_vec_base.h"
+#include "candid_type_text.h"
+#include "vec_bytes.h"
 
-class CandidTypeVecPrincipal : public CandidTypeVecBase {
+class CandidTypeVecText : public CandidTypeVecBase {
 public:
   // Constructors
-  CandidTypeVecPrincipal();
-  CandidTypeVecPrincipal(const std::vector<std::string> v);
+  CandidTypeVecText();
+  CandidTypeVecText(const std::vector<std::string> v);
 
-  CandidTypeVecPrincipal(std::vector<std::string> *p_v);
+  CandidTypeVecText(std::vector<std::string> *p_v);
 
   // Destructor
-  ~CandidTypeVecPrincipal();
+  ~CandidTypeVecText();
 
   bool decode_M(VecBytes B, __uint128_t &offset, std::string &parse_error);
   std::vector<std::string> get_v() { return m_v; }
 
 protected:
   void set_pv(std::vector<std::string> *v) { m_pv = v; }
   void set_v(const std::vector<std::string> &v) { m_v = v; }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/candid/vec_bytes.cpp` & `icpp-candid-3.0.0/src/icpp_candid/candid/vec_bytes.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 //  Wrapper around a std::vector<std::byte>
 
 #include "vec_bytes.h"
 
 #include <cassert>
 #include <cstring>
+#include <cstdint>
 
 #include <algorithm>
 #include <bit>
 #include <string>
 
 #include <limits.h>
 #include <limits>
 #include <sstream>
 
-#include "ic_api.h"
+#include "icpp_hooks.h"
 
 #define INT_STR_SIZE (sizeof(int) * CHAR_BIT / 3 + 3)
 
 VecBytes::VecBytes() { check_endian(); }
 
 VecBytes::~VecBytes() {}
 
@@ -80,15 +81,15 @@
     if (found_non_zero || i > 5) {
 
       str[j] = arr[ch];
 
       if (str[j] != '0') {
         found_non_zero = true;
         if (i < 6) {
-          IC_API::trap(
+          ICPP_HOOKS::trap(
               "PROGRAM ERROR in int_to_hex. Hex string has more than 2 "
               "characters?");
         }
       }
       ++j;
     }
   }
@@ -109,15 +110,15 @@
   } while (i);
 
   if (x < 0) {
     *(--p) = '-';
   }
   size_t len = (size_t)(&buf[INT_STR_SIZE] - p);
   if (len > size) {
-    IC_API::trap(
+    ICPP_HOOKS::trap(
         "PROGRAM ERROR in c_int_to_dec - Buffer to small to store decimal "
         "representation of int");
   }
   memcpy(str, p, len);
 }
 
 void VecBytes::append_didl() {
@@ -205,17 +206,17 @@
   numbytes = 0;
 
   __uint128_t len = m_vec.size() - offset;
 
   if (n > len) {
     parse_error =
         "Not enough bytes left. The remaining bytes in the byte stream on wire is ";
-    parse_error.append(IC_API::to_string_128(len));
+    parse_error.append(ICPP_HOOKS::to_string_128(len));
     parse_error.append(", but specified number to parse is ");
-    parse_error.append(IC_API::to_string_128(n));
+    parse_error.append(ICPP_HOOKS::to_string_128(n));
     return true;
   }
 
   std::copy(m_vec.begin() + offset, m_vec.begin() + offset + n,
             std::back_inserter(v));
 
   numbytes = n;
@@ -232,17 +233,17 @@
   numbytes = 0;
 
   __uint128_t len = m_vec.size() - offset;
 
   if (n > len) {
     parse_error =
         "Not enough bytes left. The remaining bytes in the byte stream on wire is ";
-    parse_error.append(IC_API::to_string_128(len));
+    parse_error.append(ICPP_HOOKS::to_string_128(len));
     parse_error.append(", but specified number to parse is ");
-    parse_error.append(IC_API::to_string_128(n));
+    parse_error.append(ICPP_HOOKS::to_string_128(n));
     return true;
   }
 
   std::copy(m_vec_uint8_t.begin() + offset, m_vec_uint8_t.begin() + offset + n,
             std::back_inserter(v));
 
   numbytes = n;
@@ -302,36 +303,36 @@
 void VecBytes::trap_if_vec_does_not_start_with_DIDL() {
   std::string s;
   s.append(byte_to_char(m_vec[0]));
   s.append(byte_to_char(m_vec[1]));
   s.append(byte_to_char(m_vec[2]));
   s.append(byte_to_char(m_vec[3]));
   if (s != "DIDL") {
-    IC_API::trap("ERROR: Message does not start with DIDL");
+    ICPP_HOOKS::trap("ERROR: Message does not start with DIDL");
   }
 }
 
 // Prints the bytes of the vec in hex, dec & bits
 void VecBytes::debug_print() {
-  IC_API::debug_print("  hex, decimal, char");
+  ICPP_HOOKS::debug_print("  hex, decimal, char");
 
   std::string s_hex;
   for (std::byte b : m_vec) {
     std::string s;
     s.append("   ");
     s.append(byte_to_hex(b, ""));
     s.append(", ");
     s.append(byte_to_dec(b, 8));
     s.append(", ");
     s.append(byte_to_char(b));
     s_hex.append(byte_to_hex(b, ""));
 
-    IC_API::debug_print(s); // Print a nice table: hex, decimal, char
+    ICPP_HOOKS::debug_print(s); // Print a nice table: hex, decimal, char
   }
-  IC_API::debug_print(
+  ICPP_HOOKS::debug_print(
       s_hex); // Print the whole thing in hex on one line, for didc decode !
 }
 
 void VecBytes::clear() {
   m_vec.clear();
   m_vec_uint8_t.clear();
 }
@@ -351,23 +352,23 @@
   if (in[i] == '+') {
     ++i;
   }
 
   for (; i < in.size(); ++i) {
     const char c = in[i];
     if (not std::isdigit(c))
-      IC_API::trap(std::string("Non-numeric character: ") + c);
+      ICPP_HOOKS::trap(std::string("Non-numeric character: ") + c);
 
     // TODO: implement multiplication overflow protection: https://stackoverflow.com/a/1815371/5480536
     res *= 10;
 
     res += c - '0';
     // https://stackoverflow.com/a/6472982/5480536
     if (res < c - '0') {
-      IC_API::trap(
+      ICPP_HOOKS::trap(
           std::string(
               "ERROR: Overflow - Cannot convert string to __uint128t.\n       Number is too big: ") +
           in);
     }
   }
 
   if (sign) {
@@ -385,23 +386,23 @@
   if (in[i] == '+') {
     ++i;
   }
 
   for (; i < in.size(); ++i) {
     const char c = in[i];
     if (not std::isdigit(c))
-      IC_API::trap(std::string("Non-numeric character: ") + c);
+      ICPP_HOOKS::trap(std::string("Non-numeric character: ") + c);
 
     // TODO: implement multiplication overflow protection: https://stackoverflow.com/a/1815371/5480536
     res *= 10;
 
     res += c - '0';
     // https://stackoverflow.com/a/6472982/5480536
     if (res < c - '0') {
-      IC_API::trap(
+      ICPP_HOOKS::trap(
           std::string(
               "ERROR: Overflow - Cannot convert string to __uint128t.\n       Number is too big: ") +
           in);
     }
   }
 
   return res;
@@ -552,12 +553,126 @@
 void VecBytes::check_endian() {
   if (is_little_endian()) m_endian_type = "little";
   else if (is_big_endian()) {
     m_endian_type = "big";
   } else if (is_mixed_endian()) {
     m_endian_type = "mixed";
   } else {
-    IC_API::trap("Could not determine endianness of architecture. ");
+    ICPP_HOOKS::trap("Could not determine endianness of architecture. ");
   }
 }
 
-void VecBytes::trap(const std::string &msg) { IC_API::trap(msg); }
+void VecBytes::trap(const std::string &msg) { ICPP_HOOKS::trap(msg); }
+
+// -----------------------------------------------------------------------------
+// template definitions with Explicit Template Instantiations
+// Doing it this way avoids the COMDAT warnings & multiple definitions errors
+
+template <typename T>
+  requires MyFixedWidthInts<T>
+void VecBytes::append_int_fixed_width(const T &v) {
+  uint8_t *bytes{nullptr};
+  if (is_little_endian()) bytes = (uint8_t *)&v;
+  else
+    // Probably best to do a memcpy and then a byteswap
+    trap(
+        "ERROR: append_int_fixed_width not yet implemented on big endian architecture");
+
+  append_bytes(bytes, sizeof(v));
+}
+// clang-format off
+template void VecBytes::append_int_fixed_width<int8_t>  (const int8_t   &v);
+template void VecBytes::append_int_fixed_width<int16_t> (const int16_t  &v);
+template void VecBytes::append_int_fixed_width<int32_t> (const int32_t  &v);
+template void VecBytes::append_int_fixed_width<int64_t> (const int64_t  &v);
+template void VecBytes::append_int_fixed_width<uint8_t> (const uint8_t  &v);
+template void VecBytes::append_int_fixed_width<uint16_t>(const uint16_t &v);
+template void VecBytes::append_int_fixed_width<uint32_t>(const uint32_t &v);
+template void VecBytes::append_int_fixed_width<uint64_t>(const uint64_t &v);
+// clang-format on
+
+// --
+template <typename T>
+  requires MyFloats<T>
+void VecBytes::append_float_ieee754(const T &v) {
+  if (is_float_ieee754()) {
+    // https://github.com/dfinity/candid/blob/master/spec/Candid.md#floating-point-numbers
+    // Floating-point values are represented in IEEE 754 binary format and are
+    // supported in single precision (32 bit) and double precision (64 bit).
+    // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
+    // M(z : float<N>) = f<N>(z)
+    uint32_t off_now = 0;
+    uint8_t *bytes = (uint8_t *)&v;
+    append_bytes(bytes, sizeof(v));
+  } else
+    trap("ERROR in " + std::string(__func__) +
+         ". The encoding method requires that your system is using IEEE "
+         "754 floating point which it does not. "
+         "(std::numeric_limits<double>::is_iec559 == false)");
+}
+// clang-format off
+template void VecBytes::append_float_ieee754<float>  (const float &v);
+template void VecBytes::append_float_ieee754<double> (const double &v);
+// clang-format on
+
+// --
+template <typename T>
+  requires MyFixedWidthInts<T>
+bool VecBytes::parse_int_fixed_width(__uint128_t &offset, T &v,
+                                     std::string &parse_error) {
+  __uint128_t len = m_vec.size() - offset;
+
+  uint8_t *buf = &m_vec_uint8_t[offset];
+  uint8_t *buf_end = &m_vec_uint8_t[offset + len];
+
+  parse_error = "";
+  std::memcpy(&v, buf, sizeof(v));
+
+  offset += sizeof(v);
+
+  return false;
+}
+
+// clang-format off
+template bool VecBytes::parse_int_fixed_width<int8_t>  (__uint128_t &offset, int8_t   &v, std::string &parse_error);
+template bool VecBytes::parse_int_fixed_width<int16_t> (__uint128_t &offset, int16_t  &v, std::string &parse_error);
+template bool VecBytes::parse_int_fixed_width<int32_t> (__uint128_t &offset, int32_t  &v, std::string &parse_error);
+template bool VecBytes::parse_int_fixed_width<int64_t> (__uint128_t &offset, int64_t  &v, std::string &parse_error);
+template bool VecBytes::parse_int_fixed_width<uint8_t> (__uint128_t &offset, uint8_t  &v, std::string &parse_error);
+template bool VecBytes::parse_int_fixed_width<uint16_t>(__uint128_t &offset, uint16_t &v, std::string &parse_error);
+template bool VecBytes::parse_int_fixed_width<uint32_t>(__uint128_t &offset, uint32_t &v, std::string &parse_error);
+template bool VecBytes::parse_int_fixed_width<uint64_t>(__uint128_t &offset, uint64_t &v, std::string &parse_error);
+// clang-format on
+
+// --
+template <typename T>
+  requires MyFloats<T>
+bool VecBytes::parse_float_ieee754(__uint128_t &offset, T &v,
+                                   std::string &parse_error) {
+  if (is_float_ieee754()) {
+    // https://github.com/dfinity/candid/blob/master/spec/Candid.md#floating-point-numbers
+    // Floating-point values are represented in IEEE 754 binary format and are
+    // supported in single precision (32 bit) and double precision (64 bit).
+    // https://github.com/dfinity/candid/blob/master/spec/Candid.md#memory
+    // M(z : float<N>) = f<N>(z)
+    __uint128_t len = m_vec.size() - offset;
+
+    uint8_t *buf = &m_vec_uint8_t[offset];
+    uint8_t *buf_end = &m_vec_uint8_t[offset + len];
+
+    parse_error = "";
+    std::memcpy(&v, buf, sizeof(v));
+
+    offset += sizeof(v);
+
+  } else
+    trap("ERROR in " + std::string(__func__) +
+         ". The encoding method requires that your system is using IEEE "
+         "754 floating point which it does not. "
+         "(std::numeric_limits<double>::is_iec559 == false)");
+
+  return false;
+}
+// clang-format off
+template bool VecBytes::parse_float_ieee754<float>  (__uint128_t &offset, float  &v, std::string &parse_error);
+template bool VecBytes::parse_float_ieee754<double> (__uint128_t &offset, double &v, std::string &parse_error);
+// clang-format on
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/LICENSE` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/LICENSE`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_crockford.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_hex.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_hex.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_default_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_default_url.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_default_url_unpadded.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_rfc4648.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_url.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_url.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/base64_url_unpadded.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/data/access.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/data/access.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/data/raw_result_buffer.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/base32.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/base32.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 #include <stdlib.h> // for abort()
 
 #include "../data/access.hpp"
 #include "../parse_error.hpp"
 #include "config.hpp"
 #include "stream_codec.hpp"
 
-#include "ic_api.h" // for trap iso throw
+#include "icpp_hooks.h" // for trap iso throw
 
 namespace cppcodec {
 namespace detail {
 
 template <typename CodecVariant>
 class base32 : public CodecVariant::template codec_impl<base32<CodecVariant>> {
 public:
@@ -60,15 +60,15 @@
     //                                     "invalid number of bytes in a tail block");
 
     uint8_t v = (num_bytes == 1)   ? 2 // 2 symbols, 6 padding characters
                 : (num_bytes == 2) ? 4 // 4 symbols, 4 padding characters
                 : (num_bytes == 3) ? 5 // 5 symbols, 3 padding characters
                 : (num_bytes == 4) ? 7 // 7 symbols, 1 padding characters
                                    : 0;
-    if (v == 0) IC_API::trap("invalid number of bytes in a tail block");
+    if (v == 0) ICPP_HOOKS::trap("invalid number of bytes in a tail block");
     return v;
   }
 
   template <uint8_t I>
   static CPPCODEC_ALWAYS_INLINE constexpr uint8_t
   index(const uint8_t *b /*binary block*/) noexcept {
     static_assert(I >= 0 && I < encoded_block_size(),
@@ -96,15 +96,15 @@
                ? ((b[2] << 1) & 0x1E)             // abbreviated 5th symbol
                : /*I == 6*/ ((b[3] << 3) & 0x18); // abbreviated 7th symbol
   }
 
   template <uint8_t I>
   static CPPCODEC_ALWAYS_INLINE uint8_if<I != 1 && I != 3 && I != 4 && I != 6>
   index_last(const uint8_t * /*binary block*/) {
-    IC_API::trap("invalid last encoding symbol index in a tail");
+    ICPP_HOOKS::trap("invalid last encoding symbol index in a tail");
     return 0; // AB - avoid compiler warning
     // throw std::domain_error("invalid last encoding symbol index in a tail");
   }
 
   template <typename Result, typename ResultState>
   static CPPCODEC_ALWAYS_INLINE void
   decode_block(Result &decoded, ResultState &, const alphabet_index_t *idx);
@@ -141,27 +141,27 @@
 
 template <typename CodecVariant>
 template <typename Result, typename ResultState>
 CPPCODEC_ALWAYS_INLINE void
 base32<CodecVariant>::decode_tail(Result &decoded, ResultState &state,
                                   const alphabet_index_t *idx, size_t idx_len) {
   if (idx_len == 1) {
-    IC_API::trap(
+    ICPP_HOOKS::trap(
         "invalid number of symbols in last base32 block: found 1, expected 2, 4, 5 or 7");
     // throw invalid_input_length(
     // "invalid number of symbols in last base32 block: found 1, expected 2, 4, 5 or 7");
   }
   if (idx_len == 3) {
-    IC_API::trap(
+    ICPP_HOOKS::trap(
         "invalid number of symbols in last base32 block: found 3, expected 2, 4, 5 or 7");
     // throw invalid_input_length(
     //         "invalid number of symbols in last base32 block: found 3, expected 2, 4, 5 or 7");
   }
   if (idx_len == 6) {
-    IC_API::trap(
+    ICPP_HOOKS::trap(
         "invalid number of symbols in last base32 block: found 6, expected 2, 4, 5 or 7");
     // throw invalid_input_length(
     // "invalid number of symbols in last base32 block: found 6, expected 2, 4, 5 or 7");
   }
 
   // idx_len == 2: decoded size 1
   put(decoded, state,
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/base64.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/base64.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 #include <stdint.h>
 
 #include "../data/access.hpp"
 #include "../parse_error.hpp"
 #include "config.hpp"
 #include "stream_codec.hpp"
 
-#include "ic_api.h" // for trap iso throw
+#include "icpp_hooks.h" // for trap iso throw
 
 namespace cppcodec {
 namespace detail {
 
 template <typename CodecVariant>
 class base64 : public CodecVariant::template codec_impl<base64<CodecVariant>> {
 public:
@@ -54,15 +54,15 @@
     //            : (num_bytes == 2) ? 3 // 3 symbols, 1 padding character
     //                               : throw std::domain_error(
     //                                     "invalid number of bytes in a tail block");
 
     uint8_t v = (num_bytes == 1)   ? 2 // 2 symbols, 2 padding characters
                 : (num_bytes == 2) ? 3 // 3 symbols, 1 padding character
                                    : 0;
-    if (v == 0) IC_API::trap("invalid number of bytes in a tail block");
+    if (v == 0) ICPP_HOOKS::trap("invalid number of bytes in a tail block");
     return v;
   }
 
   template <uint8_t I>
   static CPPCODEC_ALWAYS_INLINE constexpr uint8_t
   index(const uint8_t *b /*binary block*/) noexcept {
     static_assert(I >= 0 && I < encoded_block_size(),
@@ -82,15 +82,15 @@
     return (I == 1) ? ((b[0] & 0x3) << 4)             // abbreviated 2nd symbol
                     : /*I == 2*/ ((b[1] & 0xF) << 2); // abbreviated 3rd symbol
   }
 
   template <uint8_t I>
   static CPPCODEC_ALWAYS_INLINE uint8_if<I != 1 && I != 2>
   index_last(const uint8_t * /*binary block*/) {
-    IC_API::trap("invalid last encoding symbol index in a tail");
+    ICPP_HOOKS::trap("invalid last encoding symbol index in a tail");
     // throw std::domain_error("invalid last encoding symbol index in a tail");
   }
 
   template <typename Result, typename ResultState>
   static CPPCODEC_ALWAYS_INLINE void
   decode_block(Result &decoded, ResultState &, const alphabet_index_t *idx);
 
@@ -113,15 +113,15 @@
 
 template <typename CodecVariant>
 template <typename Result, typename ResultState>
 CPPCODEC_ALWAYS_INLINE void
 base64<CodecVariant>::decode_tail(Result &decoded, ResultState &state,
                                   const alphabet_index_t *idx, size_t idx_len) {
   if (idx_len == 1) {
-    IC_API::trap(
+    ICPP_HOOKS::trap(
         "invalid number of symbols in last base64 block: found 1, expected 2 or 3");
     // throw invalid_input_length(
     // "invalid number of symbols in last base64 block: found 1, expected 2 or 3");
   }
 
   // idx_len == 2: decoded size 1
   data::put(decoded, state,
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/codec.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/codec.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/config.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/config.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/hex.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/hex.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #include <stdint.h>
 #include <stdlib.h> // for abort()
 
 #include "../data/access.hpp"
 #include "../parse_error.hpp"
 #include "stream_codec.hpp"
 
-#include "ic_api.h" // for trap iso throw
+#include "icpp_hooks.h" // for trap iso throw
 
 namespace cppcodec {
 namespace detail {
 
 template <typename CodecVariant>
 class hex : public CodecVariant::template codec_impl<hex<CodecVariant>> {
 public:
@@ -70,15 +70,15 @@
   index_last(const uint8_t * /*binary block*/) noexcept {
     return 0;
   }
 
   template <uint8_t I>
   static CPPCODEC_ALWAYS_INLINE uint8_if<I != 0>
   index_last(const uint8_t * /*binary block*/) {
-    IC_API::trap("invalid last encoding symbol index in a tail");
+    ICPP_HOOKS::trap("invalid last encoding symbol index in a tail");
     // throw std::domain_error("invalid last encoding symbol index in a tail");
   }
 
   template <typename Result, typename ResultState>
   static CPPCODEC_ALWAYS_INLINE void
   decode_block(Result &decoded, ResultState &, const alphabet_index_t *idx);
 
@@ -97,15 +97,15 @@
 }
 
 template <typename CodecVariant>
 template <typename Result, typename ResultState>
 CPPCODEC_ALWAYS_INLINE void
 hex<CodecVariant>::decode_tail(Result &, ResultState &,
                                const alphabet_index_t *, size_t) {
-  IC_API::trap(
+  ICPP_HOOKS::trap(
       "odd-length hex input is not supported by the streaming octet decoder, "
       "use a place-based number decoder instead");
   //   throw invalid_input_length(
   //       "odd-length hex input is not supported by the streaming octet decoder, "
   //       "use a place-based number decoder instead");
 }
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/detail/stream_codec.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #include <limits>
 #include <stdint.h>
 #include <stdlib.h> // for abort()
 
 #include "../parse_error.hpp"
 #include "config.hpp"
 
-#include "ic_api.h" // for trap iso throw
+#include "icpp_hooks.h" // for trap iso throw
 
 namespace cppcodec {
 namespace detail {
 
 using alphabet_index_t = uint_fast16_t;
 
 template <typename Codec, typename CodecVariant> class stream_codec {
@@ -391,57 +391,57 @@
     if (alphabet_index_ptr == alphabet_index_end) {
       Codec::decode_block(binary_result, state, alphabet_indexes);
       alphabet_index_ptr = alphabet_index_start;
     }
   }
 
   if (alphabet_index_info<CodecVariant>::is_invalid(*alphabet_index_ptr)) {
-    IC_API::trap("Symbol Error");
+    ICPP_HOOKS::trap("Symbol Error");
     // throw symbol_error(*src);
   }
   ++src;
 
   alphabet_index_t *last_index_ptr = alphabet_index_ptr;
   if (alphabet_index_info<CodecVariant>::is_padding(*last_index_ptr)) {
     if (last_index_ptr == alphabet_index_start) {
       // Don't accept padding at the start of a block.
       // The encoder should have omitted that padding altogether.
-      IC_API::trap("Padding Error");
+      ICPP_HOOKS::trap("Padding Error");
       // throw padding_error();
     }
     // We're in here because we just read a (first) padding character. Try to read more.
     // Count with last_index_ptr, but store in alphabet_index_ptr so we don't
     // overflow the array in case the input data is too long.
     ++last_index_ptr;
     while (src < src_end) {
       *alphabet_index_ptr = alphabet_index_lookup::for_symbol(*(src++));
 
       if (alphabet_index_info<CodecVariant>::is_eof(*alphabet_index_ptr)) {
         *alphabet_index_ptr = alphabet_index_info<CodecVariant>::padding_idx;
         break;
       }
       if (!alphabet_index_info<CodecVariant>::is_padding(*alphabet_index_ptr)) {
-        IC_API::trap("Padding Error");
+        ICPP_HOOKS::trap("Padding Error");
         // throw padding_error();
       }
 
       ++last_index_ptr;
       if (last_index_ptr > alphabet_index_end) {
-        IC_API::trap("Padding Error");
+        ICPP_HOOKS::trap("Padding Error");
         // throw padding_error();
       }
     }
   }
 
   if (last_index_ptr != alphabet_index_start) {
     if ((CodecVariant::requires_padding() ||
          alphabet_index_info<CodecVariant>::is_padding(*alphabet_index_ptr)) &&
         last_index_ptr != alphabet_index_end) {
       // If the input is not a multiple of the block size then the input is incorrect.
-      IC_API::trap("Padding Error");
+      ICPP_HOOKS::trap("Padding Error");
       // throw padding_error();
     }
     if (alphabet_index_ptr >= alphabet_index_end) {
       abort();
       return;
     }
     Codec::decode_tail(
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/hex_default_lower.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/hex_default_upper.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/hex_lower.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/hex_lower.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/hex_upper.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/hex_upper.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/cppcodec/parse_error.hpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/cppcodec/parse_error.hpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/LICENSE` & `icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/LICENSE`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/crc32.cpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/crc32.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/crc32.h` & `icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/crc32.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/readme.md` & `icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/readme.md`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/sha256.cpp` & `icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/sha256.cpp`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid/vendors/hash-library/sha256.h` & `icpp-candid-3.0.0/src/icpp_candid/vendors/hash-library/sha256.h`

 * *Files identical despite different names*

### Comparing `icpp-candid-2.9.0/src/icpp_candid.egg-info/PKG-INFO` & `icpp-candid-3.0.0/src/icpp_candid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpp-candid
-Version: 2.9.0
+Version: 3.0.0
 Summary: C++ Candid Library
 Home-page: https://docs.icpp.world/
 Author: icppWorld
 Author-email: icpp@icpp.world
 License: MIT
 Keywords: C++ Candid Library,Internet Computer,C++,Candid,blockchain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `icpp-candid-2.9.0/src/icpp_candid.egg-info/SOURCES.txt` & `icpp-candid-3.0.0/src/icpp_candid.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 src/icpp_candid/py.typed
 src/icpp_candid/version.py
 src/icpp_candid.egg-info/PKG-INFO
 src/icpp_candid.egg-info/SOURCES.txt
 src/icpp_candid.egg-info/dependency_links.txt
 src/icpp_candid.egg-info/requires.txt
 src/icpp_candid.egg-info/top_level.txt
-src/icpp_candid/candid/candid.h
+src/icpp_candid/candid/candid_args.cpp
+src/icpp_candid/candid/candid_args.h
 src/icpp_candid/candid/candid_assert.cpp
 src/icpp_candid/candid/candid_assert.h
 src/icpp_candid/candid/candid_deserialize.cpp
 src/icpp_candid/candid/candid_deserialize.h
 src/icpp_candid/candid/candid_opcode.cpp
 src/icpp_candid/candid/candid_opcode.h
 src/icpp_candid/candid/candid_serialize.cpp
 src/icpp_candid/candid/candid_serialize.h
+src/icpp_candid/candid/candid_type.h
+src/icpp_candid/candid/candid_type_all_includes.h
 src/icpp_candid/candid/candid_type_base.cpp
 src/icpp_candid/candid/candid_type_base.h
 src/icpp_candid/candid/candid_type_bool.cpp
 src/icpp_candid/candid/candid_type_bool.h
 src/icpp_candid/candid/candid_type_empty.cpp
 src/icpp_candid/candid/candid_type_empty.h
 src/icpp_candid/candid/candid_type_float32.cpp
@@ -79,16 +82,14 @@
 src/icpp_candid/candid/candid_type_opt_nat64.h
 src/icpp_candid/candid/candid_type_opt_nat8.cpp
 src/icpp_candid/candid/candid_type_opt_nat8.h
 src/icpp_candid/candid/candid_type_opt_principal.cpp
 src/icpp_candid/candid/candid_type_opt_principal.h
 src/icpp_candid/candid/candid_type_opt_text.cpp
 src/icpp_candid/candid/candid_type_opt_text.h
-src/icpp_candid/candid/candid_type_prim.cpp
-src/icpp_candid/candid/candid_type_prim.h
 src/icpp_candid/candid/candid_type_principal.cpp
 src/icpp_candid/candid/candid_type_principal.h
 src/icpp_candid/candid/candid_type_record.cpp
 src/icpp_candid/candid/candid_type_record.h
 src/icpp_candid/candid/candid_type_reserved.cpp
 src/icpp_candid/candid/candid_type_reserved.h
 src/icpp_candid/candid/candid_type_table.cpp
@@ -127,14 +128,16 @@
 src/icpp_candid/candid/candid_type_vec_nat8.h
 src/icpp_candid/candid/candid_type_vec_principal.cpp
 src/icpp_candid/candid/candid_type_vec_principal.h
 src/icpp_candid/candid/candid_type_vec_text.cpp
 src/icpp_candid/candid/candid_type_vec_text.h
 src/icpp_candid/candid/vec_bytes.cpp
 src/icpp_candid/candid/vec_bytes.h
+src/icpp_candid/hooks/icpp_hooks.cpp
+src/icpp_candid/hooks/icpp_hooks.h
 src/icpp_candid/vendors/cppcodec/LICENSE
 src/icpp_candid/vendors/cppcodec/base32_crockford.hpp
 src/icpp_candid/vendors/cppcodec/base32_default_crockford.hpp
 src/icpp_candid/vendors/cppcodec/base32_default_hex.hpp
 src/icpp_candid/vendors/cppcodec/base32_default_rfc4648.hpp
 src/icpp_candid/vendors/cppcodec/base32_hex.hpp
 src/icpp_candid/vendors/cppcodec/base32_rfc4648.hpp
```

