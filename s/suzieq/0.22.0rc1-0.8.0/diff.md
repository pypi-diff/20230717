# Comparing `tmp/suzieq-0.22.0rc1.tar.gz` & `tmp/suzieq-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suzieq-0.22.0rc1.tar", max compression
+gzip compressed data, was "suzieq-0.8.0.tar", last modified: Tue Dec 15 21:03:12 2020, max compression
```

## Comparing `suzieq-0.22.0rc1.tar` & `suzieq-0.8.0.tar`

### file list

```diff
@@ -1,351 +1,134 @@
--rw-r--r--   0        0        0    11357 2022-03-18 00:37:24.944678 suzieq-0.22.0rc1/LICENSE
--rw-r--r--   0        0        0     9787 2023-05-09 02:11:05.242507 suzieq-0.22.0rc1/README.md
--rw-r--r--   0        0        0     2309 2023-07-17 09:45:32.285625 suzieq-0.22.0rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-04 21:32:22.000000 suzieq-0.22.0rc1/suzieq/__init__.py
--rw-r--r--   0        0        0        0 2020-02-04 21:32:22.000000 suzieq-0.22.0rc1/suzieq/cli/__init__.py
--rw-r--r--   0        0        0     3404 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/nubia_patch.py
--rwxr-xr-x   0        0        0      456 2022-04-16 06:58:37.928770 suzieq-0.22.0rc1/suzieq/cli/sq_cli.py
--rw-r--r--   0        0        0     1666 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sq_nubia_context.py
--rw-r--r--   0        0        0     3279 2022-03-18 00:37:24.960678 suzieq-0.22.0rc1/suzieq/cli/sq_nubia_plugin.py
--rw-r--r--   0        0        0     2050 2022-03-18 00:37:24.960678 suzieq-0.22.0rc1/suzieq/cli/sq_nubia_statusbar.py
--rw-r--r--   0        0        0     2029 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/AddressCmd.py
--rw-r--r--   0        0        0     1689 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/ArpndCmd.py
--rw-r--r--   0        0        0     2979 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/BgpCmd.py
--rw-r--r--   0        0        0     1212 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/DevconfigCmd.py
--rw-r--r--   0        0        0     2056 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/DeviceCmd.py
--rw-r--r--   0        0        0     2107 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/EvpnVniCmd.py
--rw-r--r--   0        0        0     2243 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/FsCmd.py
--rw-r--r--   0        0        0     3891 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/InterfaceCmd.py
--rw-r--r--   0        0        0     2133 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/InventoryCmd.py
--rw-r--r--   0        0        0     1481 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/LldpCmd.py
--rw-r--r--   0        0        0     1908 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/MacCmd.py
--rw-r--r--   0        0        0      902 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/MlagCmd.py
--rw-r--r--   0        0        0     2047 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/NamespaceCmd.py
--rw-r--r--   0        0        0     7423 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/NetworkCmd.py
--rw-r--r--   0        0        0     2449 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/OspfCmd.py
--rw-r--r--   0        0        0     1343 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/PathCmd.py
--rw-r--r--   0        0        0     3388 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/RouteCmd.py
--rw-r--r--   0        0        0     1793 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/SqPollerCmd.py
--rw-r--r--   0        0        0      904 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/TableCmd.py
--rw-r--r--   0        0        0      859 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/TopcpuCmd.py
--rw-r--r--   0        0        0      881 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/TopmemCmd.py
--rw-r--r--   0        0        0     2276 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/TopologyCmd.py
--rw-r--r--   0        0        0     1470 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/VlanCmd.py
--rw-r--r--   0        0        0      477 2021-12-02 00:15:34.959206 suzieq-0.22.0rc1/suzieq/cli/sqcmds/__init__.py
--rw-r--r--   0        0        0    21059 2023-06-08 14:24:02.743137 suzieq-0.22.0rc1/suzieq/cli/sqcmds/command.py
--rw-r--r--   0        0        0     7697 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/cli/sqcmds/context_commands.py
--rw-r--r--   0        0        0     3628 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/arpnd.yml
--rw-r--r--   0        0        0    11771 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/bgp.yml
--rw-r--r--   0        0        0     1023 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/devconfig.yml
--rw-r--r--   0        0        0     4044 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/device.yml
--rw-r--r--   0        0        0     2037 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/etc/cert.pem
--rw-r--r--   0        0        0        0 2021-12-22 06:19:16.262410 suzieq-0.22.0rc1/suzieq/config/etc/inventory/inventory.yaml
--rw-r--r--   0        0        0     3272 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/etc/key.pem
--rw-r--r--   0        0        0     1675 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/etc/ssh_insecure_key
--rw-r--r--   0        0        0     3014 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/etc/suzieq-cfg.yml
--rw-r--r--   0        0        0     4340 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/config/evpnVni.yml
--rw-r--r--   0        0        0      686 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/fs.yml
--rw-r--r--   0        0        0      887 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/ifCounters.yml
--rw-r--r--   0        0        0     8207 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/interfaces.yml
--rw-r--r--   0        0        0     2102 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/inventory.yml
--rw-r--r--   0        0        0     5001 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/lldp.yml
--rw-r--r--   0        0        0     2510 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/macs.yml
--rw-r--r--   0        0        0     4209 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/mlag.yml
--rw-r--r--   0        0        0     4275 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/ospfIf.yml
--rw-r--r--   0        0        0     2948 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/ospfNbr.yml
--rw-r--r--   0        0        0     5093 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/routes.yml
--rw-r--r--   0        0        0     3079 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/address.avsc
--rw-r--r--   0        0        0     2148 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/arpnd.avsc
--rw-r--r--   0        0        0     9960 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/bgp.avsc
--rw-r--r--   0        0        0     1443 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/devconfig.avsc
--rw-r--r--   0        0        0     2558 2023-07-17 03:03:47.380079 suzieq-0.22.0rc1/suzieq/config/schema/device.avsc
--rw-r--r--   0        0        0     3718 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/evpnVni.avsc
--rw-r--r--   0        0        0     2314 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/fs.avsc
--rw-r--r--   0        0        0     2424 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/ifCounters.avsc
--rw-r--r--   0        0        0     5526 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/interfaces.avsc
--rw-r--r--   0        0        0     2719 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/inventory.avsc
--rw-r--r--   0        0        0     2558 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/lldp.avsc
--rw-r--r--   0        0        0     2801 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/macs.avsc
--rw-r--r--   0        0        0     5113 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/mlag.avsc
--rw-r--r--   0        0        0     2344 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/config/schema/namespace.avsc
--rw-r--r--   0        0        0     1830 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/network.avsc
--rw-r--r--   0        0        0     5808 2022-03-29 21:28:27.020830 suzieq-0.22.0rc1/suzieq/config/schema/ospf.avsc
--rw-r--r--   0        0        0     3050 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/ospfIf.avsc
--rw-r--r--   0        0        0     2826 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/ospfNbr.avsc
--rw-r--r--   0        0        0     3718 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/path.avsc
--rw-r--r--   0        0        0     4890 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/routes.avsc
--rw-r--r--   0        0        0     1638 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/schema/sqCoalescer.avsc
--rw-r--r--   0        0        0     4910 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/config/schema/sqPoller.avsc
--rw-r--r--   0        0        0     1687 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/tables.avsc
--rw-r--r--   0        0        0     1573 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/time.avsc
--rw-r--r--   0        0        0     2757 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/topcpu.avsc
--rw-r--r--   0        0        0     2757 2023-05-09 02:11:05.250507 suzieq-0.22.0rc1/suzieq/config/schema/topmem.avsc
--rw-r--r--   0        0        0     2964 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/schema/topology.avsc
--rw-r--r--   0        0        0     2030 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/schema/vlan.avsc
--rw-r--r--   0        0        0     1791 2022-07-19 03:49:42.211126 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/cl_interfaces.tfsm
--rw-r--r--   0        0        0     1018 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/cl_meminfo.tfsm
--rw-r--r--   0        0        0      316 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/cl_showsys.tfsm
--rw-r--r--   0        0        0      981 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/cl_top.tfsm
--rw-r--r--   0        0        0     7608 2022-06-03 18:42:41.138821 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/cls_device.tfsm
--rw-r--r--   0        0        0     7609 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/cls_model_rel.tfsm
--rw-r--r--   0        0        0       74 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/cls_uptime_hostname.tfsm
--rw-r--r--   0        0        0      634 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/eos_ospfif.tfsm
--rw-r--r--   0        0        0      635 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/eos_ospfnbr.tfsm
--rw-r--r--   0        0        0     6992 2022-07-27 18:46:47.956085 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/eos_show_bgp_nbr.tfsm
--rw-r--r--   0        0        0      131 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/eos_showclock.tfsm
--rw-r--r--   0        0        0      373 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/eos_showver.tfsm
--rw-r--r--   0        0        0      314 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/eos_vlan.tfsm
--rw-r--r--   0        0        0     3006 2022-05-14 04:51:00.016375 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/frr_ospfif.tfsm
--rw-r--r--   0        0        0     2101 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/frr_ospfnbr.tfsm
--rw-r--r--   0        0        0      702 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/frr_ospfnbr_brief.tfsm
--rw-r--r--   0        0        0     1684 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/fs.tfsm
--rw-r--r--   0        0        0      680 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/ifCounters.tfsm
--rw-r--r--   0        0        0      964 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_arp.tfsm
--rw-r--r--   0        0        0    18218 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_bgp_neigh.tfsm
--rw-r--r--   0        0        0     2411 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_bgp_summ.tfsm
--rw-r--r--   0        0        0    15040 2022-05-06 19:33:54.146513 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_int.tfsm
--rw-r--r--   0        0        0     2020 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_int_trunk.tfsm
--rw-r--r--   0        0        0      643 2022-03-29 21:28:27.024830 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_inventory.tfsm
--rw-r--r--   0        0        0     3235 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_ip_int.tfsm
--rw-r--r--   0        0        0     4046 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_ip_ospf.tfsm
--rw-r--r--   0        0        0     6077 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_ip_ospfif.tfsm
--rw-r--r--   0        0        0     1965 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_ip_ospfnbr.tfsm
--rw-r--r--   0        0        0     1273 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_ipv6_int.tfsm
--rw-r--r--   0        0        0      569 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_ipv6_neigh.tfsm
--rw-r--r--   0        0        0     1775 2022-06-06 18:11:21.916410 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_lldp_neigh.tfsm
--rw-r--r--   0        0        0     3672 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_mac.tfsm
--rw-r--r--   0        0        0     9150 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_route.tfsm
--rw-r--r--   0        0        0     2553 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_version.tfsm
--rw-r--r--   0        0        0      272 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_vlan.tfsm
--rw-r--r--   0        0        0     1656 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxe_show_vrf.tfsm
--rw-r--r--   0        0        0      523 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_arp.tfsm
--rw-r--r--   0        0        0     6317 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_bgp_neigh.tfsm
--rw-r--r--   0        0        0     4019 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_bgp_summ.tfsm
--rw-r--r--   0        0        0      785 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_clock.tfsm
--rw-r--r--   0        0        0      443 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_fs.tfsm
--rw-r--r--   0        0        0    10141 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_int.tfsm
--rw-r--r--   0        0        0     2043 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_ip_int.tfsm
--rw-r--r--   0        0        0      451 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_ipv6_int.tfsm
--rw-r--r--   0        0        0     2043 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_ipv6_neigh.tfsm
--rw-r--r--   0        0        0     1112 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_lldp_neigh.tfsm
--rw-r--r--   0        0        0      820 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_ntp.tfsm
--rw-r--r--   0        0        0     5416 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_route.tfsm
--rw-r--r--   0        0        0      327 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_version.tfsm
--rw-r--r--   0        0        0     1099 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_vrf_detail.tfsm
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/iosxr_show_vrf_tfsm
--rw-r--r--   0        0        0     1689 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/junos_vpls_mac.tfsm
--rw-r--r--   0        0        0     2705 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/linux_fdb.tfsm
--rw-r--r--   0        0        0      966 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/linux_ipaddr.tfsm
--rw-r--r--   0        0        0      332 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/linux_ipneigh.tfsm
--rw-r--r--   0        0        0      296 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/linux_meminfo.tfsm
--rw-r--r--   0        0        0     1323 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/linux_routes.tfsm
--rw-r--r--   0        0        0      252 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/linux_showsys.tfsm
--rw-r--r--   0        0        0      981 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/linux_top.tfsm
--rw-r--r--   0        0        0      184 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/linux_topproc.tfsm
--rw-r--r--   0        0        0      188 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/linux_vlan.tfsm
--rw-r--r--   0        0        0     2335 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/lldpd.tfsm
--rw-r--r--   0        0        0     2358 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_if_fabric.tfsm
--rw-r--r--   0        0        0    15873 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_bgp_nbr.tfsm
--rw-r--r--   0        0        0     3246 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_bgp_summ.tfsm
--rw-r--r--   0        0        0      201 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_clock.tfsm
--rw-r--r--   0        0        0     1735 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_int_brief.tfsm
--rw-r--r--   0        0        0     2444 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_int_grep.tfsm
--rw-r--r--   0        0        0      254 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_int_nve.tfsm
--rw-r--r--   0        0        0     1453 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_int_xcvr.tfsm
--rw-r--r--   0        0        0     1632 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_inventory.tfsm
--rw-r--r--   0        0        0      303 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_ip_arp.tfsm
--rw-r--r--   0        0        0      632 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_ip_int.tfsm
--rw-r--r--   0        0        0      416 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_ip_ospf.tfsm
--rw-r--r--   0        0        0     2355 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_ip_ospfif.tfsm
--rw-r--r--   0        0        0      561 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_ip_ospfnbr.tfsm
--rw-r--r--   0        0        0     2125 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_ip_route.tfsm
--rw-r--r--   0        0        0      489 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_ipv6_int.tfsm
--rw-r--r--   0        0        0      349 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_lldp.tfsm
--rw-r--r--   0        0        0      302 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_mac.tfsm
--rw-r--r--   0        0        0      331 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_nve_ifname.tfsm
--rw-r--r--   0        0        0      851 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_version.tfsm
--rw-r--r--   0        0        0      333 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_vlan.tfsm
--rw-r--r--   0        0        0      935 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_vpc.tfsm
--rw-r--r--   0        0        0       72 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_vpc_ka.tfsm
--rw-r--r--   0        0        0       95 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_vpc_orphans.tfsm
--rw-r--r--   0        0        0      284 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_vpc_role.tfsm
--rw-r--r--   0        0        0      220 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/nxos_show_vrf.tfsm
--rw-r--r--   0        0        0     1358 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/sonic_mclag_dump_state.tfsm
--rw-r--r--   0        0        0      305 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/sonic_show_version.tfsm
--rw-r--r--   0        0        0      387 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/sonic_showsys.tfsm
--rw-r--r--   0        0        0      217 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/system.tfsm
--rw-r--r--   0        0        0      264 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/config/textfsm_templates/timedatectl.tfsm
--rw-r--r--   0        0        0      571 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/time.yml
--rw-r--r--   0        0        0      511 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/topcpu.yml
--rw-r--r--   0        0        0      534 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/topmem.yml
--rw-r--r--   0        0        0     2129 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/config/vlan.yml
--rw-r--r--   0        0        0      184 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/db/__init__.py
--rw-r--r--   0        0        0     2970 2023-05-09 02:11:05.254507 suzieq-0.22.0rc1/suzieq/db/base_db.py
--rw-r--r--   0        0        0     2309 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/db/dblib.py
--rw-r--r--   0        0        0      498 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/db/parquet/__init__.py
--rw-r--r--   0        0        0      956 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/db/parquet/dataset_utils.py
--rw-r--r--   0        0        0     6705 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/db/parquet/migratedb.py
--rw-r--r--   0        0        0    35741 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/db/parquet/parquetdb.py
--rw-r--r--   0        0        0    14905 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/db/parquet/pq_coalesce.py
--rw-r--r--   0        0        0      930 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/engines/__init__.py
--rw-r--r--   0        0        0     1344 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/base_engine.py
--rw-r--r--   0        0        0      860 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/engines/pandas/__init__.py
--rw-r--r--   0        0        0    10582 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/address.py
--rw-r--r--   0        0        0     3434 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/arpnd.py
--rw-r--r--   0        0        0    12412 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/bgp.py
--rw-r--r--   0        0        0      269 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/engines/pandas/devconfig.py
--rw-r--r--   0        0        0     7047 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/engines/pandas/device.py
--rw-r--r--   0        0        0    27694 2023-07-17 09:12:01.706609 suzieq-0.22.0rc1/suzieq/engines/pandas/engineobj.py
--rw-r--r--   0        0        0    14234 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/evpnVni.py
--rw-r--r--   0        0        0      596 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/fs.py
--rw-r--r--   0        0        0      270 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/engines/pandas/ifCounters.py
--rw-r--r--   0        0        0    30391 2023-07-17 03:03:47.380079 suzieq-0.22.0rc1/suzieq/engines/pandas/interfaces.py
--rw-r--r--   0        0        0     4082 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/inventory.py
--rw-r--r--   0        0        0     7978 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/lldp.py
--rw-r--r--   0        0        0     3980 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/macs.py
--rw-r--r--   0        0        0     1052 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/engines/pandas/mlag.py
--rw-r--r--   0        0        0     4691 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/engines/pandas/namespace.py
--rw-r--r--   0        0        0    25614 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/network.py
--rw-r--r--   0        0        0    22067 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/ospf.py
--rw-r--r--   0        0        0      149 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/engines/pandas/ospfIf.py
--rw-r--r--   0        0        0      150 2022-03-18 00:37:24.964679 suzieq-0.22.0rc1/suzieq/engines/pandas/ospfNbr.py
--rw-r--r--   0        0        0    58920 2023-07-17 09:12:01.706609 suzieq-0.22.0rc1/suzieq/engines/pandas/path.py
--rw-r--r--   0        0        0     8781 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/routes.py
--rw-r--r--   0        0        0     3233 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/engines/pandas/sqPoller.py
--rw-r--r--   0        0        0     3227 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/engines/pandas/tables.py
--rw-r--r--   0        0        0      250 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/engines/pandas/time.py
--rw-r--r--   0        0        0      256 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/engines/pandas/topcpu.py
--rw-r--r--   0        0        0      256 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/engines/pandas/topmem.py
--rw-r--r--   0        0        0    16577 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/engines/pandas/topology.py
--rw-r--r--   0        0        0     2070 2023-06-27 04:10:06.055081 suzieq-0.22.0rc1/suzieq/engines/pandas/vlan.py
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/engines/rest/__init__.py
--rw-r--r--   0        0        0     3977 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/engines/rest/engineobj.py
--rw-r--r--   0        0        0    15051 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/gui/Suzieq-logo-2.jpg
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/gui/__init__.py
--rw-r--r--   0        0        0     2007 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/gui/help-pages/Path.md
--rw-r--r--   0        0        0     2459 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/gui/images/helps.png
--rw-r--r--   0        0        0    18748 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/gui/images/logo-small.jpg
--rw-r--r--   0        0        0     3366 2021-09-28 05:32:34.000000 suzieq-0.22.0rc1/suzieq/gui/pages/gui_topo.py
--rw-r--r--   0        0        0     2290 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/gui/sq_gui.py
--rw-r--r--   0        0        0      877 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/gui/stlit/__init__.py
--rw-r--r--   0        0        0     7928 2023-07-17 03:03:47.384079 suzieq-0.22.0rc1/suzieq/gui/stlit/guiutils.py
--rw-r--r--   0        0        0     1426 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/gui/stlit/help.py
--rw-r--r--   0        0        0     3418 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/gui/stlit/pagecls.py
--rw-r--r--   0        0        0    18161 2023-07-17 03:03:47.384079 suzieq-0.22.0rc1/suzieq/gui/stlit/path.py
--rw-r--r--   0        0        0    11271 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/gui/stlit/path_debug.py
--rw-r--r--   0        0        0    14373 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/gui/stlit/search.py
--rw-r--r--   0        0        0     9666 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/gui/stlit/status.py
--rw-r--r--   0        0        0     7121 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/gui/stlit/suzieq-gui.py
--rw-r--r--   0        0        0    26593 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/gui/stlit/xplore.py
--rw-r--r--   0        0        0       56 2020-04-24 22:57:23.000000 suzieq-0.22.0rc1/suzieq/local.yml
--rw-r--r--   0        0        0        0 2020-03-06 14:10:17.000000 suzieq-0.22.0rc1/suzieq/poller/__init__.py
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/controller/__init__.py
--rw-r--r--   0        0        0     2458 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/poller/controller/base_controller_plugin.py
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/controller/chunker/__init__.py
--rw-r--r--   0        0        0     1036 2022-03-29 21:28:27.024830 suzieq-0.22.0rc1/suzieq/poller/controller/chunker/base_chunker.py
--rw-r--r--   0        0        0     6004 2022-03-29 21:28:27.024830 suzieq-0.22.0rc1/suzieq/poller/controller/chunker/static.py
--rw-r--r--   0        0        0    14045 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/controller/controller.py
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/controller/credential_loader/__init__.py
--rw-r--r--   0        0        0     4764 2022-07-27 18:46:47.956085 suzieq-0.22.0rc1/suzieq/poller/controller/credential_loader/base_credential_loader.py
--rw-r--r--   0        0        0     6331 2022-03-29 21:28:27.024830 suzieq-0.22.0rc1/suzieq/poller/controller/credential_loader/cred_file.py
--rw-r--r--   0        0        0     3544 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/controller/credential_loader/static.py
--rw-r--r--   0        0        0      715 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/controller/inventory_async_plugin.py
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/controller/manager/__init__.py
--rw-r--r--   0        0        0     1600 2022-03-29 21:28:27.024830 suzieq-0.22.0rc1/suzieq/poller/controller/manager/base_manager.py
--rw-r--r--   0        0        0    16026 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/controller/manager/static.py
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/controller/source/__init__.py
--rw-r--r--   0        0        0     4993 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/poller/controller/source/ansible.py
--rw-r--r--   0        0        0    11331 2023-07-17 03:03:47.384079 suzieq-0.22.0rc1/suzieq/poller/controller/source/base_source.py
--rw-r--r--   0        0        0     5030 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/controller/source/native.py
--rw-r--r--   0        0        0    14511 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/controller/source/netbox.py
--rw-r--r--   0        0        0     1984 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/controller/utils/inventory_models.py
--rw-r--r--   0        0        0    11631 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/controller/utils/inventory_utils.py
--rw-r--r--   0        0        0     1154 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/controller/utils/proc_utils.py
--rw-r--r--   0        0        0     5939 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/sq_poller.py
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/worker/__init__.py
--rw-r--r--   0        0        0     5369 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/worker/coalescer_launcher.py
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/worker/inventory/__init__.py
--rw-r--r--   0        0        0     1238 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/worker/inventory/dir.py
--rw-r--r--   0        0        0     8230 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/worker/inventory/inventory.py
--rw-r--r--   0        0        0     3112 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/worker/inventory/static.py
--rw-r--r--   0        0        0       69 2022-04-23 15:48:37.520659 suzieq-0.22.0rc1/suzieq/poller/worker/nodes/__init__.py
--rw-r--r--   0        0        0     7018 2023-05-09 02:11:05.258507 suzieq-0.22.0rc1/suzieq/poller/worker/nodes/files.py
--rw-r--r--   0        0        0    99507 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/poller/worker/nodes/node.py
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/worker/services/__init__.py
--rw-r--r--   0        0        0     4954 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/arpnd.py
--rw-r--r--   0        0        0    29894 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/bgp.py
--rw-r--r--   0        0        0     1637 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/devconfig.py
--rw-r--r--   0        0        0     7501 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/device.py
--rw-r--r--   0        0        0    10702 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/evpnVni.py
--rw-r--r--   0        0        0    43524 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/poller/worker/services/interfaces.py
--rw-r--r--   0        0        0    10914 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/inventory.py
--rw-r--r--   0        0        0     9105 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/lldp.py
--rw-r--r--   0        0        0     8539 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/macs.py
--rw-r--r--   0        0        0     5625 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/mlag.py
--rw-r--r--   0        0        0     8247 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/ospfIf.py
--rw-r--r--   0        0        0     6029 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/ospfNbr.py
--rw-r--r--   0        0        0    14652 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/poller/worker/services/routes.py
--rw-r--r--   0        0        0    38565 2023-06-08 14:24:02.747137 suzieq-0.22.0rc1/suzieq/poller/worker/services/service.py
--rw-r--r--   0        0        0    16973 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/service_manager.py
--rw-r--r--   0        0        0    22679 2023-06-08 14:24:02.751137 suzieq-0.22.0rc1/suzieq/poller/worker/services/svcparser.py
--rw-r--r--   0        0        0      626 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/worker/services/topcpu.py
--rw-r--r--   0        0        0      643 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/worker/services/topmem.py
--rw-r--r--   0        0        0     7289 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/services/vlan.py
--rwxr-xr-x   0        0        0     3732 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/sq_worker.py
--rw-r--r--   0        0        0    10447 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/worker.py
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/worker/writers/__init__.py
--rw-r--r--   0        0        0      720 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/worker/writers/gather.py
--rw-r--r--   0        0        0     1261 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/poller/worker/writers/output_worker.py
--rw-r--r--   0        0        0     2423 2022-03-29 21:28:27.028831 suzieq-0.22.0rc1/suzieq/poller/worker/writers/output_worker_manager.py
--rw-r--r--   0        0        0     2607 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/poller/worker/writers/parquet.py
--rwxr-xr-x   0        0        0    36248 2023-07-17 03:03:47.384079 suzieq-0.22.0rc1/suzieq/restServer/query.py
--rwxr-xr-x   0        0        0      134 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/restServer/sq_rest_server.py
--rw-r--r--   0        0        0        0 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/shared/__init__.py
--rw-r--r--   0        0        0     6006 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/shared/confutils.py
--rw-r--r--   0        0        0     1682 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/shared/context.py
--rw-r--r--   0        0        0     1285 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/shared/exceptions.py
--rw-r--r--   0        0        0     2380 2023-06-08 14:24:02.751137 suzieq-0.22.0rc1/suzieq/shared/poller_error_codes.py
--rw-r--r--   0        0        0    11947 2023-06-08 14:24:02.751137 suzieq-0.22.0rc1/suzieq/shared/schema.py
--rw-r--r--   0        0        0     3302 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/shared/sq_plugin.py
--rw-r--r--   0        0        0    40593 2023-06-08 14:24:02.751137 suzieq-0.22.0rc1/suzieq/shared/utils.py
--rw-r--r--   0        0        0     1032 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/sqobjects/__init__.py
--rw-r--r--   0        0        0     1294 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/address.py
--rw-r--r--   0        0        0     1587 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/arpnd.py
--rw-r--r--   0        0        0    21533 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/basicobj.py
--rw-r--r--   0        0        0     1629 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/bgp.py
--rw-r--r--   0        0        0      511 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/devconfig.py
--rw-r--r--   0        0        0     1328 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/device.py
--rw-r--r--   0        0        0      998 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/evpnVni.py
--rw-r--r--   0        0        0      407 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/sqobjects/fs.py
--rw-r--r--   0        0        0      363 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/sqobjects/ifCounters.py
--rw-r--r--   0        0        0     2151 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/interfaces.py
--rw-r--r--   0        0        0      466 2022-03-25 17:56:48.393319 suzieq-0.22.0rc1/suzieq/sqobjects/inventory.py
--rw-r--r--   0        0        0      412 2022-03-29 21:28:27.028831 suzieq-0.22.0rc1/suzieq/sqobjects/lldp.py
--rw-r--r--   0        0        0     1430 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/macs.py
--rw-r--r--   0        0        0      327 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/sqobjects/mlag.py
--rw-r--r--   0        0        0     1198 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/namespace.py
--rw-r--r--   0        0        0     3092 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/network.py
--rw-r--r--   0        0        0     2099 2023-05-09 02:11:05.262507 suzieq-0.22.0rc1/suzieq/sqobjects/ospf.py
--rw-r--r--   0        0        0      443 2022-07-27 18:46:47.960085 suzieq-0.22.0rc1/suzieq/sqobjects/ospfIf.py
--rw-r--r--   0        0        0      432 2022-07-27 18:46:47.960085 suzieq-0.22.0rc1/suzieq/sqobjects/ospfNbr.py
--rw-r--r--   0        0        0      733 2023-05-09 02:11:05.266507 suzieq-0.22.0rc1/suzieq/sqobjects/path.py
--rw-r--r--   0        0        0     2237 2023-05-09 02:11:05.266507 suzieq-0.22.0rc1/suzieq/sqobjects/routes.py
--rw-r--r--   0        0        0      477 2022-03-29 21:28:27.028831 suzieq-0.22.0rc1/suzieq/sqobjects/sqPoller.py
--rw-r--r--   0        0        0     1348 2023-06-08 14:24:02.751137 suzieq-0.22.0rc1/suzieq/sqobjects/tables.py
--rw-r--r--   0        0        0      327 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/sqobjects/time.py
--rw-r--r--   0        0        0      333 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/sqobjects/topcpu.py
--rw-r--r--   0        0        0      333 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/sqobjects/topmem.py
--rw-r--r--   0        0        0     2219 2023-05-09 02:11:05.266507 suzieq-0.22.0rc1/suzieq/sqobjects/topology.py
--rw-r--r--   0        0        0      470 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/sqobjects/vlan.py
--rw-r--r--   0        0        0     2649 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/utilities/convert_legacy_dataset.py
--rw-r--r--   0        0        0     1302 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/utilities/find_invalid_parquet.py
--rw-r--r--   0        0        0     6402 2022-03-18 00:37:24.968679 suzieq-0.22.0rc1/suzieq/utilities/gen_schema.py
--rw-r--r--   0        0        0     3586 2022-03-18 00:37:24.972679 suzieq-0.22.0rc1/suzieq/utilities/migrate_data.py
--rw-r--r--   0        0        0    15941 2022-03-18 00:37:24.972679 suzieq-0.22.0rc1/suzieq/utilities/sq_anonymizer.py
--rwxr-xr-x   0        0        0     7188 2023-05-09 02:11:05.266507 suzieq-0.22.0rc1/suzieq/utilities/sq_coalescer.py
--rw-r--r--   0        0        0     5075 2022-03-18 00:37:24.972679 suzieq-0.22.0rc1/suzieq/utilities/sq_simnode.py
--rw-r--r--   0        0        0     3141 2022-03-18 00:37:24.972679 suzieq-0.22.0rc1/suzieq/utilities/sq_simnode_rest.py
--rw-r--r--   0        0        0     6143 2023-05-09 02:11:05.266507 suzieq-0.22.0rc1/suzieq/utilities/sq_simnode_ssh.py
--rwxr-xr-x   0        0        0      146 2023-07-17 09:45:19.185464 suzieq-0.22.0rc1/suzieq/version.py
--rw-r--r--   0        0        0   541802 1970-01-01 00:00:00.000000 suzieq-0.22.0rc1/setup.py
--rw-r--r--   0        0        0    11823 1970-01-01 00:00:00.000000 suzieq-0.22.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2020-02-03 20:03:05.167695 suzieq-0.8.0/LICENSE
+-rw-r--r--   0        0        0      975 2020-12-15 21:01:29.367762 suzieq-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4794 2020-04-23 19:42:12.686360 suzieq-0.8.0/suzieq/.ropeproject/config.py
+-rw-r--r--   0        0        0        0 2020-02-04 21:32:22.985194 suzieq-0.8.0/suzieq/__init__.py
+-rw-r--r--   0        0        0    32704 2020-04-24 22:57:23.174106 suzieq-0.8.0/suzieq/cli/Untitled.ipynb
+-rw-r--r--   0        0        0        0 2020-02-04 21:32:22.985194 suzieq-0.8.0/suzieq/cli/__init__.py
+-rw-r--r--   0        0        0     1637 2020-11-14 06:49:48.303491 suzieq-0.8.0/suzieq/cli/sq_nubia_context.py
+-rw-r--r--   0        0        0     4018 2020-04-17 03:14:20.967647 suzieq-0.8.0/suzieq/cli/sq_nubia_plugin.py
+-rw-r--r--   0        0        0     1971 2020-11-14 06:49:48.303491 suzieq-0.8.0/suzieq/cli/sq_nubia_statusbar.py
+-rw-r--r--   0        0        0     1742 2020-09-14 04:22:57.167193 suzieq-0.8.0/suzieq/cli/sqcmds/AddressCmd.py
+-rw-r--r--   0        0        0     1780 2020-11-04 18:53:11.599016 suzieq-0.8.0/suzieq/cli/sqcmds/ArpndCmd.py
+-rw-r--r--   0        0        0     4923 2020-12-10 20:07:52.457969 suzieq-0.8.0/suzieq/cli/sqcmds/BgpCmd.py
+-rw-r--r--   0        0        0     3064 2020-12-10 20:07:52.457969 suzieq-0.8.0/suzieq/cli/sqcmds/DeviceCmd.py
+-rw-r--r--   0        0        0     2026 2020-11-24 06:42:41.135975 suzieq-0.8.0/suzieq/cli/sqcmds/EvpnVniCmd.py
+-rw-r--r--   0        0        0     2338 2020-09-15 17:36:46.041840 suzieq-0.8.0/suzieq/cli/sqcmds/FsCmd.py
+-rw-r--r--   0        0        0     4662 2020-12-10 20:07:52.457969 suzieq-0.8.0/suzieq/cli/sqcmds/InterfaceCmd.py
+-rw-r--r--   0        0        0     1503 2020-11-04 18:53:11.599016 suzieq-0.8.0/suzieq/cli/sqcmds/LldpCmd.py
+-rw-r--r--   0        0        0     2606 2020-09-15 17:36:46.041840 suzieq-0.8.0/suzieq/cli/sqcmds/MacCmd.py
+-rw-r--r--   0        0        0     1488 2020-09-14 04:22:57.179193 suzieq-0.8.0/suzieq/cli/sqcmds/MlagCmd.py
+-rw-r--r--   0        0        0     4506 2020-12-10 20:07:52.457969 suzieq-0.8.0/suzieq/cli/sqcmds/OspfCmd.py
+-rw-r--r--   0        0        0     3247 2020-09-14 04:22:57.183194 suzieq-0.8.0/suzieq/cli/sqcmds/PathCmd.py
+-rw-r--r--   0        0        0     4096 2020-11-24 14:38:08.305189 suzieq-0.8.0/suzieq/cli/sqcmds/RouteCmd.py
+-rw-r--r--   0        0        0     1688 2020-11-24 16:39:31.235499 suzieq-0.8.0/suzieq/cli/sqcmds/SqPollerCmd.py
+-rw-r--r--   0        0        0     2398 2020-04-24 22:57:23.178106 suzieq-0.8.0/suzieq/cli/sqcmds/TableCmd.py
+-rw-r--r--   0        0        0     1386 2020-09-14 04:22:57.187193 suzieq-0.8.0/suzieq/cli/sqcmds/TopcpuCmd.py
+-rw-r--r--   0        0        0     1387 2020-09-14 04:22:57.187193 suzieq-0.8.0/suzieq/cli/sqcmds/TopmemCmd.py
+-rw-r--r--   0        0        0     2932 2020-11-03 14:48:53.320419 suzieq-0.8.0/suzieq/cli/sqcmds/TopologyCmd.py
+-rw-r--r--   0        0        0     1720 2020-11-24 19:18:17.813972 suzieq-0.8.0/suzieq/cli/sqcmds/VlanCmd.py
+-rw-r--r--   0        0        0      477 2020-04-17 03:14:20.967647 suzieq-0.8.0/suzieq/cli/sqcmds/__init__.py
+-rw-r--r--   0        0        0     8196 2020-12-10 20:07:52.461969 suzieq-0.8.0/suzieq/cli/sqcmds/command.py
+-rw-r--r--   0        0        0     2239 2020-11-14 06:49:48.303491 suzieq-0.8.0/suzieq/cli/sqcmds/context_commands.py
+-rwxr-xr-x   0        0        0      320 2020-03-05 03:45:12.766758 suzieq-0.8.0/suzieq/cli/suzieq-cli
+-rw-r--r--   0        0        0       99 2020-03-05 03:45:12.766758 suzieq-0.8.0/suzieq/engines/__init__.py
+-rw-r--r--   0        0        0      390 2020-03-05 03:45:12.766758 suzieq-0.8.0/suzieq/engines/base_engine.py
+-rw-r--r--   0        0        0        0 2020-02-04 21:32:22.997196 suzieq-0.8.0/suzieq/engines/pandas/__init__.py
+-rw-r--r--   0        0        0     8014 2020-12-10 20:07:52.461969 suzieq-0.8.0/suzieq/engines/pandas/address.py
+-rw-r--r--   0        0        0      797 2020-09-14 13:07:21.435893 suzieq-0.8.0/suzieq/engines/pandas/arpnd.py
+-rw-r--r--   0        0        0    10897 2020-12-10 20:07:52.461969 suzieq-0.8.0/suzieq/engines/pandas/bgp.py
+-rw-r--r--   0        0        0     1773 2020-12-11 03:55:58.218713 suzieq-0.8.0/suzieq/engines/pandas/device.py
+-rw-r--r--   0        0        0    10340 2020-12-10 20:07:52.461969 suzieq-0.8.0/suzieq/engines/pandas/engine.py
+-rw-r--r--   0        0        0    16895 2020-12-14 04:51:26.607815 suzieq-0.8.0/suzieq/engines/pandas/engineobj.py
+-rw-r--r--   0        0        0    12016 2020-12-10 20:07:52.461969 suzieq-0.8.0/suzieq/engines/pandas/evpnVni.py
+-rw-r--r--   0        0        0       99 2020-02-21 02:55:19.901131 suzieq-0.8.0/suzieq/engines/pandas/fs.py
+-rw-r--r--   0        0        0      107 2020-02-21 02:55:19.905131 suzieq-0.8.0/suzieq/engines/pandas/ifCounters.py
+-rw-r--r--   0        0        0     9422 2020-12-10 20:07:52.461969 suzieq-0.8.0/suzieq/engines/pandas/interfaces.py
+-rw-r--r--   0        0        0      557 2020-09-14 13:07:21.435893 suzieq-0.8.0/suzieq/engines/pandas/lldp.py
+-rw-r--r--   0        0        0     1155 2020-09-15 17:36:45.997839 suzieq-0.8.0/suzieq/engines/pandas/macs.py
+-rw-r--r--   0        0        0      847 2020-07-15 22:29:40.038546 suzieq-0.8.0/suzieq/engines/pandas/mlag.py
+-rw-r--r--   0        0        0    13120 2020-12-13 23:04:59.445214 suzieq-0.8.0/suzieq/engines/pandas/ospf.py
+-rw-r--r--   0        0        0      103 2020-02-21 02:55:19.905131 suzieq-0.8.0/suzieq/engines/pandas/ospfIf.py
+-rw-r--r--   0        0        0      104 2020-02-21 02:55:19.905131 suzieq-0.8.0/suzieq/engines/pandas/ospfNbr.py
+-rw-r--r--   0        0        0    34290 2020-12-10 20:07:52.465969 suzieq-0.8.0/suzieq/engines/pandas/path.py
+-rw-r--r--   0        0        0     8417 2020-12-10 20:07:52.465969 suzieq-0.8.0/suzieq/engines/pandas/routes.py
+-rw-r--r--   0        0        0      927 2020-11-04 21:05:04.904354 suzieq-0.8.0/suzieq/engines/pandas/sqPoller.py
+-rw-r--r--   0        0        0      102 2020-02-21 02:55:19.905131 suzieq-0.8.0/suzieq/engines/pandas/tables.py
+-rw-r--r--   0        0        0      101 2020-02-21 02:55:19.905131 suzieq-0.8.0/suzieq/engines/pandas/time.py
+-rw-r--r--   0        0        0       82 2020-03-05 03:45:12.774757 suzieq-0.8.0/suzieq/engines/pandas/topcpu.py
+-rw-r--r--   0        0        0       82 2020-03-05 03:45:12.774757 suzieq-0.8.0/suzieq/engines/pandas/topmem.py
+-rw-r--r--   0        0        0    10387 2020-11-03 14:48:53.320419 suzieq-0.8.0/suzieq/engines/pandas/topology.py
+-rw-r--r--   0        0        0     1991 2020-12-14 00:13:54.842733 suzieq-0.8.0/suzieq/engines/pandas/vlan.py
+-rw-r--r--   0        0        0     1504 2020-04-28 04:40:20.265386 suzieq-0.8.0/suzieq/eos.yml
+-rw-r--r--   0        0        0      197 2020-04-09 05:24:00.074925 suzieq-0.8.0/suzieq/exceptions.py
+-rw-r--r--   0        0        0     6258 2020-04-24 22:57:23.178106 suzieq-0.8.0/suzieq/gen_schema.py
+-rw-r--r--   0        0        0     2224 2020-04-28 04:40:16.309373 suzieq-0.8.0/suzieq/genhosts.py
+-rw-r--r--   0        0        0    15051 2020-12-10 20:07:52.465969 suzieq-0.8.0/suzieq/gui/Suzieq-logo-2.jpg
+-rw-r--r--   0        0        0        0 2020-12-10 20:07:52.465969 suzieq-0.8.0/suzieq/gui/__init__.py
+-rw-r--r--   0        0        0     1211 2020-07-15 22:52:49.637272 suzieq-0.8.0/suzieq/gui/gui-dash.py
+-rw-r--r--   0        0        0      144 2020-07-15 22:52:49.637272 suzieq-0.8.0/suzieq/gui/gui-dtale.py
+-rw-r--r--   0        0        0     4907 2020-12-10 20:07:52.465969 suzieq-0.8.0/suzieq/gui/guiutils.py
+-rw-r--r--   0        0        0     9966 2020-05-09 13:49:54.524226 suzieq-0.8.0/suzieq/gui/notebooks/Untitled.ipynb
+-rw-r--r--   0        0        0      266 2020-12-10 20:07:52.465969 suzieq-0.8.0/suzieq/gui/pages/__init__.py
+-rw-r--r--   0        0        0     4110 2020-12-10 20:07:52.469969 suzieq-0.8.0/suzieq/gui/pages/gui_path.py
+-rw-r--r--   0        0        0     5016 2020-12-12 02:22:50.714429 suzieq-0.8.0/suzieq/gui/pages/search.py
+-rw-r--r--   0        0        0     6606 2020-12-11 04:06:11.948614 suzieq-0.8.0/suzieq/gui/pages/status.py
+-rw-r--r--   0        0        0    12882 2020-12-14 04:51:26.607815 suzieq-0.8.0/suzieq/gui/pages/xplore.py
+-rw-r--r--   0        0        0      810 2020-07-15 22:36:37.914061 suzieq-0.8.0/suzieq/gui/pyproject.toml
+-rw-r--r--   0        0        0     2611 2020-12-10 20:07:52.469969 suzieq-0.8.0/suzieq/gui/session_state.py
+-rw-r--r--   0        0        0     4450 2020-12-11 03:50:26.689692 suzieq-0.8.0/suzieq/gui/suzieq-gui.py
+-rw-r--r--   0        0        0       56 2020-04-24 22:57:23.178106 suzieq-0.8.0/suzieq/local.yml
+-rw-r--r--   0        0        0        0 2020-03-06 14:10:17.729894 suzieq-0.8.0/suzieq/poller/__init__.py
+-rw-r--r--   0        0        0     4730 2020-11-24 04:00:45.328403 suzieq-0.8.0/suzieq/poller/genhosts.py
+-rw-r--r--   0        0        0      107 2020-07-29 14:08:02.126500 suzieq-0.8.0/suzieq/poller/nodes/__init__.py
+-rw-r--r--   0        0        0     5888 2020-11-01 07:19:39.835485 suzieq-0.8.0/suzieq/poller/nodes/files.py
+-rw-r--r--   0        0        0    38815 2020-12-12 02:30:13.944569 suzieq-0.8.0/suzieq/poller/nodes/node.py
+-rw-r--r--   0        0        0     7458 2020-11-24 04:00:47.620429 suzieq-0.8.0/suzieq/poller/services/__init__.py
+-rw-r--r--   0        0        0     2604 2020-11-14 06:49:48.307491 suzieq-0.8.0/suzieq/poller/services/arpnd.py
+-rw-r--r--   0        0        0     9248 2020-08-19 05:49:16.328664 suzieq-0.8.0/suzieq/poller/services/bgp.py
+-rw-r--r--   0        0        0     3338 2020-12-10 20:07:52.469969 suzieq-0.8.0/suzieq/poller/services/device.py
+-rw-r--r--   0        0        0     7595 2020-12-10 20:07:52.469969 suzieq-0.8.0/suzieq/poller/services/evpnVni.py
+-rw-r--r--   0        0        0    18746 2020-12-03 13:14:56.788557 suzieq-0.8.0/suzieq/poller/services/interfaces.py
+-rw-r--r--   0        0        0     1357 2020-09-14 13:07:21.435893 suzieq-0.8.0/suzieq/poller/services/lldp.py
+-rw-r--r--   0        0        0     5200 2020-11-24 04:00:45.244402 suzieq-0.8.0/suzieq/poller/services/macs.py
+-rw-r--r--   0        0        0     4692 2020-11-26 04:27:27.269017 suzieq-0.8.0/suzieq/poller/services/mlag.py
+-rw-r--r--   0        0        0     3372 2020-11-24 04:00:45.272402 suzieq-0.8.0/suzieq/poller/services/ospfIf.py
+-rw-r--r--   0        0        0     3101 2020-09-14 13:07:21.435893 suzieq-0.8.0/suzieq/poller/services/ospfNbr.py
+-rw-r--r--   0        0        0     5405 2020-11-14 06:49:48.307491 suzieq-0.8.0/suzieq/poller/services/routes.py
+-rw-r--r--   0        0        0    28199 2020-11-24 04:00:47.512428 suzieq-0.8.0/suzieq/poller/services/service.py
+-rw-r--r--   0        0        0    20596 2020-11-14 06:49:48.311492 suzieq-0.8.0/suzieq/poller/services/svcparser.py
+-rw-r--r--   0        0        0      595 2020-08-19 05:49:16.332664 suzieq-0.8.0/suzieq/poller/services/topcpu.py
+-rw-r--r--   0        0        0      594 2020-08-19 05:49:16.332664 suzieq-0.8.0/suzieq/poller/services/topmem.py
+-rw-r--r--   0        0        0     2833 2020-11-24 04:00:47.492428 suzieq-0.8.0/suzieq/poller/services/vlan.py
+-rwxr-xr-x   0        0        0    10607 2020-12-12 04:55:33.140361 suzieq-0.8.0/suzieq/poller/sq-poller
+-rw-r--r--   0        0        0     3587 2020-09-13 06:30:31.770772 suzieq-0.8.0/suzieq/poller/writer.py
+-rw-r--r--   0        0        0     3051 2020-03-05 03:45:12.774757 suzieq-0.8.0/suzieq/purge-old-cntrs.py
+-rwxr-xr-x   0        0        0    20118 2020-12-10 20:07:52.469969 suzieq-0.8.0/suzieq/restServer/query.py
+-rwxr-xr-x   0        0        0     2038 2020-11-05 02:45:32.304771 suzieq-0.8.0/suzieq/restServer/sq-rest-server.py
+-rw-r--r--   0        0        0      253 2020-03-05 03:45:12.778757 suzieq-0.8.0/suzieq/sqobjects/__init__.py
+-rw-r--r--   0        0        0      305 2020-12-10 20:07:52.469969 suzieq-0.8.0/suzieq/sqobjects/address.py
+-rw-r--r--   0        0        0      304 2020-12-10 20:07:52.473969 suzieq-0.8.0/suzieq/sqobjects/arpnd.py
+-rw-r--r--   0        0        0     7053 2020-12-10 20:07:52.473969 suzieq-0.8.0/suzieq/sqobjects/basicobj.py
+-rw-r--r--   0        0        0     1271 2020-12-13 23:30:08.321185 suzieq-0.8.0/suzieq/sqobjects/bgp.py
+-rw-r--r--   0        0        0      936 2020-12-10 20:07:52.473969 suzieq-0.8.0/suzieq/sqobjects/device.py
+-rw-r--r--   0        0        0      860 2020-12-13 23:30:21.545165 suzieq-0.8.0/suzieq/sqobjects/evpnVni.py
+-rw-r--r--   0        0        0      295 2020-12-10 20:07:52.473969 suzieq-0.8.0/suzieq/sqobjects/fs.py
+-rw-r--r--   0        0        0     1345 2020-12-13 23:30:34.449145 suzieq-0.8.0/suzieq/sqobjects/interfaces.py
+-rw-r--r--   0        0        0      280 2020-12-10 20:07:52.473969 suzieq-0.8.0/suzieq/sqobjects/lldp.py
+-rw-r--r--   0        0        0     1067 2020-12-10 20:07:52.473969 suzieq-0.8.0/suzieq/sqobjects/macs.py
+-rw-r--r--   0        0        0      270 2020-12-10 20:07:52.473969 suzieq-0.8.0/suzieq/sqobjects/mlag.py
+-rw-r--r--   0        0        0     2246 2020-12-14 04:51:26.607815 suzieq-0.8.0/suzieq/sqobjects/ospf.py
+-rw-r--r--   0        0        0      511 2020-11-14 06:49:48.311492 suzieq-0.8.0/suzieq/sqobjects/path.py
+-rw-r--r--   0        0        0     1456 2020-12-14 04:23:33.332549 suzieq-0.8.0/suzieq/sqobjects/routes.py
+-rw-r--r--   0        0        0      389 2020-12-10 20:07:52.473969 suzieq-0.8.0/suzieq/sqobjects/sqPoller.py
+-rw-r--r--   0        0        0     3197 2020-11-01 07:19:39.839485 suzieq-0.8.0/suzieq/sqobjects/tables.py
+-rw-r--r--   0        0        0      274 2020-12-10 20:07:52.473969 suzieq-0.8.0/suzieq/sqobjects/topcpu.py
+-rw-r--r--   0        0        0      274 2020-12-10 20:07:52.473969 suzieq-0.8.0/suzieq/sqobjects/topmem.py
+-rw-r--r--   0        0        0     1477 2020-12-13 23:46:46.525112 suzieq-0.8.0/suzieq/sqobjects/topology.py
+-rw-r--r--   0        0        0      369 2020-12-10 20:07:52.473969 suzieq-0.8.0/suzieq/sqobjects/vlan.py
+-rw-r--r--   0        0        0     2657 2020-09-21 06:57:19.689637 suzieq-0.8.0/suzieq/utilities/convert_legacy_dataset.py
+-rw-r--r--   0        0        0     1233 2020-09-09 17:28:30.111325 suzieq-0.8.0/suzieq/utilities/find_invalid_parquet.py
+-rw-r--r--   0        0        0     3578 2020-09-14 13:07:21.435893 suzieq-0.8.0/suzieq/utilities/migrate_data.py
+-rw-r--r--   0        0        0    15594 2020-09-09 17:51:03.239258 suzieq-0.8.0/suzieq/utilities/sq-anonymize.py
+-rw-r--r--   0        0        0    17697 2020-12-13 12:22:21.300176 suzieq-0.8.0/suzieq/utils.py
+-rw-r--r--   0        0        0     1320 2020-12-15 21:03:17.539719 suzieq-0.8.0/setup.py
+-rw-r--r--   0        0        0     1019 2020-12-15 21:03:17.539997 suzieq-0.8.0/PKG-INFO
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sq_nubia_plugin.py` & `suzieq-0.8.0/suzieq/cli/sq_nubia_plugin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import argparse
-from nubia import PluginInterface
-from nubia.internal.blackcmd import CommandBlacklist
-
+from suzieq.cli.sqcmds import *
+from suzieq.cli.sqcmds import context_commands
+from suzieq.cli.sqcmds import sqcmds_all
 from suzieq.cli.sq_nubia_context import NubiaSuzieqContext
 from suzieq.cli.sq_nubia_statusbar import NubiaSuzieqStatusBar
-from suzieq.cli.sqcmds.context_commands import SqHelpCommand
+from nubia import PluginInterface, CompletionDataSource
+from nubia.internal.blackcmd import CommandBlacklist
+from nubia.internal.cmdbase import AutoCommand
 
 
 class NubiaSuzieqPlugin(PluginInterface):
     """
-    The PluginInterface class is a way to customize nubia for Suzieq
-    use case. Mainly used to build the list of commands
+    The PluginInterface class is a way to customize nubia for every customer
+    use case. It allowes custom argument validation, control over command
+    loading, custom context objects, and much more.
     """
 
     def create_context(self):
         """
         Must create an object that inherits from `Context` parent class.
         The plugin can return a custom context but it has to inherit from the
         correct parent class.
@@ -25,18 +28,22 @@
         """
         This will be executed when starting nubia, the args passed is a
         dict-like object that contains the argparse result after parsing the
         command line arguments. The plugin can choose to update the context
         with the values, and/or decide to raise `ArgsValidationError` with
         the error message.
         """
+        pass
 
     def get_commands(self):
-
-        return [SqHelpCommand()]
+        cmds = [AutoCommand(getattr(globals()[x], x))
+                for x in sqcmds_all if not x.startswith('_')]
+        cmds.append(AutoCommand(context_commands.set_ctxt))
+        cmds.append(AutoCommand(context_commands.clear_ctxt))
+        return cmds
 
     def get_opts_parser(self, add_help=True):
         """
         Builds the ArgumentParser that will be passed to , use this to
         build your list of arguments that you want for your shell.
         """
         opts_parser = argparse.ArgumentParser(
@@ -44,17 +51,14 @@
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             add_help=add_help,
         )
         opts_parser.add_argument(
             "--config", "-c", default="", type=str, help="Configuration File"
         )
         opts_parser.add_argument(
-            "-V", type=str, default='', help='print suzieq version'
-        )
-        opts_parser.add_argument(
             "--verbose",
             "-v",
             action="count",
             default=0,
             help="Increase verbosity, can be specified " "multiple times",
         )
         opts_parser.add_argument(
@@ -63,20 +67,23 @@
             action="store_true",
             default=True,
             help="By default the logging output goes to stderr "
             "Enable this feature to send it to a temporary logfile"
         )
         # we only support pandas now, so we don't want this option
         # opts_parser.add_argument(
-        #    "--use-engine", "-e", help="Which analysis engine to use",
-        #     default="pandas"
+        #    "--use-engine", "-e", help="Which analysis engine to use", default="pandas"
         # )
         return opts_parser
 
-    def get_completion_datasource_for_global_argument(self, _):
+    def get_completion_datasource_for_global_argument(self, argument):
+        if argument == "--config":
+            return ConfigFileCompletionDataSource()
+        if argument == "--use-engine":
+            return ConfigEngineCompletionDataSource()
         return None
 
     def create_usage_logger(self, context):
         """
         Override this and return you own usage logger.
         Must be a subtype of UsageLoggerInterface.
         """
@@ -90,7 +97,17 @@
         return NubiaSuzieqStatusBar(context)
 
     def getBlacklistPlugin(self):
         blacklister = CommandBlacklist()
         blacklister.add_blocked_command("topcpu")
         blacklister.add_blocked_command("topmem")
         return blacklister
+
+
+class ConfigFileCompletionDataSource(CompletionDataSource):
+    def get_all(self):
+        return ["/tmp/c1", "/tmp/c2"]
+
+
+class ConfigEngineCompletionDataSource(CompletionDataSource):
+    def get_all(self):
+        return ["pandas"]
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/ArpndCmd.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/ArpndCmd.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,60 @@
-from nubia import command
-from suzieq.cli.nubia_patch import argument
+import time
+from nubia import command, argument
 
-from suzieq.cli.sqcmds.command import SqTableCommand
+from suzieq.cli.sqcmds.command import SqCommand
 from suzieq.sqobjects.arpnd import ArpndObj
 
 
 @command("arpnd", help="Act on ARP/ND data")
-@argument("prefix",
-          description=("Show all the addresses in this "
-                       "subnet prefix (in quotes)"))
-@argument("address",
-          description="IP Address(es), in quotes, space separated")
-@argument("macaddr",
-          description="MAC address(es), in quotes, space separated")
-@argument("oif", description="Outgoing interface(s), space separated")
-class ArpndCmd(SqTableCommand):
-    """ARP/Neighbor Discovery information"""
-
+class ArpndCmd(SqCommand):
     def __init__(
-            self,
-            engine: str = "",
-            hostname: str = "",
-            start_time: str = "",
-            end_time: str = "",
-            view: str = "",
-            namespace: str = "",
-            format: str = "",  # pylint: disable=redefined-builtin
-            columns: str = "default",
-            query_str: str = ' ',
-            prefix: str = '',
-            address: str = '',
-            macaddr: str = '',
-            oif: str = '',
+        self,
+        engine: str = "",
+        hostname: str = "",
+        start_time: str = "",
+        end_time: str = "",
+        view: str = "latest",
+        namespace: str = "",
+        format: str = "",
+        columns: str = "default",
     ) -> None:
         super().__init__(
             engine=engine,
             hostname=hostname,
             start_time=start_time,
             end_time=end_time,
             view=view,
             namespace=namespace,
             columns=columns,
             format=format,
-            query_str=query_str,
             sqobj=ArpndObj,
         )
-        self.lvars = {
-            'prefix': prefix.split(),
-            'ipAddress': address.split(),
-            'macaddr': macaddr.split(),
-            'oif': oif.split(),
-        }
+
+    @command("show")
+    @argument("address", description="IP address, in quotes, to qualify output")
+    @argument("macaddr", description="MAC address, in quotes, to qualify output")
+    @argument("oif", description="outgoing interface to qualify")
+    def show(self, address: str = "", macaddr: str = '', oif: str = ''):
+        """
+        Show ARP/ND info
+        """
+        if self.columns is None:
+            return
+
+        # Get the default display field names
+        now = time.time()
+        if self.columns != ["default"]:
+            self.ctxt.sort_fields = None
+        else:
+            self.ctxt.sort_fields = []
+
+        df = self.sqobj.get(
+            hostname=self.hostname,
+            ipAddress=address.split(),
+            oif=oif.split(),
+            columns=self.columns,
+            namespace=self.namespace,
+            macaddr=macaddr.split()
+        )
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        return self._gen_output(df)
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/BgpCmd.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/DeviceCmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,103 @@
 import time
-from datetime import timedelta
-from nubia import command
-
+from nubia import command, argument
 import pandas as pd
 
-from suzieq.cli.nubia_patch import argument
-from suzieq.cli.sqcmds.command import SqTableCommand
-from suzieq.sqobjects.bgp import BgpObj
+from suzieq.cli.sqcmds.command import SqCommand
+from suzieq.sqobjects.device import DeviceObj
 
 
-@command("bgp", help="Act on BGP data")
-@argument("vrf", description="VRF(s), space separated")
-@argument("state", description="status of the session to match",
-          choices=["Established", "NotEstd", "dynamic"])
-@argument("peer",
-          description=("IP address(es), in quotes, or the interface name(s), "
-                       "space separated"))
-@argument("afiSafi", description="AFI SAFI string to filter by")
-class BgpCmd(SqTableCommand):
-    """BGP protocol information"""
+@command("device", help="Act on device data")
+class DeviceCmd(SqCommand):
+    """device command"""
 
     def __init__(
             self,
             engine: str = "",
             hostname: str = "",
             start_time: str = "",
             end_time: str = "",
-            view: str = "",
+            view: str = "latest",
             namespace: str = "",
-            format: str = "",  # pylint: disable=redefined-builtin
+            format: str = "",
             columns: str = "default",
-            query_str: str = ' ',
-            vrf: str = '',
-            state: str = '',
-            peer: str = '',
-            afiSafi: str = '',
     ) -> None:
         super().__init__(
             engine=engine,
             hostname=hostname,
             start_time=start_time,
             end_time=end_time,
             view=view,
             namespace=namespace,
             columns=columns,
             format=format,
-            query_str=query_str,
-            sqobj=BgpObj,
+            sqobj=DeviceObj,
+        )
+
+    def _get(self):
+        # Get the default display field names
+        if self.columns != ["default"]:
+            self.ctxt.sort_fields = None
+        else:
+            self.ctxt.sort_fields = []
+
+        df = self.sqobj.get(
+            hostname=self.hostname, columns=self.columns,
+            namespace=self.namespace,
         )
-        self.lvars = {
-            'vrf': vrf.split(),
-            'state': state,
-            'peer': peer.split(),
-            'afiSafi': afiSafi,
-        }
-
-    def _clean_output(self, df) -> pd.DataFrame:
-        """Make upTime look good"""
-        if df.empty:
-            return df
-
-        if "estdTime" in df.columns:
-            df['estdTime'] = df.estdTime.apply(
-                lambda x: str(timedelta(milliseconds=int(x))))
-        elif 'upTimeStat' in df.columns:
-            df.loc['upTimeStat'] = df \
-              .loc['upTimeStat'] \
-              .map(lambda x: [str(timedelta(milliseconds=int(i))) for i in x])
-
-        return df.dropna(how='any')
-
-    @command("assert")
-    @argument("result", description="Show only assert that matches this value",
-              choices=["all", "fail", "pass"])
-    def aver(self, result: str = "all") -> pd.DataFrame:
-        """Assert BGP is functioning properly"""
+
+        df = self.sqobj.humanize_fields(df)
+
+        return df
+
+    @command("show", help="Show device information")
+    def show(self):
+        """
+        Show device info
+        """
+        if self.columns is None:
+            return
 
         now = time.time()
+        df = self._get()
+
+        if 'uptime' in df.columns:
+            df.drop(columns=['uptime'], inplace=True)
 
-        df = self._invoke_sqobj(self.sqobj.aver,
-                                namespace=self.namespace,
-                                hostname=self.hostname,
-                                columns=self._add_result_columns(self.columns),
-                                result=result,
-                                **self.lvars,
-                                )
         self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
 
-        return self._assert_gen_output(df)
+        return self._gen_output(df)
+
+    @command("top")
+    @argument("what", description="Field you want to see top for",
+              choices=["uptime"])
+    @argument("count", description="How many top entries")
+    @argument("reverse", description="True see Bottom n",
+              choices=["True", "False"])
+    def top(self, what: str = "flaps", count: int = 5, reverse: str = "False"):
+        """
+        Show top n entries based on specific field
+        """
+
+        # Device uptime is a field whose value is derived and calculated at
+        # this level. So call get and then perform top on the data obtained
+
+        now = time.time()
+        if (self.columns != ['default'] and self.columns != ['*']
+                and 'uptime' not in self.columns):
+            self.columns.append('bootupTimestamp')
+        df = self._get()
+        if 'bootupTimestamp' in self.columns:
+            self.columns.remove('bootupTimestamp')
+
+        if not df.empty:
+            if reverse == "True":
+                topdf = df.nsmallest(count, columns='uptime', keep="all") \
+                          .head(count)
+            else:
+                topdf = df.nlargest(count, columns='uptime', keep="all") \
+                          .head(count)
+        else:
+            topdf = df
+
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        self._gen_output(topdf, sort=False)
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/DevconfigCmd.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/AddressCmd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,59 @@
-from nubia import command
+import time
 
-from suzieq.cli.sqcmds.command import SqTableCommand
-from suzieq.sqobjects.devconfig import DevconfigObj
+from nubia import command, argument
 
+from suzieq.cli.sqcmds.command import SqCommand
+from suzieq.sqobjects.address import AddressObj
 
-@command("devconfig", help="Act on device data")
-class DevconfigCmd(SqTableCommand):
-    """Device configurations"""
 
+@command("address", help="Act on address data")
+class AddressCmd(SqCommand):
     def __init__(
-            self,
-            engine: str = "",
-            hostname: str = "",
-            start_time: str = "",
-            end_time: str = "",
-            view: str = "",
-            namespace: str = "",
-            format: str = "",  # pylint: disable=redefined-builtin
-            query_str: str = " ",
-            columns: str = "default",
+        self,
+        engine: str = "",
+        hostname: str = "",
+        start_time: str = "",
+        end_time: str = "",
+        view: str = "latest",
+        namespace: str = "",
+        format: str = "",
+        columns: str = "default",
     ) -> None:
         super().__init__(
             engine=engine,
             hostname=hostname,
             start_time=start_time,
             end_time=end_time,
             view=view,
             namespace=namespace,
-            columns=columns,
             format=format,
-            query_str=query_str,
-            sqobj=DevconfigObj,
+            columns=columns,
+            sqobj=AddressObj,
         )
 
-    @command("show", help="Show device information")
-    def show(self):
-        """Show device config info
+    @command("show")
+    @argument("address", description="Address, in quotes, to show info for")
+    @argument("vrf", description="VRF to qualify the address")
+    @argument("ipvers", description="type of address, v4, v6 or l2",
+              choices=["v4", "v6", "l2"])
+    def show(self, address: str = "", ipvers: str = "", vrf: str = ""):
+        """
+        Show address info
         """
-        if not self.format or (self.format == 'text'):
-            self.format = 'devconfig'
-        return super().show()
+        # Get the default display field names
+        now = time.time()
+        if self.columns != ["default"]:
+            self.ctxt.sort_fields = None
+        else:
+            self.ctxt.sort_fields = []
+
+        df = self.sqobj.get(
+            hostname=self.hostname,
+            columns=self.columns,
+            address=address.split(),
+            ipvers=ipvers,
+            vrf=vrf,
+            namespace=self.namespace,
+        )
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        return self._gen_output(df)
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/DeviceCmd.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/MacCmd.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,83 @@
-import shlex
-from nubia import command
-from suzieq.cli.nubia_patch import argument
-
-from suzieq.cli.sqcmds.command import SqTableCommand
-from suzieq.sqobjects.device import DeviceObj
-
-
-@command("device", help="Act on device data")
-@argument("status", description="filter by polling status",)
-@argument("os", description="NOS(s), space separated")
-@argument("version", description="NOS version(s), space separated")
-@argument("vendor", description="Vendor(s), space separated")
-@argument("model", description="Model(s), space separated")
-class DeviceCmd(SqTableCommand):
-    """Basic device information such as OS, version, model etc."""
+import time
+import pandas as pd
+from nubia import command, argument
 
+from suzieq.cli.sqcmds.command import SqCommand
+from suzieq.sqobjects.macs import MacsObj
+
+
+@command("mac", help="Act on MAC Table data")
+class MacCmd(SqCommand):
     def __init__(
-            self,
-            engine: str = "",
-            hostname: str = "",
-            start_time: str = "",
-            end_time: str = "",
-            view: str = "",
-            namespace: str = "",
-            format: str = "",  # pylint: disable=redefined-builtin
-            query_str: str = " ",
-            columns: str = "default",
-            os: str = '',
-            version: str = '',
-            status: str = '',
-            vendor: str = '',
-            model: str = '',
+        self,
+        engine: str = "",
+        hostname: str = "",
+        start_time: str = "",
+        end_time: str = "",
+        view: str = "latest",
+        namespace: str = "",
+        format: str = "",
+        columns: str = "default",
     ) -> None:
         super().__init__(
             engine=engine,
             hostname=hostname,
             start_time=start_time,
             end_time=end_time,
             view=view,
             namespace=namespace,
             columns=columns,
             format=format,
-            query_str=query_str,
-            sqobj=DeviceObj,
+            sqobj=MacsObj,
         )
 
-        # Nubia eats up the first and last quote. Detect and add back
-        model = model.strip()
-        if model.count("'") % 2 != 0:
-            if not model.startswith("'"):
-                model = f"'{model}"
-            elif not model.endswith("'"):
-                model = f"{model}'"
-        if model:
-            model = shlex.split(model)
-
-        self.lvars = {
-            'os': os.split(),
-            'version': version.split(),
-            'status': status.split(),
-            'model': model,
-            'vendor': vendor.split()
-        }
+    @command("show")
+    @argument("vlan", description="VLAN(s) to qualify output")
+    @argument("macaddr",
+              description="MAC address(es), in quotes, to qualify output")
+    @argument("remoteVtepIp", description="only with this remoteVtepIp; use any for all")
+    @argument("bd", description="filter entries with this bridging domain")
+    @argument("local", description="filter entries with no remoteVtep")
+    def show(self, vlan: str = '', macaddr: str = '', remoteVtepIp: str = '',
+             bd: str = '', local: bool = False):
+        """Show MAC table info
+
+        The remoteVtepInfo is set to "-" to allow to fetch local entries only
+        """
+        if self.columns is None:
+            return
+
+        # Get the default display field names
+        now = time.time()
+        if self.columns != ["default"]:
+            self.ctxt.sort_fields = None
+        else:
+            self.ctxt.sort_fields = []
+
+        drop_cols = []
+
+        if vlan and (self.columns != ['default'] and self.columns != ['*'] and
+                     'vlan' not in self.columns):
+            addnl_fields = ['vlan']
+            drop_cols.append('vlan')
+        else:
+            addnl_fields = []
+
+        df = self.sqobj.get(
+            hostname=self.hostname,
+            macaddr=macaddr.split(),
+            addnl_fields=addnl_fields,
+            remoteVtepIp=remoteVtepIp.split(),
+            vlan=vlan.split(),
+            localOnly=local,
+            bd=bd,
+            columns=self.columns,
+            namespace=self.namespace,
+        )
+        if not df.empty and "mackey" in df.columns:
+            drop_cols.append('mackey')
+
+        df.drop(columns=drop_cols, inplace=True)
+
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        return self._gen_output(df)
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/EvpnVniCmd.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/TableCmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,79 @@
 import time
-from nubia import command
-from suzieq.cli.nubia_patch import argument
 
-from suzieq.cli.sqcmds.command import SqTableCommand
-from suzieq.sqobjects.evpnVni import EvpnvniObj
+from nubia import command, argument
+import pandas as pd
 
+from suzieq.cli.sqcmds.command import SqCommand
+from suzieq.sqobjects.tables import TablesObj
 
-@command("evpnVni", help="Act on EVPN VNI data")
-@argument("vni", description="VNI ID(s), space separated")
-@argument("priVtepIp", description="Primary VTEP IP(s), space separated")
-class EvpnVniCmd(SqTableCommand):
-    """EVPN information such as VNI/VLAN mapping, VTEP IPs etc."""
 
+@command("table", help="Information about the various tables")
+class TableCmd(SqCommand):
     def __init__(
-            self,
-            engine: str = "",
-            hostname: str = "",
-            start_time: str = "",
-            end_time: str = "",
-            view: str = "",
-            namespace: str = "",
-            format: str = "",  # pylint: disable=redefined-builtin
-            query_str: str = " ",
-            columns: str = "default",
-            vni: str = '',
-            priVtepIp: str = '',
+        self,
+        engine: str = "",
+        hostname: str = "",
+        start_time: str = "",
+        end_time: str = "",
+        view: str = "latest",
+        namespace: str = "",
+        format: str = "",
+        columns: str = "default",
     ) -> None:
         super().__init__(
             engine=engine,
             hostname=hostname,
             start_time=start_time,
             end_time=end_time,
             view=view,
             namespace=namespace,
             columns=columns,
             format=format,
-            query_str=query_str,
-            sqobj=EvpnvniObj,
+            sqobj=TablesObj,
         )
-        self.lvars = {
-            'vni': vni,
-            'priVtepIp': priVtepIp.split()
-        }
-
-    @command("assert")
-    @argument("result", description="Show only assert that matches this value",
-              choices=["all", "fail", "pass"])
-    def aver(self, result: str = 'all'):
-        """Assert VXLAN Forwarding is functioning properly"""
 
+    @command("show")
+    def show(self, **kwargs):
+        """
+        Show Tables
+        """
         now = time.time()
+        df = self.sqobj.get(hostname=self.hostname, namespace=self.namespace)
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        return self._gen_output(df)
+
+    @command("describe")
+    @argument("table", description="interface name to qualify")
+    def describe(self, table: str = "", **kwargs):
+        """
+        Describe fields in table
+        """
+
+        if not table:
+            df = pd.DataFrame({'error': ['ERROR: Must specify a table']})
+            return self._gen_output(df)
+
+        if self.columns != ['default']:
+            df = pd.DataFrame(
+                {'error': ['ERROR: Cannot specify columns for command']})
+            return self._gen_output(df)
 
-        df = self._invoke_sqobj(self.sqobj.aver,
-                                hostname=self.hostname,
-                                namespace=self.namespace,
-                                columns=self._add_result_columns(self.columns),
-                                result=result,
-                                **self.lvars,
-                                )
+        now = time.time()
+        df = self.sqobj.describe(table=table)
         self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
 
-        return self._assert_gen_output(df)
+        return self._gen_output(df, dont_strip_cols=True)
+
+    @command("summarize", help="Summarize info about this resource")
+    def summarize(self, **kwargs):
+
+        msg = 'ERROR: Summarize not supported for this object'
+        df = pd.DataFrame({'error': [msg]})
+        return self._gen_output(df, dont_strip_cols=True)
+
+    @command("unique", help="find the list of unique items in a column")
+    def unique(self, **kwargs):
+
+        msg = 'ERROR: Unique not supported for this object'
+        df = pd.DataFrame({'error': [msg]})
+        return self._gen_output(df, dont_strip_cols=True)
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/FsCmd.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/SqPollerCmd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,60 @@
-from nubia import command
-import pandas as pd
+import time
+from nubia import command, argument
 
-from suzieq.cli.nubia_patch import argument
-from suzieq.cli.sqcmds.command import SqTableCommand
-from suzieq.sqobjects.fs import FsObj
+from suzieq.cli.sqcmds.command import SqCommand
+from suzieq.sqobjects.sqPoller import SqPollerObj
 
 
-@command("fs", help="Act on File System data")
-@argument("used_percent", description="must be of the form "
-          "[<|<=|>=|>|!]value. Eg: '<=20'")
-@argument("mountPoint", description="Mount point(s), space separated")
-class FsCmd(SqTableCommand):
-    """Filesystem information such as total disk space, filesystems etc"""
-
+@command("sqpoller", help="Act on SqPoller data")
+class SqPollerCmd(SqCommand):
     def __init__(
-            self,
-            engine: str = "",
-            hostname: str = "",
-            start_time: str = "",
-            end_time: str = "",
-            view: str = "",
-            namespace: str = "",
-            format: str = "",  # pylint: disable=redefined-builtin
-            query_str: str = " ",
-            columns: str = "default",
-            used_percent: str = '',
-            mountPoint: str = ''
+        self,
+        engine: str = "",
+        hostname: str = "",
+        start_time: str = "",
+        end_time: str = "",
+        view: str = "latest",
+        namespace: str = "",
+        format: str = "",
+        columns: str = "default",
     ) -> None:
         super().__init__(
             engine=engine,
             hostname=hostname,
             start_time=start_time,
             end_time=end_time,
             view=view,
             namespace=namespace,
             columns=columns,
             format=format,
-            query_str=query_str,
-            sqobj=FsObj,
+            sqobj=SqPollerObj,
         )
-        self.lvars = {
-            'usedPercent': used_percent,
-            'mountPoint': mountPoint.split()
-        }
 
     @command("show")
-    def show(self):
-        """Show File System info
+    @argument("service", description="name of service to match")
+    @argument("status", description="status of service to match",
+              choices=["all", "pass", "fail"])
+    def show(self, service: str = "", status: str = "all"):
         """
-        # Get the default display field names
-        used_percent = self.lvars.get('usedPercent')
-        if used_percent and not any(used_percent.startswith(x)
-                                    for x in ['<=', '>=', '<', '>', '!']):
-            try:
-                int(used_percent)
-            except ValueError:
-                df = pd.DataFrame(
-                    {'error': ['ERROR invalid used-percent operation']})
-                return self._gen_output(df)
+        Show SqPoller info
+        """
+        if self.columns is None:
+            return
 
-        return super().show()
+        # Get the default display field names
+        now = time.time()
+        if self.columns != ["default"]:
+            self.ctxt.sort_fields = None
+        else:
+            self.ctxt.sort_fields = []
+
+        df = self.sqobj.get(
+            hostname=self.hostname,
+            columns=self.columns,
+            service=service,
+            status=status,
+            namespace=self.namespace,
+        )
 
-    @command("summarize")
-    def summarize(self, **kwargs):
-        """
-        Summarize the filesystem/storage info
-        """
-        df = pd.DataFrame({'error': ['Summarize not yet supported for FS']})
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
         return self._gen_output(df)
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/LldpCmd.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/TopmemCmd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,54 @@
-from nubia import command
-from suzieq.cli.nubia_patch import argument
+import time
+from nubia import command, argument
 
-from suzieq.cli.sqcmds.command import SqTableCommand
-from suzieq.sqobjects.lldp import LldpObj
+from suzieq.cli.sqcmds.command import SqCommand
+from suzieq.sqobjects.topmem import TopmemObj
 
 
-@command("lldp", help="Act on LLDP data")
-@argument("ifname", description="Interface name(s), space separated")
-@argument("peerHostname", description="Peer hostname(s), space separated")
-@argument("peerMacaddr", description="Peer mac address(es), space separated")
-class LldpCmd(SqTableCommand):
-    """LLDP protocol information"""
-
+@command("topmem", help="Act on topmem data")
+class TopmemCmd(SqCommand):
     def __init__(
-            self,
-            engine: str = "",
-            hostname: str = "",
-            start_time: str = "",
-            end_time: str = "",
-            view: str = "",
-            namespace: str = "",
-            format: str = "",  # pylint: disable=redefined-builtin
-            query_str: str = ' ',
-            columns: str = "default",
-            ifname: str = '',
-            peerHostname: str = '',
-            peerMacaddr: str = ''
+        self,
+        engine: str = "",
+        hostname: str = "",
+        start_time: str = "",
+        end_time: str = "",
+        view: str = "latest",
+        namespace: str = "",
+        format: str = "",
+        columns: str = "default",
     ) -> None:
         super().__init__(
             engine=engine,
             hostname=hostname,
             start_time=start_time,
             end_time=end_time,
             view=view,
             namespace=namespace,
             columns=columns,
             format=format,
-            query_str=query_str,
-            sqobj=LldpObj,
+            sqobj=TopmemObj,
+        )
+
+    @command("show")
+    def show(self):
+        """
+        Show topmem info
+        """
+        if self.columns is None:
+            return
+
+        # Get the default display field names
+        now = time.time()
+        if self.columns != ["default"]:
+            self.ctxt.sort_fields = None
+        else:
+            self.ctxt.sort_fields = []
+
+        df = self.sqobj.get(
+            hostname=self.hostname, columns=self.columns,
+            namespace=self.namespace
         )
-        self.lvars = {
-            'peerHostname': peerHostname.split(),
-            'ifname': ifname.split(),
-            'peerMacaddr': peerMacaddr.split(),
-        }
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        return self._gen_output(df)
+
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/NamespaceCmd.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/EvpnVniCmd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,71 @@
 import time
-from nubia import command
-from suzieq.cli.nubia_patch import argument
+from nubia import command, argument
 
-from suzieq.cli.sqcmds.command import SqTableCommand
-from suzieq.sqobjects.namespace import NamespaceObj
+from suzieq.cli.sqcmds.command import SqCommand
+from suzieq.sqobjects.evpnVni import EvpnvniObj
 
 
-@command("namespace", help="Summarize namespace-wide network data")
-class NamespaceCmd(SqTableCommand):
-    """Overall network information such as device count, bgp enabled etc."""
-
+@command("evpnVni", help="Act on EVPN VNI data")
+class EvpnVniCmd(SqCommand):
     def __init__(
-            self,
-            engine: str = "",
-            hostname: str = "",
-            start_time: str = "",
-            end_time: str = "",
-            view: str = "",
-            namespace: str = "",
-            format: str = "",  # pylint: disable=redefined-builtin
-            query_str: str = " ",
-            columns: str = "default",
+        self,
+        engine: str = "",
+        hostname: str = "",
+        start_time: str = "",
+        end_time: str = "",
+        view: str = "latest",
+        namespace: str = "",
+        format: str = "",
+        columns: str = "default",
     ) -> None:
         super().__init__(
             engine=engine,
             hostname=hostname,
             start_time=start_time,
             end_time=end_time,
             view=view,
             namespace=namespace,
             columns=columns,
             format=format,
-            query_str=query_str,
-            sqobj=NamespaceObj,
+            sqobj=EvpnvniObj,
         )
 
-    @command("show", help="Show namespace information")
-    @argument("model", description="Device model(s), space separated")
-    @argument("os", description='Device NOS(es), space separated')
-    @argument('vendor', description='Device vendor(s), space separated')
-    @argument('version', description='Device NOS version(s), space separated')
-    def show(self, os: str = "", vendor: str = "", model: str = "",
-             version: str = "") -> int:
-        """Show namespace info
+    @command("show")
+    @argument("vni", description="VNI ID to qualify")
+    def show(self, vni: str = ""):
+        """
+        Show EVPN VNI info
         """
+        if self.columns is None:
+            return
 
+        # Get the default display field names
         now = time.time()
+        if self.columns != ["default"]:
+            self.ctxt.sort_fields = None
+        else:
+            self.ctxt.sort_fields = []
+
+        df = self.sqobj.get(
+            hostname=self.hostname,
+            vni=vni.split(),
+            columns=self.columns,
+            namespace=self.namespace,
+        )
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        return self._gen_output(df)
 
-        df = self._invoke_sqobj(self.sqobj.get,
-                                namespace=self.namespace, os=os.split(),
-                                vendor=vendor.split(), model=model.split(),
-                                version=version, query_str=self.query_str,
-                                hostname=self.hostname)
-
+    @command("assert")
+    @argument("status", description="Show only assert that matches this value",
+              choices=["all", "fail", "pass"])
+    def aver(self, status: str = 'pass'):
+        """Assert BGP is functioning properly"""
+        now = time.time()
+        df = self.sqobj.aver(
+            hostname=self.hostname,
+            namespace=self.namespace,
+            status=status,
+        )
         self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
 
-        return self._gen_output(df)
+        return self._assert_gen_output(df)
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/OspfCmd.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/FsCmd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 import time
-
-from nubia import command
+from nubia import command, argument
 import pandas as pd
 
-from suzieq.cli.nubia_patch import argument
-from suzieq.cli.sqcmds.command import SqTableCommand
-from suzieq.sqobjects.ospf import OspfObj
-
-
-@command("ospf", help="Act on OSPF data")
-@argument(
-    "ifname",
-    description="Interface name(s), space separated"
-)
-@argument("vrf", description="VRF(s), space separated")
-@argument("area", description="Area(s), space separated")
-@argument("state", description="Select view based on OSPF state",
-          choices=["full", "other", "passive", "!full", "!passive",
-                   "!other"])
-class OspfCmd(SqTableCommand):
-    """OSPFv2 protocol information"""
+from suzieq.cli.sqcmds.command import SqCommand
+from suzieq.sqobjects.fs import FsObj
+
 
+@command("fs", help="Act on File System data")
+class FsCmd(SqCommand):
     def __init__(
-            self,
-            engine: str = "",
-            hostname: str = "",
-            start_time: str = "",
-            end_time: str = "",
-            view: str = "",
-            namespace: str = "",
-            format: str = "",  # pylint: disable=redefined-builtin
-            query_str: str = ' ',
-            columns: str = "default",
-            ifname: str = '',
-            vrf: str = '',
-            area: str = '',
-            state: str = ''
+        self,
+        engine: str = "",
+        hostname: str = "",
+        start_time: str = "",
+        end_time: str = "",
+        view: str = "latest",
+        namespace: str = "",
+        format: str = "",
+        columns: str = "default",
     ) -> None:
         super().__init__(
             engine=engine,
             hostname=hostname,
             start_time=start_time,
             end_time=end_time,
             view=view,
             namespace=namespace,
             columns=columns,
             format=format,
-            query_str=query_str,
-            sqobj=OspfObj,
+            sqobj=FsObj,
         )
-        self.lvars = {
-            'ifname': ifname.split(),
-            'vrf': vrf.split(),
-            'area': area.split(),
-            'state': state
-        }
-
-    @command("assert")
-    @argument("result", description="Show only assert that matches this value",
-              choices=["all", "fail", "pass"])
-    def aver(self, result: str = 'all') -> pd.DataFrame:
+
+    @command("show")
+    @argument("mountPoint", description="The mount point inside the FileSystem")
+    @argument("used_percent", description="must be of the form "
+              "[<|<=|>=|>|!]value. Eg: '<=20'")
+    def show(self, mountPoint: str = '', used_percent: str = ''):
         """
-        Test OSPF runtime state is without errors
+        Show File System info
         """
-        now = time.time()
+        if self.columns is None:
+            return
 
-        df = self._invoke_sqobj(self.sqobj.aver,
-                                namespace=self.namespace,
-                                hostname=self.hostname,
-                                columns=self._add_result_columns(self.columns),
-                                result=result,
-                                **self.lvars,
-                                )
+        # Get the default display field names
+        now = time.time()
+        if self.columns != ["default"]:
+            self.ctxt.sort_fields = None
+        else:
+            self.ctxt.sort_fields = []
+
+        if used_percent and not any(used_percent.startswith(x)
+                                    for x in ['<=', '>=', '<', '>', '!']):
+            try:
+                int(used_percent)
+            except ValueError:
+                df = pd.DataFrame(
+                    {'error': ['ERROR invalid used-percent operation']})
+                return self._gen_output(df)
+
+        df = self.sqobj.get(
+            hostname=self.hostname,
+            columns=self.columns,
+            namespace=self.namespace,
+            mountPoint=mountPoint.split(),
+            usedPercent=used_percent,
+        )
         self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        return self._gen_output(df)
 
-        return self._assert_gen_output(df)
+    @command("summarize")
+    def summarize(self):
+        """
+        Summarize the filesystem/storage info
+        """
+        df = pd.DataFrame({'error': ['Summarize not yet supported for FS']})
+        return self._gen_output(df)
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/RouteCmd.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/RouteCmd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,139 @@
 import time
 import ipaddress
+from nubia import command, argument
 import pandas as pd
 
-from nubia import command
-from suzieq.cli.nubia_patch import argument
-
-from suzieq.cli.sqcmds.command import SqTableCommand
+from suzieq.cli.sqcmds.command import SqCommand
 from suzieq.sqobjects.routes import RoutesObj
 
 
 @command("route", help="Act on Routes")
-@argument("vrf", description="VRF(s), space separated")
-@argument("protocol", description="Routing protocol(s), space separated")
-@argument("prefix", description="Prefix(es), in quotes, space separated")
-@argument("prefixlen", description="must be of the form "
-          "[<|<=|>=|>|!] length")
-class RouteCmd(SqTableCommand):
-    """Routing table information"""
-
+class RouteCmd(SqCommand):
     def __init__(
-            self,
-            engine: str = "",
-            hostname: str = "",
-            start_time: str = "",
-            end_time: str = "",
-            view: str = "",
-            namespace: str = "",
-            format: str = "",  # pylint: disable=redefined-builtin
-            query_str: str = ' ',
-            columns: str = "default",
-            vrf: str = "",
-            protocol: str = "",
-            prefix: str = '',
-            prefixlen: str = '',
+        self,
+        engine: str = "",
+        hostname: str = "",
+        start_time: str = "",
+        end_time: str = "",
+        view: str = "latest",
+        namespace: str = "",
+        format: str = "",
+        columns: str = "default",
     ) -> None:
         super().__init__(
             engine=engine,
             hostname=hostname,
             start_time=start_time,
             end_time=end_time,
             view=view,
             namespace=namespace,
             columns=columns,
             format=format,
-            query_str=query_str,
             sqobj=RoutesObj,
         )
-        self.lvars = {
-            'protocol': protocol.split(),
-            'vrf': vrf.split(),
-            'prefix': prefix.split(),
-            'prefixlen': prefixlen
-        }
+        self.json_print_handler = self._json_print_handler
 
-    def _json_print_handler(self, in_data):  # pylint: disable=method-hidden
+    def _json_print_handler(self, input):
         """This handler calls the code to print the IPNetwork as a string"""
-        if isinstance(in_data, ipaddress.IPv4Network):
-            return ipaddress.IPv4Network.__str__(in_data)
-        elif isinstance(in_data, ipaddress.IPv6Network):
-            return ipaddress.IPv6Network.__str__(in_data)
-        return in_data
+        if isinstance(input, ipaddress.IPv4Network):
+            return ipaddress.IPv4Network.__str__(input)
+        elif isinstance(input, ipaddress.IPv6Network):
+            return ipaddress.IPv6Network.__str__(input)
+        return input
 
     def _get_ipvers(self, value: str) -> int:
         """Return the IP version in use"""
 
         if ':' in value:
             ipvers = 6
         elif '.' in value:
             ipvers = 4
         else:
             ipvers = ''
 
         return ipvers
 
+    @command("show")
+    @argument("prefix", description="Prefix, in quotes, to filter show on")
+    @argument("vrf", description="VRF to qualify")
+    @argument("protocol", description="routing protocol to qualify")
+    @argument("prefixlen", description="must be of the form "
+              "[<|<=|>=|>|!] length")
+    def show(self, prefix: str = "", vrf: str = '', protocol: str = "",
+             prefixlen: str = ""):
+        """
+        Show Routes info
+        """
+        if self.columns is None:
+            return
+
+        # Get the default display field names
+        now = time.time()
+
+        if self.columns != ["default"]:
+            self.ctxt.sort_fields = None
+        else:
+            self.ctxt.sort_fields = []
+
+        df = self.sqobj.get(
+            hostname=self.hostname,
+            prefix=prefix.split(),
+            vrf=vrf.split(),
+            protocol=protocol.split(),
+            columns=self.columns,
+            namespace=self.namespace,
+            prefixlen=prefixlen,
+        )
+
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        return self._gen_output(df)
+
+    @command("summarize")
+    @argument("vrf", description="VRF to qualify")
+    def summarize(self, vrf: str = ''):
+        """
+        Show Routes info
+        """
+        # Get the default display field names
+        now = time.time()
+
+        df = self.sqobj.summarize(
+            hostname=self.hostname,
+            vrf=vrf.split(),
+            namespace=self.namespace,
+        )
+
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        return self._gen_output(df, json_orient='columns')
+
     @command('lpm')
     @argument("address", description="IP Address, in quotes, for lpm query")
-    def lpm(self, address: str = ''):
-        """Show the Longest Prefix Match(LPM) on a given prefix, vrf
+    @argument("vrf", description="specific VRF to qualify")
+    def lpm(self, address: str = '', vrf: str = ''):
         """
+        Show the Longest Prefix Match on a given prefix, vrf
+        """
+        if self.columns is None:
+            return
+
         now = time.time()
         if self.columns != ["default"]:
             self.ctxt.sort_fields = None
         else:
             self.ctxt.sort_fields = []
 
         if not address:
-            df = pd.DataFrame({'error': ['Must specify address for lpm']})
-            return self._gen_output(df)
+            print('address is mandatory parameter')
+            return
 
-        df = self._invoke_sqobj(self.sqobj.lpm,
-                                hostname=self.hostname,
-                                address=address,
-                                ipvers=self._get_ipvers(address),
-                                columns=self.columns,
-                                namespace=self.namespace,
-                                query_str=self.query_str,
-                                **self.lvars
-                                )
+        df = self.sqobj.lpm(
+            hostname=self.hostname,
+            address=address,
+            vrf=vrf.split(),
+            ipvers=self._get_ipvers(address),
+            columns=self.columns,
+            namespace=self.namespace,
+        )
 
         self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
         return self._gen_output(df)
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/VlanCmd.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/VlanCmd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,45 @@
-from nubia import command
-from suzieq.cli.nubia_patch import argument
+import time
 
-from suzieq.cli.sqcmds.command import SqTableCommand
+from nubia import command, argument
+
+from suzieq.cli.sqcmds.command import SqCommand
 from suzieq.sqobjects.vlan import VlanObj
 
 
 @command('vlan', help="Act on vlan data")
-@argument("state", description="State of VLAN to query",
-          choices=['active', 'suspended'])
-@argument("vlan",
-          description="VLAN(s), space separated, can use <, >, <=, >=, !")
-@argument('vlanName',
-          description="VLAN name(s), space separated")
-class VlanCmd(SqTableCommand):
-    """Information about VLANs including interfaces belonging to a VLAN"""
-
-    # pylint: disable=redefined-builtin
-    def __init__(
-            self,
-            engine: str = '',
-            hostname: str = '',
-            start_time: str = '',
-            end_time: str = '',
-            view: str = '',
-            namespace: str = '',
-            query_str: str = ' ',
-            format: str = "",
-            columns: str = 'default',
-            vlan: str = '',
-            vlanName: str = '',
-            state: str = '',
-    ) -> None:
+class VlanCmd(SqCommand):
+
+    def __init__(self, engine: str = '', hostname: str = '',
+                 start_time: str = '', end_time: str = '',
+                 view: str = 'latest', namespace: str = '',
+                 format: str = "", columns: str = 'default') -> None:
         super().__init__(engine=engine, hostname=hostname,
                          start_time=start_time, end_time=end_time,
-                         view=view, namespace=namespace, query_str=query_str,
+                         view=view, namespace=namespace,
                          format=format, columns=columns, sqobj=VlanObj)
-        self.lvars = {
-            'vlan': vlan.split(),
-            'vlanName': vlanName.split(),
-            'state': state
-        }
+
+    @command('show')
+    @argument("vlan", description="Space separated list of vlan IDs to show")
+    @argument('vlanName',
+              description="Space separated list of VLAN names to show")
+    @argument("state", description="State of VLAN to query",
+              choices=['active', 'suspended'])
+    def show(self, vlan: str = '', vlanName: str = '', state: str = ''):
+        """
+        Show vlan info
+        """
+        if self.columns is None:
+            return
+
+        # Get the default display field names
+        now = time.time()
+        if self.columns != ['default']:
+            self.ctxt.sort_fields = None
+        else:
+            self.ctxt.sort_fields = []
+
+        df = self.sqobj.get(hostname=self.hostname, vlan=vlan.split(),
+                            state=state, vlanName=vlanName.split(),
+                            columns=self.columns, namespace=self.namespace)
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        return self._gen_output(df)
```

### Comparing `suzieq-0.22.0rc1/suzieq/cli/sqcmds/context_commands.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/command.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,263 +1,250 @@
-import typing
-import os
-from nubia import command, context
-from nubia.internal.commands.help import HelpCommand
-from nubia.internal.cmdbase import Command
-from prompt_toolkit.completion import Completion
-from termcolor import cprint, colored
-
-from suzieq.cli.nubia_patch import argument
-from suzieq.shared.utils import SUPPORTED_ENGINES, print_version
+import time
+import pandas as pd
+from nubia import command, argument, context
+from io import StringIO
+import shutil
+from prompt_toolkit import prompt
 
 
-@command("set")
-@argument("namespace", description="namespace to qualify selection")
-@argument("hostname", description="Name of host to qualify selection")
-@argument(
-    "start_time",
-    description="Start of time window in YYYY-MM-dd HH:mm:SS format"
-)
-@argument("end_time",
-          description="End of time window in YYYY-MM-dd HH:mm:SS format")
-@argument("pager", description="Enable pagination prompt on longer outputs",
-          choices=['on', 'off'])
-@argument('col_width', description='Max Width of each column in table display')
-@argument('max_rows',
-          description='Max rows to display before ellipsis is shown')
-@argument('all_columns',
-          description='Display all columns wrapping around if necessary',
-          choices=['yes', 'no'])
 @argument(
     "engine",
-    choices=SUPPORTED_ENGINES,
-    description="What backend analyzer engine to use",
-)
-@argument(
-    "debug", choices=['True', 'False'], description="Enable debug mode",
+    description="which analytical engine to use",
+    choices=["pandas"],
 )
 @argument(
-    "datadir",
-    description="Set the data directory for the command"
+    "namespace", description="Space separated list of namespaces to qualify"
 )
+@argument("hostname", description="Space separated list of hostnames to qualify")
 @argument(
-    'rest_server_ip', description='IP address of the REST server'
+    "start_time", description="Start of time window, try natural language spec"
 )
 @argument(
-    'rest_server_port', description='Port of the REST server'
+    "end_time", description="End of time window, try natural language spec "
 )
 @argument(
-    'rest_api_key', description='API key for the REST server'
+    "view",
+    description="view all records or just the latest",
+    choices=["all", "latest"],
 )
+@argument("columns", description="Space separated list of columns, * for all")
 @argument(
-    'rest_use_https', description='Use HTTPS for the REST server',
-    choices=['True', 'False']
+    "format",
+    description="select the pformat of the output",
+    choices=["text", "json", "csv", "markdown"],
 )
-def set_ctxt(
-        pager: str = "",
-        hostname: typing.List[str] = None,
-        start_time: str = "",
-        end_time: str = "",
-        namespace: typing.List[str] = None,
-        engine: str = "",
-        datadir: str = "",
-        debug: str = '',
-        col_width: int = 50,
-        max_rows: int = None,
-        all_columns: str = None,
-        rest_server_ip: str = "",
-        rest_server_port: str = "",
-        rest_api_key: str = "",
-        rest_use_https: str = ""
-):
-    """set certain contexts for subsequent commands. Cmd is additive"""
-    plugin_ctx = context.get_context()
-    ctxt = plugin_ctx.ctxt
-
-    if namespace:
-        ctxt.namespace = namespace
-
-    if hostname:
-        ctxt.hostname = hostname
-
-    if start_time:
-        ctxt.start_time = start_time
-
-    if end_time:
-        ctxt.end_time = end_time
-
-    if engine:
-        plugin_ctx.change_engine(engine)
-
-    if debug:
-        ctxt.debug = debug == 'True'
-
-    if datadir:
-        if os.path.isdir(datadir):
-            ctxt.cfg['data-directory'] = datadir
-        else:
-            print(f'{datadir} is not a valid directory')
+class SqCommand:
+    """Base Command Class for use with all verbs"""
 
-    if col_width:
-        ctxt.col_width = int(col_width)
+    def __init__(
+            self,
+            engine: str = "",
+            hostname: str = "",
+            start_time: str = "",
+            end_time: str = "",
+            view: str = "latest",
+            namespace: str = "",
+            format: str = "",
+            columns: str = "default",
+            sqobj=None,
+    ) -> None:
+        self.ctxt = context.get_context()
+        self._cfg = self.ctxt.cfg
+        self._schemas = self.ctxt.schemas
 
-    if max_rows is not None:
-        if max_rows == 0:
-            ctxt.max_rows = None
+        if not isinstance(namespace, str):
+            print('namespace must be a space separated list of strings')
+            return
+        if not isinstance(hostname, str):
+            print('hostname must be a space separated list of strings')
+            return
+        if not isinstance(columns, str):
+            print('columns must be a space separated list of strings')
+            return
+
+        if not namespace and self.ctxt.namespace:
+            self.namespace = self.ctxt.namespace
+        else:
+            self.namespace = namespace.split()
+        if not hostname and self.ctxt.hostname:
+            self.hostname = self.ctxt.hostname
         else:
-            ctxt.max_rows = max_rows
+            self.hostname = hostname.split()
 
-    if all_columns is not None:
-        ctxt.all_columns = all_columns == "yes"
+        if not start_time and self.ctxt.start_time:
+            self.start_time = self.ctxt.start_time
+        else:
+            self.start_time = start_time
 
-    if pager == 'on':
-        ctxt.pager = True
-    elif pager == 'off':
-        ctxt.pager = False
+        if not end_time and self.ctxt.end_time:
+            self.end_time = self.ctxt.end_time
+        else:
+            self.end_time = end_time
 
-    if rest_server_ip:
-        ctxt.rest_server_ip = rest_server_ip
+        if self.start_time and self.end_time:
+            self.view = "all"
+        else:
+            self.view = view
+        self.columns = columns.split()
+        self.format = format or "text"
+        self.json_print_handler = None
+
+        if not sqobj:
+            raise AttributeError('mandatory parameter sqobj missing')
+
+        self.sqobj = sqobj(context=self.ctxt,
+                           hostname=self.hostname,
+                           start_time=self.start_time,
+                           end_time=self.end_time,
+                           view=self.view,
+                           namespace=self.namespace,
+                           columns=self.columns)
+
+    @property
+    def cfg(self):
+        return self._cfg
+
+    @property
+    def schemas(self):
+        return self._schemas
+
+    def _pager_print(self, df: pd.DataFrame) -> None:
+        '''To support paging'''
+
+        if df.index.dtype == 'int64':
+            df.reset_index(drop=True, inplace=True)
+
+        if self.ctxt.pager:
+            screen_lines = (shutil.get_terminal_size((80, 20)).lines - 2)
+            bufio = StringIO()
+
+            print(df, file=bufio)
+            lines = bufio.getvalue().split('\n')
+            curline = 0
+            total_lines = len(lines)
+            while curline < total_lines:
+                print('\n'.join(lines[curline:curline+screen_lines]))
+                curline += screen_lines
+                if curline < total_lines:
+                    try:
+                        _ = prompt('Hit <ENTER> to continue, <CTRL-D> to quit')
+                    except EOFError:
+                        break
+        else:
+            print(df)
 
-    if rest_server_port:
-        ctxt.rest_server_port = rest_server_port
+        return
 
-    if rest_api_key:
-        ctxt.rest_api_key = rest_api_key
+    def _gen_output(self, df: pd.DataFrame, json_orient: str = "records",
+                    dont_strip_cols: bool = False, sort: bool = True):
 
-    if rest_use_https == 'True':
-        ctxt.rest_transport = 'https'
-    elif rest_use_https == 'False':
-        ctxt.rest_transport = 'http'
+        if df.columns.to_list() == ['error']:
+            retcode = 1
+            max_colwidth = None
+            cols = df.columns
+            is_error = True
+        else:
+            max_colwidth = 50
+            retcode = 0
+            if self.columns != ['default'] and self.columns != ['*']:
+                cols = self.columns
+            else:
+                cols = df.columns
+            is_error = False
 
+        if dont_strip_cols or not all(item in df.columns for item in cols):
+            cols = df.columns
 
-@command("clear")
-@argument("namespace", description="namespace to qualify selection")
-@argument("hostname", description="Name of host to qualify selection")
-@argument(
-    "start_time",
-    description="Start of time window in YYYY-MM-dd HH:mm:SS format"
-)
-@argument("end_time",
-          description="End of time window in YYYY-MM-dd HH:mm:SS format")
-@argument("pager",
-          description="End of time window in YYYY-MM-dd HH:mm:SS format")
-@argument(
-    "debug", choices=['True'], description="Disable debug mode",
-)
-def clear_ctxt(
-        pager: str = 'off',
-        hostname: str = "",
-        start_time: str = "",
-        end_time: str = "",
-        namespace: str = "",
-        debug: str = '',
-):
-    """clear certain contexts for subsequent commands. Cmd is additive"""
-    plugin_ctx = context.get_context()
-    ctxt = plugin_ctx.ctxt
-
-    if namespace:
-        ctxt.namespace = []
-
-    if hostname:
-        ctxt.hostname = []
-
-    if start_time:
-        ctxt.start_time = ""
-
-    if end_time:
-        ctxt.end_time = ""
-
-    if pager:
-        ctxt.pager = False
-
-    if debug:
-        ctxt.debug = False
-
-
-@command('version', help='print the suzieq version')
-def sq_version():
-    '''Print suzieq version'''
-    print_version()
-
-
-class SqHelpCommand (Command):
-    '''Class to handle processing CLI help'''
-    HELP = 'Get help on a command'
-    thiscmd = ["help", "?"]
-
-    def __init__(self):
-        super().__init__()
-        self._allcmds = self._sqcmds = None
-
-    def run_interactive(self, cmd, args, raw):
-        arglist = args.split()
-        return self._help_cmd(*arglist)
-
-    def get_command_names(self):
-        return self.thiscmd
-
-    def add_arguments(self, parser):
-        parser.add_parser("help")
-
-    def get_help(self, cmd, *args):
-        return self.thiscmd[0]
-
-    def get_completions(self, cmd, document, complete_event):
-        exploded = document.text.lstrip().split(" ", 1)
-        self._build_cmd_verb_list()
-        if len(exploded) <= 1:
-            if not document.text:
-                return [Completion(x)
-                        for x in self._sqcmds]
-            completions = [Completion(text=x,
-                                      start_position=-len(document.text))
-                           for x in self._sqcmds
-                           if x.startswith(document.text)]
-            return completions
-
-        service = exploded[0].lower()
-        verb = exploded[1]
-
-        verbs = [x[0].replace('aver', 'assert')
-                 for x in self._allcmds[service].metadata.subcommands
-                 if service in self._sqcmds]
-        if not verb:
-            return [Completion(x) for x in verbs]
-        completions = [Completion(text=x, start_position=-len(verb))
-                       for x in sorted(verbs)
-                       if x.startswith(verb)]
-        return completions
-
-    def _help_cmd(self, *args):
-        """Show help for a service"""
-        if len(args) == 0:
-            helpcmd = HelpCommand()
-            helpcmd.run_interactive('', '', '')
-            cprint(
-                "Use "
-                f"{colored('help <name of command/service> [<verb>]', 'cyan')}"
-                " to get more help")
-            cprint(f"For example: {colored('help route', 'cyan')}"
-                   f" or {colored('help route show', 'cyan')}")
-            return
-        if len(args) == 1:
-            service = args[0]
-            verb = ''
+        if self.format == 'json':
+            if self.json_print_handler:
+                print(df[cols].to_json(
+                    default_handler=self.json_print_handler,
+                    orient=json_orient))
+            else:
+                print(df[cols].to_json(orient=json_orient))
+        elif self.format == 'csv':
+            print(df[cols].to_csv())
+        elif self.format == 'markdown':
+            print(df[cols].to_markdown())
         else:
-            service = args[0]
-            verb = args[1]
+            with pd.option_context('precision', 3,
+                                   'display.max_colwidth', max_colwidth,
+                                   'display.max_rows', 256):
+                if df.empty:
+                    print(df)
+                elif sort:
+                    if is_error:
+                        print(df[cols])
+                    else:
+                        sort_fields = [x for x in self.sqobj._sort_fields
+                                       if x in df.columns and x in cols]
+                        if sort_fields:
+                            self._pager_print(
+                                df[cols].sort_values(by=sort_fields))
+                        else:
+                            self._pager_print(df[cols])
+                else:
+                    self._pager_print(df[cols])
+
+        return retcode
+
+    def _assert_gen_output(self, df):
+        if df.empty:
+            result = 0
+        elif df.columns.to_list() == ['error']:
+            result = 1
+        elif df.loc[df['assert'] != "pass"].empty:
+            result = 0
+        else:
+            result = -1
 
-        self._build_cmd_verb_list()
-        if service in self._sqcmds:
-            if verb:
-                self._allcmds[service].run_interactive(
-                    service, f'help command={verb}', '')
+        self._gen_output(df)
+        if self.format == 'text':
+            if result == 0:
+                print("Assert passed")
             else:
-                self._allcmds[service].run_interactive(service, 'help', '')
+                print("Assert failed")
+        return result
+
+    def show(self, **kwargs):
+        raise NotImplementedError
+
+    def analyze(self, **kwargs):
+        raise NotImplementedError
 
-    def _build_cmd_verb_list(self):
-        if not self._allcmds:
-            ctx = context.get_context()
-            self._allcmds = ctx.registry.get_all_commands_map()
-            self._sqcmds = [x for x in sorted(self._allcmds)
-                            if not self._allcmds[x].built_in]
+    def aver(self, **kwargs):
+        raise NotImplementedError
+
+    @ command("summarize", help='produce a summarize of the data')
+    def summarize(self):
+        self._init_summarize()
+        return self._post_summarize()
+
+    def top(self, **kwargs):
+        raise NotImplementedError
+
+    @command("unique", help="find the list of unique items in a column")
+    @argument("groupby", description="List of columns to group by")
+    @argument("type", description="Unique per host or table entry",
+              choices=['entry', 'host'])
+    def unique(self, groupby='', type='entry', **kwargs):
+        now = time.time()
+        try:
+            df = self.sqobj.unique(hostname=self.hostname,
+                                   namespace=self.namespace,
+                                   groupby=groupby, type=type,
+                                   )
+        except Exception as e:
+            df = pd.DataFrame({'error': ['ERROR: {}'.format(str(e))]})
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        return self._gen_output(df, dont_strip_cols=True)
+
+    def _init_summarize(self):
+        self.now = time.time()
+
+        self.summarize_df = self.sqobj.summarize(
+            namespace=self.namespace, hostname=self.hostname,
+        )
+
+    def _post_summarize(self):
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - self.now)
+        return self._gen_output(self.summarize_df, json_orient='columns')
```

### Comparing `suzieq-0.22.0rc1/suzieq/engines/pandas/bgp.py` & `suzieq-0.8.0/suzieq/engines/pandas/evpnVni.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,313 +1,301 @@
 import numpy as np
 import pandas as pd
+import ipaddress
 
-from suzieq.engines.pandas.engineobj import SqPandasEngine
-from suzieq.shared.utils import build_query_str, humanize_timestamp
-
-
-class BgpObj(SqPandasEngine):
-    '''Backend class to handle manipulating BGP table with pandas'''
-
-    def __init__(self, baseobj):
-        super().__init__(baseobj)
-        self._assert_result_cols = ['namespace', 'hostname', 'vrf', 'peer',
-                                    'asn', 'peerAsn', 'state', 'peerHostname',
-                                    'result', 'assertReason', 'timestamp']
-
-    @staticmethod
-    def table_name():
-        '''Table name'''
-        return 'bgp'
-
-    def get(self, **kwargs):
-        """Replacing the original interface name in returned result"""
-
-        columns = kwargs.pop('columns', ['default'])
-        vrf = kwargs.pop('vrf', None)
-        peer = kwargs.pop('peer', None)
-        hostname = kwargs.pop('hostname', None)
-        user_query = kwargs.pop('query_str', None)
-        afi_safi = kwargs.pop('afiSafi', '')
-
-        addnl_fields = ['origPeer']
-        sch = self.schema
-        fields = sch.get_display_fields(columns)
-
-        self._add_active_to_fields(kwargs.get('view', self.iobj.view), fields,
-                                   addnl_fields)
-
-        for col in ['peerIP', 'updateSource', 'state', 'namespace', 'vrf',
-                    'peer', 'hostname']:
-            if col not in fields:
-                addnl_fields.append(col)
-
-        if afi_safi and afi_safi not in fields:
-            addnl_fields.append('afiSafi')
-
-        user_query_cols = self._get_user_query_cols(user_query)
-        addnl_fields += [x for x in user_query_cols if x not in addnl_fields]
-
-        try:
-            df = super().get(addnl_fields=addnl_fields, columns=fields,
-                             **kwargs)
-        except KeyError as ex:
-            if ('afi' in str(ex)) or ('safi' in str(ex)):
-                df = pd.DataFrame(
-                    {'error':
-                     ['ERROR: Migrate BGP data first using sq-coalescer']})
-                return df
+from .engineobj import SqEngineObject
+from suzieq.sqobjects.macs import MacsObj
+from suzieq.sqobjects.interfaces import IfObj
+from suzieq.sqobjects.routes import RoutesObj
+
+
+class EvpnvniObj(SqEngineObject):
+
+    def get(self, **kwargs) -> pd.DataFrame:
+        """Class-specific to extract info from addnl tables"""
+
+        drop_cols = []
+        addnl_fields = kwargs.pop('addnl_fields', [])
+        columns = kwargs.get('columns', [])
+        if 'ifname' not in columns and 'ifname' not in addnl_fields:
+            addnl_fields.append('ifname')
+            drop_cols.append('ifname')
+
+        if (columns == ['default'] or columns == ['*'] or
+                'remoteVtepCnt' in columns):
+            getVtepCnt = True
+            if columns != ['*'] and 'remoteVtepList' not in columns:
+                addnl_fields.append('remoteVtepList')
+                drop_cols.append('remoteVtepList')
+        else:
+            getVtepCnt = False
 
+        df = super().get(addnl_fields=addnl_fields, **kwargs)
         if df.empty:
-            # We cannot add df[fields] here because we haven't added the
-            # augmented columns yet and so can fail.
             return df
 
-        if afi_safi or 'afiSafi' in fields or (columns == ['*']):
-            df['afiSafi'] = df['afi'] + ' ' + df['safi']
-        query_str = build_query_str([], sch, vrf=vrf, peer=peer,
-                                    hostname=hostname, afiSafi=afi_safi,
-                                    ignore_regex=False)
-        if 'peer' in df.columns:
-            df['peer'] = np.where(df['origPeer'] != "",
-                                  df['origPeer'], df['peer'])
-
-        if 'asndot' in fields:
-            df['asndot'] = df.asn.apply(lambda x: f'{int(x/65536)}.{x%65536}')
-
-        if 'peerAsndot' in fields:
-            df['peerAsndot'] = df.peerAsn.apply(
-                lambda x: f'{int(x/65536)}.{x%65536}')
-
-        # Convert old data into new 2.0 data format
-        if 'peerHostname' in df.columns:
-            mdf = self._get_peer_matched_df(df)
+        if getVtepCnt:
+            insidx = df.columns.tolist().index('remoteVtepList')
+            df.insert(insidx+1, 'remoteVtepCnt',
+                      df.remoteVtepList.str.len())
+
+        # See if we can retrieve the info to fill out the rest of the data
+        # Start with VLAN values
+        if 'vlan' not in df.columns:
+            return df.drop(columns=drop_cols, errors='ignore')
+
+        iflist = df[df.vlan == 0]['ifname'].to_list()
+        if iflist:
+            ifdf = IfObj(context=self.ctxt).get(
+                namespace=kwargs.get('namespace', []), ifname=iflist,
+                columns=['namespace', 'hostname', 'ifname', 'state', 'vlan',
+                         'vni'])
+
+            if not ifdf.empty:
+                df = df.merge(ifdf, on=['namespace', 'hostname', 'ifname',
+                                        'vni'], how='left',
+                              suffixes=('', '_y')) \
+                    .drop(columns=['timestamp_y', 'state_y'])
+
+                df['vlan'] = np.where(df['vlan_y'], df['vlan_y'], df['vlan'])
+                df.drop(columns=['vlan_y'], inplace=True)
+
+        # Fill out the numMacs and numArps columns if we can
+        if 'numMacs' in df.columns:
+            vlanlist = list(set(df[df.numMacs == 0]['vlan'].to_list()))
         else:
-            mdf = df
-
-        mdf = self._handle_user_query_str(mdf, user_query)
-
-        if query_str:
-            return mdf.query(query_str).reset_index(drop=True)[fields]
-        else:
-            return mdf.reset_index(drop=True)[fields]
-
-    def summarize(self, **kwargs) -> pd.DataFrame:
-        """Summarize key information about BGP"""
-
-        self._init_summarize(**kwargs)
-        if self.summary_df.empty or ('error' in self.summary_df.columns):
+            vlanlist = []
+        if vlanlist:
+            if 'numMacs' in df.columns:
+                macdf = MacsObj(context=self.ctxt).get(
+                    namespace=kwargs.get('namespace'))
+                df['numMacs'] = df.apply(self._count_macs, axis=1,
+                                         args=(macdf, ))
+        return df.drop(columns=drop_cols, errors='ignore')
+
+    def _count_macs(self, x, df):
+        return df[(df.namespace == x['namespace']) & (df.vlan == x['vlan']) &
+                  (df.hostname == x['hostname'])].count()
+
+    def summarize(self, **kwargs):
+        self._init_summarize(self.iobj._table, **kwargs)
+        if self.summary_df.empty:
             return self.summary_df
 
-        self.summary_df['afiSafi'] = (
-            self.summary_df['afi'] + ' ' + self.summary_df['safi'])
-
-        afi_safi_count = self.summary_df.groupby(by=['namespace'])['afiSafi'] \
-                                        .nunique()
-
-        self.summary_df = self.summary_df \
-                              .set_index(['namespace', 'hostname', 'vrf',
-                                          'peer']) \
-                              .query('~index.duplicated(keep="last")') \
-                              .reset_index()
-        self.ns = {i: {} for i in self.summary_df['namespace'].unique()}
-        self.nsgrp = self.summary_df.groupby(by=["namespace"],
-                                             observed=True)
-
         self._summarize_on_add_field = [
-            ('deviceCnt', 'hostname', 'nunique'),
-            ('totalPeerCnt', 'peer', 'count'),
-            ('uniqueAsnCnt', 'asn', 'nunique'),
-            ('uniqueVrfsCnt', 'vrf', 'nunique')
+            ('uniqueVtepCnt', 'hostname', 'nunique'),
+            ('uniqueVniCnt', 'vni', 'nunique'),
         ]
 
+        l3vni_count = self.summary_df.query('type == "L3" and vni != 0') \
+                                     .groupby(by=['namespace'])['vni'].count()
+        for ns in self.ns.keys():
+            if l3vni_count.get(ns, 0):
+                self.ns[ns]['mode'] = 'symmetric'
+            else:
+                self.ns[ns]['mode'] = 'asymmetric'
+        self.summary_row_order.append('mode')
+
         self._summarize_on_add_with_query = [
-            ('failedPeerCnt', 'state == "NotEstd"', 'peer'),
-            ('iBGPPeerCnt', 'asn == peerAsn', 'peer', 'count'),
-            ('eBGPPeerCnt', 'asn != peerAsn', 'peer', 'count'),
-            ('rrClientPeerCnt', 'rrclient.str.lower() == "true"', 'peer',
-             'count'),
+            ('uniqueL3VniCnt', 'type == "L3" and vni != 0', 'vrf', 'nunique'),
+            ('uniqueL2VniCnt', 'type == "L2"', 'vni', 'nunique'),
+            ('uniqueMulticastGroups', 'mcastGroup != "0.0.0.0"', 'mcastGroup',
+             'nunique'),
+            ('vnisUsingMulticast',
+             'type == "L2" and replicationType == "multicast"',
+             'vni', 'nunique'),
+            ('vnisUsingIngressRepl',
+             'type == "L2" and replicationType == "ingressBGP"',
+             'vni', 'nunique')
         ]
 
         self._gen_summarize_data()
 
-        # pylint: disable=expression-not-assigned
-        {self.ns[i].update({'activeAfiSafiCnt': afi_safi_count[i]})
-         for i in self.ns.keys()}
-        self.summary_row_order.append('activeAfiSafiCnt')
-
-        self.summary_df['estdTime'] = humanize_timestamp(
-            self.summary_df.estdTime,
-            self.cfg.get('analyzer', {}).get('timezone', None))
-
-        self.summary_df['estdTime'] = (
-            self.summary_df['timestamp'] - self.summary_df['estdTime'])
-        self.summary_df['estdTime'] = self.summary_df['estdTime'] \
-                                          .apply(lambda x: x.round('s'))
-        # Now come the BGP specific ones
-        established = self.summary_df.query("state == 'Established'") \
-            .groupby(by=['namespace'])
-
-        uptime = established["estdTime"]
-        rx_updates = established["updatesRx"]
-        tx_updates = established["updatesTx"]
-        self._add_stats_to_summary(uptime, 'upTimeStat')
-        self._add_stats_to_summary(rx_updates, 'updatesRxStat')
-        self._add_stats_to_summary(tx_updates, 'updatesTxStat')
+        # To summarize accurately, we need to explode the remoteVteps
+        # column from a list to an individual entry for each
+        # remoteVteps in that list. The resulting set can be huge if them
+        # number of Vteps times the ports is huge.
+        #
+        # the 'explode' only works post pandas 0.25
+
+        self.summary_df = self.summary_df.explode(
+            'remoteVtepList').dropna(how='any')
+        self.nsgrp = self.summary_df.groupby(by=["namespace"])
+
+        if not self.summary_df.empty:
+            herPerVtepCnt = self.summary_df.groupby(
+                by=['namespace', 'hostname'])['remoteVtepList'].nunique()
+            self._add_stats_to_summary(herPerVtepCnt, 'remoteVtepsPerVtepStat',
+                                       filter_by_ns=True)
+        self.summary_row_order.append('remoteVtepsPerVtepStat')
 
-        self.summary_row_order.extend(['upTimeStat', 'updatesRxStat',
-                                       'updatesTxStat'])
-
-        self._post_summarize()
+        self._post_summarize(check_empty_col='uniqueVtepCnt')
         return self.ns_df.convert_dtypes()
 
-    def _get_peer_matched_df(self, df) -> pd.DataFrame:
-        """Get a BGP dataframe that also contains a session's matching peer"""
-
-        if 'peerHostname' not in df.columns:
-            return df
-
-        # We have to separate out the Established and non Established entries
-        # for the merge. Otherwise we end up with a mess
-        df_1 = df[['namespace', 'hostname', 'vrf', 'peer', 'peerIP',
-                   'updateSource']] \
-            .drop_duplicates() \
-            .reset_index(drop=True)
-        df_2 = df[['namespace', 'hostname', 'vrf', 'updateSource']] \
-            .drop_duplicates() \
-            .reset_index(drop=True)
-
-        mdf = df_1.merge(df_2,
-                         left_on=['namespace', 'peerIP'],
-                         right_on=['namespace', 'updateSource'],
-                         suffixes=('', '_y')) \
-            .drop_duplicates(subset=['namespace', 'hostname', 'vrf',
-                                     'peerIP']) \
-            .rename(columns={'hostname_y': 'peerHost'}) \
-            .fillna(value={'peerHostname': '', 'peerHost': ''}) \
-            .reset_index(drop=True)
-
-        df = df.merge(mdf[['namespace', 'hostname', 'vrf', 'peer',
-                           'peerHost']],
-                      on=['namespace', 'hostname', 'vrf', 'peer'], how='left')
-
-        df['peerHostname'] = np.where((df['peerHostname'] == '') &
-                                      (df['state'] == "Established"),
-                                      df['peerHost'],
-                                      df['peerHostname'])
-        df = df.fillna(value={'peerHostname': ''}) \
-            .drop(columns=['peerHost'])
-
-        for i in df.select_dtypes(include='category'):
-            df[i].cat.add_categories('', inplace=True)
-
-        return df
-
     def aver(self, **kwargs) -> pd.DataFrame:
-        """BGP Assert"""
-
-        def _check_if_state(row, if_df):
+        """Assert for EVPN Data"""
 
-            if not if_df.empty:
-                thisif = if_df.query(f'namespace=="{row.namespace}" and '
-                                     f'hostname=="{row.hostname}" and '
-                                     f'ifname=="{row.ifname}"')
-                if not thisif.empty:
-                    if thisif.adminState.unique()[0] != 'up':
-                        return ['interface admin down']
-                    elif thisif.state.unique()[0] != 'up':
-                        return ['interface down']
-                    else:
-                        return []
-
-            return []
-
-        assert_cols = ["namespace", "hostname", "vrf", "peer", "peerHostname",
-                       "afi", "safi", "asn", "state", "peerAsn", "bfdStatus",
-                       "reason", "notificnReason", "afisAdvOnly", 'ifname',
-                       "afisRcvOnly", "peerIP", "updateSource", "timestamp"]
+        assert_cols = ["namespace", "hostname", "vni", "remoteVtepList", "vrf",
+                       "mcastGroup", "type", "priVtepIp", "state", "l2VniList",
+                       "ifname", "secVtepIp"]
 
         kwargs.pop("columns", None)  # Loose whatever's passed
-        result = kwargs.pop("result", 'all')
-        state = kwargs.pop('state', '!dynamic')
-
-        df = self.get(columns=assert_cols, state=state, **kwargs)
-        if 'error' in df:
-            return df
+        status = kwargs.pop('status', 'all')
 
+        df = self.get(columns=assert_cols, **kwargs)
         if df.empty:
-            if result != "pass":
-                df['result'] = 'fail'
-                df['assertReason'] = 'No data'
+            df = pd.DataFrame(columns=assert_cols)
+            if status != 'pass':
+                df['assertReason'] = 'No data found'
+                df['assert'] = 'fail'
             return df
 
-        df = self._get_peer_matched_df(df)
-        if df.empty:
-            if result != "pass":
-                df['result'] = 'fail'
-                df['assertReason'] = 'No data'
-            return df
+        df["assertReason"] = [[] for _ in range(len(df))]
 
-        # We can get rid of sessions with duplicate peer info since we're
-        # interested only in session info here
-        df = df.drop_duplicates(
-            subset=['namespace', 'hostname', 'vrf', 'peer'])
-
-        failed_df = df.query("state != 'Established'").reset_index(drop=True)
-        passed_df = df.query("state == 'Established'").reset_index(drop=True)
-
-        # Get the interface information
-        if_df = self._get_table_sqobj('interfaces').get(
-            namespace=failed_df.namespace.unique().tolist(),
-            hostname=failed_df.hostname.unique().tolist(),
-            ifname=failed_df.ifname.unique().tolist(),
-            columns=['namespace', 'hostname', 'ifname', 'state', 'adminState']
-        )
-
-        failed_df['assertReason'] = [[] for _ in range(len(failed_df))]
-        passed_df['assertReason'] = [[] for _ in range(len(passed_df))]
-
-        if not failed_df.empty:
-            # For not established entries, check if route/ARP entry exists
-            failed_df['assertReason'] += failed_df.apply(
-                _check_if_state, args=(if_df,), axis=1)
-
-            failed_df['assertReason'] += failed_df.apply(
-                lambda x: ["asn mismatch"]
-                if (x['peerHostname'] and ((x["asn"] != x["peerAsn_y"]) or
-                                           (x['asn_y'] != x['peerAsn'])))
-                else [], axis=1)
-
-            failed_df['assertReason'] += failed_df.apply(
-                lambda x: [f"{x['reason']}:{x['notificnReason']}"]
-                if ((x['reason'] and x['reason'] != 'None' and
-                     x['reason'] != "No error"))
-                else [], axis=1)
-
-            failed_df['result'] = 'fail'
-
-        # Get list of peer IP addresses for peer not in Established state
-        # Returning to performing checks even if we didn't get LLDP/Intf info
-
-        if not passed_df.empty:
-            passed_df['assertReason'] += passed_df.apply(
-                lambda x: ['Not all Afi/Safis enabled']
-                if x['afisAdvOnly'].any() or x['afisRcvOnly'].any() else [],
-                axis=1)
-
-            passed_df['result'] = passed_df.apply(
-                lambda x: 'pass'
-                if len(x.assertReason) == 0 else 'fail',
-                axis=1)
+        # Gather the unique set of VTEPs per VNI
+        vteps_df = df.explode(column='remoteVtepList') \
+            .dropna(how='any') \
+            .groupby(by=['vni', 'type'])['remoteVtepList'] \
+            .aggregate(lambda x: x.unique().tolist()) \
+            .reset_index() \
+            .dropna(how='any') \
+            .rename(columns={'remoteVtepList': 'allVteps'})
 
-        df = pd.concat([failed_df, passed_df])
+        if not vteps_df.empty:
+            her_df = df.merge(vteps_df)
+        else:
+            her_df = pd.DataFrame()
 
-        result_df = df[self._assert_result_cols] \
-            .explode(column="assertReason") \
+        if (not her_df.empty and
+                (her_df.remoteVtepList.str.len() != 0).any()):
+            # Check if every VTEP we know is reachable
+            rdf = RoutesObj(context=self.ctxt).get(
+                namespace=kwargs.get('namespace'), vrf='default')
+            if not rdf.empty:
+                rdf['prefixlen'] = rdf['prefix'].str.split('/') \
+                                                    .str[1].astype('int')
+            self._routes_df = rdf
+
+            her_df["assertReason"] += her_df.apply(
+                self._is_vtep_reachable, axis=1)
+
+        mcast_df = df.query('mcastGroup != "0.0.0.0"')
+        if not mcast_df.empty:
+            # Ensure that all VNIs have at most one multicast group associated
+            # per namespace
+
+            mismatched_vni_df = mcast_df \
+                .groupby(by=['namespace', 'vni'])['mcastGroup'] \
+                .unique() \
+                .reset_index() \
+                .dropna() \
+                .query('mcastGroup.str.len() != 1')
+
+            if not mismatched_vni_df.empty:
+                df['assertReason'] += df.apply(
+                    lambda x, err_df: ['VNI has multiple mcast group']
+                    if (x['namespace'] in err_df['namespace'] and
+                        x['vni'] in err_df['vni']) else [], axis=1,
+                    args=(mismatched_vni_df, ))
+        elif not her_df.empty:
+            # Every VTEP has info about every other VTEP for a given VNI
+            her_df["assertReason"] += her_df.apply(
+                self._all_vteps_present, axis=1)
+
+        # State is up
+        df["assertReason"] += df.apply(
+            lambda x: ['interface is down']
+            if x['type'] == "L2" and x['state'] != "up"
+            else [], axis=1)
+
+        devices = df["hostname"].unique().tolist()
+        ifdf = IfObj(context=self.ctxt) \
+            .get(namespace=kwargs.get("namespace", ""), hostname=devices,
+                 type='vxlan')
+
+        df = df.merge(ifdf[['namespace', 'hostname', 'ifname', 'master',
+                            'vlan']],
+                      on=['namespace', 'hostname', 'ifname'], how='left')
+
+        # vxlan interfaces, if defined, for every VNI is part of bridge
+        # We ensure this is true artificially for NXOS, ignored for JunOS.
+        df["assertReason"] += df.apply(
+            lambda x: ['vni not in bridge']
+            if (x['type'] == "L2" and x['ifname'] != '-'
+                and x['master'] != "bridge") else [],
+            axis=1)
+
+        # mac_df = MacsObj(context=self.ctxt) \
+        #     .get(namespace=kwargs.get("namespace", ""),
+        #          macaddr=["00:00:00:00:00:00"])
+
+        # # Assert that we have HER for every remote VTEP
+        # df['assertReason'] += df.apply(self._is_her_good,
+        #                                args=(mac_df, ), axis=1)
+
+        # Fill out the assert column
+        df['assert'] = df.apply(lambda x: 'pass'
+                                if not len(x.assertReason) else 'fail',
+                                axis=1)
+
+        if status == 'fail':
+            df = df.query('assertReason.str.len() != 0')
+        elif status == "pass":
+            df = df.query('assertReason.str.len() == 0')
+
+        return df[['namespace', 'hostname', 'vni', 'type',
+                   'assertReason', 'assert', 'timestamp']] \
+            .explode(column='assertReason') \
             .fillna({'assertReason': '-'})
 
-        if result == "fail":
-            result_df = result_df.query('assertReason != "-"')
-        elif result == "pass":
-            result_df = result_df.query('assertReason == "-"')
+    def _all_vteps_present(self, row):
+        if row['secVtepIp'] == '0.0.0.0':
+            myvteps = set([row['priVtepIp']])
+        else:
+            myvteps = set([row['secVtepIp'], row['priVtepIp']])
+
+        isitme = set(row['allVteps']).difference(set(row['remoteVtepList']))
+        if (isitme.intersection(myvteps) or
+                (row['type'] == "L3" and row['remoteVtepList'] == ["-"])):
+            return []
+
+        return (['some remote VTEPs missing'])
 
-        return result_df.reset_index(drop=True)
+    def _is_vtep_reachable(self, row):
+        reason = []
+        defrt = ipaddress.IPv4Network("0.0.0.0/0")
+        for vtep in row['remoteVtepList'].tolist():
+            if vtep == '-':
+                continue
+
+            # Have to hardcode lpm query here sadly to avoid reading of the
+            # data repeatedly. The time for asserting the state of 500 VNIs
+            # came down from 194s to 4s with the below piece of code instead
+            # of invoking route's lpm to accomplish the task.
+            cached_df = self._routes_df \
+                            .query(f'namespace=="{row.namespace}" and hostname=="{row.hostname}"')
+            route = RoutesObj(context=self.ctxt).lpm(vrf='default',
+                                                     address=vtep,
+                                                     cached_df=cached_df)
+
+            if route.empty:
+                reason += [f"{vtep} not reachable"]
+                continue
+            if route.prefix.tolist() == [defrt]:
+                reason += [f"{vtep} reachable via default"]
+
+        return reason
+
+    def _is_her_good(self, row, mac_df):
+        reason = []
+
+        if row['type'] == 'L3':
+            return reason
+
+        her_list = mac_df[(mac_df['hostname'] == row['hostname']) &
+                          (mac_df['namespace'] == row['namespace']) &
+                          (mac_df['oif'] == row['ifname'])]['remoteVtepIp'] \
+            .tolist()
+        missing_hers = set(row['remoteVtepList']).difference(set(her_list))
+        if not missing_hers:
+            return reason
+        return [f'HER is missing VTEPs {missing_hers}']
```

### Comparing `suzieq-0.22.0rc1/suzieq/engines/pandas/engineobj.py` & `suzieq-0.8.0/suzieq/poller/services/service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,735 +1,714 @@
-from typing import List
-import re
-from ipaddress import ip_address, ip_network
-
-import dateparser
-import numpy as np
-import pandas as pd
-from pandas.core.groupby import DataFrameGroupBy
-
-from suzieq.shared.utils import build_query_str, humanize_timestamp
-from suzieq.shared.schema import Schema, SchemaForTable
-from suzieq.engines.base_engine import SqEngineObj
-from suzieq.sqobjects import get_sqobject
-from suzieq.db import get_sqdb_engine
-from suzieq.shared.exceptions import UserQueryError
-
-
-class SqPandasEngine(SqEngineObj):
-    '''Base class to handle manipulating tables with pandas'''
-
-    def __init__(self, baseobj):
-        self.ctxt = baseobj.ctxt
-        self.iobj = baseobj
-        self.summary_row_order = []
-        self.nsgrp = None
-        self.ns_df = pd.DataFrame()
-        self.ns = []
-        self.summary_df = pd.DataFrame()
-        self._summarize_on_add_field = []
-        self._summarize_on_add_with_query = []
-        self._summarize_on_add_list_or_count = []
-        self._summarize_on_add_stat = []
-        self._summarize_on_perdevice_stat = []
-        self._check_empty_col = 'namespace'
-        self._dbeng = get_sqdb_engine(baseobj.ctxt.cfg, baseobj.table, '',
-                                      None)
-
-    @property
-    def all_schemas(self) -> Schema:
-        '''Return dict of all schemas'''
-        return self.ctxt.schemas
-
-    @property
-    def cfg(self):
-        '''Return config dicttionary'''
-        return self.iobj.cfg
-
-    @property
-    def name(self):
-        return 'pandas'
-
-    @property
-    def table(self):
-        '''Table name'''
-        return self.iobj.table
-
-    @property
-    def schema(self) -> SchemaForTable:
-        '''Return schema for this table'''
-        return self.iobj.schema
-
-    def _get_ipvers(self, value: str) -> int:
-        """Return the IP version in use"""
-
-        if ':' in value:
-            ipvers = 6
-        elif '.' in value:
-            ipvers = 4
-        else:
-            ipvers = ''
-
-        return ipvers
-
-    def _handle_user_query_str(self, df: pd.DataFrame,
-                               query_str: str) -> pd.DataFrame:
-        """Handle user query, trapping errors and returning exception
-
-        Args:
-            df (pd.DataFrame): The dataframe to run the query on
-            query_str (str): pandas query string
-
-        Raises:
-            UserQueryError: Exception if pandas query aborts with errmsg
-
-        Returns:
-            pd.DataFrame: dataframe post query
-        """
-        if query_str:
-            try:
-                df = df.query(query_str)
-            except Exception as ex:
-                raise UserQueryError(ex) from Exception
-
-        return df
-
-    def _is_any_in_list(self, column: pd.Series, values: List) -> pd.Series:
-        """Given a column of arrays, check if any of the values is present in
-        the list.
-        Args:
-            column (pd.Series): pandas dataframe column of lists
-            values (List): list of values representing the filtering values
-        Returns:
-            pd.Series: A collection of bool reporting the filtered result
-        """
-        return column.apply(lambda x: any(v in x for v in values))
-
-    def _is_in_subnet(self, addr: pd.Series, net: str) -> pd.Series:
-        """check which of the addresses belongs to a given subnet
-
-        Used to implement the prefix filter of arpnd/address/dhcp
-        Args:
-            addr (pd.Series): the pandas series of ip addresses to check
-            net: (str): the IP network to check the addresses against
-
-        Returns:
-            pd.Series: A collection of bool reporting the result
-        """
-        network = ip_network(net)
-        if isinstance(addr.iloc[0], np.ndarray):
-            return addr.apply(lambda x, network:
-                              False if not x.any()
-                              else any(ip_address(a.split("/")[0]) in network
-                                       for a in x),
-                              args=(network,))
+import os
+import asyncio
+from datetime import datetime
+import time
+import copy
+import logging
+import json
+import yaml
+from tempfile import mkstemp
+from dataclasses import dataclass
+from http import HTTPStatus
+from collections import defaultdict
+
+import pyarrow as pa
+
+from suzieq.poller.services.svcparser import cons_recs_from_json_template
+from suzieq.utils import known_devtypes
+
+HOLD_TIME_IN_MSECS = 60000  # How long b4 declaring node dead
+
+
+@dataclass
+class RsltToken:
+    start_time: int    # When this cmd was first posted to node
+    nodename: str      # Name of node, used to get poller cb again
+    bootupTimestamp: int
+    nodeQsize: int        # Size of the node q at queuing time
+    service: str          # Name of this service, if node needs it
+    timeout: int          # timeout value for cmd to complete
+
+
+@dataclass
+class ServiceStats:
+    total_time = list()
+    gather_time = list()
+    svcQsize = list()
+    nodeQsize = list()
+    wrQsize = list()
+    empty_count: int = 0
+    time_excd_count: int = 0    # Number of times total_time > poll period
+    next_update_time: int = 0   # When results will be logged
+
+
+class Service(object):
+
+    def get_poller_schema(self):
+        return self._poller_schema
+
+    def set_poller_schema(self, value: dict):
+        self._poller_schema = value
+
+    def __init__(self, name, defn, period, stype, keys, ignore_fields, schema,
+                 queue, run_once="forever"):
+        self.name = name
+        self.defn = defn
+        self.ignore_fields = ignore_fields or []
+        self.writer_queue = queue
+        self.keys = keys
+        self.schema = schema.get_arrow_schema()
+        self.period = period
+        self.stype = stype
+        self.logger = logging.getLogger(__name__)
+        self.run_once = run_once
+        self.post_timeout = 5
+        self.sigend = False
+        self.version = schema.version
+
+        self.update_nodes = False  # we have a new node list
+        self.rebuild_nodelist = False  # used only when a node gets init
+        self.node_postcall_list = {}
+        self.new_node_postcall_list = {}
+        self.previous_results = {}
+        self._poller_schema = {}
+        self.node_boot_times = defaultdict(int)
+        self._failed_node_set = set()
+
+        self.poller_schema = property(
+            self.get_poller_schema, self.set_poller_schema)
+
+        # The queue to which all nodes will post the result of the command
+        self.result_queue = asyncio.Queue()
+
+        # Add the hidden fields to ignore_fields
+        self.ignore_fields.append("timestamp")
+
+        if "namespace" not in self.keys:
+            self.keys.insert(0, "namespace")
+
+        if "hostname" not in self.keys:
+            self.keys.insert(1, "hostname")
+
+        self.partition_cols = schema.get_partition_columns()
+
+        # Setup dictionary of NOS specific extracted data cleaners
+        self.dev_clean_fn = {}
+        common_dev_clean_fn = getattr(self, '_common_data_cleaner', None)
+        for x in known_devtypes():
+            if x.startswith('junos'):
+                dev = 'junos'
+            else:
+                dev = x
+            self.dev_clean_fn[x] = getattr(
+                self, f'_clean_{dev}_data', None) or common_dev_clean_fn
+
+    @ staticmethod
+    def is_status_ok(status: int) -> bool:
+        if status == 0 or status == HTTPStatus.OK:
+            return True
+        return False
+
+    def get_data(self):
+        """provide the data that is interesting for a service
+
+        does not include queue or schema"""
+
+        r = {}
+        for field in 'name defn ignore_fields keys period stype partition_cols'.split(' '):
+            r[field] = getattr(self, field)
+        # textFSM objects can't be jsoned, so changing it
+        for device in r['defn']:
+            if 'textfsm' in r['defn'][device]:
+                r['defn'][device]['textfsm'] = str(
+                    r['defn'][device]['textfsm'])
+        return r
+
+    def set_nodes(self, node_call_list):
+        """New node list for this service"""
+        if self.node_postcall_list:
+            self.new_node_postcall_list = node_call_list
+            self.update_nodes = True
         else:
-            return addr.apply(lambda a: (
-                False if not a else ip_address(a.split("/")[0]) in network)
-            )
-
-    def _in_subnet_series(self, addr: str, net: pd.Series) -> pd.Series:
-        """Check if an addr is in any of series' subnets
+            self.node_postcall_list = node_call_list
 
-        unlike is_in_subnet which checks if a pandas series of addresses
-        belongs in a given subnet, this routine checks if a given address
-        belongs to any of the provided pandas series of subnets. THis is
-        currently used in path to identify an SVI for a given address
-
-        Args:
-            addr (str): the address we're checking for
-            net: (pd.Series): the pandas series of subnets
-
-        Returns:
-            pd.Series: A collection of bool reporting the result
-        """
-        address = ip_address(addr)
-        if isinstance(net.iloc[0], np.ndarray):
-            return net.apply(lambda x, network:
-                             False if not x.any()
-                             else any(address in ip_network(a, strict=False)
-                                      for a in x if a != '0.0.0.0/0'),
-                             args=(address,))
+    def _get_default_vals(self) -> dict:
+        return({
+            pa.string(): "",
+            pa.int32(): 0,
+            pa.int64(): 0,
+            pa.float32(): 0.0,
+            pa.float64(): 0.0,
+            pa.date64(): 0.0,
+            pa.bool_(): False,
+            pa.list_(pa.string()): [],
+            pa.list_(pa.int64()): [],
+        })
+
+    def get_empty_record(self):
+        map_defaults = self._get_default_vals()
+
+        defaults = [map_defaults[x] for x in self.schema.types]
+        rec = dict(zip(self.schema.names, defaults))
+
+        return rec
+
+    def _dump_output(self, outputs) -> str:
+        """Dump the output to a YAML file"""
+        if outputs:
+            yml = {"service": self.name,
+                   "type": self.run_once,
+                   "output": outputs}
+            fd, name = mkstemp(suffix=f"-{self.name}-poller.yml")
+            f = os.fdopen(fd, "w")
+            f.write(yaml.dump(yml))
+            f.close()
+            return name
+        return ""
+
+    def get_diff(self, old, new):
+        """Compare list of dictionaries ignoring certain fields
+        Return list of adds and deletes
+        """
+        adds = []
+        dels = []
+        koldvals = {}
+        knewvals = {}
+        koldkeys = []
+        knewkeys = []
+
+        # keys that start with _ are transient and must be ignored
+        # from comparison
+        for i, elem in enumerate(old):
+            vals = [v for k, v in elem.items()
+                    if k not in self.ignore_fields and not k.startswith('_')]
+            kvals = [v for k, v in elem.items() if k in self.keys]
+            koldvals.update({tuple(str(vals)): i})
+            koldkeys.append(kvals)
+
+        for i, elem in enumerate(new):
+            vals = [v for k, v in elem.items()
+                    if k not in self.ignore_fields and not k.startswith('_')]
+            kvals = [v for k, v in elem.items() if k in self.keys]
+            knewvals.update({tuple(str(vals)): i})
+            knewkeys.append(kvals)
+
+        addlist = [v for k, v in knewvals.items() if k not in koldvals.keys()]
+        dellist = [v for k, v in koldvals.items() if k not in knewvals.keys()]
+
+        adds = [new[v] for v in addlist]
+        dels = [old[v] for v in dellist if koldkeys[v] not in knewkeys]
+
+        if adds and self.stype == "counters":
+            # If there's a change in any field of the counters, update them all
+            # simplifies querying
+            adds = new
+
+        return adds, dels
+
+    def textfsm_data(self, raw_input, fsm_template, schema, data):
+        """Convert unstructured output to structured output"""
+
+        records = []
+        fsm_template.Reset()
+        res = fsm_template.ParseText(raw_input)
+
+        for entry in res:
+            metent = dict(zip(fsm_template.header, entry))
+            records.append(metent)
+
+        return records
+
+    async def post_results(self, result, token) -> None:
+        """The callback that nodes use to post the results back to the service"""
+        if self.result_queue:
+            self.result_queue.put_nowait((token, result))
         else:
-            return net.apply(lambda a: (
-                False if not a or a == '0.0.0.0/0'
-                else address in ip_network(a, strict=False))
-            )
-
-    def _check_ipvers(self,  addr: pd.Series, version: int) -> pd.Series:
-        """Check if the IP version of addresses in a Pandas dataframe
-        correspond to the given version
-
-        Args:
-            addr (PandasObject): the collection of ip addresses to check
-            version: (int): IP version (4 or 6)
-
-        Returns:
-            PandasObject: A collection of bool reporting the result
-        """
-
-        return addr.apply(lambda a: (self._get_ipvers(a) == version))
-
-    # pylint: disable=too-many-statements
-    def get_valid_df(self, **kwargs) -> pd.DataFrame:
-        """The heart of the engine: retrieving the data from the backing store
+            self.logger.error(f"No queue for service {self.name}")
 
-        Args:
-            kwargs: keyword args passed by caller, varies depending on table
-
-        Returns:
-            pd.DataFrame: The data as a pandas dataframe
+    def call_node_postcmd(self, postcall, nodename) -> None:
+        """Start data gathering by calling the post command list"""
+        if postcall and postcall['postq']:
+            token = RsltToken(int(time.time()*1000), nodename, 0, 0, self.name,
+                              self.period-5)
+            postcall['postq'](self.post_results, self.defn, token)
+
+    def clean_json_input(self, data):
+        """Clean the JSON input data that is sometimes messed up
+        Each service can implement its own version of the cleanup
+        """
+        return None
+
+    async def start_data_gather(self) -> None:
+        """Start data gathering by calling the post command list
+        This is only used to fire up the calls the first time. After this,
+        each node gets into a self-adapting curve of calling at least after
+        the duration specified for the service period. If nodes are slower,
+        they'll be scheduled to run after the specified service period after
+        their return. We could use this to track slow nodes.
         """
-        if not self.ctxt.engine:
-            print("Specify an analysis engine using set engine command")
-            return pd.DataFrame(columns=["namespace", "hostname"])
-
-        # Thanks to things like OSPF, we cannot use self.schema here
-        sch = self.schema
-        phy_table = sch.get_phy_table_for_table()
-
-        columns = kwargs.pop('columns', ['default'])
-        addnl_fields = kwargs.pop('addnl_fields', [])
-        view = kwargs.pop('view', self.iobj.view)
-        # active_only tells the db to get only the active records (discarding
-        # everything have been deleted).
-        # If view=all, by default, we would like to show all the records,
-        # included the ones that have been deleted, in all the other cases
-        # we want to see only the active records.
-        active_only = kwargs.pop('active_only', view != 'all')
-        hostname = kwargs.pop('hostname', [])
-        query_str = kwargs.pop('query_str', '')
-
-        fields = sch.get_display_fields(columns)
-        key_fields = sch.key_fields()
-
-        # Lets also get the fields required to satisfy user-specified filters
-        # We cannot use sets because we want to preserve the order of fields
-        filter_fields = [x for x in self.iobj.get_filter_fields
-                         if x not in addnl_fields]
-        user_query_cols = [x for x in self._get_user_query_cols(query_str)
-                           if x not in addnl_fields]
-        fields += [x for x in user_query_cols+filter_fields+addnl_fields
-                   if x not in fields]
-
-        aug_fields = sch.get_augmented_fields(fields)
-
-        self._add_active_to_fields(view, fields, addnl_fields)
-        # Order matters. Don't put this before the missing key fields insert
-        for f in aug_fields:
-            dep_fields = sch.get_parent_fields(f)
-            dep_fields = [x for x in dep_fields if x not in aug_fields and
-                          x not in fields]
-            fields += dep_fields
-            addnl_fields += dep_fields
-
-        # Remove augmented fields from being passed to DB read.
-        # Augmented fields are computed from other fields
-        fields = [x for x in fields if x not in aug_fields]
-
-        for fld in key_fields:
-            if fld not in fields+addnl_fields:
-                addnl_fields.insert(0, fld)
-
-        getcols = list(set(fields+addnl_fields+['timestamp']))
-
-        tz = self.ctxt.cfg.get('analyzer', {}).get('timezone', 'UTC')
-        settings = {'TIMEZONE': tz}
 
-        if self.iobj.start_time:
+        for node in self.node_postcall_list:
             try:
-                start_time = int(dateparser.parse(
-                    self.iobj.start_time.replace('last night', 'yesterday'),
-                    settings=settings)
-                    .timestamp()*1000)
-            except Exception:
-                # pylint disable=raise-missing-from
-                raise ValueError(
-                    f"unable to parse start-time: {self.iobj.start_time}")
-        else:
-            start_time = ''
-
-        if self.iobj.start_time and not start_time:
-            # Something went wrong with our parsing
-            # pylint disable=raise-missing-from
-            raise ValueError(
-                f"unable to parse start-time: {self.iobj.start_time}")
-
-        if self.iobj.end_time:
-            try:
-                end_time = int(dateparser.parse(
-                    self.iobj.end_time.replace('last night', 'yesterday'),
-                    settings=settings)
-                    .timestamp()*1000)
-            except Exception:
-                # pylint disable=raise-missing-from
-                raise ValueError(
-                    f"unable to parse end-time: {self.iobj.end_time}")
+                self.call_node_postcmd(self.node_postcall_list[node],
+                                       node),
+            except TimeoutError:
+                self.logger.warning(f"Node post failed for {node}")
+                continue
+
+    def _process_each_output(self, elem_num, data):
+        """Workhorse processing routine for each element in output"""
+
+        result = []
+        if (Service.is_status_ok(data.get('status', -1))):
+            if not data["data"]:
+                return result
+
+            # Check host-specific normalization if any
+            nfn = self.defn.get(data.get("hostname"), None)
+            if not nfn:
+                nfn = self.defn.get(data.get("devtype"), None)
+            if nfn:
+                # If we're riding on the coattails of another device
+                # get that device's normalization function
+                copynfn = nfn.get("copy", None)
+                if copynfn:
+                    nfn = self.defn.get(copynfn, {})
+                norm_str = nfn.get("normalize", None)
+                if norm_str is None and isinstance(nfn.get('command', None),
+                                                   list):
+                    # Can happen because we've a list of commands associated
+                    # Pick the normalization function associated with this
+                    # output
+                    norm_str = nfn.get('command', [])[elem_num].get(
+                        'normalize', None)
+                if norm_str:
+                    if isinstance(data["data"], str):
+                        try:
+                            in_info = json.loads(data["data"])
+                        except json.JSONDecodeError:
+                            in_info = self.clean_json_input(data)
+                            if not in_info:
+                                self.logger.error(
+                                    "Received non-JSON output where "
+                                    "JSON was expected for {} on "
+                                    "node {}, {}".format(
+                                        data["cmd"], data["hostname"],
+                                        data["data"]
+                                    )
+                                )
+                                return result
+                            try:
+                                in_info = json.loads(in_info)
+                            except json.JSONDecodeError:
+                                self.logger.error(
+                                    "Received non-JSON output where "
+                                    "JSON was expected for {} on "
+                                    "node {}, {}".format(
+                                        data["cmd"], data["hostname"],
+                                        data["data"]
+                                    )
+                                )
+                                return result
+                    else:
+                        in_info = data["data"]
+
+                    if in_info:
+                        # EOS' HTTP returns errors like this.
+                        if isinstance(in_info, dict):
+                            tmp = in_info.get('data', [])
+                            if tmp and tmp[0].get('errors', {}):
+                                return []
+
+                        result = cons_recs_from_json_template(
+                            norm_str, in_info)
+
+                else:
+                    tfsm_template = nfn.get("textfsm", None)
+
+                    if tfsm_template is None and elem_num:
+                        # Can happen because we've a list of cmds associated
+                        # Pick the normalization function associated with this
+                        # output
+                        tfsm_template = nfn.get('command', [])[elem_num].get(
+                            'textfsm', None)
+
+                    if not tfsm_template:
+                        return result
+
+                    in_info = []
+                    if isinstance(data['data'], dict):
+                        if "output" in data["data"]:
+                            in_info = data["data"]["output"]
+                        elif "messages" in data["data"]:
+                            # This is Arista's bash output format
+                            in_info = data["data"]["messages"][0]
+                    if not in_info:
+                        in_info = data["data"]
+                    # Clean data is invoked inside this due to the way we
+                    # munge the data and force the types to adhere to the
+                    # specified type
+                    result = self.textfsm_data(
+                        in_info, tfsm_template, self.schema, data
+                    )
+            else:
+                self.logger.error(
+                    "{}: No normalization/textfsm function for device {}"
+                    .format(self.name, data["hostname"]))
+
+        return result
+
+    def process_data(self, data):
+        """Derive the data to be stored from the raw input"""
+        result_list = []
+        for i, item in enumerate(data):
+            tmpres = self._process_each_output(i, item)
+            result_list.append(tmpres)
+
+        result = self.merge_results(result_list, data)
+        return self.clean_data(result, data)
+
+    def get_key_flds(self):
+        """Get the key fields associated with this service. 
+        Its a function because we want to override it.
+        """
+        return list(filter(lambda x: x not in ['namespace', 'hostname'],
+                           self.keys))
+
+    def merge_results(self, result_list, data):
+        int_res = {}
+        keyflds = self.get_key_flds()
+
+        for result in result_list:
+            for entry in result:
+                keyvals = []
+                for kfld in keyflds:
+                    if not entry.get(kfld, None):
+                        keyvals.append('_default')
+                    else:
+                        val = entry.get(kfld, '')
+                        if not isinstance(val, str):
+                            val = str(val)
+                        keyvals.append(val)
+
+                if entry.get('_entryType', ''):
+                    keyvals.append(entry['_entryType'])
+
+                key = '-'.join(keyvals)
+
+                if key not in int_res:
+                    int_res[key] = entry
+                else:
+                    existing = int_res[key]
+                    for fld in entry:
+                        if entry[fld] and not existing.get(fld, None):
+                            existing[fld] = entry[fld]
+                        elif entry[fld]:
+                            # cleanup routine specific to service can resolve
+                            existing[fld+"-_2nd"] = entry[fld]
+
+        final_res = list(int_res.values())
+
+        return(final_res)
+
+    def _get_devtype_from_input(self, input):
+        if isinstance(input, list):
+            return input[0].get('devtype', None)
         else:
-            end_time = ''
+            return input.get('devtype', None)
 
-        if self.iobj.end_time and not end_time:
-            # Something went wrong with our parsing
-            # pylint disable=raise-missing-from
-            raise ValueError(
-                f"unable to parse end-time: {self.iobj.end_time}")
-
-        table_df = self._dbeng.read(
-            phy_table,
-            'pandas',
-            start_time=start_time,
-            end_time=end_time,
-            columns=getcols,
-            view=view,
-            key_fields=key_fields,
-            **kwargs
-        )
-
-        if not table_df.empty:
-            # hostname may not have been filtered if using regex
-            if hostname:
-                table_df = self._filter_hostname(table_df, hostname)
-            if active_only:
-                table_df = table_df.query('active').reset_index(drop=True)
-
-            if 'timestamp' in table_df.columns and not table_df.empty:
-                table_df['timestamp'] = humanize_timestamp(
-                    table_df.timestamp, self.cfg.get('analyzer', {})
-                    .get('timezone', None))
-
-            if query_str:
-                table_df = self._handle_user_query_str(table_df, query_str)
-
-        return table_df.reset_index(drop=True)[fields]
-
-    def _filter_hostname(self, df: pd.DataFrame, hostname: List[str]) \
-            -> pd.DataFrame:
-        """filter dataframe with the input hostnames
-
-        Args:
-            hostname (List[str]): hostname used for filter df
-            df (pd.Dataframe): input dataframe
+    def clean_data(self, processed_data, raw_data):
+        """Massage the extracted data to match record specified by schema"""
 
-        Returns:
-            pd.DataFrame: filtered dataframe
-        """
-
-        if not hostname or df.empty:
-            return df
-
-        hostname_filter = build_query_str(
-            [], self.schema, False, hostname=hostname)
-
-        res_df = df.query(hostname_filter)
-
-        return res_df
-
-    def get(self, **kwargs) -> pd.DataFrame:
-        """The default get method for all tables
-
-        Use this for a table if nothing special is desired. No table uses
-        this routine today.
-
-        Raises:
-            NotImplementedError: If no table has been defined
-
-        Returns:
-            pd.DataFrame: pandas dataframe of the object
-        """
-        if not self.iobj.table:
-            raise NotImplementedError
+        dev_clean_fn = self.dev_clean_fn.get(self._get_devtype_from_input(
+            raw_data), None)
+        if dev_clean_fn:
+            processed_data = dev_clean_fn(processed_data, raw_data)
+
+        return self.clean_data_common(processed_data, raw_data)
+
+    def clean_data_common(self, processed_data, raw_data):
+        """Fix the type and default value of of each extracted field
+
+        This routine is common to all services. It ensures that all the missing
+        fields, as defined by the schema, are added to the records extracted.
+        Furthermore, each field is set to the specified type.
+        """
+
+        # Build default data structure
+        schema_rec = {}
+        def_vals = self._get_default_vals()
+
+        ptype_map = {
+            pa.string(): str,
+            pa.int32(): int,
+            pa.int64(): int,
+            pa.float32(): float,
+            pa.float64(): float,
+            pa.date64(): float,
+            pa.list_(pa.string()): list,
+            pa.list_(pa.int64()): list,
+            pa.bool_(): bool,
+        }
+
+        for field in self.schema:
+            default = def_vals[field.type]
+            schema_rec.update({field.name: default})
 
-        df = self.get_valid_df(**kwargs)
-
-        return df
-
-    def get_table_info(self, **kwargs) -> dict:
-        """Returns information about the data available for a table
-
-        Used by table show command exclusively.
-        Args:
-            kwargs: keyword args passed by caller, varies depending on table
-
-        Returns:
-            dict: The desired data as a dictionary
-        """
-        # You can't use view from user because we need to see all the data
-        # to compute data required.
-        kwargs.pop('view', None)
-
-        all_time_df = self.get_valid_df(view='all', **kwargs)
-        times = all_time_df['timestamp'].unique()
-        ret = {'firstTime': all_time_df.timestamp.min(),
-               'lastTime': all_time_df.timestamp.max(),
-               'intervals': len(times),
-               'allRows': len(all_time_df),
-               'namespaceCnt': all_time_df.get('namespace',
-                                               pd.Series(dtype='category'))
-               .nunique(),
-               'deviceCnt': all_time_df.get('hostname',
-                                            pd.Series(dtype='category'))
-               .nunique(),
-               }
-        return ret
-
-    def summarize(self, **kwargs):
-        """Summarize the info about this resource/service.
-
-        There is a pattern of how to do these
-        use self._init_summarize():
-           - creates self.summary_df, which is the initial pandas dataframe
-             based on the table
-           - creates self.nsgrp of data grouped by namespace
-           - self.ns is the dict to add data to which will be turned into a
-             dataframe and then returned
-
-        if you want to simply take a field and run a pandas functon, then use
-          self._add_field_to_summary
-
-        at the end of te summarize
-        return pd.DataFrame(self.ns).convert_dtypes()
-
-        If you don't override this, then you get a default summary of all
-        columns
-        """
-        self._init_summarize(**kwargs)
-        if self.summary_df.empty:
-            return self.summary_df
-
-        self._gen_summarize_data()
-        self._post_summarize()
-        return self.ns_df.convert_dtypes()
-
-    def unique(self, **kwargs) -> pd.DataFrame:
-        """Return the unique elements as per user specification
-
-        Raises:
-            ValueError: If len(columns) != 1
-
-        Returns:
-            pd.DataFrame: Pandas dataframe of unique values for given column
-        """
-        count = kwargs.pop("count", 'False') == 'True'
-        query_str = kwargs.pop('query_str', '')
-        get_query_str = kwargs.pop('get_query_str', '')
-
-        columns = kwargs.pop("columns", None)
-
-        column = columns[0]
-
-        df = self.get(columns=columns, query_str=get_query_str, **kwargs)
-        if df.empty:
-            return df
-
-        # check if column we're looking at is a list, and if so explode it
-        if df[column].apply(
-                lambda x: isinstance(x, (list, np.ndarray))).any():
-            df = df.explode(column).dropna(how='any')
-
-        if count:
-            r = df[column].value_counts()
-            df = pd.DataFrame({column: r}) \
-                .reset_index() \
-                .rename(columns={column: 'numRows',
-                                 'index': column}) \
-                   .sort_values(column)
+        if isinstance(raw_data, list):
+            read_from = raw_data[0]
         else:
-            df = pd.DataFrame({f'{column}': df[column].unique()})
-
-        if query_str:
-            df = self._handle_user_query_str(df, query_str)
-
-        return df
-
-    def aver(self, **kwargs):
-        '''Assert'''
-        raise NotImplementedError
-
-    def top(self, **kwargs):
-        """Default implementation of top.
-        The basic fields this assumes are present include the "what" keyword
-        which contains the name of the field we're getting the transitions on,
-        the "n" field which tells the count of the top entries you're
-        looking for, and the reverse field which tells whether you're looking
-        for the largest (default, and so reverse is False) or the smallest(
-        reverse is True). This invokes the default object's get routine. It
-        is upto the caller to ensure that the desired column is in the output.
-        """
-        what = kwargs.pop("what", None)
-        reverse = kwargs.pop("reverse", False)
-        sqTopCount = kwargs.pop("count", 5)
-        columns = kwargs.pop("columns", ['default'])
-
-        if not what:
-            return pd.DataFrame()
-
-        fields = self.schema.get_display_fields(columns)
-        if columns == ['default'] and what not in fields:
-            fields.insert(-1, what)
-
-        getcols = list(set(fields + self.schema.key_fields() + [what]))
-
-        df = self.get(columns=getcols, **kwargs)
-        if 'error' in df.columns or df.empty:
-            return df
-
-        columns_by = [x for x in [what] + self.schema.key_fields()
-                      if x in df.columns]
-
-        return df.sort_values(by=columns_by, ascending=reverse) \
-                 .head(sqTopCount)[fields]
-
-    def lpm(self, **kwargs):
-        '''Default implementation to return not supported'''
-        return pd.Dataframe(
-            {'error': [f'Unsupported verb "lpm" for {self.iobj.table}']})
-
-    def find(self, **kwargs):
-        '''Default implementation to return not supported'''
-        return pd.Dataframe(
-            {'error': [f'Unsupported verb "find" for {self.iobj.table}']})
-
-    def _get_table_sqobj(self, table: str, start_time: str = None,
-                         end_time: str = None, view=None):
-        """Normalize pulling data from other tables into this one function
-
-        Typically pulling data involves calling get_sqobject with a bunch of
-        parameters that need to be passed to it, that a caller can forget to
-        pass. A classic example is passing the view, start-time and end-time
-        which is often forgotten. This function fixes this issue.
-
-        Args:
-            table (str): The table to retrieve the info from
-            verb (str): The verb to use in the get_sqobject call
-        """
+            read_from = raw_data
+        for entry in processed_data:
+            entry.update({"hostname": read_from["hostname"]})
+            entry.update({"namespace": read_from["namespace"]})
+            entry.update({"timestamp": read_from["timestamp"]})
+            entry.update({"sqvers": self.version})
+            for fld in schema_rec:
+                if fld not in entry:
+                    if fld == "active":
+                        entry.update({fld: True})
+                    else:
+                        entry.update({fld: schema_rec[fld]})
+                else:
+                    fld_type = self.schema.field(fld).type
+                    if not isinstance(entry[fld], ptype_map[fld_type]):
+                        try:
+                            entry[fld] = ptype_map[fld_type](entry[fld])
+                        except (ValueError, TypeError):
+                            entry[fld] = schema_rec[fld]
+                    elif isinstance(entry[fld], list):
+                        for i, ele in enumerate(entry[fld]):
+                            if not isinstance(ele,
+                                              ptype_map[fld_type.value_type]):
+                                try:
+                                    if ptype_map[fld_type.value_type] == int:
+                                        entry[fld][i] = int(entry[fld][i])
+                                    elif ptype_map[fld_type.value_type] == str:
+                                        entry[fld][i] = str(entry[fld][i])
+                                    else:
+                                        raise ValueError
+                                except (ValueError, TypeError):
+                                    entry[fld][i] = schema_rec[fld]
+        return processed_data
+
+    async def commit_data(self, result, namespace, hostname):
+        """Write the result data out"""
+        records = []
+        prev_res = self.previous_results.get(hostname, [])
+
+        if result or prev_res:
+            adds, dels = self.get_diff(prev_res, result)
+            if adds or dels:
+                self.previous_results[hostname] = copy.deepcopy(result)
+                for entry in adds:
+                    records.append(entry)
+                for entry in dels:
+                    if entry.get("active", True):
+                        # If there's already an entry marked as deleted
+                        # No point in adding one more
+                        entry.update({"active": False})
+                        entry.update(
+                            {"timestamp":
+                             int(datetime.utcnow().timestamp() * 1000)}
+                        )
+                        records.append(entry)
+
+                self._post_work_to_writer(records)
+
+    def _post_work_to_writer(self, records: dict):
+        """This posts the data to be written to the worker queue"""
+        if records:
+            self.writer_queue.put_nowait(
+                {
+                    "records": records,
+                    "topic": self.name,
+                    "schema": self.schema,
+                    "partition_cols": self.partition_cols
+                }
+            )
 
-        if start_time is None:
-            start_time = self.iobj.start_time
-        if end_time is None:
-            end_time = self.iobj.end_time
-        if view is None:
-            view = self.iobj.view
-        return get_sqobject(table)(engine_name=self.iobj.engine.name,
-                                   context=self.ctxt, view=view,
-                                   start_time=start_time, end_time=end_time)
+    def compute_basic_stats(self, statsList, newval: int) -> None:
+        """Compute min/max/avg for given stats with the new value
 
-    def _init_summarize(self, **kwargs) -> None:
-        """Initialize the data structures for use with generating summary
+        :param statsList: list consisting of 3 values in order: min, max, avg
+        :type statsList: list_
 
+        :param newval: The newval to update the list with
+        :type newval: int
         """
-        kwargs.pop('columns', None)
-        columns = ['*']
-
-        df = self.get(columns=columns, **kwargs)
-        if 'error' in df.columns:
-            self.summary_df = df
+        if not statsList:
+            statsList = [newval, newval, newval]
             return
 
-        self.summary_df = df
-        if df.empty:
-            return
+        if newval < statsList[0]:
+            statsList[0] = newval
+        if newval > statsList[1]:
+            statsList[1] = newval
+        statsList[2] = (statsList[2]+newval)/2
+
+    def update_stats(self, stats: ServiceStats, gather_time: int,
+                     total_time: int, qsize: int, wrQsize: int,
+                     nodeQsize: int) -> bool:
+        """Update per-node stats"""
+        write_stat = False
+        now = int(time.time()*1000)
+
+        self.compute_basic_stats(stats.total_time, total_time)
+        self.compute_basic_stats(stats.gather_time, gather_time)
+        self.compute_basic_stats(stats.svcQsize, qsize)
+        self.compute_basic_stats(stats.wrQsize, wrQsize)
+        self.compute_basic_stats(stats.nodeQsize, nodeQsize)
+
+        if total_time > self.period*1000:
+            stats.time_excd_count += 1
+            write_stat = True
+
+        if now > stats.next_update_time:
+            stats.next_update_time = now + 5*60*1000  # 5 mins
+            write_stat = True
+
+        return write_stat
+
+    async def run(self):
+        """Start the service"""
+        self.logger.info(f"running service {self.name} ")
 
-        self.ns = {i: {} for i in df['namespace'].unique()}
-        self.nsgrp = df.groupby(by=["namespace"], observed=True)
-
-    def _gen_summarize_data(self):
-        """Generate the data required for summary"""
-
-        if not self._summarize_on_add_field:
-            # Add the only field we truly know to add
-            self._summarize_on_add_field = [
-                ('deviceCnt', 'hostname', 'nunique'),
-            ]
-        for field_name, col, function in self._summarize_on_add_field:
-            if col not in ['namespace', 'timestamp']:
-                self._add_field_to_summary(col, function, field_name)
-                self.summary_row_order.append(field_name)
-
-        for flds in self._summarize_on_add_with_query:
-            field_name = flds[0]
-            query_str = flds[1]
-            field = flds[2]
-            if len(flds) == 4:
-                func = flds[3]
-            else:
-                func = 'count'
-            fld_df = self.summary_df.query(query_str)
-            if not fld_df.empty:
-                fld_per_ns = fld_df.groupby(by=['namespace'],
-                                            observed=True)[field] \
-                    .agg(func)
-                for i in self.ns.keys():
-                    self.ns[i].update({field_name: fld_per_ns.get(i, 0)})
-            else:
-                for i in self.ns.keys():
-                    self.ns[i].update({field_name: 0})
-
-            self.summary_row_order.append(field_name)
-
-        for field_name, field in self._summarize_on_add_list_or_count:
-            self._add_list_or_count_to_summary(field, field_name)
-            self.summary_row_order.append(field_name)
-
-        for field_name, query_str, field in self._summarize_on_add_stat:
-            if query_str:
-                statfld = self.summary_df.query(query_str) \
-                    .groupby(by=['namespace'],
-                             observed=True)[field]
-            else:
-                statfld = self.summary_df.groupby(
-                    by=['namespace'], observed=True)[field]
-
-            self._add_stats_to_summary(statfld, field_name)
-            self.summary_row_order.append(field_name)
-
-        for field_name, query_str, field, func in \
-                self._summarize_on_perdevice_stat:
-            if query_str:
-                statfld = self.summary_df \
-                    .query(query_str) \
-                    .groupby(by=['namespace', 'hostname'],
-                             observed=True)[field].agg(func)
-            else:
-                statfld = self.summary_df \
-                    .groupby(by=['namespace', 'hostname'],
-                             observed=True)[field].agg(func)
-
-            self._add_stats_to_summary(statfld, field_name, filter_by_ns=True)
-            self.summary_row_order.append(field_name)
-
-    def _post_summarize(self, check_empty_col: str = 'deviceCnt') -> None:
-        """Once summary data has been generated, finalize summary dataframe
-
-        Args:
-            check_empty_col (str, optional): column name to check to remove
-                                             namespace that's empty.
-                                             Defaults to 'deviceCnt'.
-        """
-        # this is needed in the case that there is a namespace that has no
-        # data for this command
-
-        if not check_empty_col:
-            check_empty_col = self._check_empty_col
-
-        delete_keys = []
-        for ns in self.ns:
-            if self.ns[ns][check_empty_col] == 0:
-                delete_keys.append(ns)
-        for ns in delete_keys:
-            del (self.ns[ns])
-
-        ns_df = pd.DataFrame(self.ns)
-        if len(self.summary_row_order) > 0:
-            ns_df = ns_df.reindex(self.summary_row_order, axis=0)
-        self.ns_df = ns_df
-
-    def _add_constant_to_summary(self, field: str, value):
-        """And a constant value to specified field name in summary"""
-        if field:
-            # pylint disable=expression-not-assigned
-            _ = {self.ns[i].update({field: value}) for i in self.ns.keys()}
-
-    def _add_field_to_summary(self, field: str, method: str = 'nunique',
-                              field_name: str = None):
-        """Add a summary field to summary dataframe based on method on field
-
-        This assumes that self.summary_df has been populated.
-        Args:
-            field (str): Column name to add in the summary dataframe
-            method (str, optional): pandas method name. Defaults to 'nunique'.
-            field_name (str, optional): column to compute on. Defaults to None.
-        """
-        if not field_name:
-            field_name = field
-        field_per_ns = getattr(self.nsgrp[field], method)()
-        _ = {self.ns[i].update({field_name: field_per_ns.get(i, 0)})
-             for i in self.ns.keys()}
-
-    def _add_list_or_count_to_summary(self, field: str,
-                                      field_name: str = None) -> None:
-        """add as a list if < 3 things, otherwise return the count"""
-        if not field_name:
-            field_name = field
-
-        for n in self.ns.keys():
-            unique_for_ns = self.nsgrp.get_group(n)[field].value_counts()
-            value = unique_for_ns.to_dict()
-            # Filter numm entries if category because of how pandas
-            # behaves here
-            if self.nsgrp[field].dtype[n].name == 'category':
-                value = dict(filter(lambda x: x[1] != 0, value.items()))
-
-            self.ns[n].update({field_name: value})
-
-    def _add_stats_to_summary(self, groupedby: DataFrameGroupBy,
-                              fieldname: str,
-                              filter_by_ns: bool = False) -> None:
-        """Takes grouped stats and adds min, max, and median to stats"""
-
-        _ = {self.ns[i].update({fieldname: []}) for i in self.ns.keys()}
-        if filter_by_ns:
-            _ = {self.ns[i][fieldname].append(groupedby[i].min())
-                 if i in groupedby else self.ns[i][fieldname].append(0)
-                 for i in self.ns.keys()}
-            # pylint disable=expression-not-assigned
-            _ = {self.ns[i][fieldname].append(groupedby[i].max())
-                 if i in groupedby else self.ns[i][fieldname].append(0)
-                 for i in self.ns.keys()}
-            # pylint disable=expression-not-assigned
-            _ = {self.ns[i][fieldname].append(
-                groupedby[i].median(numeric_only=False))
-                if i in groupedby else self.ns[i][fieldname].append(0)
-                for i in self.ns.keys()}
+        if self.run_once:
+            total_nodes = len(self.node_postcall_list)
         else:
-            min_field = groupedby.min()
-            max_field = groupedby.max()
-            med_field = groupedby.median(numeric_only=False)
-
-            _ = {self.ns[i][fieldname].append(min_field[i])
-                 if i in min_field else self.ns[i][fieldname].append(0)
-                 for i in self.ns.keys()}
-            _ = {self.ns[i][fieldname].append(max_field[i])
-                 if i in max_field else self.ns[i][fieldname].append(0)
-                 for i in self.ns.keys()}
-            _ = {self.ns[i][fieldname].append(med_field[i])
-                 if i in med_field else self.ns[i][fieldname].append(0)
-                 for i in self.ns.keys()}
-
-    def _get_user_query_cols(self, query_str: str) -> List[str]:
-        """Returns the list of fields inside the query_str
-
-        Args:
-            query_str (str): query string
-            table (str): table from which get the fields
-
-        Returns:
-            List[str]: list of fields inside the query string
-        """
-        if query_str:
-            table_fields = self.schema.fields
-            return [f for f in table_fields if re.search(rf'\b{f}\b',
-                                                         query_str)]
-        return []
-
-    def _add_active_to_fields(self, view: str, fields: List[str],
-                              addnl_fields: List[str]) -> None:
-        """Add 'active' field to returned cols
-
-        Depending on the user specification, if we have to return all
-        records within a time window or if view=all, we must also
-        return the active field because it marks if the record was
-        added or deleted
-
-        Args:
-            view(str): value of view specified by user
-            fields(List[str]): the columns to be returned so far
-            addnl_fields(List[str]): the addnl fields to be retrieved so far
-
-        Returns:
-            None
-        """
-
-        if view == "all" or (self.iobj.start_time and self.iobj.end_time):
-            if 'active' not in fields:
-                fields.insert(0, 'active')
-        elif addnl_fields is not None:
-            addnl_fields.append('active')
+            total_nodes = 0
+        # Fire up the initial posts
+        await self.start_data_gather()
+        loop = asyncio.get_running_loop()
+        pernode_stats = defaultdict(lambda: ServiceStats())
+
+        while True:
+            token, output = await self.result_queue.get()
+            if self.sigend:
+                self.logger.warning(
+                    f'Service: {self.name}: Received signal to terminate')
+                return
+            qsize = self.result_queue.qsize()
+
+            self.logger.debug(f"Extracted response for {self.name} service")
+            if isinstance(token, list):
+                token = token[0]
+            gather_time = int(time.time()*1000) - token.start_time
+
+            status = HTTPStatus.NO_CONTENT        # Empty content
+            write_poller_stat = False
+
+            if output:
+                ostatus = [x.get('status', -1) for x in output]
+
+                write_poller_stat = not all([Service.is_status_ok(x)
+                                             for x in ostatus])
+                status = ostatus[0]
+
+                # We don't expect the output from two different hostnames
+                nodename = output[0]["hostname"]
+                self.logger.debug(f"Extracted response from {nodename} for "
+                                  f"{self.name} service")
+                # We can terminate processing if we've no data returned
+                # and we're reading inputs from a file
+                if nodename == '_filedata' and status == HTTPStatus.NO_CONTENT:
+                    return
+                # Don't write the error every time the failure happens
+                if write_poller_stat:
+                    if nodename in self._failed_node_set:
+                        write_poller_stat = False
+                    else:
+                        self._failed_node_set.add(nodename)
+                elif nodename in self._failed_node_set:
+                    # So there was no error in this command that had failed b4
+                    self._failed_node_set.remove(nodename)
+
+                # Process data independent of status to return an empty list
+                # so that the output can be updated. For example, if a service
+                #  is disabled, this can be the condition.
+                if self.run_once == "gather":
+                    if self.is_status_ok(status):
+                        self._post_work_to_writer(json.dumps(output, indent=4))
+                    total_nodes -= 1
+                    if total_nodes <= 0:
+                        self.logger.warning(
+                            f'Service: {self.name}: Finished gathering data')
+                        return
+                    continue
+
+                try:
+                    result = self.process_data(output)
+                except Exception:
+                    self.logger.exception(
+                        f'Processing data failed for service '
+                        f'{self.name} on node {nodename}')
+                    result = []
+                # If a node from init state to good state, hostname will change
+                # So fix that in the node list
+                hostname = output[0]["hostname"]
+                if self.run_once == "process":
+                    if self.is_status_ok(status):
+                        self._post_work_to_writer(json.dumps(result, indent=4))
+                    total_nodes -= 1
+                    if total_nodes <= 0:
+                        return
+                    continue
+
+                if token.bootupTimestamp != self.node_boot_times[hostname]:
+                    self.node_boot_times[hostname] = token.bootupTimestamp
+                    # Flush the prev results data for this node
+                    self.previous_results[hostname] = []
+                await self.commit_data(result, output[0]["namespace"],
+                                       hostname)
+                empty_count = False
+            else:
+                if self.run_once == "gather" or self.run_once == "process":
+                    total_nodes -= 1
+                    if total_nodes <= 0:
+                        self.logger.warning(
+                            f'Service: {self.name}: Finished gathering data')
+                        return
+                    continue
+                empty_count = True
+
+            total_time = int(time.time()*1000) - token.start_time
+
+            if not empty_count:
+                statskey = output[0]["namespace"] + '/' + output[0]["hostname"]
+                write_poller_stat = (write_poller_stat or
+                                     self.update_stats(
+                                         pernode_stats[statskey], total_time,
+                                         gather_time, qsize,
+                                         self.writer_queue.qsize(),
+                                         token.nodeQsize))
+                stats = pernode_stats[statskey]
+                poller_stat = [
+                    {"hostname": output[0]["hostname"],
+                     "sqvers": self.version,
+                     "namespace": output[0]["namespace"],
+                     "active": True,
+                     "service": self.name,
+                     "status": status,
+                     "svcQsize": stats.svcQsize,
+                     "wrQsize": stats.wrQsize,
+                     "nodeQsize": stats.nodeQsize,
+                     "pollExcdPeriodCount": stats.time_excd_count,
+                     "gatherTime": stats.gather_time,
+                     "totalTime": stats.total_time,
+                     "timestamp": int(datetime.utcnow().timestamp() * 1000)}]
+
+            if write_poller_stat:
+                self.writer_queue.put_nowait(
+                    {
+                        "records": poller_stat,
+                        "topic": "sqPoller",
+                        "schema": self.poller_schema,
+                        "partition_cols": self.partition_cols
+                    })
+
+            # Post a cmd to fire up the next poll after the specified period
+            self.logger.debug(
+                f"Rescheduling service for {self.name} service")
+            loop.call_later(self.period, self.call_node_postcmd,
+                            self.node_postcall_list.get(token.nodename),
+                            token.nodename)
```

### Comparing `suzieq-0.22.0rc1/suzieq/engines/pandas/path.py` & `suzieq-0.8.0/suzieq/engines/pandas/path.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,225 +1,114 @@
-from typing import Optional, List, Any, Iterable
 from ipaddress import ip_network, ip_address
 from collections import OrderedDict
 from itertools import repeat
 from functools import lru_cache
-from collections import defaultdict
-from copy import copy
 
 import numpy as np
 import pandas as pd
 
-from suzieq.shared.exceptions import EmptyDataframeError
-from suzieq.engines.pandas.engineobj import SqPandasEngine
-from suzieq.shared.utils import expand_nxos_ifname, MAX_MTU
-
-# TODO: What timestamp to use (arpND, mac, interface, route..)
+from suzieq.sqobjects import interfaces, routes, arpnd, macs, basicobj
+from suzieq.exceptions import EmptyDataframeError, PathLoopError
+from suzieq.engines.pandas.engineobj import SqEngineObject
 
 
-class PathObj(SqPandasEngine):
-    '''Backend class to handle manipulating virtual table, path, with pandas'''
-
-    @staticmethod
-    def table_name() -> str:
-        '''Table name'''
-        return 'path'
+# TODO: What timestamp to use (arpND, mac, interface, route..)
+class PathObj(SqEngineObject):
 
-    # pylint: disable=too-many-statements, attribute-defined-outside-init
-    def _init_dfs(self, ns, source, dest):
+    def _init_dfs(self, namespace, source, dest):
         """Initialize the dataframes used in this path hunt"""
 
         self.source = source
         self.dest = dest
-        # Recursive route handling, handle 2 levels of recursion only
-        # Why? Just to stop infinite recursion in case of a bug
-        self.max_rr_recursion = 2
-
         self._underlay_dfs = {}  # lpm entries for each vtep IP
-        self._srcnode_via_arp = False
 
-        namespace = [ns]
         try:
-            self._if_df = self._get_table_sqobj('interfaces') \
-                .get(namespace=namespace, state='up',
-                     columns=['namespace', 'hostname', 'ifname', 'mtu', 'type',
-                              'ipAddressList', 'ip6AddressList', 'state',
-                              'vlan', 'master', 'macaddr', 'timestamp',
-                              'portmode']) \
-                .explode('ipAddressList') \
-                .fillna({'ipAddressList': ''}) \
-                .explode('ip6AddressList') \
-                .fillna({'ip6AddressList': ''}) \
-                .reset_index(drop=True)
+            self._if_df = interfaces.IfObj(context=self.ctxt) \
+                                    .get(namespace=namespace,
+                                         addnl_fields=['macaddr']) \
+                                    .explode('ipAddressList') \
+                                    .fillna({'ipAddressList': ''}) \
+                                    .explode('ip6AddressList') \
+                                    .fillna({'ip6AddressList': ''}) \
+                                    .reset_index(drop=True)
             if self._if_df.empty:
                 raise EmptyDataframeError
         except (EmptyDataframeError, KeyError):
             raise EmptyDataframeError(
                 f"No interface information found for {namespace}")
 
-        # Need this in determining L2 peer
-        mlag_df = self._get_table_sqobj('mlag').get(namespace=namespace)
-        mlag_peers = defaultdict(str)
-        mlag_peerlink = defaultdict(str)
-        if not mlag_df.empty:
-            peerlist = [x.tolist()
-                        for x in mlag_df.groupby(by=['systemId'])['hostname']
-                        .unique().tolist()]
-            for peers in peerlist:
-                if len(peers) > 1:
-                    mlag_peers[peers[0]] = peers[1]
-                    mlag_peers[peers[1]] = peers[0]
-            for row in mlag_df.itertuples():
-                mlag_peerlink[row.hostname] = expand_nxos_ifname(row.peerLink)
-        self._mlag_peers = mlag_peers
-        self._mlag_peerlink = mlag_peerlink
-
         try:
-            # access-internal is an internal Junos route we want to
-            # ignore
-            self._rdf = self._get_table_sqobj('routes') \
-                .lpm(namespace=namespace, address=dest) \
-                .query('protocol != "access-internal"') \
-                .reset_index(drop=True)
+            self._rdf = routes.RoutesObj(context=self.ctxt) \
+                              .lpm(namespace=namespace, address=dest) \
+                              .reset_index(drop=True)
             if self._rdf.empty:
                 raise EmptyDataframeError
         except (KeyError, EmptyDataframeError):
             raise EmptyDataframeError("No Routes information found for {}".
                                       format(dest))
 
-        try:
-            self._rpf_df = self._get_table_sqobj('routes') \
-                .lpm(namespace=namespace, address=source) \
-                .query('protocol != "access-internal"') \
-                .reset_index(drop=True)
-            if self._rpf_df.empty:
-                raise EmptyDataframeError
-        except (KeyError, EmptyDataframeError):
-            raise EmptyDataframeError("No Routes information found for {}".
-                                      format(source))
-
         # We ignore the lack of ARPND for now
-        self._arpnd_df = self._get_table_sqobj('arpnd') \
-            .get(namespace=namespace)
+        self._arpnd_df = arpnd.ArpndObj(
+            context=self.ctxt).get(namespace=namespace)
         if self._arpnd_df.empty:
             raise EmptyDataframeError(
                 f"No ARPND information found for {dest}")
 
         # Enhance the ARPND table with the VRF field
         self._arpnd_df = self._arpnd_df.merge(
             self._if_df[['namespace', 'hostname', 'ifname', 'master']],
             left_on=['namespace', 'hostname', 'oif'],
             right_on=['namespace', 'hostname', 'ifname'], how='left') \
             .drop(columns=['ifname']) \
             .rename(columns={'master': 'vrf'}) \
             .replace({'vrf': {'': 'default'}}) \
             .query('state != "failed"') \
-            .drop_duplicates(subset=['namespace', 'hostname', 'ipAddress',
-                                     'oif']) \
             .reset_index(drop=True)
 
-        self._macsobj = self._get_table_sqobj('macs')
+        self._macsobj = macs.MacsObj(context=self.ctxt, namespace=namespace)
 
         if ':' in source:
             self._src_df = self._if_df[self._if_df.ip6AddressList.astype(str)
-                                       .str.startswith(source + "/")]
+                                       .str.contains(source + "/")]
         else:
             self._src_df = self._if_df[self._if_df.ipAddressList.astype(str)
-                                       .str.startswith(source + "/")]
+                                       .str.contains(source + "/")]
 
         if self._src_df.empty:
             # TODO: No host with this src addr. Is addr a local ARP entry?
-            self._src_df = self._find_fhr_df(None, source)
-
-            # We use check_arp to identify whether we look up the source's
-            # interface table to identify its IP address and subnet to
-            # determine if the destination is in the same subnet or not.
-            # We cannot just use the ARP table in this case because the ARP
-            # table may not have been populated yet.
-            self._srcnode_via_arp = True
+            self._src_df = self._find_fhr_df(source)
 
         if self._src_df.empty:
-            # See if we can find an mlag pair of devices that contains the SVI
-            # pandas has a bug that prevents us from using startswith with a
-            # tuple such as ("Vlan", "vlan", "irb.") directly instead of using
-            # the @svi_names trick
-            # pylint: disable=unused-variable
-            svi_names = tuple(["Vlan", "vlan", "irb."])  # noqa: F841
-            if ':' in source:
-                self._src_df = (
-                    self._if_df.query(
-                        f'@self._in_subnet_series("{source}", ip6AddressList)'
-                        ' and ifname.str.startswith(@svi_names)')
-                )
-            else:
-                self._src_df = (
-                    self._if_df.query(
-                        f'@self._in_subnet_series("{source}", ipAddressList)'
-                        ' and ifname.str.startswith(@svi_names)')
-                )
-            if not self._src_df.empty:
-                hosts = self._src_df.hostname.unique().tolist()
-                if len(hosts) > 2:
-                    raise ValueError(
-                        'source not in ARP and SVI on too many hosts')
-                self._srcnode_via_arp = True
-
-        if self._src_df.empty:
-            raise AttributeError(f"Unable to find starting node for {source}")
-
-        src_hostname = self._src_df.hostname.unique().tolist()[0]
-
-        if self._src_df.hostname.nunique() == 1 and len(self._src_df) > 1:
-            # Multiple interfaces with the same IP address. Possible case
-            # of Unnumbered interfaces. See if there's a loopback in there
-            if 'loopback' in self._src_df.type.unique().tolist():
-                self._src_df = self._src_df.query('type == "loopback"')
+            raise AttributeError(f"Invalid src {source}")
 
         if ':' in dest:
             self._dest_df = self._if_df[self._if_df.ip6AddressList.astype(str)
-                                        .str.startswith(dest + "/")]
+                                        .str.contains(dest + "/")]
         else:
             self._dest_df = self._if_df[self._if_df.ipAddressList.astype(str)
-                                        .str.startswith(dest + "/")]
+                                        .str.contains(dest + "/")]
 
-        if self._dest_df.empty:
-            # Check if addr is in any switch's local ARP
-            self._dest_df = self._find_fhr_df(None, dest)
-
-        if self._srcnode_via_arp:
-            # If the dest is in the source host's ARP table, its L2
-            if not self._arpnd_df.query(f'namespace=="{namespace}" and '
-                                        f'hostname=="{src_hostname}" and '
-                                        f'ipAddress=="{self.dest}"').empty:
-                self.is_l2 = True
-            else:
-                self.is_l2 = False
+        srcnet = self._src_df.ipAddressList.tolist()[0]
+        if ip_address(dest) in ip_network(srcnet, strict=False):
+            self.is_l2 = True
         else:
-            srcnet = self._src_df.ipAddressList.tolist()[0]
-            if ip_address(dest) in ip_network(srcnet, strict=False):
-                self.is_l2 = True
-            else:
-                self.is_l2 = False
+            self.is_l2 = False
 
-        if not self._dest_df.empty:
-            if (self._dest_df.hostname.nunique() == 1 and
-                    len(self._dest_df) > 1):
-                # Multiple interfaces with the same IP address. Possible case
-                # of Unnumbered interfaces. See if there's a loopback in there
-                if 'loopback' in self._dest_df.type.unique().tolist():
-                    self._dest_df = self._dest_df.query('type == "loopback"')
+        if self._dest_df.empty:
+            # TODO: No host with this dest addr. Is addr a local ARP entry?
+            self._dest_df = self._find_fhr_df(dest)
 
-            self.dest_device = self._dest_df["hostname"].unique()
-        else:
-            self.dest_device = []
+        if self._dest_df.empty:
+            raise AttributeError(f"Invalid dest {dest}")
 
+        self.dest_device = self._dest_df["hostname"].unique()
         self.src_device = self._src_df["hostname"].unique()
 
         # Start with the source host and find its route to the destination
-        if self._rdf.query(f"hostname.isin({self.src_device.tolist()})").empty:
+        if self._rdf[self._rdf["hostname"].isin(self.src_device)].empty:
             raise EmptyDataframeError(f"No routes found for {self.src_device}")
 
     def _get_vrf(self, hostname: str, ifname: str, addr: str) -> str:
         """Determine the VRF given either the ifname or ipaddr"""
         vrf = ''
         if addr and ':' in addr:
             ipvers = 6
@@ -247,16 +136,15 @@
                     f'ip6AddressList.str.startswith("{addr}")')
             elif addr and ipvers == 4:
                 iifdf = self._if_df.query(
                     f'hostname=="{hostname}" and '
                     f'ipAddressList.str.startswith("{addr}")')
             else:
                 # No address, but a bridge interface as the master
-                if (iifdf.iloc[0]['vlan'] and
-                   iifdf.iloc[0]['portmode'] != 'trunk'):
+                if iifdf.iloc[0]['vlan']:
                     # Check if there's an SVI, assuming format is vlan*
                     # TODO: Handle trunk
                     vlan = iifdf.iloc[0]['vlan']
                     vdf = self._if_df.query(f'hostname=="{hostname}" and '
                                             f'(ifname=="vlan{vlan}" or '
                                             f'ifname=="Vlan{vlan}")')
                     if not vdf.empty:
@@ -265,16 +153,16 @@
         if not iifdf.empty and not vrf:
             vrf = iifdf.iloc[0].master.strip()
             if vrf == "bridge":
                 vrf = ''
 
         return vrf
 
-    def _find_fhr_df(self, device: Optional[str], ip: str) -> pd.DataFrame:
-        """Find Firstt Hop Router's iface DF for a given IP and device.
+    def _find_fhr_df(self, ip: str) -> pd.DataFrame:
+        """Find Firstt Hop Router's iface DF for a given IP.
         The logic in finding the next hop router is:
           find the arp table entry corresponding to the IP provided;
           if this result is empty or the MAC addr is not unique:
              return null;
           extract unique MAC and search MAC table for this MAC;
           if the MAC table search is empty:
              return null;
@@ -282,84 +170,76 @@
           Return the concat if_df as FHR
         """
         fhr_df = pd.DataFrame()
         if not ip or self._arpnd_df.empty:
             return fhr_df
 
         rslt_df = self._arpnd_df.query(
-            f'ipAddress=="{ip}" and not remote')
+            f'ipAddress=="{ip}"')
 
         if rslt_df.empty:
             return fhr_df
 
+        if len(rslt_df) == 1:
+            # If a single result avoid more queries
+            fhr_df = self._if_df.query(
+                'hostname=="{}" and ifname=="{}"'.format(
+                    rslt_df["hostname"].unique().tolist()[0],
+                    rslt_df["oif"].unique().tolist()[0]))
+            return fhr_df
+
         # If we have more than one MAC addr, its hard to know which one
         uniq_mac = rslt_df['macaddr'].unique().tolist()
         if len(uniq_mac) != 1:
             return fhr_df
 
-        macdf = self._macsobj.get(namespace=[rslt_df.iloc[0].namespace],
-                                  macaddr=[uniq_mac[0]], local=True)
+        macdf = self._macsobj.get(namespace=rslt_df.iloc[0].namespace,
+                                  macaddr=uniq_mac[0], localOnly=True)
         if not macdf.empty:
-            ign_ifs = ["bridge", "Vxlan1"]
-            if device:
-                macdf = macdf.query(
-                    f'vlan != 0 and not oif.isin({ign_ifs}) and '
-                    f' hostname != "{self._mlag_peers[device]}"')
-            else:
-                macdf = macdf.query(f'vlan != 0 and not oif.isin({ign_ifs})')
-
-        for row in rslt_df.itertuples():
-            mac_entry = macdf.query(f'hostname == "{row.hostname}"')
-            if not mac_entry.empty:
-                # for row in macdf.iterrows():
+            macdf = macdf.query('vlan != 0 and oif != "bridge"')
+            for row in macdf.iterrows():
                 idf = self._if_df.query(
-                    f'hostname=="{row.hostname}" and '
-                    f'ifname=="{mac_entry.oif.iloc[0]}"').copy()
-
+                    # Row 0 is the index,row 1 contains the real data
+                    'hostname=="{}" and ifname=="{}"'.format(
+                        row[1]['hostname'], row[1]['oif'])).copy()
                 # We need to replace the VLAN in the if_df with what
                 # is obtained from the MAC because of trunk ports.
                 if idf.empty:
                     continue
-                idfidx = idf.index.values[0]
-                idf.at[idfidx, 'vlan'] = mac_entry.vlan.iloc[0]
-
+                idf.at[idf.index, 'vlan'] = row[1].vlan
                 if (idf.master == 'bridge').all():
-                    idf.at[idfidx, 'ipAddressList'] = f'{ip}/32'
+                    idf.at[idf.index, 'ipAddressList'] = ip
                     # Assuming the VRF is identical across multiple entries
-                    idf.at[idfidx, 'master'] = rslt_df.iloc[0].vrf
-            else:
-                idf = self._if_df.query(f'hostname=="{row.hostname}" and '
-                                        f'ifname=="{row.oif}" and '
-                                        f'type=="vlan"').copy()
-                if idf.empty:
-                    continue
-            if fhr_df.empty:
-                fhr_df = idf
-                fhr_df['master'] = rslt_df.vrf.unique().tolist()[0]
-            else:
-                fhr_df = pd.concat([fhr_df, idf])
-                fhr_df['master'] = rslt_df.vrf.unique().tolist()[0]
+                    idf.at[idf.index, 'master'] = rslt_df.iloc[0].vrf
+                if fhr_df.empty:
+                    fhr_df = idf
+                else:
+                    fhr_df = pd.concat([fhr_df, idf])
         return fhr_df
 
+    def _is_mtu_match(self, device, iface, peer, peerif) -> bool:
+        return (
+            self._if_df[(self._if_df["hostname"] == peer) &
+                        (self._if_df["ifname"] == peerif)].iloc[0].mtu
+            ==
+            self._if_df[(self._if_df["hostname"] == device) &
+                        (self._if_df["ifname"] == iface)].iloc[0].mtu
+        )
+
     def _get_if_vlan(self, device: str, ifname: str) -> int:
         oif_df = self._if_df[(self._if_df["hostname"] == device) &
                              (self._if_df["ifname"] == ifname)]
 
         if oif_df.empty:
-            return -1
+            return []
 
         return oif_df.iloc[0]["vlan"]
 
-    def _get_l2_nexthop(self, device: str, vrf: str, dest: str,
-                        macaddr: Optional[str], protocol: str) -> list:
-        """Get the bridged/tunnel nexthops
-        We're passing protocol because we need to keep the return
-        match the other get nexthop function returns. We don't really
-        use protocol or determine it.
-        """
+    def _get_l2_nexthop(self, device: str, vrf: str, dest: str) -> list:
+        """Get the bridged/tunnel nexthops"""
 
         if self._arpnd_df.empty:
             return []
 
         rslt = self._arpnd_df[(self._arpnd_df['hostname'] == device) &
                               (self._arpnd_df['ipAddress'] == dest)]
         # the end of knowledge
@@ -367,208 +247,111 @@
             # Check if we have an EVPN entry as a route (symmetric routing)
             rslt = self._rdf.query(
                 f'hostname == "{device}" and vrf == "{vrf}"')
             if not rslt.empty:
                 # Check that we have a host route at this point
                 ipvers = 6 if ':' in dest else 4
                 if ((ipvers == 4 and rslt.iloc[0].prefix == f'{dest}/32') or
-                        (ipvers == 6 and
-                         rslt.iloc[0].prefix == f'{dest}/128')):
+                        (ipvers == 6 and rslt.iloc[0].prefix == f'{dest}/128')):
                     overlay = rslt.iloc[0].nexthopIps[0]
-                    if not overlay:
-                        raise AttributeError('missing overlay')
                     return self._get_underlay_nexthop(device, [overlay],
-                                                      ['default'], True)
+                                                      ['default'])
             return []
 
         if rslt.empty:
             return []
 
-        if not macaddr:
-            macaddr = rslt.iloc[0]["macaddr"]
+        macaddr = rslt.iloc[0]["macaddr"]
         oif = rslt.iloc[0]["oif"]
         # This is to handle the VRR interface on Cumulus Linux machines
         if oif.endswith("-v0"):
             oif = oif.split("-v0")[0]
 
         vlan = self._get_if_vlan(device, oif)
 
         if macaddr:
-            mac_df = self._macsobj.get(namespace=[rslt.iloc[0]['namespace']],
-                                       hostname=[device], macaddr=[macaddr],
+            mac_df = self._macsobj.get(namespace=rslt.iloc[0]['namespace'],
+                                       hostname=device, macaddr=macaddr,
                                        vlan=[str(vlan)])
 
             if mac_df.empty:
                 # On servers there's no bridge and thus no MAC table entry
-                return [('', rslt.iloc[0].oif, False, protocol == "l2",
-                         protocol, np.nan)]
+                return [(dest, rslt.iloc[0].oif, False, True)]
 
             overlay = mac_df.iloc[0].remoteVtepIp or False
             if not overlay:
-                return ([('', mac_df.iloc[0].oif, overlay, protocol == "l2",
-                          protocol,
-                          mac_df.iloc[0].timestamp)])
+                return ([(dest, mac_df.iloc[0].oif, overlay, True)])
             else:
                 # We assume the default VRF as the underlay. Can this change?
-                return self._get_underlay_nexthop(device, [overlay],
-                                                  ['default'], True)
+                return self._get_underlay_nexthop(device, [overlay], ['default'])
         return []
 
-    def _get_underlay_nexthop(self, hostname: str, vtep_list: list,
-                              vrf_list: list,
-                              is_overlay: bool) -> List[Any]:
+    def _get_underlay_nexthop(self, hostname: str,
+                              vtep_list: list, vrf_list: list) -> pd.DataFrame:
         """Return the underlay nexthop given the Vtep and VRF"""
 
         # WARNING: This function is incomplete right now
         result = []
 
         if len(set(vrf_list)) != 1:
             # VTEP underlay can only be in a single VRF
             return result
 
         vrf = vrf_list[0].split(':')[-1]
         for vtep in vtep_list:
             if vtep not in self._underlay_dfs:
-                if not vtep:
-                    raise AttributeError(
-                        f'false vtep {vtep_list}: vrf {vrf_list}')
-                self._underlay_dfs[vtep] = self._get_table_sqobj('routes') \
-                    .lpm(namespace=[self.namespace],
-                         address=[vtep], vrf=[vrf])
+                self._underlay_dfs[vtep] = routes.RoutesObj(
+                    context=self.ctxt).lpm(namespace=self.namespace,
+                                           address=vtep, vrf=vrf)
             vtep_df = self._underlay_dfs[vtep]
             rslt = vtep_df.query(
                 f'hostname == "{hostname}" and vrf == "{vrf}"')
             if not rslt.empty:
-                if is_overlay:
-                    intres = zip(rslt.nexthopIps.iloc[0].tolist(),
-                                 rslt.oifs.iloc[0].tolist(),
-                                 repeat(vtep), repeat(is_overlay),
-                                 repeat(rslt.protocol.iloc[0]),
-                                 repeat(rslt.timestamp.iloc[0])
-                                 )
-                elif rslt.protocol.iloc[0] == 'direct':
-                    intres = zip([vtep], [rslt.oifs.iloc[0][0]], [False],
-                                 [False], [rslt.protocol.iloc[0]],
-                                 [rslt.timestamp.iloc[0]])
-
-                else:
-                    intres = zip(rslt.nexthopIps.iloc[0].tolist(),
-                                 rslt.oifs.iloc[0].tolist(),
-                                 repeat(False), repeat(is_overlay),
-                                 repeat(rslt.protocol.iloc[0]),
-                                 repeat(rslt.timestamp.iloc[0])
-                                 )
-
+                intres = zip(rslt.nexthopIps.iloc[0].tolist(),
+                             rslt.oifs.iloc[0].tolist(),
+                             repeat(vtep), repeat(True))
                 result.extend(list(intres))
 
         return result
 
-    def _handle_recursive_route(self, df: pd.DataFrame,
-                                max_recurse: int) -> pd.DataFrame:
-        '''Handle recursive routes which are routes without an OIF.
-
-        NXOS, Panos, IOS and others have this scenario when showing BGP routes
-
-        Args:
-            df (pd.DataFrame): The route DF with the routes to resolve
-            max_recurse(int): Recurse this many times to resolve a route
-
-        Returns:
-            pd.DataFrame: The original dataframe with the OIF filled in
-        '''
-        if not max_recurse:
-            return df
-
-        for row in df.itertuples():
-            oifs = []
-            nhops = []
-            for i, nhop in enumerate(row.nexthopIps):
-                if row.oifs and '_nexthopVrf:' in row.oifs[i]:
-                    vrf = row.oifs[i].split('_nexthopVrf:')[1]
-                else:
-                    vrf = row.vrf
-                rrdf = self._get_table_sqobj('routes') \
-                           .lpm(namespace=[row.namespace],
-                                hostname=[row.hostname], address=[nhop],
-                                vrf=[vrf])
-
-                if not rrdf.empty:
-                    if not rrdf.oifs.size:
-                        # Recurse once more
-                        rrdf = self._handle_recursive_route(rrdf,
-                                                            max_recurse-1)
-                    oif = rrdf.oifs.tolist()[0]
-                    oifs.extend(oif)
-                    # Not all NOS fill in usable values for nexthop for a
-                    # connected route. So don't copy nexthop IP if the result
-                    # of this lookup was a connected route. It also doesn't
-                    # matter if we've a connected route because recursive
-                    # resolution is over when we hit a connected route.
-                    if ~rrdf.protocol.isin(['direct', 'local', 'connected',
-                                            'kernel']).all():
-                        nhops.extend(rrdf.nexthopIps.tolist()[0])
-
-            df.at[row.Index, 'oifs'] = np.array(oifs)
-            if nhops:
-                df.at[row.Index, 'nexthopIps'] = np.array(nhops)
-
-        return df
-
     def _get_nexthops(self, device: str, vrf: str, dest: str, is_l2: bool,
-                      vtep: str, macaddr: str) -> Iterable:
+                      vtep: str) -> list:
         """Get nexthops (oif + IP + overlay) or just oif for given host/vrf.
 
         The overlay is a bit indicating we're getting into overlay or not.
         """
 
         if is_l2:
             if vtep:
-                return self._get_underlay_nexthop(device, [vtep], [vrf], True)
+                return self._get_underlay_nexthop(device, [vtep], [vrf])
             else:
-                return self._get_l2_nexthop(device, vrf, dest, macaddr, 'l2')
+                return self._get_l2_nexthop(device, vrf, dest)
 
         rslt = self._rdf.query(f'hostname == "{device}" and vrf == "{vrf}"')
-        # The following condition is checking that we have a pure L3 nexthop or
-        # the start of an underlay route. if its a pure L3 route, the nexthopIp
-        # is not empty OR the protocol is not hmm--NXOS' host mobility
-        # protocol--which also puts a final subnet route with EVPN as an L3
-        # route.
         if not rslt.empty and (len(rslt.nexthopIps.iloc[0]) != 0 and
-                               rslt.nexthopIps.iloc[0][0] != '') and (
-                                   rslt.protocol.iloc[0] != 'hmm'):
-            if not rslt.oifs.iloc[0].size:
-                rslt = self._handle_recursive_route(rslt,
-                                                    self.max_rr_recursion)
-
+                               rslt.nexthopIps.iloc[0][0] != ''):
             # Handle overlay routes given how NXOS programs its FIB
             if rslt.oifs.explode().str.startswith('_nexthopVrf:').any():
                 # We need to find the true NHIP
-                if rslt.oifs.iloc[0].tolist() == [False]:
-                    raise AttributeError('mising vtep')
                 return self._get_underlay_nexthop(
-                    device, rslt.nexthopIps.iloc[0].tolist(),
-                    rslt.oifs.iloc[0].tolist(), True)
+                    device,
+                    rslt.nexthopIps.iloc[0].tolist(),
+                    rslt.oifs.iloc[0].tolist())
 
             return zip(rslt.nexthopIps.iloc[0].tolist(),
                        rslt.oifs.iloc[0].tolist(),
-                       repeat(False), repeat(False),
-                       repeat(rslt.protocol.iloc[0]),
-                       repeat(rslt.timestamp.iloc[0]))
+                       repeat(False), repeat(False))
 
         # We've either reached the end of routing or the end of knowledge
         # Look for L2 nexthop
-        if rslt.empty:
-            protocol = ''
-        else:
-            protocol = rslt.protocol.iloc[0]
-        return self._get_l2_nexthop(device, vrf, dest, None, protocol)
+        return self._get_l2_nexthop(device, vrf, dest)
 
     @ lru_cache(maxsize=256)
     def _get_nh_with_peer(self, device: str, vrf: str, dest: str, is_l2: bool,
-                          vtep_ip: str, macaddr: str) -> list:
+                          vtep_ip) -> list:
         """Get the nexthops & peer node for each nexthop for a given device/vrf
         This uses the cached route lpm DF to get the nexthops. It
         also handles vlan subinterfaces, MLAG and plain bonds to get the
         valid nexthop peers.
 
         :param device: devicename to query in lpm DF for nexthop
         :type device: str
@@ -576,719 +359,451 @@
         :param vrf: VRF to qualify lpm DF for nexthop
         :type vrf: str
 
         :param dest: Destination IP we're searching forever, needed for arp/nd
         :type dest: str
 
         :param is_l2: If this is an L2 lookup
-        :type is_l2: bool
+        :type dest: bool
 
         :param vtep_ip: VTEP IP address, can be empty string if not in underlay
-        :type vtep_ip: str
-
-        :param macaddr: Look for this MAC addr, not dest, as this is L2hop
-        :type macaddr: str
+        :type dest: bool
 
         :rtype: list
         :return:
         list of tuples where each tuple is (oif, peerdevice, peerif, overlay)
         """
 
         nexthops = []
 
         # TODO: Can we have ECMP nexthops, one with NH IP and one without?
-        nexthop_list = self._get_nexthops(
-            device, vrf, dest, is_l2, vtep_ip, macaddr)
+        nexthop_list = self._get_nexthops(device, vrf, dest, is_l2, vtep_ip)
         new_nexthop_list = []
         # Convert each OIF into its actual physical list
         is_l2 = False
-        for nhip, iface, overlay, l2hop, protocol, timestamp in nexthop_list:
-            if macaddr and is_l2 and not overlay:
-                new_nexthop_list.append((nhip, iface, overlay, l2hop,
-                                         protocol, timestamp))
-                continue
-
-            if (not nhip or nhip == 'None') and iface:
-                addr = dest
-            else:
-                addr = nhip
+        for nhip, iface, overlay, is_l2 in nexthop_list:
             if iface.endswith('-v0'):
                 # Replace Cumulus' VRR entry with actual SVI
                 iface = iface.split('-v0')[0]
             # This first pass is to handle Cumulus symmetric EVPN routes
             arpdf = self._arpnd_df.query(f'hostname=="{device}" and '
-                                         f'ipAddress=="{addr}" and '
+                                         f'ipAddress=="{nhip}" and '
                                          f'oif=="{iface}"')
             if not arpdf.empty and arpdf.remote.all():
-                macdf = self._macsobj.get(namespace=[self.namespace],
-                                          hostname=[device],
-                                          macaddr=[arpdf.iloc[0].macaddr])
+                macdf = self._macsobj.get(namespace=self.namespace,
+                                          hostname=device,
+                                          macaddr=arpdf.iloc[0].macaddr)
                 if not macdf.empty and macdf.remoteVtepIp.all():
                     overlay = macdf.iloc[0].remoteVtepIp
 
-                # you don't always have an overlay if the network is
-                # transitioning
-                if overlay:
-                    underlay_nh = self._get_underlay_nexthop(device, [overlay],
-                                                             ['default'], True)
-                    new_nexthop_list.extend(underlay_nh)
+                underlay_nh = self._get_underlay_nexthop(device, [overlay],
+                                                         ['default'])
+                new_nexthop_list.extend(underlay_nh)
             else:
-                new_nexthop_list.append((nhip, iface, overlay, l2hop,
-                                         protocol, timestamp))
+                new_nexthop_list.append((nhip, iface, overlay, is_l2))
 
-        on_src_node = device in self.src_device
-        # pylint: disable=too-many-nested-blocks
-        for (nhip, iface, overlay, l2hop, protocol,
-             timestamp) in new_nexthop_list:
+        for nhip, iface, overlay, is_l2 in new_nexthop_list:
             df = pd.DataFrame()
-            arpdf = pd.DataFrame()
-            errormsg = ''
-            if l2hop and macaddr and not overlay:
-                if (not nhip or nhip == 'None') and iface:
-                    addr = dest + '/'
-                else:
-                    addr = nhip + '/'
+            if (not nhip or nhip == 'None') and iface:
+                nhip = dest
+            arpdf = self._arpnd_df.query(f'hostname=="{device}" and '
+                                         f'ipAddress=="{nhip}" and '
+                                         f'oif=="{iface}"')
+            if not arpdf.empty:
+                addr = nhip + '/'
                 df = self._if_df.query(
-                    f'macaddr=="{macaddr}" '
+                    f'macaddr=="{arpdf.iloc[0].macaddr}" '
                     f'and type != "bond_slave" '
                     f'and state != "down" '
                     f'and ipAddressList.str.startswith("{addr}")')
                 if df.empty:
-                    df = self._if_df.query(
-                        f'ipAddressList.str.startswith("{addr}") and '
-                        f'type !="bond_slave"')
-                    if df.empty:
-                        continue
-            else:
-                if not nhip:
-                    nhip = dest
-                arpdf = self._arpnd_df.query(f'hostname=="{device}" and '
-                                             f'ipAddress=="{nhip}" and '
-                                             f'oif=="{iface}"')
-                if not arpdf.empty:
-                    addr = nhip + '/'
+                    # In case of L2 interfaces as the nexthop, there'll be
+                    # no IP address on the interface with matching NHIP.
                     df = self._if_df.query(
                         f'macaddr=="{arpdf.iloc[0].macaddr}" '
-                        f'and type != "bond_slave" '
-                        f'and state != "down" '
-                        f'and ipAddressList.str.startswith("{addr}")')
-                    if df.empty:
-                        # In case of L2 interfaces as the nexthop, there'll be
-                        # no IP address on the interface with matching NHIP.
-                        df = self._if_df.query(
-                            f'macaddr=="{arpdf.iloc[0].macaddr}" '
-                            f'and type != "bond_slave"')
-                elif protocol == 'direct':
-                    continue
-                nhip_df = self._if_df.query(
-                    f'ipAddressList.str.startswith("{nhip}/") and '
-                    f'type != "bond_slave" and hostname != "{device}"')
-                if df.empty and not nhip_df.empty:
-                    df = nhip_df
-                elif on_src_node and not df.empty and not nhip_df.empty:
-                    if ((df.hostname.unique().tolist() !=
-                         nhip_df.hostname.unique().tolist()) and
-                        (df.macaddr.unique().tolist() !=
-                         nhip_df.macaddr.unique().tolist())):
-                        errormsg = 'Possible anycast IP without anycast MAC'
-                        l2hop = True
-
+                        f'and type != "bond_slave"')
+            if df.empty:
+                df = self._if_df.query(
+                    f'ipAddressList.str.startswith("{nhip}") and '
+                    f'type !="bond_slave"')
                 if df.empty:
                     continue
 
             # In case of centralized EVPN, its possible to find the NHIP on
             # unconnected devices if this is still the source device i.e.
             # server. If so, find FHR to get the real connected dev
             if device in self.src_device:
                 check_fhr = self.source
-            elif l2hop and (df.iloc[0].hostname in self.dest_device):
+            elif is_l2 and (df.iloc[0].hostname in self.dest_device):
                 check_fhr = self.dest
             else:
                 check_fhr = None
 
             if check_fhr:
-                fhr_df = self._find_fhr_df(device, check_fhr)
+                fhr_df = self._find_fhr_df(check_fhr)
                 if not fhr_df.empty:
-                    fhr_hosts = set(fhr_df['hostname'].tolist())
-
+                    fhr_hosts = fhr_df['hostname'].tolist()
                     if check_fhr != self.dest and device not in fhr_hosts:
                         # Avoid looping everytime we hit the dest device
                         # We only need to do it once
-                        df = df.query(f'hostname.isin({list(fhr_hosts)})')
+                        df = df.query(f'hostname.isin({fhr_hosts})')
                         if df.empty:
                             # The L3 nexthop is not the next L2 hop
                             df = fhr_df
-                            l2hop = True
-                            # But what we're going to be forwarding on when
-                            # we hit the next L2 hop is the MAC addr from the
-                            # ARP entry, and so set the macaddr to that for now
-                            if not arpdf.empty:
-                                macaddr = arpdf.macaddr.unique().tolist()[0]
+                            is_l2 = True
                         else:
                             # Fix the incoming interface
                             df = df.merge(fhr_df[['namespace', 'hostname',
                                                   'ifname']],
                                           on=['namespace', 'hostname'],
-                                          how='outer') \
-                                .fillna(method='ffill') \
+                                          how='left') \
                                 .drop(columns=['ifname_x']) \
                                 .rename(columns={'ifname_y': 'ifname'})
 
-            # In case of some NOS such as NXOS with OSPF unnumbered, multiple
-            # interfaces from the same device have the same IP and MAC. This
-            # needs to be filtered to the precise interface. We do this by
-            # matching the IP/MAC of this device's OIF with the ARP/ND table
-            # on the nexthop device
-            if (df.hostname.nunique() == 1) and (df.ifname.nunique() > 1):
-                oif_df = self._if_df.query(f'hostname=="{device}" and '
-                                           f' ifname=="{iface}"')
-                if not oif_df.empty and oif_df.ipAddressList.iloc[0]:
-                    revip = oif_df.ipAddressList.iloc[0].split('/')[0]
-                    revvrf = "default" if overlay else vrf
-                    revarp_df = self._arpnd_df.query(
-                        f'hostname=="{df.hostname.unique()[0]}" and '
-                        f'ipAddress=="{revip}" and vrf=="{revvrf}" and '
-                        'state!="failed"')
-                    if not revarp_df.empty:
-                        df = df.query(f'ifname == "{revarp_df.oif.iloc[0]}"')
-            df.apply(lambda x, nexthops:   # type: ignore
+            df.apply(lambda x, nexthops:
                      nexthops.append((iface, x['hostname'],
-                                      x['ifname'],  overlay,
-                                      l2hop, nhip,
-                                      macaddr or x.macaddr, protocol, errormsg,
-                                      timestamp))
+                                      x['ifname'],  overlay, is_l2, nhip))
                      if (x['namespace'] in self.namespace) else None,
                      args=(nexthops,), axis=1)
 
         if not nexthops and is_l2:
-            return [(None, None, None, False, is_l2, None, None, "l2", "",
-                     np.nan)]
+            return [(None, None, None, False, is_l2, None)]
 
-        return sorted(nexthops, key=lambda x: x[1])
+        return nexthops
 
     def get(self, **kwargs) -> pd.DataFrame:
         """return a pandas dataframe with the paths between src and dest
         :param kwargs:
         :return:
         :rtype: pd.DataFrame
         """
 
         if not self.ctxt.engine:
             raise AttributeError(
-                "Specify an analysis engine using 'set engine' command"
+                "Specify an analysis engine using set engine " "command"
             )
 
         namespaces = kwargs.get("namespace", self.ctxt.namespace)
         if not namespaces:
             raise AttributeError("Must specify namespace to run the trace in")
 
         self.namespace = namespaces[0]
-        src = kwargs.get("src", None)
+        src = kwargs.get("source", None)
         dest = kwargs.get("dest", None)
         dvrf = kwargs.get("vrf", "")
-        query_str = kwargs.pop('query_str', "")
 
         if not src or not dest:
             raise AttributeError("Must specify trace source and dest")
 
-        srcvers = ip_network(src, strict=False).version
-        dstvers = ip_network(dest, strict=False).version
+        srcvers = ip_network(src, strict=False)._version
+        dstvers = ip_network(dest, strict=False)._version
         if srcvers != dstvers:
             raise AttributeError(
                 "Source and Dest MUST belong to same address familt")
         # All exceptions in the initial data gathering will happen in this init
         # After this, at least we know we have the data to work on
         self._init_dfs(self.namespace, src, dest)
 
         devices_iifs = OrderedDict()
-        src_mtu: int = MAX_MTU + 1
-        item = None
         for i in range(len(self._src_df)):
             item = self._src_df.iloc[i]
             devices_iifs[f'{item.hostname}/'] = {
                 "iif": item["ifname"],
                 "mtu": item["mtu"],
-                "outMtu": item["mtu"],
                 "overlay": '',
-                "protocol": '',
-                "hopError": [],
-                "lookup": dest,
-                "macaddr": None,
-                "vrf": dvrf or item['master'],  # pick user pref if given
-                'mtuMatch': True,  # Its the first node
+                "vrf": item['master'],
                 "is_l2": self.is_l2,
-                "nhip": '',
+                "nhip": self.dest,  # Greased to handle a pure l2 path
                 "overlay_nhip": '',
                 "oif": item["ifname"],
                 "timestamp": item["timestamp"],
-                "l3_visited_devices": set(),
-                "l2_visited_devices": set()
             }
-            if (src_mtu > MAX_MTU) or (item.get('mtu', 0) < src_mtu):
-                src_mtu = item.get('mtu', 0)  # type: ignore
-        if not dvrf and item is not None:
+        src_device_iifs = devices_iifs
+        if not dvrf:
             dvrf = item['master']
         if not dvrf:
             dvrf = "default"
 
         dest_device_iifs = OrderedDict()
         for i in range(len(self._dest_df)):
             item = self._dest_df.iloc[i]
-            error = []
             dest_device_iifs[f'{item.hostname}/'] = {
-                "iif": '',
-                # this is what the dest is, so user pref doesn't come in
-                "vrf": item["master"] or dvrf,
+                "iif": item["ifname"],
+                "vrf": item["master"] or "default",
                 "mtu": item["mtu"],
-                "outMtu": item["mtu"],
-                "macaddr": None,
-                "hopError": error,
                 "overlay": '',
                 "is_l2": False,
                 "overlay_nhip": '',
-                "oif": item["ifname"],
-                "protocol": '',
-                "lookup": '',
+                "oif": '',
                 "timestamp": item["timestamp"],
             }
 
-        final_paths = []
         paths = []
-        on_src_node = True
+        for x in src_device_iifs:
+            paths.append([OrderedDict({x: devices_iifs[x]})])
+
+        l3_visited_devices = set()
+        l2_visited_devices = set()
 
         # The logic is to loop through the nexthops till you reach the dest
-        # node The topmost while is this looping. The next loop within handles
+        # device The topmost while is this looping. The next loop within handles
         # one nexthop at a time.The paths are constructed as a list of lists,
         # where each element of the outermost loop is one complete path and
         # each inner list represents one hop in that path. Each hop is the
         # list of devicename and incoming interface. loops are detected by
         # ensuring that no device is visited twice in the same VRF. The VRF
         # qualification is required to ensure packets coming back from a
         # firewall or load balancer are not tagged as duplicates.
-        # pylint: disable=too-many-nested-blocks
+
+        on_src_node = True
         while devices_iifs:
             nextdevices_iifs = OrderedDict()
             newpaths = []
-            revdf_check = True
+            l3_devices_this_round = set()
+            l2_devices_this_round = set()
 
             for devkey in devices_iifs:
                 device = devkey.split('/')[0]
                 iif = devices_iifs[devkey]["iif"]
                 devvrf = devices_iifs[devkey]["vrf"]
                 ioverlay = devices_iifs[devkey]["overlay"]
-                macaddr = devices_iifs[devkey]['macaddr']
-                l3_visited_devices = devices_iifs[devkey]['l3_visited_devices']
-                l2_visited_devices = devices_iifs[devkey]['l2_visited_devices']
-                is_l2 = devices_iifs[devkey]['is_l2']
 
                 # We've reached the destination, so stop this loop
                 destdevkey = f'{device}/'
                 if destdevkey in dest_device_iifs:
-                    if revdf_check:
-                        vrfchk = dest_device_iifs[destdevkey]["vrf"]
-                        rev_df = self._rpf_df.query(
-                            f'hostname == "{device}" and vrf == "{vrfchk}"')
-                        if rev_df.empty and is_l2:
-                            # for the case if this node is the ingress VTEP
-                            rev_df = self._arpnd_df.query(
-                                f'hostname == "{device}" and '
-                                f'ipAddress == "{dest}"')
-                            if rev_df.empty:
-                                dest_device_iifs[destdevkey]['hopError'] \
-                                    .append('no reverse path, possible flood')
-                        elif rev_df.empty:
-                            dest_device_iifs[destdevkey]['hopError'] \
-                                .append('no reverse path')
-                        revdf_check = False
                     pdev1 = devkey.split('/')[1]
                     for x in paths:
                         pdev2 = list(x[-1].keys())[0].split('/')[0]
-                        if (pdev1 != pdev2) and not on_src_node:
+                        if pdev1 != pdev2:
                             continue
-                        copy_dest = copy(dest_device_iifs[destdevkey])
-                        if not on_src_node:
-                            copy_dest['oif'] = devices_iifs[devkey]['oif']
-                        copy_dest['iif'] = iif
-                        copy_dest['mtu'] = devices_iifs[devkey]['mtu']
-                        dst_mtu = copy_dest.get('outMtu', 0)
-                        if dst_mtu > MAX_MTU:
-                            dst_mtu = copy_dest.get('mtu', 0)
-                        if dst_mtu != src_mtu:
-                            if ('Dst MTU != Src MTU' not in
-                                    copy_dest['hopError']):
-                                copy_dest['hopError']\
-                                    .append('Dst MTU != Src MTU')
-                        # This is weird because we have no room to store the
-                        # prev hop's outgoing IIF MTU on the last hop
-                        copy_dest['outMtu'] = \
-                            f'{devices_iifs[devkey]["outMtu"]}/' \
-                            f'{dest_device_iifs[destdevkey]["outMtu"]}'
-                        copy_dest['is_l2'] = is_l2
-                        if not is_l2:
-                            copy_dest['nhip'] = dest
-                        copy_dest['mtuMatch'] = \
-                            devices_iifs[devkey]['mtuMatch']
+                        dest_device_iifs[destdevkey]['oif'] = devices_iifs[devkey]['oif']
                         z = x + [OrderedDict(
-                            {destdevkey: copy_dest})]
-                        if z not in final_paths:
-                            final_paths.append(z)
-
-                    if not paths:
-                        copy_dest = copy(dest_device_iifs[destdevkey])
-                        # This is because the src and dst nodes are the same
-                        # So ignore the OIF coming out of devices_iifs
-                        copy_dest['iif'] = iif
-                        copy_dest['mtu'] = devices_iifs[devkey]['mtu']
-                        dst_mtu = copy_dest.get('outMtu', 0)
-                        if dst_mtu > MAX_MTU:
-                            dst_mtu = copy_dest.get('mtu', 0)
-                        if dst_mtu != src_mtu:
-                            if ('Dst MTU != Src MTU' not in
-                                    copy_dest['hopError']):
-                                copy_dest['hopError']\
-                                    .append('Dst MTU != Src MTU')
-                        # This is weird because we have no room to store the
-                        # prev hop's outgoing IIF MTU on the last hop
-                        copy_dest['outMtu'] = \
-                            f'{devices_iifs[devkey]["outMtu"]}/' \
-                            f'{dest_device_iifs[destdevkey]["outMtu"]}'
-                        copy_dest['is_l2'] = is_l2
-                        if not is_l2:
-                            copy_dest['nhip'] = dest
-                        copy_dest['mtuMatch'] = \
-                            devices_iifs[devkey]['mtuMatch']
-
-                        paths = [[OrderedDict({destdevkey: copy_dest})]]
+                            {destdevkey: dest_device_iifs[destdevkey]})]
+                        if z not in newpaths:
+                            newpaths.append(z)
                     continue
 
-                newdevices_iifs = {}  # NHs from this NH added to next round
+                newdevices_iifs = {}  # NHs from this NH to add to the next round
+                is_l2 = devices_iifs[devkey]['is_l2']
+
                 end_overlay = True
                 if is_l2 or ioverlay:
                     if ioverlay:
                         ndst = ioverlay
                     else:
                         ndst = devices_iifs[devkey].get('nhip', None)
                     # Check if this is the end of the L2 path or overlay
                     nhdf = self._if_df.query(f'hostname=="{device}"')
                     if not nhdf.empty:
                         if srcvers == 4:
                             nhdf = nhdf.query(
-                                f'ipAddressList.str.startswith("{ndst}/")')
+                                f'ipAddressList.str.contains("{ndst}")')
                         else:
                             nhdf = nhdf.query(
-                                f'ip6AddressList.str.startswith("{ndst}/")')
+                                f'ip6AddressList.str.contains("{ndst}")')
                     if not nhdf.empty:
-                        ifmac = nhdf.macaddr.unique().tolist()
-                        if (not macaddr) or (macaddr in ifmac):
-                            ndst = dest
-                            is_l2 = self.is_l2
-                            ioverlay = ''
-                            l2_visited_devices = set()
+                        ndst = dest
+                        is_l2 = self.is_l2
+                        ioverlay = ''
+                        l2_visited_devices = set()
                     elif ioverlay:
                         end_overlay = False
                 else:
                     ndst = dest
                 if not ndst:
                     ndst = dest
 
                 if not end_overlay:
                     ivrf = 'default'
                 elif end_overlay and devices_iifs[devkey]['overlay_nhip']:
                     ivrf = self._get_vrf(device, '',
                                          devices_iifs[devkey]['overlay_nhip'])
                     if not ivrf:
                         ivrf = devvrf
-                elif (not devices_iifs[devkey]['nhip'] or
-                      (devices_iifs[devkey]['nhip'] == "169.254.0.1")):
-                    ivrf = self._get_vrf(device, iif, '')
-                else:
+                elif not devices_iifs[devkey]['nhip']:
+                    ivrf = self._get_vrf(device, iif, src)
+                elif devices_iifs[devkey]['nhip'] != "169.254.0.1":
                     ivrf = self._get_vrf(device, '',
                                          devices_iifs[devkey]['nhip'])
                     if not ivrf:
                         ivrf = self._get_vrf(device, iif, '')
+                elif devices_iifs[devkey]['nhip'] == "169.254.0.1":
+                    ivrf = self._get_vrf(device, iif, '')
 
                 if not ivrf:
                     ivrf = dvrf
 
                 skey = device + ivrf
                 if is_l2:
                     if skey in l2_visited_devices:
                         # This is a loop
                         if ioverlay:
-                            devices_iifs[devkey]['hopError'] \
-                                .append("Loop in underlay")
+                            raise PathLoopError(
+                                f"Loop detected in underlay on node {device}",
+                                self._path_cons_result(paths))
                         else:
-                            devices_iifs[devkey]['hopError'] \
-                                .append("L2 Loop detected")
-                        for x in paths:
-                            z = x + [OrderedDict({devkey:
-                                                  devices_iifs[devkey]})]
-                            if z not in final_paths:
-                                final_paths.append(z)
-                        continue
-
-                    l2_visited_devices.add(skey)
+                            raise PathLoopError(
+                                f"L2 Loop detected on node {device}",
+                                self._path_cons_result(paths))
+                    else:
+                        l2_devices_this_round.add(skey)
                 else:
                     if skey in l3_visited_devices:
-                        devices_iifs[devkey]['hopError'].append("L3 loop")
-                        for x in paths:
-                            z = x + [OrderedDict({devkey:
-                                                  devices_iifs[devkey]})]
-                            if z not in final_paths:
-                                final_paths.append(z)
-                        continue
-
-                    l3_visited_devices.add(skey)
-
-                devices_iifs[devkey]['vrf'] = ivrf
-                rt_ts = None
-                if not (is_l2 or ioverlay):
-                    rslt = self._rdf.query('hostname == "{}" and vrf == "{}"'
-                                           .format(device, ivrf))
-                    if not rslt.empty:
-                        devices_iifs[devkey]['timestamp'] = \
-                            rslt.timestamp.iloc[0]
-                        devices_iifs[devkey]['protocol'] = \
-                            rslt.protocol.iloc[0]
-                        devices_iifs[devkey]['lookup'] = rslt.prefix.iloc[0]
-
-                        rev_df = self._rpf_df.query(
-                            f'hostname == "{device}" and vrf == "{ivrf}"')
-                        if rev_df.empty and not on_src_node:
-                            devices_iifs[devkey]['hopError'] \
-                                .append('no reverse path')
+                        # This is a loop
+                        raise PathLoopError(f"Loop detected on node {device}",
+                                            self._path_cons_result(paths))
                     else:
-                        devices_iifs[devkey]['lookup'] = ''
+                        l3_devices_this_round.add(skey)
 
-                elif macaddr:
-                    devices_iifs[devkey]['lookup'] = ''
-                else:
-                    devices_iifs[devkey]['lookup'] = ndst
+                devices_iifs[devkey]['vrf'] = ivrf
+                rslt = self._rdf.query('hostname == "{}" and vrf == "{}"'
+                                       .format(device, ivrf))
+                if not rslt.empty:
+                    timestamp = str(rslt["timestamp"].max())
 
                 for i, nexthop in enumerate(self._get_nh_with_peer(
-                        device, ivrf, ndst, is_l2, ioverlay, macaddr)):
-                    error = []
-                    (iface, peer_device, peer_if, overlay, is_l2,
-                     nhip, macaddr, protocol, errmsg, timestamp) = nexthop
-                    if not devices_iifs[devkey].get('protocol', ''):
-                        devices_iifs[devkey]['protocol'] = protocol
-                    if not rt_ts:
-                        devices_iifs[devkey]['timestamp'] = timestamp
-                    if (errmsg and
-                            errmsg not in devices_iifs[devkey]['hopError']):
-                        devices_iifs[devkey]['hopError'].append(errmsg)
-
+                        device, ivrf, ndst, is_l2, ioverlay)):
+                    iface, peer_device, peer_if, overlay, is_l2, nhip = nexthop
                     if iface is not None:
-                        if iface.startswith('vPC Peer'):
-                            iface = self._mlag_peerlink[device]
-                        elif iface.startswith('sup-eth1'):
-                            iface = 'loopback0'
-                        if peer_if.startswith('vPC Peer'):
-                            peer_if = self._mlag_peerlink[peer_device]
-                        elif peer_if.startswith('sup-eth1'):
-                            peer_if = 'loopback0'
-                        in_mtu = self._if_df[
-                            (self._if_df["hostname"] == peer_device) &
-                            (self._if_df["ifname"] == peer_if)
-                        ].iloc[-1].mtu
-                        out_mtu = self._if_df[
-                            (self._if_df["hostname"] == device) &
-                            (self._if_df["ifname"] == iface)
-                        ].iloc[-1].mtu
-                        if on_src_node and src_mtu > MAX_MTU:
-                            src_mtu = out_mtu
-                        mtu_match = in_mtu == out_mtu
-                        if (in_mtu < src_mtu) or (out_mtu < src_mtu):
-                            error.append('Hop MTU < Src Mtu')
+                        try:
+                            mtu_match = self._is_mtu_match(device, iface,
+                                                           peer_device,
+                                                           peer_if)
+                        except Exception:
+                            mtu_match = np.NaN
+
                         if not end_overlay:
                             overlay = ioverlay
                             vrf = devvrf
                         else:
                             vrf = ivrf
-                        if not nhip:
-                            nhip = ndst
                         if overlay and not ioverlay:
                             overlay_nhip = ndst
                         elif not end_overlay:
                             overlay_nhip = devices_iifs[devkey]['overlay_nhip']
                         else:
                             overlay_nhip = ''
-                        if overlay or not is_l2:
-                            # We don't need to track MACaddr if its not a pure
-                            # (non-overlay) L2 hop
-                            macaddr = None
-
                         newdevices_iifs[f'{peer_device}/{device}'] = {
                             "iif": peer_if,
                             "vrf": vrf,
-                            "macaddr": macaddr,
                             "overlay": overlay,
-                            "mtu": in_mtu,
-                            "outMtu": out_mtu,  # prev hop's outMTU, fixed ltr
+                            "mtu": self._if_df[
+                                (self._if_df["hostname"] == peer_device) &
+                                (self._if_df["ifname"] == peer_if)].iloc[-1].mtu,
                             "mtuMatch": mtu_match,
                             "is_l2": is_l2,
                             "nhip": nhip,
                             "oif": iface,
-                            "hopError": error,
                             "overlay_nhip": overlay_nhip,
-                            'l3_visited_devices': l3_visited_devices.copy(),
-                            'l2_visited_devices': l2_visited_devices.copy()
+                            "timestamp": timestamp,
                         }
 
-                if not paths:
-                    newpaths.append(
-                        [OrderedDict({devkey: devices_iifs[devkey]})])
-
-                # matching to attach the hop to the appropriate path
-                pdev1 = devkey.split('/')[1]
-                for x in paths:
-                    xkey = list(x[-1].keys())[0]
-                    pdev2 = xkey.split('/')[0]
-                    if pdev1 != pdev2:
-                        continue
-                    z = x + [OrderedDict({devkey: devices_iifs[devkey]})]
-                    if z not in newpaths:
-                        newpaths.append(z)
-
-                for k, v in newdevices_iifs.items():
-                    if k not in nextdevices_iifs:
-                        nextdevices_iifs[k] = v
+                if not on_src_node:
+                    pdev1 = devkey.split('/')[1]
+                    for x in paths:
+                        xkey = list(x[-1].keys())[0]
+                        pdev2 = xkey.split('/')[0]
+                        if pdev1 != pdev2:
+                            continue
+                        z = x + [OrderedDict({devkey: devices_iifs[devkey]})]
+                        if z not in newpaths:
+                            newpaths.append(z)
+
+                if not newdevices_iifs:
+                    break
+
+                for x in newdevices_iifs:
+                    if x not in nextdevices_iifs:
+                        nextdevices_iifs[x] = newdevices_iifs[x]
 
             if newpaths:
                 paths = newpaths
 
+            l3_visited_devices = l3_visited_devices.union(
+                l3_devices_this_round)
+            l2_visited_devices = l3_visited_devices.union(
+                l2_devices_this_round)
             devices_iifs = nextdevices_iifs
             on_src_node = False
 
-        if not final_paths:
-            # This occurs when a path traversal terminates due to an error such
-            # as loop detected
-            final_paths = paths
-        return self._handle_user_query_str(
-            self._path_cons_result(final_paths, **kwargs), query_str)\
-            .reset_index(drop=True)
+        # Add the final destination to all paths
+        # for x in paths:
+        #    for device in dest_device_iifs:
+        #        x.append(OrderedDict({device: dest_device_iifs[device]}))
+
+        # Construct the pandas dataframe.
+        # Constructing the dataframe in one shot here as that's more efficient
+        # for pandas
+        return self._path_cons_result(paths)
 
-    def _path_cons_result(self, paths, **kwargs):
+    def _path_cons_result(self, paths):
         df_plist = []
-        columns = kwargs.get('columns', ['default'])
-        fields = self.schema.get_display_fields(columns)
-        # TODO: handle hostname filtering
-        # hostname = kwargs.get('hostname')
-        prev_hop = hop = None
         for i, path in enumerate(paths):
-            if prev_hop:
-                # Taking advantage of python's shallow copy, that this
-                # also changes what's in df_plist
-                if not self._dest_df.empty:
-                    prev_hop['oif'] = self._dest_df.iloc[0]['ifname']
-                if (isinstance(prev_hop['outMtu'], str) and
-                        '/' in prev_hop['outMtu']):
-                    prev_hop['outMtu'] = int(prev_hop['outMtu'].split('/')[1])
-                prev_hop['isL2'] = False
-                prev_hop['nexthopIp'] = ''
-                prev_hop['vtepLookup'] = ''
-                prev_hop = None
+            prev_device = None
+            prev_hopid = 0
             for j, ele in enumerate(path):
                 item = list(ele)[0]
-                overlay = bool(ele[item]['overlay'])
-                lookup = ele[item].get("lookup", "")
-
-                hop = {
-                    "pathid": i + 1,
-                    "hopCount": j,
-                    "namespace": self.namespace,
-                    "hostname": item.split('/')[0],
-                    "iif": ele[item]["iif"],
-                    "oif": ele[item]['oif'],
-                    "vrf": ele[item]["vrf"],
-                    "isL2": ele[item].get("is_l2", False),
-                    "overlay": overlay,
-                    "mtuMatch": ele[item].get("mtuMatch", np.nan),
-                    "inMtu": ele[item].get("mtu", 0),
-                    "outMtu": ele[item].get("outMtu", 0),
-                    "protocol": ele[item].get('protocol', ''),
-                    "ipLookup": lookup,
-                    "vtepLookup": "",
-                    "macLookup": "",
-                    "nexthopIp": ele[item].get('nhip', ''),
-                    "hopError": ', '.join(ele[item].get('hopError', [])),
-                    "timestamp": ele[item].get("timestamp", np.nan)
-                }
-                df_plist.append(hop)
-                # Update some of the edge info in the prev rowerr
-                # Some path specific info cannot be populated in a hop
-                # because of the algorithm. So, we save the info associated
-                # with each hop of the path in the nexthop and have to do
-                # this logic to populate the prev hop
-                if prev_hop:
-                    # Taking advantage of python's shallow copy, that this
-                    # also changes what's in df_plist
-                    prev_hop['nexthopIp'] = hop['nexthopIp']
-                    if overlay:
-                        prev_hop['vtepLookup'] = ele[item]["overlay"]
-                    elif hop["isL2"]:
-                        prev_hop["macLookup"] = ele[item]["macaddr"]
-                    if not self._srcnode_via_arp or hop['hopCount'] != 1:
-                        # When we're starting from the first hop switch rather
-                        # than the true source endpoint, and we're jumping into
-                        # VXLAN, its not correct to use the isL2 from nexthop.
-                        prev_hop['isL2'] = hop['isL2']
-                    prev_hop['oif'] = hop['oif']
-                    if isinstance(hop['outMtu'], str) and '/' in hop['outMtu']:
-                        prev_hop['outMtu'] = int(hop['outMtu'].split('/')[0])
-                    else:
-                        prev_hop['outMtu'] = hop['outMtu']
-                prev_hop = hop
-        if prev_hop:
-            # Taking advantage of python's shallow copy, that this
-            # also changes what's in df_plist
-            if not self._dest_df.empty:
-                prev_hop['oif'] = self._dest_df.iloc[0]['ifname']
-            if (isinstance(prev_hop['outMtu'], str) and
-                    '/' in prev_hop['outMtu']):
-                prev_hop['outMtu'] = int(prev_hop['outMtu'].split('/')[1])
-            prev_hop['isL2'] = False
-            prev_hop['nexthopIp'] = ''
-            prev_hop['vtepLookup'] = ''
+                if item == prev_device:
+                    hopid = prev_hopid
+                else:
+                    hopid = j
+                    prev_device = item
+                    prev_hopid = hopid
+                if ele[item]['overlay']:
+                    overlay = True
+                else:
+                    overlay = False
+                df_plist.append(
+                    {
+                        "pathid": i + 1,
+                        "hopCount": hopid,
+                        "namespace": self.namespace,
+                        "hostname": item.split('/')[0],
+                        "iif": ele[item]["iif"],
+                        "oif": ele[item]['oif'],
+                        "vrf": ele[item]["vrf"],
+                        "isL2": ele[item].get("is_l2", False),
+                        "overlay": overlay,
+                        "mtuMatch": ele[item].get("mtuMatch", np.nan),
+                        "mtu": ele[item].get("mtu", 0),
+                        "timestamp": ele[item].get("timestamp", np.nan)
+                    }
+                )
+                if j:
+                    df_plist[-2]['oif'] = ele[item]['oif']
+            df_plist[-1]['oif'] = ''
         paths_df = pd.DataFrame(df_plist)
-        paths_df.drop_duplicates(inplace=True)
-        ret_cols = [f for f in fields if (f in paths_df.columns)]
-        return paths_df[ret_cols]
+        return paths_df.drop_duplicates()
 
     def summarize(self, **kwargs):
         """return a pandas dataframe summarizing the path info between src/dest
-
-        A copy of this function is in gui_path.py for reasons of efficiency
         :param kwargs:
         :return:
         :rtype: pd.DataFrame
         """
 
         path_df = self.get(**kwargs)
 
         if path_df.empty:
             return pd.DataFrame()
 
         namespace = self.namespace
         ns = {}
         ns[namespace] = {}
 
-        perhopEcmp = path_df.query('hopCount != 0') \
-                            .groupby(by=['hopCount'])['hostname']
+        perhopEcmp = path_df.groupby(by=['hopCount'])['hostname']
         ns[namespace]['totalPaths'] = path_df['pathid'].max()
         ns[namespace]['perHopEcmp'] = perhopEcmp.nunique().tolist()
         ns[namespace]['maxPathLength'] = path_df.groupby(by=['pathid'])[
             'hopCount'].max().max()
         ns[namespace]['avgPathLength'] = path_df.groupby(by=['pathid'])[
             'hopCount'].max().mean()
         ns[namespace]['uniqueDevices'] = path_df['hostname'].nunique()
         ns[namespace]['mtuMismatch'] = not all(path_df['mtuMatch'])
         ns[namespace]['usesOverlay'] = any(path_df['overlay'])
-        ns[namespace]['pathMtu'] = min(
-            path_df.query('iif != "lo"')['inMtu'].min(),
-            path_df.query('iif != "lo"')['outMtu'].min())
+        ns[namespace]['pathMtu'] = path_df.query('iif != "lo"')['mtu'].min()
 
         summary_fields = ['totalPaths', 'perHopEcmp', 'maxPathLength',
                           'avgPathLength', 'uniqueDevices', 'pathMtu',
                           'usesOverlay', 'mtuMismatch']
         return pd.DataFrame(ns).reindex(summary_fields, axis=0) \
                                .convert_dtypes()
```

### Comparing `suzieq-0.22.0rc1/suzieq/engines/pandas/routes.py` & `suzieq-0.8.0/suzieq/engines/pandas/routes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,43 @@
-from typing import List
-from ipaddress import ip_address, ip_network
 from collections import defaultdict
-
-import numpy as np
+from suzieq.engines.pandas.engineobj import SqEngineObject
 import pandas as pd
+from ipaddress import ip_address, ip_network
 
-from suzieq.engines.pandas.engineobj import SqPandasEngine
-
-
-class RoutesObj(SqPandasEngine):
-    '''Backend class to handle manipulating routes table with pandas'''
 
-    @staticmethod
-    def table_name():
-        '''Table name'''
-        return 'routes'
+class RoutesObj(SqEngineObject):
 
-    def _cons_addnl_fields(self, columns: List[str], addnl_fields: List[str],
-                           add_prefixlen: bool) -> List[str]:
+    def _cons_addnl_fields(self, columns: list, addnl_fields: list) -> (list, list):
         '''get all the additional columns we need'''
 
+        drop_cols = []
+
         if columns == ['default']:
-            # Thanks to Linux, we need metric and weed out some routes
             addnl_fields.append('metric')
-        elif columns != ['*']:
-            for col in ['metric', 'ipvers', 'protocol', 'prefix']:
-                if col not in columns:
-                    addnl_fields.append(col)
-
-        if add_prefixlen:
-            if columns != ['*'] and all('prefixlen' not in x
-                                        for x in [columns, addnl_fields]):
-                addnl_fields.append('prefixlen')
+            drop_cols += ['metric']
+        elif columns != ['*'] and 'metric' not in columns:
+            addnl_fields.append('metric')
+            drop_cols += ['metric']
+
+            if 'ipvers' not in columns:
+                addnl_fields.append('ipvers')
+                drop_cols += ['ipvers']
 
-        return addnl_fields
+        return addnl_fields, drop_cols
 
     def get(self, **kwargs):
-        '''Return the routes table for the given filters'''
 
-        prefixlen = kwargs.pop('prefixlen', '')
+        prefixlen = kwargs.pop('prefixlen', None)
         prefix = kwargs.pop('prefix', [])
         ipvers = kwargs.pop('ipvers', '')
-        user_query = kwargs.pop('query_str', '')
-
-        columns = kwargs.pop('columns', ['default'])
-        fields = self.schema.get_display_fields(columns)
+        addnl_fields = kwargs.pop('addnl_fields', [])
 
-        addnl_fields = []
-        addnl_fields = self._cons_addnl_fields(
-            columns, addnl_fields, prefixlen != '')
-
-        self._add_active_to_fields(kwargs.get('view', self.iobj.view), fields,
-                                   addnl_fields)
+        columns = kwargs.get('columns', ['default'])
+        addnl_fields, drop_cols = self._cons_addnl_fields(
+            columns, addnl_fields)
 
         # /32 routes are stored with the /32 prefix, so if user doesn't specify
         # prefix as some folks do, assume /32
         newpfx = []
         for item in prefix:
             ipvers = self._get_ipvers(item)
 
@@ -63,29 +45,34 @@
                 if ipvers == 4:
                     item += '/32'
                 else:
                     item += '/128'
 
             newpfx.append(item)
 
-        user_query_cols = self._get_user_query_cols(user_query)
-        addnl_fields += [x for x in user_query_cols if x not in addnl_fields]
+        if 'prefixlen' in columns:
+            need_prefixlen = True
+            columns.remove('prefixlen')
+            if 'prefix' not in columns:
+                columns.insert(-1, 'prefix')
+                drop_cols.append('prefix')
+        else:
+            need_prefixlen = False
 
         df = super().get(addnl_fields=addnl_fields, prefix=newpfx,
-                         ipvers=ipvers, columns=fields, **kwargs)
+                         ipvers=ipvers, **kwargs)
 
-        if df.empty:
-            return df
+        if need_prefixlen:
+            columns.insert(-1, 'prefixlen')
 
-        if 'prefix' in df.columns:
+        if not df.empty and 'prefix' in df.columns:
             df = df.loc[df['prefix'] != "127.0.0.0/8"]
             df['prefix'].replace('default', '0.0.0.0/0', inplace=True)
 
-            if (prefixlen or (columns == ['*']) or
-                    any('prefixlen' in x for x in [columns, addnl_fields])):
+            if prefixlen or ('prefixlen' in columns or columns == ['*']):
                 # This convoluted logic to handle the issue of invalid entries
                 # for prefix in JUNOS routing table
                 df['prefixlen'] = df['prefix'].str.split('/')
                 df = df[df.prefixlen.str.len() == 2]
                 df['prefixlen'] = df['prefixlen'].str[1].astype('int')
 
             if prefixlen:
@@ -95,30 +82,25 @@
                     query_str = f'prefixlen != {prefixlen[1:]}'
                 else:
                     query_str = f'prefixlen == {prefixlen}'
 
                 # drop in reset_index to not add an additional index col
                 df = df.query(query_str).reset_index(drop=True)
 
-        if 'numNexthops' in columns or (columns == ['*']):
-            srs_oif = df['oifs'].str.len()
-            srs_hops = df['nexthopIps'].str.len()
-            srs = np.array(list(zip(srs_oif, srs_hops)))
-            srs_max = np.amax(srs, 1)
-            df['numNexthops'] = srs_max
+            if columns != ['*'] and 'prefixlen' not in columns:
+                drop_cols.append('prefixlen')
 
-        if user_query:
-            df = self._handle_user_query_str(df, user_query)
+        if drop_cols:
+            df.drop(columns=drop_cols, inplace=True, errors='ignore')
 
-        return df.reset_index(drop=True)[fields]
+        return df
 
     def summarize(self, **kwargs):
-        '''Summarize routing table info'''
 
-        self._init_summarize(**kwargs)
+        self._init_summarize(self.iobj._table, **kwargs)
         if self.summary_df.empty:
             return self.summary_df
 
         self._summarize_on_add_field = [
             ('deviceCnt', 'hostname', 'nunique'),
             ('uniquePrefixCnt', 'prefix', 'nunique'),
             ('uniqueVrfsCnt', 'vrf', 'nunique'),
@@ -133,16 +115,15 @@
              'prefixlen == 30 or prefixlen == 31', 'prefix'),
             ('hostRoutesCnt', 'prefixlen == 32', 'prefix'),
             ('totalV4RoutesinNs', 'ipvers == 4', 'prefix'),
             ('totalV6RoutesinNs', 'ipvers == 6', 'prefix'),
         ]
 
         self._summarize_on_add_list_or_count = [
-            ('routingProtocolCnt', 'protocol'),
-            ('nexthopCnt', 'numNexthops'),
+            ('routingProtocolCnt', 'protocol')
         ]
 
         self._gen_summarize_data()
 
         # Now for the stuff that is specific to routes
         routes_per_vrfns = self.summary_df.groupby(by=["namespace", "vrf"])[
             "prefix"].count().groupby("namespace")
@@ -152,71 +133,75 @@
         device_with_defrt_per_vrfns = self.summary_df \
             .query('prefix == "0.0.0.0/0"') \
             .groupby(by=["namespace", "vrf"])[
                 "hostname"].nunique()
         devices_per_vrfns = self.summary_df.groupby(by=["namespace", "vrf"])[
             "hostname"].nunique()
 
-        # pylint: disable=expression-not-assigned
         {self.ns[i[0]].update({
             "deviceWithNoDefRoute":
             device_with_defrt_per_vrfns[i] == devices_per_vrfns[i]})
          for i in device_with_defrt_per_vrfns.keys() if i[0] in self.ns.keys()}
         self.summary_row_order.append('deviceWithNoDefRoute')
 
         self._post_summarize()
         return self.ns_df.convert_dtypes()
 
     def lpm(self, **kwargs):
-        '''Run longest prefix match on routing table for specified addr'''
+        if not self.iobj._table:
+            raise NotImplementedError
+
+        drop_cols = []
 
         addr = kwargs.pop('address')
         kwargs.pop('ipvers', None)
         df = kwargs.pop('cached_df', pd.DataFrame())
+        addnl_fields = kwargs.pop('addnl_fields', [])
+
+        try:
+            ipaddr = ip_address(addr)
+            ipvers = ipaddr._version
+        except ValueError as e:
+            raise ValueError(e)
+
+        cols = kwargs.pop("columns", ["namespace", "hostname", "vrf", "metric",
+                                      "prefix", "prefixlen", "nexthopIps",
+                                      "oifs", "protocol", "ipvers"])
+
+        if cols != ['default'] and cols != ['*']:
+            if 'prefix' not in cols:
+                addnl_fields.insert(-1, 'prefix')
+                drop_cols.append('prefix')
 
-        addnl_fields = []
-        ipaddr = ip_address(addr)
-        ipvers = ipaddr._version
-
-        # User may specify a different set of columns than what we're after
-        usercols = kwargs.pop('columns', ['default'])
-        if usercols == ['default']:
-            usercols = self.schema.get_display_fields(usercols)
-            if 'timestamp' not in usercols:
-                usercols.append('timestamp')
-        else:
-            usercols = self.schema.get_display_fields(usercols)
-        cols = self.schema.get_display_fields(["default"])
-        for col in usercols:
-            if col not in cols:
-                cols.append(col)
-
-        addnl_fields = self._cons_addnl_fields(
-            cols, addnl_fields, True)
-        cols += addnl_fields
         rslt = pd.DataFrame()
 
         # if not using a pre-populated dataframe
         if df.empty:
-            df = self.get(ipvers=ipvers, columns=cols, **kwargs)
+            df = self.get(ipvers=ipvers, columns=cols,
+                          addnl_fields=addnl_fields, **kwargs)
         else:
             df = df.query(f'ipvers=={ipvers}')
 
         if df.empty:
             return df
 
+        if 'prefixlen' not in df.columns:
+            df['prefixlen'] = df['prefix'].str.split('/')
+            df = df[df.prefixlen.str.len() == 2]
+            df['prefixlen'] = df['prefixlen'].str[1].astype('int')
+            drop_cols.append('prefixlen')
+
         # Vectorized operation for faster results with IPv4:
         if ipvers == 4:
             intaddr = df.prefix.str.split('/').str[0] \
                 .map(lambda y: int(''.join(['%02x' % int(x)
                                             for x in y.split('.')]),
                                    16))
             netmask = df.prefixlen \
                 .map(lambda x: (0xffffffff << (32 - x)) & 0xffffffff)
-
             match = (ipaddr._ip & netmask) == (intaddr & netmask)
             rslt = df.loc[match.loc[match].index] \
                 .sort_values('prefixlen', ascending=False) \
                 .drop_duplicates(['namespace', 'hostname', 'vrf'])
         else:
             selected_entries = {}
             max_plens = defaultdict(int)
@@ -229,11 +214,19 @@
                         selected_entries[key] = row
             if selected_entries:
                 rslt = pd.DataFrame(list(selected_entries.values())) \
                     .drop(columns=['Index'], errors='ignore')
             else:
                 rslt = pd.DataFrame()
 
-        if rslt.empty:
+        if drop_cols:
+            return rslt.drop(columns=drop_cols, errors='ignore')
+        else:
             return rslt
 
-        return rslt[usercols]
+    def aver(self, **kwargs) -> pd.DataFrame:
+        """Verify that the routing table is consistent
+        The only check for now is to ensure every host has a default route/vrf'
+        """
+        df = self.get(**kwargs)
+        if df.empty:
+            return df
```

### Comparing `suzieq-0.22.0rc1/suzieq/engines/pandas/tables.py` & `suzieq-0.8.0/suzieq/cli/sqcmds/PathCmd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,97 @@
+import time
 import pandas as pd
+from nubia import command, argument
 
-from suzieq.engines.pandas.engineobj import SqPandasEngine
+from suzieq.cli.sqcmds.command import SqCommand
+from suzieq.sqobjects.path import PathObj
 
 
-class TableObj(SqPandasEngine):
-    '''Backend class for virtual table, tables, with pandas'''
+@command("path", help="build and act on path data")
+class PathCmd(SqCommand):
+    def __init__(
+        self,
+        engine: str = "",
+        hostname: str = "",
+        start_time: str = "",
+        end_time: str = "",
+        view: str = "latest",
+        namespace: str = "",
+        format: str = "",
+        columns: str = "default",
+    ) -> None:
+        super().__init__(
+            engine=engine,
+            hostname=hostname,
+            start_time=start_time,
+            end_time=end_time,
+            view=view,
+            namespace=namespace,
+            columns=columns,
+            format=format,
+            sqobj=PathObj
+        )
+
+    @command("show")
+    @argument("src", description="Source IP address, in quotes")
+    @argument("dest", description="Destination IP address, in quotes")
+    @argument("vrf", description="VRF to trace path in")
+    def show(self, src: str = "", dest: str = "", vrf: str = ''):
+        """show paths between specified from source to target ip addresses"""
+        # Get the default display field names
+        if self.columns is None:
+            return
+
+        now = time.time()
+        if self.columns != ["default"]:
+            self.ctxt.sort_fields = None
+        else:
+            self.ctxt.sort_fields = []
 
-    @staticmethod
-    def table_name():
-        '''Table name'''
-        return 'tables'
-
-    def get(self, **kwargs):
-        """Show the known tables for which we have information"""
-
-        table_list = self._dbeng.get_tables()
-        df = pd.DataFrame()
-        columns = kwargs.pop('columns', ['default'])
-        fields = self.schema.get_display_fields(columns)
-        tables = []
-
-        for table in table_list:
-            try:
-                table_inst = self._get_table_sqobj(table)
-            except ModuleNotFoundError:
-                # ignore unknown tables
-                continue
-
-            info = {'table': table}
-            info.update(table_inst.get_table_info(
-                columns=['namespace', 'hostname', 'timestamp'],
-                **kwargs))
-            tables.append(info)
-
-        df = pd.DataFrame.from_dict(tables)
-        if df.empty:
-            return df
-
-        df = df.sort_values(by=['table']).reset_index(drop=True)
-        cols = df.columns
-        total = pd.DataFrame([['TOTAL',  df['firstTime'].min(),
-                               df['lastTime'].max(),
-                               df['intervals'].max(),
-                               df['allRows'].sum(),
-                               df['namespaceCnt'].max(),
-                               df['deviceCnt'].max()]],
-                             columns=cols)
-        df = pd.concat([df, total]).dropna().reset_index(drop=True)
-        return df[fields]
-
-    def summarize(self, **kwargs):
-        '''Summarize metainfo about the various DB tables'''
-
-        df = self.get(**kwargs)
-
-        if df.empty or ('error' in df.columns):
-            return df
-
-        df = df.set_index(['table'])
-
-        sdf = pd.DataFrame({
-            'serviceCnt': [df.index.nunique()-1],
-            'namespaceCnt': [df.at['TOTAL', 'namespaceCnt']],
-            'deviceCnt': [df.at['device', 'deviceCnt']],
-            'earliestTimestamp': [df.firstTime.min()],
-            'lastTimestamp': [df.lastTime.max()],
-            'firstTime99': [df.firstTime.quantile(0.99)],
-            'lastTime99': [df.lastTime.quantile(0.99)],
-        })
-        return sdf.T.rename(columns={0: 'summary'})
-
-    def top(self, **kwargs):
-        "Tables implementation of top has to eliminate the TOTAL row"
-
-        what = kwargs.pop("what", None)
-        reverse = kwargs.pop("reverse", False)
-        sqTopCount = kwargs.pop("count", 5)
-
-        if not what:
-            return pd.DataFrame()
-
-        columns = kwargs.pop('columns', ['default'])
-        fields = self.schema.get_display_fields(columns)
-
-        df = self.get(**kwargs)
-        if ('error' in df.columns) or df.empty:
-            return df
-
-        if reverse:
-            df = df.query('table != "TOTAL"') \
-                .nsmallest(sqTopCount, columns=what, keep="all") \
-                .head(sqTopCount)
+        try:
+            df = self.sqobj.get(
+                hostname=self.hostname, columns=self.columns,
+                namespace=self.namespace, source=src, dest=dest,
+                vrf=vrf
+            )
+        except Exception as e:
+            df = pd.DataFrame({'error': ['ERROR: {}'.format(str(e))]})
+
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        if not df.empty:
+            return self._gen_output(df, sort=False)
+
+    @command("summarize")
+    @argument("src", description="Source IP address, in quotes")
+    @argument("dest", description="Destination IP address, in quotes")
+    @argument("vrf", description="VRF to trace path in")
+    def summarize(self, src: str = "", dest: str = "", vrf: str = ''):
+        """Summarize paths between specified from source to target ip addresses"""
+        # Get the default display field names
+        if self.columns is None:
+            return
+
+        now = time.time()
+        if self.columns != ["default"]:
+            self.ctxt.sort_fields = None
         else:
-            df = df.query('table != "TOTAL"') \
-                .nlargest(sqTopCount, columns=what, keep="all") \
-                .head(sqTopCount)
+            self.ctxt.sort_fields = []
 
-        return df[fields]
+        try:
+            df = self.sqobj.summarize(
+                hostname=self.hostname, columns=self.columns,
+                namespace=self.namespace, source=src, dest=dest,
+                vrf=vrf
+            )
+        except Exception as e:
+            df = pd.DataFrame({'error': ['ERROR: {}'.format(str(e))]})
+
+        self.ctxt.exec_time = "{:5.4f}s".format(time.time() - now)
+        if not df.empty:
+            return self._gen_output(df)
+
+    @command("unique", help="find the list of unique items in a column")
+    def unique(self, **kwargs):
+
+        msg = 'ERROR: Unique not supported for this object'
+        df = pd.DataFrame({'error': [msg]})
+        return self._gen_output(df, dont_strip_cols=True)
```

### Comparing `suzieq-0.22.0rc1/suzieq/engines/pandas/topology.py` & `suzieq-0.8.0/suzieq/utilities/sq-anonymize.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,403 +1,406 @@
-from dataclasses import dataclass
-from typing import List
+#!/usr/bin/env python
 
-import networkx as nx
-import numpy as np
-import pandas as pd
-
-from suzieq.engines.pandas.engineobj import SqPandasEngine
-from suzieq.shared.utils import build_query_str
-
-# TODO:
-# topology for different VRFs?
-# iBGP vs eBGP?
-# color by device type?
-# physical topology without LLDP -- is this possible?
-# how to draw multiple topologies
-# be able to ask if a node has neighbors by type (physical, overlay, protocol,
-# etc) questions
-# * without knowing hierarchy, labels or tags it's unclear how to group things
-#   for good picture
-# how could we add state of connection (like Established) per protocol
-
-
-class TopologyObj(SqPandasEngine):
-    '''Backend class to operate on virtual table, topology, with pandas'''
-
-    def __init__(self, baseobj):
-        super().__init__(baseobj)
-        self.lsdb = pd.DataFrame()
-        self._a_df = pd.DataFrame()
-        self._ip_table = pd.DataFrame()
-
-    @staticmethod
-    def table_name():
-        '''Table name'''
-        return 'topology'
-
-    # pylint: disable=attribute-defined-outside-init
-    def _init_dfs(self, namespaces):
-        """Initialize the dataframes used for the given namespace"""
-
-        self._if_df = self._get_table_sqobj('interfaces') \
-            .get(namespace=namespaces, state="up",
-                 columns=['namespace', 'hostname', 'ifname', 'ipAddressList',
-                          'ip6AddressList', 'state', 'type', 'master',
-                          'macaddr'])
+import os
+try:
+    import simplejson as json
+except ModuleNotFoundError:
+    import json
+import re
+import time
+import argparse
+from pathlib import Path
+from netconan.ip_anonymization import IpAnonymizer, IpV6Anonymizer
+from netconan.ip_anonymization import anonymize_ip_addr
+from collections import defaultdict
+from faker import Factory
+from jsonpath_ng import parse
+
+
+class SqAnonymizer(object):
+    """Suzieq Gather-Once output Anonymizer Class
+
+    This class implements the anonymizer for the Suzieq run-once=gather output
+    format. This anonymizes:
+    - IP adddresses (v4 and v6)
+    - MAC addresses (in NXOS/EOS or standard format)
+    - Hostnames (FQDN or otherwise)
+
+    The workflow is to point either a single file to anonymize or a directory
+    of files to anonymize. If its a directory, it only attempts to anonymize
+    the files with .output filename and excludes those ending with _anon,output
+    For every file in the directory, it produces the equivalent _anon.output
+    file that contains the anonymized data. For example, lldp.output is turned
+    into lldp_anon.output, device.output is turned into device_anon.output and
+    so on. The _anon.output file is in the run-once=gather format.
+
+    Since hostnames can appear anywhere, and do not have a unique format, we
+    require users to provide additional information. This information consists
+    of a JSONpath expression to the key that holds hostname or a prefix string
+    that comes before every hostname. The former is required for JSON outputs &
+    the latter for non-JSON output. This model is followed for all data that
+    has a non-unique format such as ASNs, VRF names and so on. This is also
+    true of MAC addresses in the EOS/NXOS format.
+
+    To ensure the same output when run at different times, the user must
+    provide a seed that remains the same across different runs. Otherwise, we
+    pick the time of day as the seed which produces different outputs when run
+    at diff times.
+    """
+
+    def __init__(self, seed: int = 0, preserve_v4_prefix: list = []):
+        """Initiaize the anonymizer with a seed"""
+
+        if not seed:
+            seed = int(time.time())
+
+        preserve_v4_prefix.append('0.0.0.0/0')
+        self.fakeit = Factory.create()
+        self.fakeit.seed(seed)
+        salt = self.fakeit.password(length=16)
+        self.anonv4 = IpAnonymizer(salt, preserve_prefixes=preserve_v4_prefix)
+        self.anonv6 = IpV6Anonymizer(salt)
+        self.hostmap = {}
+        self.macmap = defaultdict(self.fakeit.mac_address)
+
+        # Courtesy of Stackoverflow
+        # (https://stackoverflow.com/questions/1418423/the-hostname-regex)
+        self.hname_re = r'([a-zA-Z0-9](?:(?:[_a-zA-Z0-9-]*|(?<!-)\.(?![-.]))*[_a-zA-Z0-9]+)?)'
+
+        # This regex will not catch the macaddr in this format:
+        # "This is a macaddr:00:01:02:FF:cf:9b"
+        # because the macaddr is preceded by :. It will also not match:
+        # "00:01:29:AB:cf:47:01" because there's one more group (:01) after
+        # the mac address
+        self.macaddr_re = r'(?<!:)([0-9a-f]{2}(?::[0-9a-f]{2}){5})(?!:)'
+
+        # NXOS and EOS use this format
+        self.nxos_macaddr_re = r'([0-9A-F]{4}\.[0-9A-F]{4}\.[0-9A-F]{4})'
+
+        self.preset_hostname_jpaths = [
+            ['TABLE_nbor.ROW_nbor[*].chassis_id'],  # NXOS LLDP
+            # NXOS CDP
+            ['TABLE_cdp_neighbor_brief_info.ROW_cdp_neighbor_brief_info[*].device_id'],
+            ['lldpNeighbors.*.lldpNeighborInfo[*].systemName'],  # EOS
+            ['lldp[*].interface[*].chassis[*].name[*].value'],  # lldpd
+            ['lldp-neighbors-information.[0].lldp-neighbor-information[*].lldp-remote-system-name.[0].data'],  # JunOS
+            ['*.*.neighborCapabilities[*].hostName.advHostName'],  # FRR BGP
+            ['*.*.neighborCapabilities[*].hostName.rcvHostName'],  # FRR BGP
+            ['*.*.neighborCapabilities[*].hostName.advDomainName'],  # FRR BGP
+            ['*.*.neighborCapabilities[*].hostName.rcvDomainName'],  # FRR BGP
+            ['host_name']          # NXOS show version output
+        ]
 
-        if self._if_df.empty:
-            return
+        self.preset_hostname_pfxlst = [
+            ['SysName:'],
+            ['Static hostname:'],
+        ]
 
-        self._if_df['vrf'] = self._if_df.apply(
-            lambda x: x['master'] if x['type'] not in ['bridge', 'bond_slave']
-            else 'default', axis=1)
-        self._if_df['vrf'] = np.where(self._if_df['vrf'] == '', 'default',
-                                      self._if_df['vrf'])
-        self._if_df = self._if_df.explode('ipAddressList') \
-                                 .explode('ip6AddressList') \
-                                 .fillna({'ipAddressList': '0.0.0.0/0',
-                                          'ip6AddressList': '::0/0'})
-        self._if_df['plen'] = self._if_df.ipAddressList.str.split('/').str[1]
-        self._if_df['ipAddress'] = self._if_df.ipAddressList.str.split(
-            '/').str[0]
-        self._if_df = self._if_df.drop(
-            columns=['ipAddressList', 'ip6AddressList'])
-
-        self.lsdb = pd.DataFrame()
-
-    # pylint: disable=too-many-statements
-    def get(self, **kwargs):
-        '''DIsplay the topology info'''
-
-        @dataclass(frozen=True)
-        class Services:
-            '''minor class for use below. Could have been a named tuple'''
-            name: str
-            extra_args: dict
-            extra_cols: list
-            augment: any
-
-        self._namespaces = kwargs.get("namespace", self.ctxt.namespace)
-        hostname = kwargs.pop('hostname', [])
-        user_query = kwargs.pop('query_str', '')
-        polled = kwargs.pop('polled', '')
-        via = kwargs.pop('via', [])
-        ifname = kwargs.pop('ifname', '')
-        peerHostname = kwargs.pop('peerHostname', [])
-        columns = kwargs.pop('columns', ['default'])
-        asn = kwargs.pop('asn', '')
-        area = kwargs.pop('area', '')
-        vrf = kwargs.pop('vrf', '')
-        afi_safi = kwargs.pop('afiSafi', '')
-
-        if via == ['bgp'] and ifname:
-            self.lsdb = pd.DataFrame(
-                {'error': ["Cannot use 'ifname' filter with 'bgp' via"]})
-            return self.lsdb
-
-        self._init_dfs(self._namespaces)
-        if self._if_df.empty:
-            return pd.DataFrame({'error': ['No interfaces data found']})
-
-        fields = self.schema.get_display_fields(columns)
-
-        if (asn or afi_safi) and area:
-            raise AttributeError(
-                'Cannot provide asn/afiSafi and area at the same time')
-
-        if any(x in columns for x in ['asn', 'afiSafi']) or asn or afi_safi:
-            # When you don't constrain the via to bgp when asn is explicitly
-            # requested, we can have some issues. unique or any sort of sorting
-            # on the asn column will fail because all rows without BGP == true
-            # will have asn as either an undefined value, 0 or blank. The net
-            # result of this will be to confuse the user. Think of all the pain
-            # automation scripts will have to endure for this.
-            if via and via != ['bgp']:
-                raise AttributeError(
-                    'Cannot provide any via except bgp with asn')
-            via = ['bgp']
-
-        if area or 'area' in columns:
-            if via and via != ['ospf']:
-                raise AttributeError(
-                    'Cannot provide any via except ospf with area')
-            via = ['ospf']
-
-        if not via:
-            via = ['lldp', 'bgp', 'ospf']
-
-        self.services = [
-            Services('lldp', {}, ['ifname', 'vrf'],
-                     self._augment_lldp_show),
-            Services('arpnd', {},
-                     ['ipAddress', 'macaddr', 'ifname', 'vrf', 'arpndBidir'],
-                     self._augment_arpnd_show),
-            Services('bgp', {'state': 'Established', 'asn': asn,
-                             'afiSafi': afi_safi, 'vrf': vrf,
-                             'columns': ['*']},
-                     ['vrf', 'asn', 'peerAsn'],
-                     self._augment_bgp_show),
-            # Services('evpnVni', {}, 'peerHostname',
-            #    'vni', self._augment_evpnvni_show),
-            Services('ospf', {'state': 'full', 'area': area, 'vrf': vrf},
-                     ['ifname', 'vrf', 'area'], self._augment_ospf_show),
+        # Needed for NXOS and EOS which use the non-standard MACADDR format
+        self.preset_macaddr_jpaths = [
+            ['configMacAddress'],  # EOS show version output
+            ['systemMacAddress'],  # EOS show version output
+            ['hwMacAddress'],      # EOS show version output
         ]
 
-        if via:
-            self.services = [x for x in self.services if x.name in via]
-        key = 'peerHostname'
-
-        for srv in self.services:
-            if 'columns' not in srv.extra_args:
-                srv.extra_args['columns'] = ['default']
-            extra_cols = list(srv.extra_cols)
-            df = self._get_table_sqobj(srv.name).get(
-                **kwargs,
-                **srv.extra_args
-            )
-            if not df.empty:
-                if srv.augment:
-                    df = srv.augment(df)
-                cols = ['namespace', 'hostname', key]
-                if extra_cols:
-                    cols = cols + extra_cols
-                df = df[cols]
-                df.insert(len(df.columns), srv.name, True)
-                if self.lsdb.empty:
-                    self.lsdb = df
-                else:
-                    self.lsdb = self.lsdb.merge(df, how='outer')
+    def anonymize(self, file_or_dir: str, anonymize_ip=True,
+                  anonymize_mac=True, anonymize_hostname=True,
+                  host_prefixes: list = [], host_jpath: list = [],
+                  mac_jpath: list = []):
+        """Anonymizes the parameters desired in the given input file/dir """
+
+        self.host_jpath = (host_jpath or []) + self.preset_hostname_jpaths
+        self.host_pfxlst = (host_prefixes or []) + self.preset_hostname_pfxlst
+        self.mac_jpath = (mac_jpath or []) + self.preset_macaddr_jpaths
+
+        if os.path.isfile(file_or_dir):
+            self.anonymize_file(file_or_dir, host_prefixes,
+                                host_jpath, mac_jpath)
+        else:
+            # Invoke the command for each file in the directory
+            for file in Path(file_or_dir).glob('*.output'):
+                if str(file).endswith('_anon.output'):
+                    continue
+                self.anonymize_file(file, host_prefixes, host_jpath, mac_jpath)
+
+    def anonymize_file(self, file: str, host_pfxlst: list,
+                       host_jpath: list, mac_jpath, anonymize_ip=True,
+                       anonymize_mac=True, anonymize_hostname=True):
+        """Anonymize an individual file"""
+
+        name, suffix = os.path.basename(file).split('.')
+        dirname = os.path.dirname(file)
+        anon_fname = f'{dirname}/{name}_anon.{suffix}'
+
+        with open(file, 'r') as f:
+            data = f.read()
+
+        # Prepare output file by truncating it
+        with open(anon_fname, 'w') as f:
+            f.write('')
+
+        # The run-once= gather output is not proper JSON. Its
+        # written out as a list of entries, but there's no
+        # overarching list covering this list. So, we have to
+        # handcraft the entries to get them to be readable as
+        # JSON. The first entry is missing an ending ']' and the
+        # last entry is missing an opening '[' while the intermediate
+        # entries are missing both the starting and ending '['.
+        entries = re.split(r'\]\n*\[', data)
+        entlen = len(entries)
+        new_entries = []
+
+        for i, elem in enumerate(entries):
+            newelem = elem.replace('\n', '').strip()
+            if i == 0:
+                newelem = newelem + ']'
+            elif i == entlen - 1:
+                newelem = '[' + newelem
             else:
-                self.lsdb[srv.name] = False
+                newelem = '[' + newelem + ']'
 
-        self.lsdb = self.lsdb.fillna('').reset_index(drop=True)
-        self._find_polled_neighbors(polled)
-        if self.lsdb.empty:
-            return self.lsdb
-
-        if 'ipAddress' not in self.lsdb.columns:
-            self.lsdb['ipAddress'] = ''
-
-        self.lsdb = self.lsdb[~self.lsdb.hostname.isna()] \
-                        .drop_duplicates() \
-                        .rename({'ipAddress': 'peerIP', 'macaddr': 'peerMac'},
-                                axis=1, errors='ignore') \
-                        .dropna(subset=['peerHostname', 'peerIP'], how='all') \
-                        .fillna({'peerHostname': 'unknown',
-                                 'ifname': 'unknown', 'arpnd': False,
-                                 'peerIP': '', 'peerMac': '',
-                                 'arpndBidir': False,
-                                 'bgp': False, 'ospf': False,
-                                 'lldp': False, 'vrf': 'N/A'})
-
-        self.lsdb['vrf'] = np.where(self.lsdb.vrf == "bridge", "-",
-                                    self.lsdb.vrf)
-        self.lsdb['peerHostname'] = np.where(
-            self.lsdb.peerHostname == "unknown", self.lsdb.peerIP,
-            self.lsdb.peerHostname)
-        self.lsdb = self.lsdb.drop(columns=['peerIP', 'peerMac'],
-                                   errors='ignore')
-        self.lsdb = self.lsdb.query('peerHostname != ""')
-
-        # Apply the appropriate filters
-        if not self.lsdb.empty:
-            self.lsdb = self.lsdb.fillna('')
-            query_str = build_query_str([], self.schema, ignore_regex=False,
-                                        hostname=hostname,
-                                        peerHostname=peerHostname,
-                                        ifname=ifname, asn=asn, area=area,
-                                        vrf=vrf)
-            if query_str:
-                self.lsdb = self.lsdb.query(query_str)
+            try:
+                jelem = json.loads(newelem)
+                new_entries.append(jelem)
+            except Exception as e:
+                print(f"JSON load of {i} item failed with error {str(e)}")
+                jelem = []
+
+            for item in jelem:
+                # Populate the host name anonymizer as much as possible
+                item['hostname'] = re.sub(self.hname_re, self.get_anonhost,
+                                          item['hostname'])
+        for jelem in new_entries:
+
+            for item in jelem:
+                if isinstance(item['data'], str):
+                    try:
+                        jdata = json.loads(item['data'])
+                        is_json = True
+                    except json.decoder.JSONDecodeError:
+                        # non-JSON command output
+                        jdata = item['data']
+                        is_json = False
+                elif isinstance(item['data'], dict):
+                    # EOS LLDP output looks like this
+                    jdata = item['data']
+                    is_json = True
+
+                anondata = ''
+                if jdata:
+                    if is_json:
+                        anondata = json.dumps(jdata)
+                    else:
+                        anondata = jdata
 
-        if user_query and not self.lsdb.empty:
-            self.lsdb = self._handle_user_query_str(self.lsdb, user_query)
+                if anonymize_mac:
+                    anondata = self.anonymize_mac(
+                        self.macmap, anondata, is_json)
 
-        fields = [x for x in fields if x in self.lsdb.columns]
-        return self.lsdb[fields].reset_index(drop=True)
+                if anonymize_ip:
+                    anondata = self.anonymize_ip(item, anondata)
 
-    def _find_polled_neighbors(self, polled):
-        if self.lsdb.empty:
-            return
+                if anonymize_hostname:
+                    anondata = self.anonymize_hostname(item, anondata,
+                                                       is_json)
 
-        hosts = set(self.lsdb.hostname)
-        peer_hosts = set(self.lsdb.peerHostname)
-        unpolled_neighbors = peer_hosts.difference(hosts)
-
-        self.lsdb['polled'] = True
-        self.lsdb.loc[self.lsdb.peerHostname.isin(unpolled_neighbors),
-                      'polled'] = False
-
-        if polled and polled.lower() == 'true':
-            self.lsdb = self.lsdb.query('polled')
-        elif polled.lower() == 'false':
-            self.lsdb = self.lsdb.query('~polled')
-
-    def _create_graphs_from_lsdb(self):
-        self.graphs = {}
-        for ns, df in self.lsdb.groupby(by=['namespace']):
-            attrs = [srv.name for srv in self.services
-                     if srv.name in df.columns]
-            self.graphs[ns] = nx.from_pandas_edgelist(
-                df, 'hostname', 'peerHostname', attrs, nx.MultiGraph)
-
-    # TODO: eventually this needs to move to ospf after we figure out the
-    #   schema augmentation story
-    def _augment_ospf_show(self, df):
-        if not df.empty:
-            df = df.query('adjState != "passive"').reset_index(drop=True)
-            df['area'] = df['area'].astype(str)
-        return df
-
-    def _augment_lldp_show(self, df):
-        if not df.empty and not self._if_df.empty:
-            df = df[df.peerHostname != '']
-            df = df.merge(
-                self._if_df[['namespace', 'hostname', 'ifname', 'vrf']],
-                on=['namespace', 'hostname', 'ifname'], how='outer')
-
-        return df
-
-    def _augment_bgp_show(self, df):
-        return df
-
-    def _augment_evpnvni_show(self, df):
-        if not df.empty:
-            df = df.explode('remoteVtepList').dropna(how='any')
-            df = df.rename(columns={'remoteVtepList': 'peerIP'})
-            df = df.merge(self.ip_table, on=['namespace', 'peerIP'],
-                          how='left').dropna(how='any').drop_duplicates()
-        return df
-
-    def _augment_arpnd_show(self, df):
-
-        if not df.empty:
-            # weed out entries that are not reachable
-            df = df.query('state != "failed"').reset_index(drop=True)
-            # Get the VRF
-            df = df.merge(
-                self._if_df[['namespace', 'hostname', 'ifname', 'master']],
-                left_on=['namespace', 'hostname', 'oif'],
-                right_on=['namespace', 'hostname', 'ifname'],
-                suffixes=['', '_y'], how='outer') \
-                .rename(columns={'master': 'vrf'}) \
-                .dropna(subset=['ipAddress'])
-
-            df['vrf'] = np.where(df['vrf'] == '', 'default', df['vrf'])
-            df = df.drop(columns=['vlan', 'oif', 'mackey', 'remoteVtepIp',
-                                  'timestamp_y'], errors='ignore')
-
-            # address are where I find the neighbor, these own the mac
-            addr = self.address_df[['namespace', 'hostname', 'macaddr']] \
-                .drop_duplicates() \
-                .rename(columns={'hostname': 'peerHostname'})
-            df = df.merge(addr, on=['namespace', 'macaddr'], how='left') \
-                   .dropna(subset=['hostname', 'ipAddress']) \
-                   .rename(columns={'oif': 'ifname'}) \
-                   .drop_duplicates()
-
-            # Use MAC table entries to find the local port for a MAC on an SVI
-            mac_df = self._get_table_sqobj('macs')\
-                         .get(namespace=self._namespaces, local=True,
-                              columns=['namespace', 'hostname', 'vlan',
-                                       'macaddr', 'oif', 'remoteVtepIp'])
-            df = df.merge(mac_df,
-                          on=['namespace', 'hostname', 'macaddr'],
-                          how='outer') \
-                .dropna(subset=['hostname'])
-            df['ifname'] = np.where(
-                df['oif'].isnull(), df['ifname'], df['oif'])
-
-            df['arpndBidir'] = df.apply(
-                lambda x, y:
-                not y.query(f'namespace=="{x.namespace}" and '
-                            f'hostname=="{x.peerHostname}" and '
-                            f'peerHostname=="{x.hostname}"').empty,
-                args=(df,), axis=1)
-
-        self._arpnd_df = df
-        return self._arpnd_df
-
-    @property
-    def address_df(self) -> pd.DataFrame():
-        '''Return pandas dataframe of the address table'''
-
-        if self._a_df.empty:
-            self._a_df = self._if_df
-        return self._a_df
-
-    @property
-    def ip_table(self):
-        '''Return a dataframe of '''
-        if self._ip_table.empty:
-            addr = self.address_df
-            if not addr.empty:
-                self._ip_table = addr[['namespace',
-                                       'hostname', 'ipAddressList']]
-                self._ip_table = self._ip_table.explode(
-                    'ipAddressList').dropna(how='any')
-                self._ip_table = self._ip_table \
-                                     .rename(
-                                         columns={'ipAddressList': 'peerIP',
-                                                  'hostname': 'peerHostname'})
-                self._ip_table['peerIP'] = self._ip_table['peerIP'] \
-                                               .str.replace("/.+", "")
-                self._ip_table = \
-                    self._ip_table[self._ip_table['peerIP'] != '-']
-        return self._ip_table
-
-    def summarize(self, **kwargs):
-        '''Summarize the topology info'''
-        self.get(**kwargs)
-        if self.lsdb.empty or 'error' in self.lsdb:
-            return self.lsdb
-
-        namespaces = self.lsdb['namespace'].unique()
-
-        self.ns = {}
-        for i in namespaces:
-            self.ns[i] = {}
-        self._create_graphs_from_lsdb()
-        self._analyze_lsdb_graph(namespaces)
-
-        return pd.DataFrame(self.ns)
-
-    def _analyze_lsdb_graph(self, namespaces: List[str]):
-        for ns in namespaces:
-            for name in [srv.name for srv in self.services if
-                         nx.get_edge_attributes(self.graphs[ns], srv.name)]:
-
-                G = nx.Graph([(s, d, data) for s, d, data in
-                              self.graphs[ns].edges(data=True)
-                              if data[name] is True])
-                if G.nodes:
-                    self.ns[ns][f'{name}_number_of_nodes'] = len(G.nodes)
-                    self.ns[ns][f'{name}_number_of_edges'] = len(G.edges)
-                    if not nx.is_connected(G):
-                        self.ns[ns][f'{name}_is_fully_connected'] = False
-                        self.ns[ns][f'{name}_center'] = False
-                    else:
-                        self.ns[ns][f'{name}_is_fully_connected'] = True
-                        self.ns[ns][f'{name}_center'] = nx.barycenter(G)
+                if anondata:
+                    item['data'] = anondata
+
+            # Append each entry
+            with open(anon_fname, 'a') as f:
+                f.write(json.dumps(jelem, indent=4))
+
+    def anonymize_ip(self, item: dict, anondata: str) -> str:
+        """Anonymize the IP address in the data and in the item header
+
+        Anonymize the IP addresses, v4 and v6, in the supplied data. Also
+        anonymize the IP address in the data header. Both are specific to the
+        run-once=gather format of Suzieq
+        """
+        item['address'] = anonymize_ip_addr(self.anonv4, item['address'])
+        item['address'] = anonymize_ip_addr(self.anonv6, item['address'])
+
+        if not anondata:
+            return anondata
 
-                    self.ns[ns][f'{name}_self_loops'] = list(
-                        nx.nodes_with_selfloops(G))
+        anondata = anonymize_ip_addr(self.anonv4, anondata, False)
+        anondata = anonymize_ip_addr(self.anonv6, anondata, False)
 
-                    self.ns[ns][f'{name}_number_of_disjoint_sets'] = len(
-                        list(nx.connected_components(G)))
+        return anondata
+
+    def anonymize_mac(self, macmap, anondata: str, is_json: bool) -> str:
+        """Anonymize the MAC address in the data and in the item header
+
+        Both are specific to the run-once=gather format of Suzieq
+        """
+        def nxos_mac_sub(match):
+            newmac = macmap[match.group(1)]
+            newmac = newmac.split(':')
+            newmac = (''.join(newmac[0:2]) + '.' + ''.join(newmac[2:4]) + '.' +
+                      ''.join(newmac[4:]))
+            return newmac
+
+        def jp_anon_macaddr(orig_v, orig_kv, orig_k):
+            """JSONPATH update macaddress in NXOS/EOS format"""
+            orig_kv[orig_k] = macmap[orig_v]
+
+        if not anondata:
+            return
+
+        anondata = re.sub(self.macaddr_re,
+                          lambda x: macmap[x.group(1)],
+                          anondata, flags=re.IGNORECASE)
+
+        anondata = re.sub(self.nxos_macaddr_re, nxos_mac_sub, anondata,
+                          flags=re.IGNORECASE)
+
+        if is_json:
+            janon = json.loads(anondata)
+            for path in self.mac_jpath:
+                jp = parse(path[0])
+                jp.update(janon, jp_anon_macaddr)
+            anondata = json.dumps(janon)
+
+        return anondata
+
+    def get_anonhost(self, host: str) -> str:
+        """Check various conditions to return the anonymized hostname.
+
+        Sometimes hostnames are present without FQDN and sometimes with.
+        We want to map them consistently to the same anonymized hostname.
+        We won't know which format we'll encounter first and so we have to
+        handle that as well. Hence this routine
+        """
+
+        if not host:
+            return host
+
+        if isinstance(host, re.Match):
+            orighost = host.group(1)
+        else:
+            orighost = host
+
+        helem = orighost.split('.')
+        anonhost = self.hostmap.get(orighost, '')
+        if not anonhost and len(helem) > 1:
+            anonhost = self.hostmap.get(helem[0], '')
+
+        if not anonhost:
+            anonhost = self.fakeit.hostname()
+            if len(helem) > 1:
+                self.hostmap[orighost] = anonhost
+                self.hostmap[helem[0]] = anonhost
+            else:
+                self.hostmap[orighost] = anonhost
+
+        if len(helem) == 1:
+            return anonhost.split('.')[0]
+        else:
+            return anonhost
+
+    def anonymize_hostname(self, item: dict, anondata: str, is_json: bool) \
+            -> str:
+        """Anonymize the hostname in the item header and the data
+
+        """
+
+        def anon_hostname(match):
+            newhostname = self.get_anonhost(match.group(1))
+            if is_json:
+                return f'"{kwd[0]}": "{newhostname}"'
+            else:
+                return f'{kwd[0]} {newhostname}'
 
-                    self.ns[ns][f'{name}_degree_histogram'] = \
-                        nx.degree_histogram(G)
-
-                    # too many degrees => the column gets too big
-                    if len(self.ns[ns][f'{name}_degree_histogram']) > 6:
-                        self.ns[ns][f'{name}_degree_histogram'] = '...'
-
-                else:
-                    for k in [f'{name}_is_fully_connected', f'{name}_center',
-                              f'{name}_self_loops',
-                              f'{name}_number_of_disjoint_sets',
-                              f'{name}_degree_histogram',
-                              f'{name}_number_of_nodes',
-                              f'{name}_number_of_edges']:
-                        self.ns[ns][k] = None
+        def jp_anon_hostname(orig_v, orig_kv, orig_k):
+            """JSONPATH update hostname"""
+            if orig_v == 'n/a':  # handle null domainname in FRR BGP
+                return
+            orig_kv[orig_k] = self.get_anonhost(orig_v)
+
+        if not anondata:
+            return anondata
+
+        if is_json:
+            janon = json.loads(anondata)
+            for path in self.host_jpath:
+                jp = parse(path[0])
+                jp.update(janon, jp_anon_hostname)
+            anondata = json.dumps(janon)
+        else:
+            for kwd in self.host_pfxlst:
+                hpat = r'{}\s+{}'.format(kwd[0], self.hname_re)
+                anondata = re.sub(hpat, anon_hostname, anondata)
+
+        # The hostname shows up in strange places and so do one more pass with
+        # their hostnames we have to see if we can catch those entries
+        for hostname in self.hostmap:
+            anondata = anondata.replace(hostname, self.hostmap[hostname])
+        return anondata
+
+    def dump_mappings(self, file_or_dir) -> None:
+        """Dump the mappings of various fields into a file"""
+
+        if os.path.isdir(file_or_dir):
+            dirname = file_or_dir
+        else:
+            dirname = os.path.dirname(os.path.abspath(file_or_dir))
+
+        with open(f'{dirname}/mapping.txt', 'w') as f:
+            for k, v in self.hostmap.items():
+                f.write(f'{k}\t{v}\n')
+            for k, v in self.macmap.items():
+                f.write(f'{k}\t{v}\n')
+            self.anonv4.dump_to_file(f)
+            self.anonv6.dump_to_file(f)
+
+
+if __name__ == '__main__':
+
+    parser = argparse.ArgumentParser(
+        description="Anonymize suzieq run-once data files")
+    parser.add_argument(
+        "-i",
+        "--input",
+        type=str, required=True,
+        help="Directory of files or single File to anonymize",
+    )
+    parser.add_argument(
+        "-s",
+        "--seed",
+        type=str,
+        help="Value to seed the randomizer with"
+    )
+    parser.add_argument(
+        "-ph",
+        "--host-prefix",
+        nargs="+", action='append',
+        help="Keywords preceding hostname to anonymize hostname (non-JSON output)",
+    )
+    parser.add_argument(
+        "-PH",
+        "--host-jpath",
+        nargs="+", action='append',
+        help=("JSON path to get to hostname in JSON output (use option "
+              "multiple times to provide multiple values)")
+    )
+    parser.add_argument(
+        "-PM",
+        "--mac-jpath",
+        nargs="+", action='append',
+        help=("JSON path to get to NXOS/EOS Macaddr in JSON output"
+              "Use option multiple times to provide multiple values")
+    )
+    parser.add_argument(
+        "-ip",
+        "--preserve-v4-prefixes",
+        nargs="+", action='append',
+        help=("IP address prefix to NOT anonymize (default is always incl)"
+              "Use option multiple times to provide multiple values")
+    )
+    userargs = parser.parse_args()
+
+    anonymizer = SqAnonymizer(userargs.seed)
+    anonymizer.anonymize(userargs.input, host_prefixes=userargs.host_prefix,
+                         host_jpath=userargs.host_jpath,
+                         mac_jpath=userargs.mac_jpath)
+    anonymizer.dump_mappings(userargs.input)
```

### Comparing `suzieq-0.22.0rc1/suzieq/engines/pandas/vlan.py` & `suzieq-0.8.0/suzieq/engines/pandas/vlan.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-from suzieq.engines.pandas.engineobj import SqPandasEngine
+import numpy as np
 
+from .engineobj import SqEngineObject
 
-class VlanObj(SqPandasEngine):
-    '''Backend class to handle manipulating VLAN table with pandas'''
 
-    @staticmethod
-    def table_name():
-        '''Table name'''
-        return 'vlan'
+class VlanObj(SqEngineObject):
 
     def get(self, **kwargs):
         """Get VLAN info based on specified keywords"""
 
         # ifname is a deprecated field, from version 1.0
         # vlanName is the correct fieldname. SO we need to do magic
         # to fix this. And thats why this routine exists
 
+        dropcols = []
+        addnl_fields = kwargs.pop('addnl_fields', [])
         columns = kwargs.pop('columns', [])
-
-        addnl_fields = []
-        fields = self.schema.get_display_fields(columns)
-        self._add_active_to_fields(kwargs.get('view', self.iobj.view), fields,
-                                   addnl_fields)
-        if 'ifname' not in fields:
+        if (columns != ['*'] and (columns == ['default'] or
+                                  'ifname' not in columns)):
             if 'ifname' not in addnl_fields:
                 addnl_fields.append('ifname')
+                dropcols.append('ifname')
 
-        df = super().get(addnl_fields=addnl_fields, columns=fields,
+        df = super().get(addnl_fields=addnl_fields,
                          merge_fields={'ifname': 'vlanName'},
                          **kwargs)
-        return df[fields]
+        if not df.empty:
+            df.drop(columns=dropcols, errors='ignore', inplace=True)
+
+        return df
 
     def summarize(self, **kwargs):
         """Describe the IP Address data"""
 
-        self._init_summarize(**kwargs)
+        self._init_summarize(self.iobj.table, **kwargs)
         if self.summary_df.empty:
             return self.summary_df
 
         self._summarize_on_add_field = [
             ('deviceCnt', 'hostname', 'nunique'),
             ('uniqueVlanCnt', 'vlan', 'nunique')
         ]
```

### Comparing `suzieq-0.22.0rc1/suzieq/gui/Suzieq-logo-2.jpg` & `suzieq-0.8.0/suzieq/gui/Suzieq-logo-2.jpg`

 * *Files identical despite different names*

### Comparing `suzieq-0.22.0rc1/suzieq/poller/worker/nodes/files.py` & `suzieq-0.8.0/suzieq/poller/nodes/files.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 #!/usr/bin/env python3
 
 import asyncio
 import re
 import json
 import logging
+import aiofiles
 from pathlib import Path
 from http import HTTPStatus
-from datetime import datetime, timezone
-import aiofiles
+from suzieq.poller.services.service import RsltToken
+from datetime import datetime
+
+
+async def init_files(gather_datadir: str):
+    """Given a data directory, return an initialized filenode object"""
+    node = FileNode()
+    tasks = [node._init(gather_datadir)]
+
+    await asyncio.gather(*tasks)
+
+    return ({node.hostname: node})
 
-from suzieq.poller.worker.services.service import RsltToken
 
+class FileNode(object):
 
-class FileNode:
-    '''Class using run-once=gather snapshot output as mock device input'''
+    async def _init(self, datadir: str):
 
-    # pylint: disable=attribute-defined-outside-init
-    async def initialize(self, datadir: str):
-        '''Load the data to be read from files'''
         self.logger = logging.getLogger(__name__)
         self.data = {}          # The dict of command to output entries
         self.hostname = '_filedata'  # Need this for the services
+        self.sigend = False
 
         self._service_queue = asyncio.Queue()
 
         await self._load_data(datadir)
 
     async def _load_data(self, datadir: str):
         """This routine walks the dir loading the data from the files there"""
@@ -37,55 +45,53 @@
             self.logger.error(f'No files to load found in {datadir}')
             return []
 
         await asyncio.gather(*tasks)
 
     async def _load_single_file_data(self, file: str):
         """Load gathered data from specified file
-        Each entry loaded from the file is a list entry with the format:
+        Each entry loaded from the file is a list entry of the following format:
         [{'status':...
          'timestamp': ...
          'cmd': ....
          'devtype': ...
          'namespace': ...
          'hostname': ...
          'address': ...
          'version': ...
          'data': ...}]
 
-        If the service consisted of multiple commands, then the format is a
-        list, where each entry in the list is of the above format.
+        If the service consisted of multiple commands, then the format is a list,
+        where each entry in the list is of the above format.
 
         We return a dictionary keyed on the command of the format:
         {cmd1: {curpos: 0, 'entry': <list of entries>},
          cmd2: {curpos: 0, 'entry': <list of entries>,
          ...
         } where each entry in the list is of the individual entry of the input
-        format. The basic idea is that when input is requested for a given cmd,
-        we return the entry at curpos and increment curpos. When curpos
-        exceeds the length of the entries, we reset it back to 0.
+        format. The basic idea is that when input is requested for a given command,
+        we return the entry at curpos and increment curpos. When curpos exceeds the
+        length of the entries, we reset it back to 0.
         """
         async with aiofiles.open(file, 'r') as f:
             data = await f.read()
 
         required_keys = ['status', 'timestamp', 'cmd', 'devtype', 'namespace',
-                         'hostname', 'address', 'version', 'data',
-                         'cmd_timestamp']
-        entries = re.split(r'\]\n*\[\n', data)
+                         'hostname', 'address', 'version', 'data']
+        entries = re.split(r'\]\n*\[', data)
         entlen = len(entries)
 
         for i, elem in enumerate(entries):
             newelem = elem.replace('\n', '').strip()
-            if entlen > 1:
-                if i == 0:
-                    newelem = newelem + ']'
-                elif i == entlen-1:
-                    newelem = '[' + newelem
-                else:
-                    newelem = '[' + newelem + ']'
+            if i == 0:
+                newelem = newelem + ']'
+            elif i == entlen-1:
+                newelem = '[' + newelem
+            else:
+                newelem = '[' + newelem + ']'
 
             jelem = None
             try:
                 jelem = json.loads(newelem)
             except json.decoder.JSONDecodeError:
                 # This is a bug in the output of FRR's show evpn vni when
                 # there's no EVPN
@@ -93,101 +99,76 @@
                     newelem = newelem[:-1]
                     jelem = json.loads(newelem)
 
             if jelem is None:
                 self.logger.error(f"Unable to decode JSON in file {file}")
                 continue
 
-            # Add backward compatibility for the files not having the
-            # cmd_timestamp field
-            data_keys = jelem[0].keys()
-            if 'cmd_timestamp' not in data_keys:
-                for record in jelem:
-                    record['cmd_timestamp'] = record['timestamp']
-
-            if not all(key in required_keys for key in data_keys):
+            if not all(key in required_keys for key in jelem[0].keys()):
                 self.logger.error(
                     f'Ignoring entry with missing required key fields {jelem}')
                 continue
 
-            key = jelem[0]['cmd'].split('|')[0].strip()
-
+            key = jelem[0]['cmd']
             if key not in self.data:
                 self.data[key] = {'curpos': 0, 'entry': []}
-
             self.data[key]['entry'].append(jelem)
 
     def post_commands(self, service_callback, svc_defn: dict,
                       cb_token: RsltToken):
-        '''Post command outputs back to service that requested them'''
-
         if cb_token:
             cb_token.nodeQsize = self._service_queue.qsize()
         self._service_queue.put_nowait([service_callback, svc_defn, cb_token])
 
     async def run(self):
-        '''Main workhorse routine, serving data from files based on command'''
 
         while True:
+            if self.sigend:
+                return
+
             request = await self._service_queue.get()
             # request consists of callback fn, service_defn string, cb_token
             if request:
                 if not await self.exec_service(request[0], request[1],
                                                request[2]):
                     return
 
     def _create_result(self, cmd, status, data) -> dict:
-        '''Create result object to be posted back to service object'''
-
         result = {
             "status": status,
-            "timestamp": int(datetime.now(tz=timezone.utc).timestamp() * 1000),
+            "timestamp": int(datetime.utcnow().timestamp() * 1000),
             "cmd": cmd,
             "devtype": 'Unknown',
             "namespace": 'Unknown',
             "hostname": self.hostname,
             "address": '0.0.0.0',
             "version": 0,
             "data": data,
         }
         return result
 
     async def exec_service(self, service_callback, svc_defn: dict,
-                           cb_token: RsltToken) -> bool:
-        '''This looks up the command, returns the output if available'''
-
-        def _add_cmd_to_cmdset(cmd: str, cmdset: set) -> None:
-            """Add a command to the set of commands to be executed"""
-            if isinstance(cmd, list):
-                # the first command is what we need
-                subcmd = cmd[0]['command'].split('|')[0].strip()
-                cmdset.add(subcmd)
-            else:
-                cmdset.add(cmd.split('|')[0].strip())
+                           cb_token: RsltToken):
 
         cmdset = set()
         for device in svc_defn.keys():
-            defn = svc_defn[device]
-            if isinstance(defn, list):
-                for elem in defn:
-                    cmd = elem.get('command', None)
-                    if not cmd:
-                        continue
-                    _add_cmd_to_cmdset(cmd, cmdset)
-            else:
-                cmd = defn.get('command', None)
-                if not cmd:
-                    continue
+            cmd = svc_defn[device].get('command', None)
+            if not cmd:
+                continue
 
-                _add_cmd_to_cmdset(cmd, cmdset)
+            if isinstance(cmd, list):
+                # the first command is what we need
+                cmdset.add(cmd[0]['command'])
+            else:
+                cmdset.add(cmd)
 
         nodata = True
         for cmd in cmdset:
             data_entry = self.data.get(cmd, {'entry': []})
-            for _ in range(len(data_entry['entry'])):
+            for i in range(len(data_entry['entry'])):
                 retdata = data_entry['entry'].pop()
                 await service_callback(retdata, cb_token)
                 nodata = False
         if nodata:
             await service_callback([self._create_result(
                 cmd, HTTPStatus.NO_CONTENT, [])], cb_token)
```

### Comparing `suzieq-0.22.0rc1/suzieq/poller/worker/services/evpnVni.py` & `suzieq-0.8.0/suzieq/poller/services/evpnVni.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,27 @@
 import re
 import numpy as np
 
-from suzieq.poller.worker.services.service import Service
-from suzieq.shared.utils import (convert_rangestring_to_list,
-                                 convert_macaddr_format_to_colon)
+from suzieq.poller.services.service import Service
+from suzieq.utils import convert_rangestring_to_list
 
 
 class EvpnVniService(Service):
     """evpnVni service. Different class because output needs to be munged"""
 
     def clean_json_input(self, data):
-        """evpnVni JSON output is busted across many NOS. Fix it"""
+        """FRR JSON data needs some work"""
 
         devtype = data.get("devtype", None)
         if any(x == devtype for x in ["cumulus", "sonic", "linux"]):
             data['data'] = '[' + re.sub(r'}\n\n{\n', r'},\n\n{\n',
                                         data['data']) + ']'
             return data['data']
-        elif devtype.startswith('junos'):
-            data['data'] = data['data'].replace('}, \n    }\n', '} \n    }\n')
-            return data['data']
-        elif devtype == "eos":
-            if data.get('cmd', '').startswith('show interfaces Vxlan $'):
-                if data['data'].startswith('%'):
-                    data['data'] = '{}'
-                    return data['data']
-        return data['data']
-
-    def _clean_eos_data(self, processed_data, _):
-        new_entries = []
-
-        if not processed_data:
-            return processed_data
-
-        for entry in processed_data:
-            vni2vrfmap = {}
-            for vrf in entry['_vrf2VniMap']:
-                vni2vrfmap[entry['_vrf2VniMap'][vrf]] = vrf
-
-            vtepMap = entry.get('_vlan2VtepMap', {})
-            replType = entry.get('replicationType')
-            mcastGroup = entry.get('mcastGroup', '')
-            if replType == 'headendVcs':
-                replType = 'ingressBGP'
-                entry['mcastGroup'] = '0.0.0.0'
-            elif mcastGroup and mcastGroup != "0.0.0.0":
-                replType = "multicast"
-            else:
-                replType = ''
-                entry['mcastGroup'] = '0.0.0.0'
-
-            for vlan in entry['_vlan2VniMap']:
-                new_entry = {}
-                vni = entry['_vlan2VniMap'][vlan].get('vni', 0)
-                new_entry['vni'] = vni
-                new_entry['vrf'] = vni2vrfmap.get(vni, '')
-                new_entry['state'] = entry['state']
-                new_entry['ifname'] = entry['ifname']
-                new_entry['vlan'] = vlan
-                new_entry['priVtepIp'] = entry['priVtepIp']
-                vteplist = vtepMap.get(vlan, {})
-                vteplist = (vteplist.get('remoteVtepAddr', []) +
-                            vteplist.get('remoteVtepAddr6', []))
-                new_entry['remoteVtepList'] = vteplist
-                new_entry['replicationType'] = replType
-                new_entry['mcastGroup'] = entry['mcastGroup']
-                if new_entry['vrf']:
-                    new_entry['type'] = 'L3'
-                else:
-                    new_entry['type'] = 'L2'
-                new_entry['ifname'] = entry.get('ifname', '')
-
-                new_entries.append(new_entry)
 
-        processed_data = new_entries
-        return processed_data
-
-    def _clean_cumulus_data(self, processed_data, _):
+    def _clean_cumulus_data(self, processed_data, raw_data):
         """Clean out null entries among other cleanup"""
 
         del_indices = []
         for i, entry in enumerate(processed_data):
             if entry['vni'] is None:
                 del_indices.append(i)
             if entry['mcastGroup'] and entry['mcastGroup'] != "0.0.0.0":
@@ -89,36 +30,34 @@
                 entry['replicationType'] = 'ingressBGP'
                 entry['mcastGroup'] = "0.0.0.0"
             else:
                 entry['replicationType'] = ''
                 entry['mcastGroup'] = "0.0.0.0"
                 entry['remoteVtepList'] = None
 
-            entry['state'] = entry.get('state', 'up').lower()
-            entry['l2VniList'] = set(entry['l2VniList'])
         processed_data = np.delete(processed_data, del_indices).tolist()
 
         return processed_data
 
-    def _clean_nxos_data(self, processed_data, _):
+    def _clean_nxos_data(self, processed_data, raw_data):
         """Merge peer records with VNI records to yield VNI-based records"""
 
         vni_dict = {}
         drop_indices = []
 
         for i, entry in enumerate(processed_data):
             if not entry['vni']:
                 drop_indices.append(i)
                 continue
 
             if entry['_entryType'] == 'VNI':
-                etype, vrf = entry['type'].split()
-                if etype == 'L3':
+                type, vrf = entry['type'].split()
+                if type == 'L3':
                     entry['vrf'] = vrf[1:-1]  # strip off '[' and ']'
-                entry['type'] = etype
+                entry['type'] = type
                 if 'sviState' in entry:
                     entry['state'] = entry['sviState'].split()[0].lower()
                 if re.search(r'[0-9.]+', entry.get('replicationType', '')):
                     entry['mcastGroup'] = entry['replicationType']
                     entry['replicationType'] = 'multicast'
                 elif entry['type'] != 'L3':
                     entry['replicationType'] = 'ingressBGP'
@@ -133,49 +72,45 @@
                 entry['vlan'] = int(entry['vlan'])
                 vni_dict[entry['vni']] = entry
 
             elif entry['_entryType'] == 'peers':
                 vni_list = convert_rangestring_to_list(
                     entry.get('_vniList', ''))
                 for vni in vni_list:
-                    vni_entry = vni_dict.get(vni, None)
+                    vni_entry = vni_dict.get(str(vni), None)
                     if vni_entry:
                         vni_entry['remoteVtepList'].append(entry['vni'])
                 drop_indices.append(i)
 
             elif entry['_entryType'] == 'iface':
                 if entry.get('encapType', '') != "VXLAN":
                     continue
 
-                for vni, val in vni_dict.items():
-                    if val['ifname'] != entry['ifname']:
+                for vni in vni_dict:
+                    if vni_dict[vni]['ifname'] != entry['ifname']:
                         continue
-                    val['priVtepIp'] = entry.get('priVtepIp', '')
+                    vni_dict[vni]['priVtepIp'] = entry.get('priVtepIp', '')
                     secIP = entry.get('secVtepIp', '')
                     if secIP == '0.0.0.0':
                         secIP = ''
-                    val['secVtepIp'] = secIP
-                    val['routerMac'] = \
-                        convert_macaddr_format_to_colon(
-                        entry.get('routerMac', '00:00:00:00:00:00'))
-
+                    vni_dict[vni]['secVtepIp'] = secIP
+                    vni_dict[vni]['routerMac'] = entry.get('routerMac',
+                                                           '00:00:00:00:00:00')
                 drop_indices.append(i)
 
         processed_data = np.delete(processed_data, drop_indices).tolist()
 
         return processed_data
 
-    def _clean_junos_data(self, processed_data, _):
+    def _clean_junos_data(self, processed_data, raw_data):
 
         newntries = {}
 
         for entry in processed_data:
             if entry['_entryType'] == 'instance':
-                if entry['_vniList'] is None:
-                    continue
                 for i, vni in enumerate(entry['_vniList']):
                     irb_iflist = entry.get('_irbIfList', [])
                     vrflist = entry.get('_vrfList', [])
                     vlan = entry['_vlanList'][i]
                     irbif = f'irb.{vlan}'
                     try:
                         index = irb_iflist.index(irbif)
@@ -200,35 +135,28 @@
                         }
                     newntries[vni] = vni_entry
                     continue
             elif entry['_entryType'] == 'l3':
                 vni = int(entry.get('vni', '0'))
                 priVtepIp = entry.get('priVtepIp', '')
 
-                if not priVtepIp and not vni:
-                    continue
-
                 vni_entry = {
                     'vni': vni,
                     'remoteVtepList': [],
                     'priVtepIp': priVtepIp,
                     'type': 'L3',
                     'state': 'up',
                     'numRemoteVteps': 0,
                     'routerMac': entry['routerMac'],
                     'numMacs': 0,
                     'numArpNd': 0,
                     'mcastGroup': '0.0.0.0',
                     'vrf': entry['vrf'],
                     'os': 'junos'
                 }
-                # Add the primary VTEP IP into the L2 entries as well
-                for _, val in newntries.items():
-                    val['priVtepIp'] = priVtepIp
-
                 newntries[vni] = vni_entry
                 continue
             elif entry['_entryType'] == 'remote':
                 priVtepIp = entry.get('priVtepIp', '[{"data": ""}]')[0]['data']
                 for i, vni in enumerate(entry.get('_vniList', [])):
                     vni_entry = newntries.get(vni, {})
                     if not vni_entry:
@@ -254,13 +182,7 @@
                         vni_entry['mcastGroup'] = entry['replicationType'][i]
 
                     vni_entry['remoteVtepList'].append(
                         entry.get('_floodVtepList', ''))
 
         processed_data = list(newntries.values())
         return processed_data
-
-    def _clean_sonic_data(self, processed_data, raw_data):
-        return self._clean_cumulus_data(processed_data, raw_data)
-
-    def _clean_linux_data(self, processed_data, raw_data):
-        return self._clean_cumulus_data(processed_data, raw_data)
```

### Comparing `suzieq-0.22.0rc1/suzieq/poller/worker/services/macs.py` & `suzieq-0.8.0/suzieq/poller/services/macs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,12 @@
+from suzieq.poller.services.service import Service
 import re
-
+from suzieq.utils import convert_macaddr_format_to_colon
 import numpy as np
 
-from suzieq.poller.worker.services.service import Service
-from suzieq.shared.utils import convert_macaddr_format_to_colon
-from suzieq.shared.utils import (expand_nxos_ifname, expand_eos_ifname,
-                                 expand_ios_ifname)
-
 
 class MacsService(Service):
     """Mac address service. Different class because of macaddr not in key"""
 
     def get_key_flds(self):
         """The MAC table in Linux can have weird keys"""
         return ['vlan', 'macaddr', 'oif', 'remoteVtepIp', 'bd']
@@ -22,202 +18,113 @@
         1. Cumulus has all 0 MAC address with different remoteVtepIP, but
            same VLAM, as ingress replication entries.
         2. Cumulus has interface MAC entries with the same MAC and VLAN 0
         3. Juniper's VPLS entries have only BD, no VLAN
         4. The remaining regular entries where VLAN disambiguates a MAC.
         """
         # Make VLAN int first
-        vlan = entry.get('vlan', '0')
-        if vlan:
-            if isinstance(vlan, str):
-                if not vlan.isnumeric():
-                    vlan = '0'
-
-                entry['vlan'] = int(vlan)
-        else:
-            vlan = 0
-            entry['vlan'] = 0
+        if entry.get('vlan', ''):
+            entry['vlan'] = int(entry['vlan'])
 
         if entry.get('bd', ""):
+            # VPLS Entry
             if not entry.get('vlan', 0):
                 entry['mackey'] = entry['bd']
             else:
                 entry['mackey'] = f'{entry["bd"]}-{entry["vlan"]}'
         else:
-            if entry.get("remoteVtepIp", ''):
+            if not entry.get("remoteVtepIp", ''):
                 if entry['macaddr'] == '00:00:00:00:00:00':
-                    entry['mackey'] = f'{entry["oif"]}-{entry["remoteVtepIp"]}'
-                elif entry['vlan']:
-                    entry['mackey'] = entry['vlan']
+                    entry['mackey'] = f'{entry["vlan"]}-{entry["remoteVtepIp"]}'
                 else:
-                    entry['mackey'] = entry['oif']
+                    entry['mackey'] = entry['vlan']
             else:
-                if vlan:
-                    if entry['flags'] in ['static', 'permanent', 'router']:
-                        entry['mackey'] = f'{vlan}-{entry["oif"]}'
-                    else:
-                        entry['mackey'] = vlan
+                if entry.get('vlan', 0):
+                    entry['mackey'] = entry['vlan']
                 else:
-                    if entry['flags'] in ['static', 'permanent', 'router']:
-                        entry['mackey'] = f'{entry["oif"]}'
-                    else:
-                        entry['mackey'] = '0'
+                    entry['mackey'] = f'{entry["vlan"]}-{entry["oif"]}'
 
-    def _clean_linux_data(self, processed_data, _):
+    def _clean_linux_data(self, processed_data, raw_data):
         drop_indices = []
         macentries = {}
         for i, entry in enumerate(processed_data):
             macaddr = entry.get('macaddr', None)
             oif = entry.get('oif', '')
             if macaddr and (macaddr != "00:00:00:00:00:00"):
                 key = f'{macaddr}-{oif}'
-
                 old_entry = macentries.get(key, None)
                 if not old_entry:
                     macentries[key] = entry
                 elif not (old_entry['vlan'] and entry['vlan']):
                     # Ensure we don't munge entries with the diff valid VLANs
                     if not old_entry.get('vlan', ''):
                         old_entry['vlan'] = entry['vlan']
-                    elif entry['remoteVtepIp']:
+                    else:
                         old_entry['remoteVtepIp'] = entry['remoteVtepIp']
-                    if old_entry['remoteVtepIp']:
-                        old_entry['flags'] = 'remote'
+                    old_entry['flags'] = 'remote'
                     self._add_mackey_protocol(old_entry)
                     drop_indices.append(i)
                     continue
-            if 'offload' in entry['flags'] or 'extern_learn' in entry['flags']:
+            if entry['flags'] == 'offload' or entry['flags'] == 'extern_learn':
                 if entry['remoteVtepIp']:
                     entry['flags'] = 'remote'
             self._add_mackey_protocol(entry)
 
         processed_data = np.delete(processed_data, drop_indices).tolist()
         return processed_data
 
     def _clean_cumulus_data(self, processed_data, raw_data):
         return self._clean_linux_data(processed_data, raw_data)
 
-    def _clean_sonic_data(self, processed_data, raw_data):
-        return self._clean_linux_data(processed_data, raw_data)
-
-    def _clean_junos_data(self, processed_data, _):
-        drop_indices = []
-        new_entries = []
-
-        for i, entry in enumerate(processed_data):
-            if not entry.get('macaddr', ''):
-                drop_indices.append(i)
+    def _clean_junos_data(self, processed_data, raw_data):
+        for entry in processed_data:
             inflags = entry.pop('flags', '')
             flags = ''
             if inflags:
                 if 'rcvd_from_remote' in inflags:
                     flags += ' remote'
 
-            maclist = entry.get('macaddr', '')
-            if isinstance(maclist, list):
-                # MX format
-                oifs = entry.get('oif', [])
-                for j, mac in enumerate(maclist):
-                    new_entry = entry.copy()
-                    new_entry['macaddr'] = mac
-                    if not entry['bd']:
-                        if '.' in oifs[j]:
-                            new_entry['oif'], new_entry['vlan'] = \
-                                oifs[j].split('.')
-                        else:
-                            new_entry['oif'] = oifs[j].split('.')[0]
-                    else:
-                        new_entry['oif'] = oifs[j]
-
-                    new_entry['flags'] = ''
-                    self._add_mackey_protocol(new_entry)
-                    new_entries.append(new_entry)
-                drop_indices.append(i)
-            else:
-                entry['flags'] = flags.strip()
-                if entry['oif'] and not entry['oif'].startswith('vtep'):
-                    entry['oif'] = entry['oif'].split('.')[0]
-                self._add_mackey_protocol(entry)
+            if entry.get('bd', None):
+                entry['protocol'] = 'vpls'
+                flags = inflags + ' remote'
+            entry['flags'] = flags.strip()
+            self._add_mackey_protocol(entry)
 
-        processed_data = np.delete(processed_data, drop_indices).tolist()
-        processed_data.extend(new_entries)
         return processed_data
 
-    def _clean_nxos_data(self, processed_data, _):
+    def _clean_nxos_data(self, processed_data, raw_data):
 
         for entry in processed_data:
             entry['macaddr'] = convert_macaddr_format_to_colon(
                 entry.get('macaddr', '0000.0000.0000'))
             vtepIP = re.match(r'(\S+)\(([0-9.]+)\)', entry['oif'])
             if vtepIP:
                 entry['remoteVtepIp'] = vtepIP.group(2)
                 entry['oif'] = vtepIP.group(1)
                 entry['flags'] = 'remote'
             else:
-                entry['oif'] = expand_nxos_ifname(entry['oif'])
+                if entry['oif'].startswith('Eth'):
+                    entry['oif'] = entry['oif'].replace('Eth', 'Ethernet')
+                elif entry['oif'].startswith('Po'):
+                    entry['oif'] = entry['oif'].replace('Po', 'port-channel')
                 entry['remoteVtepIp'] = ''
-
-            oif = entry.get('oif', '')
-            if oif and '(R)' in oif:
-                entry['oif'] = oif.split('(R)')[0]
-                entry['flags'] = 'router'
-
             if entry.get('vlan', '-') == '-':
                 entry['vlan'] = 0
-            # Handling old NXOS
-            if entry.get('_isStatic', 'disabled') == 'enabled':
-                entry['flags'] = 'static'
-            flags = entry.get('flags').strip()
-            if not flags or (flags == '*'):
-                entry['flags'] = 'dynamic'
-
             self._add_mackey_protocol(entry)
 
         return processed_data
 
-    def _clean_iosxe_data(self, processed_data, _):
+    def _clean_eos_data(self, processed_data, raw_data):
 
         for entry in processed_data:
             entry['macaddr'] = convert_macaddr_format_to_colon(
                 entry.get('macaddr', '0000.0000.0000'))
-            oiflist = []
-            oifs = ''
-            oiflist = entry.get('_ports', [])
-            for oif in oiflist:
-                # Handles multicast entries
-                oifs += f'{expand_ios_ifname(oif)} '
-            if oifs:
-                entry['oif'] = oifs.strip()
+            vtepIP = re.match(r'(\S+)\(([0-9.]+)\)', entry['oif'])
+            if vtepIP:
+                entry['remoteVtepIp'] = vtepIP.group(2)
+                entry['oif'] = vtepIP.group(1)
+                entry['flags'] = 'remote'
             else:
-                entry['oif'] = ''
-
-            entry['remoteVtepIp'] = ''
-            vlan = entry.get('vlan', ' ').strip()
-            if vlan in ["All", "N/A"]:
-                entry['vlan'] = 0
-
-            entry['flags'] = entry.get('flags', '').lower()
-
-            self._add_mackey_protocol(entry)
-
-        return processed_data
-
-    def _clean_ios_data(self, processed_data, raw_data):
-        return self._clean_iosxe_data(processed_data, raw_data)
-
-    def _clean_eos_data(self, processed_data, _):
-
-        drop_indices = []
-
-        for i, entry in enumerate(processed_data):
-            entry['oif'] = expand_eos_ifname(entry['oif'])
-            if (entry['oif'].startswith('Vxlan') and
-                    'remoteVtepIp' not in entry):
-                drop_indices.append(i)
-                continue
-            if '.' in entry['macaddr']:
-                entry['macaddr'] = convert_macaddr_format_to_colon(
-                    entry.get('macaddr', '0000.0000.0000'))
+                entry['remoteVtepIp'] = ''
             self._add_mackey_protocol(entry)
 
-        processed_data = np.delete(processed_data, drop_indices).tolist()
         return processed_data
```

### Comparing `suzieq-0.22.0rc1/suzieq/poller/worker/services/mlag.py` & `suzieq-0.8.0/suzieq/poller/services/mlag.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-from suzieq.poller.worker.services.service import Service
-from suzieq.shared.utils import expand_nxos_ifname
+from suzieq.poller.services.service import Service
 
 
 class MlagService(Service):
     """MLAG service. Different class because output needs to be munged"""
 
     def clean_json_input(self, data):
-        """NXOS JSON data needs some work"""
+        """FRR JSON data needs some work"""
 
         devtype = data.get("devtype", None)
         if devtype in ["nxos"]:
             if data['data'].startswith('Note: \n'):
                 lines = data['data'].splitlines()
                 if len(lines) > 3:
                     data['data'] = '\n'.join(lines[2:])
                 else:
-                    data['data'] = ('{\n"TABLE_orphan_ports": \n{\n'
-                                    '"ROW_orphan_ports": [\n]\n}\n}\n\n')
+                    data['data'] = '{\n"TABLE_orphan_ports": \n{\n"ROW_orphan_ports": [\n]\n}\n}\n\n'
                 return data['data']
 
-        return data['data']
-
-    def _clean_cumulus_data(self, processed_data, _):
+    def _clean_cumulus_data(self, processed_data, raw_data):
         """Populate the different portlists and counts"""
 
         mlagDualPortsCnt = 0
         mlagSinglePortsCnt = 0
         mlagErrorPortsCnt = 0
         mlagDualPorts = []
         mlagSinglePorts = []
@@ -56,83 +52,66 @@
             entry["mlagSinglePortsCnt"] = mlagSinglePortsCnt
             entry["mlagDualPortsCnt"] = mlagDualPortsCnt
             entry["mlagErrorPortsCnt"] = mlagErrorPortsCnt
             del entry["mlagInterfacesList"]
 
         return processed_data
 
-    def _clean_nxos_data(self, processed_data, _):
+    def _clean_nxos_data(self, processed_data, raw_data):
         """NXOS VPC data massaging"""
 
         mlagDualPorts = []
         mlagSinglePorts = []
         mlagErrorPorts = []
 
         if not processed_data:
             return processed_data
 
         for entry in processed_data:
             # systemID is a mandatory parameter
-            domainid = entry.get('domainId', '')
-            if not domainid or (domainid == 'not configured'):
+            if not entry.get('domainId', ''):
                 processed_data = []
                 return processed_data
 
-            mlagSinglePorts = list(filter(
-                lambda x: x == '1',
-                entry.get('_forwardViaPeerLinkList', []) or []))
-            mlagErrorPorts = list(filter(
-                lambda x: x not in ['consistent', 'success', 'not-applicable'],
-                entry.get('_portConfigSanityList', []) or []))
-            mlagDualPorts = entry.get('_portList', []) or []
+            mlagSinglePorts = list(filter(lambda x: x == '1',
+                                          entry['_forwardViaPeerLinkList']))
+            mlagErrorPorts = list(filter(lambda x: x != 'consistent',
+                                         entry['_portConfigSanityList']))
+            mlagDualPorts = entry['_portList']
             mlagDualPorts = list(filter(
                 lambda x: x not in mlagSinglePorts and x not in mlagErrorPorts,
                 mlagDualPorts))
 
-            if entry.get('peerLinkStatus', '') in [1, "up"]:
-                entry['peerLinkStatus'] = 'up'
-            else:
-                entry['peerLinkStatus'] = 'down'
-            entry['peerLink'] = expand_nxos_ifname(entry['peerLink'])
-            entry['peerAddress'] = entry.get('peerAddress', [])
-            entry['mlagDualPortsList'] = [
-                expand_nxos_ifname(x) for x in mlagDualPorts]
+            entry['peerAddress'] = entry.get('peerAddress', [])[0]
+            entry['mlagDualPortsList'] = mlagDualPorts
             entry['mlagDualPortsCnt'] = len(mlagDualPorts)
-            entry['mlagSinglePortsList'] = [
-                expand_nxos_ifname(x) for x in mlagSinglePorts]
+            entry['mlagSinglePortsList'] = mlagSinglePorts
             entry['mlagSinglePortsCnt'] = len(mlagSinglePorts)
-            entry['mlagErrorPortsList'] = [
-                expand_nxos_ifname(x) for x in mlagErrorPorts]
+            entry['mlagErrorPortsList'] = mlagErrorPorts
             entry['mlagErrorPortsCnt'] = len(mlagErrorPorts)
-            entry['state'] = 'active' \
-                if entry['state'].strip() in ['peer-ok',
-                                              'peer adjacency formed ok'] \
-                else 'dead'
-            if entry['configSanity'] == "success":
-                entry['configSanity'] = 'consistent'
-            if entry['configSanity'] not in ['consistent', 'success']:
-                if 'reason' in entry:
-                    entry['configSanity'] = entry.get('_reason', '')
+            entry['state'] = 'active' if entry['state'] == 'peer-ok' else 'dead'
+            if entry['configSanity'] != 'consistent':
+                entry['configSanity'] = entry['_reason']
 
         return processed_data
 
-    def _clean_eos_data(self, processed_data, _):
+    def _clean_eos_data(self, processed_data, raw_data):
         '''EOS MLAG data massaging'''
 
         for entry in processed_data:
             # There's no MLAG without systemID
             if not entry['systemId']:
                 return []
 
             entry['mlagDualPortsList'] = []
             entry['mlagSinglePortsList'] = []
             entry['mlagErrorPortsList'] = []
 
-            for port_info in zip(entry.get('_localInterfaceList', []),
-                                 entry.get('_linkStateList', [])):
+            for port_info in zip(entry['_localInterfaceList'],
+                                 entry['_linkStateList']):
                 if port_info[1] == 'active-full':
                     entry['mlagDualPortsList'].append(port_info[0])
                 elif port_info[1] == 'active-partial':
                     entry['mlagSinglePortsList'].append(port_info[0])
                 elif port_info[1] in ['disabled', 'inactive']:
                     entry['mlagErrorPortsList'].append(port_info[0])
```

### Comparing `suzieq-0.22.0rc1/suzieq/poller/worker/services/ospfIf.py` & `suzieq-0.8.0/suzieq/poller/services/bgp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,203 +1,215 @@
-from ipaddress import ip_address, IPv4Interface
-
 import numpy as np
 
-from suzieq.poller.worker.services.service import Service
+from suzieq.poller.services.service import Service
+from suzieq.utils import get_timestamp_from_cisco_time
+from suzieq.utils import get_timestamp_from_junos_time
 
 
-class OspfIfService(Service):
-    """OSPF Interface service. Output needs to be munged"""
+class BgpService(Service):
+    """bgp service. Different class because of munging of output across NOS"""
 
-    def _clean_linux_data(self, processed_data, _):
-        vrf_loip = {}
+    def _clean_eos_data(self, processed_data, raw_data):
 
         for entry in processed_data:
-            if entry.get('vrf', '') == '':
-                entry['vrf'] = 'default'
-            if entry['ifname'] == "lo":
-                vrf_loip[entry['vrf']] = entry.get('ipAddress')
-            entry["networkType"] = entry["networkType"].lower()
-            if entry['networkType'] == 'pointopoint':
-                entry['networkType'] = 'p2p'
-            entry["passive"] = entry["passive"] == "Passive"
-            unnumbered = entry["isUnnumbered"] == "UNNUMBERED"
-            if unnumbered:
-                entry["isUnnumbered"] = True
-                entry['ipAddress'] = vrf_loip.get(entry['vrf'], '')
+            if entry["bfdStatus"] == 3:
+                entry["bfdStatus"] = "up"
+            elif entry["bfdStatus"] != "disabled":
+                entry["bfdStatus"] = "down"
+            entry["asn"] = int(entry["asn"])
+            entry["peerAsn"] = int(entry["peerAsn"])
+            entry['estdTime'] = raw_data[0]['timestamp'] - \
+                (entry['estdTime']*1000)
+            entry['origPeer'] = entry['peer']
 
         return processed_data
 
-    def _clean_cumulus_data(self, processed_data, raw_data):
-        return self._clean_linux_data(processed_data, raw_data)
-
-    def _clean_sonic_data(self, processed_data, raw_data):
-        return self._clean_linux_data(processed_data, raw_data)
+    def _clean_junos_data(self, processed_data, raw_data):
 
-    def _clean_eos_data(self, processed_data, _):
-
-        vrf_loip = {}
-        vrf_rtrid = {}
+        peer_uptimes = {}
         drop_indices = []
-        for i, entry in enumerate(processed_data):
-
-            if '_entryType' in entry:
-                # Retrieve the VRF and routerID
-                vrf_rtrid[entry.get('vrf', 'default')] = \
-                    entry.get('routerId', '')
-                drop_indices.append(i)
-                continue
-
-            if not entry.get('ifname', ''):
-                drop_indices.append(i)
-                continue
-
-            vrf = entry.get('vrf', '')
-            ip_addr = entry.get('ipAddress', '') + '/' + \
-                str(entry.get('maskLen', ''))
-            entry['ipAddress'] = ip_addr
-            if entry['ifname'].startswith("Loopback"):
-                if vrf not in vrf_loip or not vrf_loip[vrf]:
-                    vrf_loip[vrf] = ip_addr
-            if entry.get('passive', False):
-                entry['bfdStatus'] = "invalid"
-            entry["networkType"] = entry["networkType"].lower()
-            entry["isUnnumbered"] = False
-            if entry.get('state', '') in ['dr', 'p2p', 'backupDr']:
-                entry['state'] = 'up'
 
         for i, entry in enumerate(processed_data):
-            if entry.get('ipAddress', '') == vrf_loip.get(
-                    entry.get('vrf', ''), ''):
-                if not entry.get('type', '') == "loopback":
-                    entry['isUnnumbered'] = True
-            if entry['vrf'] in vrf_rtrid:
-                entry['routerId'] = vrf_rtrid[entry['vrf']]
-
-        processed_data = np.delete(processed_data, drop_indices).tolist()
-        return processed_data
-
-    def _clean_junos_data(self, processed_data, _):
-
-        drop_indices = []
-
-        for i, entry in enumerate(processed_data):
-            if entry['_entryType'] == 'overview':
-                routerId = entry['routerId']
-                continue
-
-            if not entry.get('ifname', ''):
+            if entry['_entryType'] == 'summary':
+                peer_uptimes[entry['peer']] = entry['estdTime']
                 drop_indices.append(i)
                 continue
+            # JunOS adds entries which includes the port as IP+Port
+            entry['peerIP'] = entry['peerIP'].split('+')[0]
+            entry['peer'] = entry['peer'].split('+')[0]
+            entry['updateSource'] = entry['updateSource'].split('+')[0]
+            entry['numChanges'] = int(entry['numChanges'])
+            entry['updatesRx'] = int(entry['updatesRx'])
+            entry['updatesTx'] = int(entry['updatesTx'])
+            entry['asn'] = int(entry['asn'])
+            entry['peerAsn'] = int(entry['peerAsn'])
+            entry['keepaliveTime'] = int(entry['keepaliveTime'])
+            entry['holdTime'] = int(entry['holdTime'])
 
-            entry['routerId'] = routerId
-            # Is this right? Don't have a down interface example
-            entry['state'] = 'up'
-            entry['passive'] = entry['passive'] == "Passive"
-            if entry['networkType'] == "LAN":
-                entry['networkType'] = "broadcast"
-            entry['stub'] = not entry['stub'] == 'Not Stub'
-            entry['ipAddress'] = IPv4Interface(
-                f'{entry["ipAddress"]}/{entry["maskLen"]}').with_prefixlen
-            entry['maskLen'] = int(entry['ipAddress'].split('/')[1])
-            entry['vrf'] = 'default'  # Juniper doesn't provide this info
-            entry['authType'] = entry['authType'].lower()
-            entry['networkType'] = entry['networkType'].lower()
-
-        # Skip the original record as we don't need the overview record
-        processed_data = np.delete(processed_data, drop_indices).tolist()
-        return processed_data[1:]
-
-    def _clean_nxos_data(self, processed_data, _):
-        areas = {}              # Need to come back to fixup entries
-        drop_indices = []
-
-        for i, entry in enumerate(processed_data):
-            if not entry.get('ifname', ''):
-                drop_indices.append(i)
-                continue
-
-            if entry['_entryType'] == 'interfaces':
-                entry["networkType"] = entry["networkType"].lower()
-                if entry['ifname'].startswith('loopback'):
-                    entry['passive'] = True
-                entry['ipAddress'] = \
-                    f"{entry['ipAddress']}/{entry['maskLen']}"
-                if entry['area'] not in areas:
-                    areas[entry['area']] = []
+            if entry['peer'] in peer_uptimes:
+                entry['estdTime'] = peer_uptimes[entry['peer']]
+            else:
+                entry['estdTime'] = '0d 00:00:00'
 
-                if entry.get('_adminState', '') == "down":
-                    entry['state'] = "adminDown"
+            # Assign counts to appropriate AFi/SAFI
+            for i, afi in enumerate(entry.get('pfxType')):
+                if entry['pfxRxList'][i] is None:
+                    entry['pfxRxList'][i] = 0
+                if afi == 'inet.0':
+                    entry['v4PfxRx'] = int(entry['pfxRxList'][i])
+                    entry['v4PfxTx'] = int(entry['pfxTxList'][i])
+                    entry['v4Enabled'] = True
+                elif afi == 'inet6.0':
+                    entry['v6PfxRx'] = int(entry['pfxRxList'][i])
+                    entry['v6PfxTx'] = int(entry['pfxTxList'][i])
+                elif afi == 'bgp.evpn.0':
+                    entry['evpnPfxRx'] = int(entry['pfxRxList'][i])
+                    entry['evpnPfxTx'] = int(entry['pfxTxList'][i])
+
+            entry.pop('pfxType')
+            entry.pop('pfxRxList')
+            entry.pop('pfxTxList')
+
+            for afi in entry['afiSafiAdvList'].split():
+                if afi == 'inet-unicast':
+                    entry['v4Advertised'] = True
+                elif afi == 'inet6-unicast':
+                    entry['v6Advertised'] = True
+                elif afi == 'evpn':
+                    entry['evpnAdvertised'] = True
+            entry.pop('afiSafiAdvList')
+
+            for afi in entry['afiSafiRcvList'].split():
+                if afi == 'inet-unicast':
+                    entry['v4Received'] = True
+                elif afi == 'inet6-unicast':
+                    entry['v6Received'] = True
+                elif afi == 'evpn':
+                    entry['evpnReceived'] = True
+
+            entry.pop('afiSafiRcvList')
+            for afi in entry['afiSafiEnabledList'].split():
+                if afi == 'inet-unicast':
+                    entry['v4Enabled'] = True
+                elif afi == 'inet6-unicast':
+                    entry['v6Enabled'] = True
+                elif afi == 'evpn':
+                    entry['evpnEnabled'] = True
 
-                areas[entry['area']].append(entry)
-            else:
-                # ifname is really the area name
-                if not entry.get('ifname', []):
-                    drop_indices.append(i)
-                    continue
+            entry.pop('afiSafiEnabledList')
+            if not entry.get('vrf', None):
+                entry['vrf'] = 'default'
 
-                for j, area in enumerate(entry['ifname']):
-                    # NXOS doesn't provide the three pieces of data below
-                    # in the same command, and so we have to stitch it
-                    # together via two diff command outputs. The area and
-                    # vrf are the keys we use to tie the records together.
-                    for ifentry in areas.get(area, []):
-                        if ifentry['vrf'] != entry['vrf']:
-                            continue
-                        ifentry['routerId'] = entry['routerId']
-                        ifentry['authType'] = entry['authType'][j]
-                        ifentry['isBackbone'] = area == "0.0.0.0"
-                drop_indices.append(i)
+            # Junos doesn't provide this data in neighbor, only in summary
+            entry['estdTime'] = get_timestamp_from_junos_time(
+                entry['estdTime'], raw_data[0]['timestamp']/1000)
 
         processed_data = np.delete(processed_data, drop_indices).tolist()
         return processed_data
 
-    def _clean_ios_data(self, processed_data, _):
+    def _clean_nxos_data(self, processed_data, raw_data):
 
+        entries_by_vrf = {}
         drop_indices = []
-        proc_vrf_map = {}
 
         for i, entry in enumerate(processed_data):
-            if entry.get('_entryType', ''):
-                proc_vrf_map[entry.get('_processId', '')] = entry['vrf']
+            if entry['_entryType'] == 'summary':
+                for ventry in entries_by_vrf.get(entry['vrf'], []):
+                    ventry['asn'] = entry['asn']
+                    ventry['routerId'] = entry['routerId']
                 drop_indices.append(i)
                 continue
 
-            if not entry.get('ifname', ''):
-                drop_indices.append(i)
-                continue
+            if not entry['peer']:
+                if not entry.get('_dynPeer', None):
+                    drop_indices.append(i)
+                    continue
+                entry['peer'] = entry['_dynPeer'].replace('/', '-')
+                entry['origPeer'] = entry['_dynPeer']
+                entry['state'] = 'dynamic'
+                entry['v4PfxRx'] = entry['_activePeers']
+                entry['v4PfxTx'] = entry['_maxconcurrentpeers']
+                entry['estdTime'] = entry['_firstconvgtime']
+
+            for i, item in enumerate(entry['afiSafi']):
+                if item == 'IPv4 Unicast':
+                    entry['v4Advertised'] = entry['afAdvertised'][i]
+                    entry['v4Received'] = entry['afRcvd'][i]
+                    if (entry['v4Advertised'] == "true" and
+                            entry['v4Received'] == "true"):
+                        entry['v4Enabled'] = True
+                    else:
+                        entry['v4Enabled'] = False
+                elif item == 'IPv6 Unicast':
+                    entry['v6Advertised'] = entry['afAdvertised'][i]
+                    entry['v6Received'] = entry['afRcvd'][i]
+                    if (entry['v6Advertised'] == "true" and
+                            entry['v6Received'] == "true"):
+                        entry['v6Enabled'] = True
+                    else:
+                        entry['v6Enabled'] = False
+                elif item == 'L2VPN EVPN':
+                    entry['evpnAdvertised'] = entry['afAdvertised'][i]
+                    entry['evpnReceived'] = entry['afRcvd'][i]
+                    if (entry['evpnAdvertised'] == "true" and
+                            entry['evpnReceived'] == "true"):
+                        entry['evpnEnabled'] = True
+                    else:
+                        entry['evpnEnabled'] = False
+
+            entry.pop('afiSafi')
+            entry.pop('afAdvertised')
+            entry.pop('afRcvd')
+
+            entry['rrClient'] = entry.get('rrclient', False) == "true"
+
+            defint_list = [0]*len(entry.get('afiPrefix', []))
+            defbool_list = [False]*len(entry.get('afiPrefix', []))
+            pfxRx_list = entry.get('pfxRcvd', []) or defint_list
+            pfxTx_list = entry.get('pfxSent', []) or defint_list
+            deforig_list = entry.get('defaultOrig', []) or defbool_list
+            extcomm_list = entry.get('extendComm', []) or defbool_list
+            comm_list = entry.get('sendComm', []) or defbool_list
+
+            for i, item in enumerate(entry['afiPrefix']):
+                if item == 'IPv4 Unicast':
+                    entry['v4PfxRx'] = pfxRx_list[i]
+                    entry['v4PfxTx'] = pfxTx_list[i]
+                    entry['v4DefaultSent'] = deforig_list[i]
+                elif item == 'IPv6 Unicast':
+                    entry['v6PfxRx'] = pfxRx_list[i]
+                    entry['v6PfxTx'] = pfxTx_list[i]
+                    entry['v6DefaultSent'] = deforig_list[i]
+                elif item == 'L2VPN EVPN':
+                    entry['evpnPfxRx'] = pfxRx_list[i]
+                    entry['evpnPfxTx'] = pfxTx_list[i]
+                    entry['evpnDefaultSent'] = deforig_list[i]
+                    if comm_list[i] == "true":
+                        if extcomm_list[i] == "true":
+                            entry['evpnSendCommunity'] = 'extendedAndstandard'
+                        else:
+                            entry['evpnSendCommunity'] = 'standard'
+                    elif extcomm_list[i] == "true":
+                        entry['evpnSendCommunity'] = 'extended'
+
+            entry.pop('afiPrefix')
+            entry.pop('pfxRcvd')
+            entry.pop('pfxSent')
+            entry.pop('sendComm')
+            entry.pop('extendComm')
+            entry.pop('defaultOrig')
+
+            if (entry.get('extnhAdvertised', False) == "true" and
+                    entry.get('extnhReceived', False) == "true"):
+                entry['extnhEnabled'] = True
+            else:
+                entry['extnhEnabled'] = False
 
-            area = entry.get('area', '')
-            if area and area.isdecimal():
-                entry['area'] = str(ip_address(int(area)))
-            entry["networkType"] = entry["networkType"].lower()
-            entry['networkType'] = entry['networkType'] \
-                .replace('point_to_point', 'p2p')
-            entry["passive"] = entry["passive"] == "stub"
-            entry["isUnnumbered"] = entry["isUnnumbered"] == "yes"
-            entry['areaStub'] = entry['areaStub'] == "yes"
-            entry['helloTime'] = int(
-                entry['helloTime']) if entry['helloTime'] else 10  # def value
-            entry['deadTime'] = int(
-                entry['deadTime']) if entry['deadTime'] else 40  # def value
-            entry['retxTime'] = int(
-                entry['retxTime']) if entry['retxTime'] else 5  # def value
-            proc_id = entry.get('_processId', '')
-            if proc_id:
-                entry['vrf'] = proc_vrf_map.get(proc_id, 'default')
-            if not entry.get('vrf', ''):
-                entry['vrf'] = 'default'
+            entry['estdTime'] = get_timestamp_from_cisco_time(
+                entry['estdTime'], raw_data[0]['timestamp']/1000)
+            if entry['vrf'] not in entries_by_vrf:
+                entries_by_vrf[entry['vrf']] = []
 
-            entry['authType'] = entry.get('authType', '').lower()
-            entry['nbrCount'] = int(
-                entry['nbrCount']) if entry['nbrCount'] else 0
-            entry['noSummary'] = entry.get('noSummary', False)
-            if entry['state'] == "administratively down":
-                entry['state'] = "adminDown"
-            else:
-                entry['state'] = entry['state'].lower()
+            entries_by_vrf[entry['vrf']].append(entry)
 
         processed_data = np.delete(processed_data, drop_indices).tolist()
         return processed_data
-
-    def _clean_iosxe_data(self, processed_data, raw_data):
-        return self._clean_ios_data(processed_data, raw_data)
```

### Comparing `suzieq-0.22.0rc1/suzieq/poller/worker/services/service.py` & `suzieq-0.8.0/suzieq/poller/nodes/node.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,947 +1,1043 @@
-import asyncio
-import copy
-import json
-import logging
-import operator
+import sys
+from collections import defaultdict
 import os
 import time
-from collections import defaultdict
-from dataclasses import dataclass, field
-from datetime import datetime, timezone
+from datetime import datetime
+import logging
+import random
 from http import HTTPStatus
-from tempfile import mkstemp
-from typing import Dict, List, Tuple
+import json
+import re
 
-import pyarrow as pa
 import yaml
-from packaging import version as version_parse
+from urllib.parse import urlparse
+
+import asyncio
+import asyncssh
+import aiohttp
+from asyncio.subprocess import PIPE
+from concurrent.futures._base import TimeoutError
+
+from suzieq.poller.services.service import RsltToken
+from suzieq.poller.genhosts import convert_ansible_inventory
+from suzieq.utils import get_timestamp_from_junos_time, known_devtypes
+
+logger = logging.getLogger(__name__)
+
+
+def get_hostsdata_from_hostsfile(hosts_file) -> dict:
+    """Read the suzieq devices file and return the data from the file"""
+
+    if not os.path.isfile(hosts_file):
+        logger.error(f"Suzieq inventory {hosts_file} must be a file")
+        print(f"ERROR: Suzieq inventory {hosts_file} must be a file")
+        sys.exit(1)
+
+    if not os.access(hosts_file, os.R_OK):
+        logger.error("Suzieq inventory file is not readable: {}", hosts_file)
+        print("ERROR: hosts Suzieq inventory file is not readable: {}",
+              hosts_file)
+        sys.exit(1)
+
+    with open(hosts_file, "r") as f:
+        try:
+            data = f.read()
+            hostsconf = yaml.safe_load(data)
+        except Exception as e:
+            logger.error("Invalid Suzieq inventory file:{}", e)
+            print("Invalid Suzieq inventory file:{}", e)
+            sys.exit(1)
+
+    if not isinstance(hostsconf, list):
+        if '_meta' in hostsconf.keys():
+            logger.error("Invalid Suzieq inventory format, Ansible format??"
+                         " Use -a instead of -D with inventory")
+            print("ERROR: Invalid Suzieq inventory format, Ansible format??"
+                  " Use -a instead of -D with inventory")
+        else:
+            logger.error("Invalid Suzieq inventory file:{}")
+            print("ERROR: Invalid hosts Suzieq inventory file:{}")
+        sys.exit(1)
+
+    for conf in hostsconf:
+        if any(x not in conf.keys() for x in ['namespace', 'hosts']):
+            logger.error("Invalid inventory:{}, no namespace/hosts sections")
+            print("ERROR: Invalid inventory:{}, no namespace/hosts sections")
+            sys.exit(1)
+
+    return hostsconf
+
+
+async def init_hosts(**kwargs):
+    """Process list of devices to gather data from.
+    This involves creating a node for each device listed, and connecting to
+    those devices and initializing state about those devices
+    """
+
+    nodes = {}
+
+    inventory = kwargs.pop('inventory', None)
+    if not inventory:
+        ans_inventory = kwargs.pop('ans_inventory', None)
+    else:
+        _ = kwargs.pop('ans_inventory', None)
+        ans_inventory = None
+
+    namespace = kwargs.pop('namespace', 'default')
+    passphrase = kwargs.pop('passphrase', None)
+    ssh_config_file = kwargs.pop('ssh_config_file', None)
+    jump_host = kwargs.pop('jump_host', None)
+    jump_host_key_file = kwargs.pop('jump_host_key_file', None)
+    ignore_known_hosts = kwargs.pop('ignore_known_hosts', False)
+    user_password = kwargs.pop('password', None)
+
+    if kwargs:
+        logger.error(f'Received unrecognized keywords {kwargs}, aborting')
+        sys.exit(1)
+
+    if inventory:
+        hostsconf = get_hostsdata_from_hostsfile(inventory)
+    else:
+        hostsconf = yaml.safe_load('\n'.join(
+            convert_ansible_inventory(ans_inventory, namespace)))
+
+    if not hostsconf:
+        logger.error("No hosts specified in inventory file")
+        print("ERROR: No hosts specified in inventory file")
+        sys.exit(1)
+
+    if jump_host_key_file:
+        if not jump_host:
+            logger.error("Jump host key file specified without jump host")
+            print("ERROR: Jump host key file specified without jump host")
+            sys.exit(1)
+        else:
+            if not os.access(jump_host_key_file, os.F_OK):
+                logger.error(
+                    f"Jump host key file {jump_host_key_file} does not exist")
+                print(f"ERROR: Jump host key file {jump_host_key_file} "
+                      f"does not exist")
+                sys.exit(1)
+            if not os.access(jump_host_key_file, os.R_OK):
+                logger.error(
+                    f"Jump host key file {jump_host_key_file} not readable")
+                print(f"ERROR: Jump host key file {jump_host_key_file} "
+                      f"not readable")
+                sys.exit(1)
+
+    for namespace in hostsconf:
+        if "namespace" not in namespace:
+            logger.warning('No namespace specified, assuming "default"')
+            nsname = "default"
+        else:
+            nsname = namespace["namespace"]
+
+        tasks = []
+        for host in namespace.get("hosts", []):
+            entry = host.get("url", None)
+            if entry:
+                words = entry.split()
+                result = urlparse(words[0])
+
+                username = result.username
+                password = result.password or user_password or "vagrant"
+                port = result.port
+                host = result.hostname
+                devtype = None
+                keyfile = None
+
+                for i in range(1, len(words[1:])+1):
+                    if words[i].startswith('keyfile'):
+                        keyfile = words[i].split("=")[1]
+                    elif words[i].startswith('devtype'):
+                        devtype = words[i].split("=")[1]
+                    elif words[i].startswith('username'):
+                        username = words[i].split("=")[1]
+                    elif words[i].startswith('password'):
+                        password = words[i].split("=")[1]
+
+                newnode = Node()
+                tasks += [newnode._init(
+                    address=host,
+                    username=username,
+                    port=port,
+                    password=password,
+                    passphrase=passphrase,
+                    transport=result.scheme,
+                    devtype=devtype,
+                    ssh_keyfile=keyfile,
+                    ssh_config_file=ssh_config_file,
+                    jump_host=jump_host,
+                    jump_host_key_file=jump_host_key_file,
+                    namespace=nsname,
+                    ignore_known_hosts=ignore_known_hosts,
+                )]
+
+        if not tasks:
+            logger.error("No hosts detected in provided inventory file")
+            return []
+
+        for f in asyncio.as_completed(tasks):
+            newnode = await f
+            if newnode.devtype is None:
+                logger.error(
+                    "Unable to determine device type for {}"
+                    .format(newnode.address))
+            else:
+                logger.info(f"Added node {newnode.hostname}")
+
+            nodes.update(
+                {"{}.{}".format(nsname, newnode.hostname): newnode})
 
-from suzieq.poller.worker.services.svcparser \
-    import cons_recs_from_json_template
-from suzieq.shared.sq_plugin import SqPlugin
-from suzieq.shared.utils import get_default_per_vals, known_devtypes
-from suzieq.version import SUZIEQ_VERSION
-
-# How long b4 declaring node dead
-HOLD_TIME_IN_MSECS = 60000
-# How many unsuccessful polls before marking records with active=false
-HYSTERESIS_FAILURE_CNT = 3
-# The boot timestamp time drift tolerance (in seconds)
-TIME_DRIFT_TOLERANCE = 5
-
-
-@dataclass
-class RsltToken:
-    '''Cookie passed between service and node objects'''
-    start_time: int    # When this cmd was first posted to node
-    nodename: str      # Name of node, used to get poller cb again
-    bootupTimestamp: int
-    nodeQsize: int        # Size of the node q at queuing time
-    service: str          # Name of this service, if node needs it
-    timeout: int          # timeout value for cmd to complete
-
-
-@dataclass
-class ServiceStats:
-    '''Capture useful stats about service'''
-    total_time: List[float] = field(default_factory=list)
-    gather_time: List[float] = field(default_factory=list)
-    svcQsize: List[float] = field(default_factory=list)
-    nodeQsize: List[float] = field(default_factory=list)
-    wrQsize: List[float] = field(default_factory=list)
-    rxBytes: List[float] = field(default_factory=list)
-    empty_count: int = 0
-    time_excd_count: int = 0    # Number of times total_time > poll period
-    next_update_time: int = 0   # When results will be logged
-
-
-class Service(SqPlugin):
-    '''Main class for handling various services/tables processing on devices'''
-
-    def get_poller_schema(self):
-        '''Return the schema used by this service'''
-        return self._poller_schema
-
-    def set_poller_schema(self, value: dict):
-        '''Set the poller schema used by this service'''
-        self._poller_schema = value
-
-    def __init__(self, name, defn, period, stype, keys, ignore_fields, schema,
-                 queue, db_access, run_once=None):
-        self.name = name
-        self.defn = defn
-        self.ignore_fields = ignore_fields or []
-        self.writer_queue = queue
-        self.keys = keys
-        self.schema = schema.get_arrow_schema()
-        self.schema_table = schema
-        self.period = period
-        self.stype = stype
+    return nodes
+
+
+class Node(object):
+    @property
+    def status(self):
+        return self._status
+
+    @property
+    def last_exception(self) -> Exception:
+        return self._last_exception
+
+    @last_exception.setter
+    def last_exception(self, val: Exception):
+        self._last_exception = val
+        self._last_exception_timestamp = int(time.time()*1000)
+
+    async def _init(self, **kwargs):
+        if not kwargs:
+            raise ValueError
+
+        self.hostname = "-"  # Device hostname
+        self.devtype = None  # Device type
+        self.pvtkey_file = ""     # SSH private keyfile
+        self.prev_result = {}  # No updates if nothing changed
+        self.nsname = None
+        self.svc_cmd_mapping = defaultdict(lambda: {})  # Not used yet
         self.logger = logging.getLogger(__name__)
-        self.run_once = run_once
-        self.post_timeout = 5
+        self.port = 0
+        self.backoff = 15  # secs to backoff
+        self.init_again_at = 0  # after this epoch secs, try init again
+        self.connect_timeout = 10  # connect timeout in seconds
+        self.cmd_timeout = 10  # default command timeout in seconds
+        self.batch_size = 4    # Number of commands to issue in parallel
+        self.bootupTimestamp = 0
+        self.version = 0                 # OS Version to pick the right defn
+        self._service_queue = None
+        self._conn = None
+        self._tunnel = None
+        self._status = "init"
+        self.svcs_proc = set()
+        self.error_svcs_proc = set()
+        self.ssh_ready = asyncio.Event()
+        self._last_exception = None
+        self._last_exception_timestamp = None
         self.sigend = False
-        self.version = schema.version
-        # Get sqobject to retrieve the data of this service
-        self._db_access = db_access
-
-        self.update_nodes = False  # we have a new node list
-        self.rebuild_nodelist = False  # used only when a node gets init
-        self.node_postcall_list = {}
-        self.new_node_postcall_list = {}
-        self.previous_results = {}
-        self._node_boot_timestamps = {}  # dictionary useful to detect reboots
-        self._poller_schema = {}
-        self.node_boot_times = defaultdict(int)
-        self._failed_node_set = set()
-        self._consecutive_failures = defaultdict(int)
-
-        self.poller_schema = property(
-            self.get_poller_schema, self.set_poller_schema)
-        self.poller_schema_version = None
-
-        # The queue to which all nodes will post the result of the command
-        self.result_queue = asyncio.Queue()
-
-        # Add the hidden fields to ignore_fields
-        self.ignore_fields += ['timestamp', 'sqvers', 'deviceSession']
-
-        if "namespace" not in self.keys:
-            self.keys.insert(0, "namespace")
-
-        if "hostname" not in self.keys:
-            self.keys.insert(1, "hostname")
-
-        self.partition_cols = schema.get_partition_columns()
-
-        # Setup dictionary of NOS specific extracted data cleaners
-        self.dev_clean_fn = {}
-        common_dev_clean_fn = getattr(self, '_common_data_cleaner', None)
-        for x in known_devtypes():
-            if x.startswith('junos'):
-                dev = 'junos'
+
+        self.address = kwargs["address"]
+        self.hostname = kwargs["address"]  # default till we get hostname
+        self.username = kwargs.get("username", "vagrant")
+        self.password = kwargs.get("password", "vagrant")
+        self.transport = kwargs.get("transport", "ssh")
+        self.nsname = kwargs.get("namespace", "default")
+        self.port = kwargs.get("port", 0)
+        self.devtype = None
+        self.ssh_config_file = kwargs.get("ssh_config_file", None)
+
+        passphrase = kwargs.get("passphrase", None)
+        jump_host = kwargs.get("jump_host", "")
+        if jump_host:
+            jump_result = urlparse(jump_host)
+            self.jump_user = jump_result.username or self.username
+            self.jump_host = jump_result.hostname
+            if jump_result.port:
+                self.jump_port = jump_result.port
             else:
-                dev = x
-            self.dev_clean_fn[x] = getattr(
-                self, f'_clean_{dev}_data', None) or common_dev_clean_fn
-
-    @ staticmethod
-    def is_status_ok(status: int) -> bool:
-        '''Did the node return a successful command output'''
-        if status in [0, HTTPStatus.OK]:
-            return True
-        return False
-
-    def get_data(self):
-        """provide the data that is interesting for a service
-
-        does not include queue or schema"""
-
-        r = {}
-        for fld in ('name defn ignore_fields keys period stype '
-                    'partition_cols').split(' '):
-            r[field] = getattr(self, fld)
-        # textFSM objects can't be jsoned, so changing it
-        for device in r['defn']:
-            if 'textfsm' in r['defn'][device]:
-                r['defn'][device]['textfsm'] = str(
-                    r['defn'][device]['textfsm'])
-        return r
-
-    async def set_nodes(self, node_call_list):
-        """New node list for this service"""
-        if self.node_postcall_list:
-            self.new_node_postcall_list = node_call_list
-            self.update_nodes = True
+                self.jump_port = 22
+            pvtkey_file = kwargs.pop('jump_host_key_file')
+            if pvtkey_file:
+                self.jump_host_key_file = self._decrypt_pvtkey(pvtkey_file,
+                                                               passphrase)
+                if not self.jump_host_key_file:
+                    self.logger.error("ERROR: terminating poller")
+                    self.jump_host_key_file = None
+                    sys.exit(1)
         else:
-            self.node_postcall_list = node_call_list
-
-    def get_empty_record(self):
-        '''Return an empty record matching schema'''
-        map_defaults = get_default_per_vals()
-
-        defaults = [map_defaults[x] for x in self.schema.types]
-        rec = dict(zip(self.schema.names, defaults))
-
-        return rec
-
-    def _dump_output(self, outputs) -> str:
-        """Dump the output to a YAML file"""
-        if outputs:
-            yml = {"service": self.name,
-                   "type": self.run_once,
-                   "output": outputs}
-            fd, name = mkstemp(suffix=f"-{self.name}-poller.yml")
-            f = os.fdopen(fd, "w")
-            f.write(yaml.dump(yml))
-            f.close()
-            return name
-        return ""
-
-    def get_diff(self, old: List[Dict], new: List[Dict],
-                 add_all: bool) -> Tuple[List, List]:
-        """Get the difference between the old and the new result
-
-        Args:
-            old (List[Dict]): previous result
-            new (List[Dict]): new result
-            add_all (bool): if True return all the records in adds, even though
-                nothing changed.
-
-        Returns:
-            Tuple[List, List]: return additions and deletions to respect the
-                previous result.
-        """
-        # If old is empty there is no need to look for differences
-        # just return adds
-        if not old:
-            return new, []
-
-        # Work out the differences between the new and the old records
-        adds = []
-        dels = []
-        koldvals = []
-        knewvals = []
-        koldkeys = []
-        knewkeys = []
-
-        fieldsToCheck = set()
-        # keys that start with _ are transient and must be ignored
-        # from comparison
-        for elem in new:
-            # Checking the __iter__ attribute to check if it is iterable
-            # is not pythonic but much faster, we need to be fast since this
-            # piece of code is executed tons of times
-            vals = {k: set(v) if hasattr(v, '__iter__') and
-                    not isinstance(v, str) and
-                    not isinstance(v, dict) else str(v)
-                    for k, v in elem.items()
-                    if k not in self.ignore_fields and not k.startswith('_')
-                    and k in self.schema_table.fields}
-            kvals = {v for k, v in elem.items() if k in self.keys}
-            knewvals.append(vals)
-            knewkeys.append(kvals)
-            fieldsToCheck.update(vals.keys())
-
-        for elem in old:
-            # Get from the old records only the fields there are in new records
-            # since we want to compare what we have, also excluding all the
-            # derived derived colums, which are not explicitly written in
-            # the data.
-            vals = {k: set(v) if hasattr(v, '__iter__') and
-                    not isinstance(v, str) and
-                    not isinstance(v, dict) else str(v)
-                    for k, v in elem.items()
-                    if k in fieldsToCheck}
-            kvals = {v for k, v in elem.items() if k in self.keys}
-            koldvals.append(vals)
-            koldkeys.append(kvals)
+            self.jump_host = None
+            self.jump_host_key_file = None
 
-        if add_all or self.stype == 'counters':
-            adds = new
+        self.ignore_known_hosts = kwargs.get('ignore_known_hosts', False)
+        pvtkey_file = kwargs.get("ssh_keyfile", None)
+        if pvtkey_file:
+            self.pvtkey = self._decrypt_pvtkey(pvtkey_file, passphrase)
+            if not self.pvtkey:
+                self.logger.error("ERROR: Falling back to password for {}"
+                                  .format(self.address))
+                self.pvtkey = None
         else:
-            adds = [new[k]
-                    for k, v in enumerate(knewvals)
-                    if v not in koldvals]
-        dels = [old[k] for k, v in enumerate(koldvals)
-                if v not in knewvals and koldkeys[k] not in knewkeys]
-
-        # The sqvers type for dels might be float, we expect str
-        for d in dels:
-            if d.get('sqvers'):
-                d['sqvers'] = str(d['sqvers'])
-
-        return adds, dels
-
-    def textfsm_data(self, raw_input, fsm_template, entry_type, _1, _2):
-        """Convert unstructured output to structured output"""
-
-        records = []
-        fsm_template.Reset()
-        res = fsm_template.ParseText(raw_input)
-
-        for entry in res:
-            metent = dict(zip(fsm_template.header, entry))
-            if entry_type:
-                metent['_entryType'] = entry_type
-            records.append(metent)
-
-        return records
-
-    async def post_results(self, result, token) -> None:
-        """Callback fn used to post the results back to the service"""
-        if self.result_queue:
-            self.result_queue.put_nowait((token, result))
-        else:
-            self.logger.error(f"No queue for service {self.name}")
+            self.pvtkey = None
+
+        self._init_service_queue()
+
+        self.ssh_ready.set()
+        if not self.port:
+            if self.transport == "ssh":
+                self.port = 22
+            elif self.transport == "https":
+                self.port = 443
+
+        if self.transport == "ssh":
+            await self._init_ssh(init_boot_time=False)
+
+        devtype = kwargs.get("devtype", None)
+        if devtype:
+            self.set_devtype(devtype)
+
+        await self.init_node()
+        if not self.hostname:
+            self.hostname = self.address
+
+        if self._status == "init":
+            self.backoff = min(600, self.backoff * 2) + \
+                (random.randint(0, 1000) / 1000)
+            self.init_again_at = time.time() + self.backoff
+        return self
 
-    def call_node_postcmd(self, postcall, nodename) -> None:
-        """Start data gathering by calling the post command list"""
-        if postcall and postcall['postq']:
-            token = RsltToken(int(time.time()*1000), nodename, 0, 0, self.name,
-                              self.period-5)
-            postcall['postq'](self.post_results, self.defn, token)
-
-    def clean_json_input(self, data):
-        """Clean the JSON input data that is sometimes messed up
-        Each service can implement its own version of the cleanup
-        """
-        return data.get('data', {})
-
-    async def start_data_gather(self) -> None:
-        """Start data gathering by calling the post command list
-        This is only used to fire up the calls the first time. After this,
-        each node gets into a self-adapting curve of calling at least after
-        the duration specified for the service period. If nodes are slower,
-        they'll be scheduled to run after the specified service period after
-        their return. We could use this to track slow nodes.
-        """
+    def _decrypt_pvtkey(self, pvtkey_file: str, passphrase: str) -> str:
+        """Decrypt private key file"""
 
-        for node in self.node_postcall_list:
+        keydata: str = None
+        if pvtkey_file:
             try:
-                self.call_node_postcmd(self.node_postcall_list[node],
-                                       node),
-            except TimeoutError:
-                self.logger.warning(f"Node post failed for {node}")
-                continue
-
-    def _get_def_for_version(self, defn: List, version: str) -> Dict:
-        '''Extract the right definition for the version'''
-        if isinstance(defn, dict):
-            return defn
-
-        if not isinstance(defn, list):
-            return defn
-
-        for item in defn:
-            os_version = item.get('version', '')
-            if os_version == "all":
-                return item
-            if version == 0:
-                # There are various outputs that due to an old parsing bug
-                # return a node version of 0. Use 'all' for those
-                continue
-            opdict = {'>': operator.gt, '<': operator.lt,
-                      '>=': operator.ge, '<=': operator.le,
-                      '=': operator.eq, '!=': operator.ne}
-            op = operator.eq
-
-            for elem, val in opdict.items():
-                if os_version.startswith(elem):
-                    os_version = os_version.replace(
-                        elem, '').strip()
-                    op = val
-                    break
+                keydata = asyncssh.public_key.read_private_key(pvtkey_file,
+                                                               passphrase)
+            except Exception as e:
+                self.logger.error(
+                    f"ERROR: Unable to read private key file {pvtkey_file}"
+                    f"for jump host due to {str(e)}")
 
-            if op(version_parse.LegacyVersion(version),
-                  version_parse.LegacyVersion(os_version)):
-                return item
-
-        return None
-
-    def _get_device_normalizer(self, data: Dict) -> Dict:
-        '''Returns the normalizer string appropriate for the data
-
-        Every NOS/version has a normalizer string specified in the
-        service config file (under suzieq/config). This function
-        returns that string for the given data input
-        '''
-        nfn = self.defn.get(data.get("hostname"), {})
-        if not nfn:
-            nfn = self.defn.get(data.get("devtype"), {})
-        if nfn:
-            # If we're riding on the coattails of another device
-            # get that device's normalization function
-            if isinstance(nfn, dict):
-                copynfn = nfn.get("copy", {})
-                if copynfn:
-                    nfn = self.defn.get(copynfn, {})
-            if isinstance(nfn, list):
-                nfn = self._get_def_for_version(nfn, data.get("version"))
+        return keydata
 
-        return nfn
+    async def init_node(self):
+        devtype = None
+        hostname = None
 
-    def _process_each_output(self, elem_num, data, nfn):
-        """Workhorse processing routine for each element in output"""
+        if self.transport == "ssh" or self.transport == "local":
+            try:
+                await self.get_device_type_hostname()
+                devtype = self.devtype
+            except Exception as e:
+                self.last_exception = e
+                devtype = None
+
+            if not devtype:
+                self.logger.debug(
+                    f"no devtype for {self.hostname} {self.last_exception}")
+                self._status = "init"
+                return
+            else:
+                self._status = "good"
+                self.set_devtype(devtype)
 
-        result = []
-        if (Service.is_status_ok(data.get('status', -1))):
-            if not data["data"]:
-                return result
-
-            # Check host-specific normalization if any
-            if nfn:
-                norm_str = nfn.get("normalize", None)
-                if norm_str is None and isinstance(nfn.get('command', None),
-                                                   list):
-                    # Can happen because we've a list of commands associated
-                    # Pick the normalization function associated with this
-                    # output
-                    norm_str = nfn.get('command', [])[elem_num].get(
-                        'normalize', None)
-                if norm_str:
-                    if isinstance(data["data"], str):
-                        try:
-                            in_info = json.loads(data["data"])
-                        except json.JSONDecodeError:
-                            in_info = self.clean_json_input(data)
-                            if not in_info:
-                                self.logger.error(
-                                    "Received non-JSON output where "
-                                    "JSON was expected for %s on "
-                                    "node %s, %s",
-                                    data["cmd"], data["hostname"],
-                                    data["data"]
-                                )
-                                return result
-                            try:
-                                in_info = json.loads(in_info)
-                            except json.JSONDecodeError:
-                                self.logger.error(
-                                    "Received non-JSON output where "
-                                    "JSON was expected for %s on "
-                                    "node %s, %s",
-                                    data["cmd"], data["hostname"],
-                                    data["data"]
-                                )
-                                return result
-                    else:
-                        in_info = data["data"]
+                if hostname:
+                    self.set_hostname(hostname)
 
-                    if in_info:
-                        # EOS' HTTP returns errors like this.
-                        if isinstance(in_info, dict):
-                            tmp = in_info.get('data', [])
-                            if tmp and tmp[0].get('errors', {}):
-                                return []
+            await self.init_boot_time()
 
-                        result = cons_recs_from_json_template(
-                            norm_str, in_info)
+    def set_devtype(self, devtype):
+        """Change the class based on the device type"""
+
+        self.devtype = devtype
+        if not devtype:
+            return
+        if devtype not in known_devtypes():
+            self.logger.error(f'An unknown devtype {devtype} is being added.'
+                              ' This will cause problems. Node {self.address}')
+            raise ValueError
+
+        if self.devtype == "cumulus":
+            self.__class__ = CumulusNode
+        elif self.devtype == "eos":
+            self.__class__ = EosNode
+        elif self.devtype.startswith("junos"):
+            self.__class__ = JunosNode
+        elif self.devtype == "nxos":
+            self.__class__ = NxosNode
+        elif self.devtype.startswith("sonic"):
+            self.__class__ == SonicNode
+
+    async def get_device_type_hostname(self):
+        """Determine the type of device we are talking to if using ssh/local"""
+        # There isn't that much of a difference in running two commands versus
+        # running them one after the other as this involves an additional ssh
+        # setup time. show version works on most networking boxes and
+        # hostnamectl on Linux systems. That's all we support today.
+        await self.exec_cmd(self._parse_device_type_hostname,
+                            ["show version", "hostnamectl",
+                             "cat /etc/os-release", "show hostname"], None)
+
+    async def _parse_device_type_hostname(self, output, cb_token) -> None:
+        devtype = ""
+        hostname = None
+
+        if output[0]["status"] == 0:
+            data = output[0]["data"]
+            if "Arista " in data:
+                devtype = "eos"
+            elif "JUNOS " in data:
+                model = re.search(r'Model:\s+(\S+)', data)
+                if model:
+                    if 'mx' in model.group(1):
+                        devtype = 'junos-mx'
+                    elif 'qfx' in model.group(1):
+                        devtype = 'junos-qfx'
+                    elif 'ex' in model.group(1):
+                        devtype = 'junos-ex'
+                if not devtype:
+                    devtype = "junos"
+            elif "NX-OS" in data:
+                devtype = "nxos"
+            elif "SONiC" in data:
+                devtype = "sonic"
+
+            if devtype.startswith("junos"):
+                hmatch = re.search(r'Hostname:\s+(\S+)\n', data)
+                if hmatch:
+                    hostname = hmatch.group(1)
+            elif devtype == "nxos":
+                data = output[3]["data"]
+                hostname = data.strip()
+            elif output[3]["status"] == 0:
+                hostname = output[3]["data"].strip()
+
+        elif output[1]["status"] == 0:
+            data = output[1]["data"]
+            if "Cumulus Linux" in data:
+                devtype = "cumulus"
+            else:
+                devtype = "linux"
+
+            # Hostname is in the first line of hostnamectl
+            hostline = data.splitlines()[0].strip()
+            if hostline.startswith("Static hostname"):
+                _, hostname = hostline.split(":")
+                hostname = hostname.strip()
+
+            if output[2]["status"] == 0:
+                data = output[2]["data"]
+                for line in data.splitlines():
+                    if line.startswith("VERSION_ID"):
+                        self.version = line.split('=')[1] \
+                                           .strip().replace('"', '')
+                        break
+
+        self.set_devtype(devtype)
+        self.set_hostname(hostname)
+
+    async def _parse_boottime_hostname(self, output, cb_token) -> None:
+        """Parse the uptime command output"""
+
+        if self.sigend:
+            return
+
+        if output[0]["status"] == 0:
+            upsecs = output[0]["data"].split()[0]
+            self.bootupTimestamp = int(int(time.time()*1000)
+                                       - float(upsecs)*1000)
+        if output[1]["status"] == 0:
+            self.hostname = output[1]["data"].strip()
+
+    def set_unreach_status(self):
+        self._status = "unreachable"
+
+    def set_good_status(self):
+        self._status = "good"
+
+    def is_alive(self):
+        return self._status == "good"
+
+    def set_hostname(self, hostname=None):
+        if hostname:
+            self.hostname = hostname
+
+    async def local_gather(self, service_callback, cmd_list, cb_token) -> None:
+        """Given a dictionary of commands, run locally and return outputs"""
+
+        result = []
+        for cmd in cmd_list:
+            proc = await asyncio.create_subprocess_shell(cmd, stdout=PIPE,
+                                                         stderr=PIPE)
+
+            try:
+                stdout, stderr = await asyncio.wait_for(
+                    proc.communicate(), timeout=self.cmd_timeout)
 
+                if not proc.returncode:
+                    d = stdout.decode('ascii', 'ignore')
+                    result.append(self._create_result(cmd))
                 else:
-                    tfsm_template = nfn.get("textfsm", None)
-                    entry_type = None
-                    if tfsm_template is None and isinstance(
-                            nfn.get('command', None), list):
-                        # Can happen because we've a list of cmds associated
-                        # Pick the normalization function associated with this
-                        # output
-                        tfsm_template = nfn.get('command', [])[elem_num].get(
-                            'textfsm', None)
-                        entry_type = nfn.get('command', [])[elem_num].get(
-                            '_entryType', None)
-                    else:
-                        entry_type = nfn.get('_entryType', None)
+                    d = stderr('ascii', 'ignore')
+                    result.append(self._create_error(cmd))
+
+            except asyncio.TimeoutError as e:
+                if self.sigend:
+                    self._terminate()
+                    return
 
-                    if not tfsm_template:
-                        return result
+                self.last_exception = e
+                result.append(self._create_error(cmd))
 
-                    in_info = []
-                    if isinstance(data['data'], dict):
-                        if "output" in data["data"]:
-                            in_info = data["data"]["output"]
-                        elif "messages" in data["data"]:
-                            # This is Arista's bash output format
-                            in_info = data["data"]["messages"][0]
-                    else:
-                        in_info = data['data']
-                    if not in_info:
-                        return result  # No data to process
-                    # Clean data is invoked inside this due to the way we
-                    # munge the data and force the types to adhere to the
-                    # specified type
-                    result = self.textfsm_data(
-                        in_info, tfsm_template, entry_type, self.schema, data
+        await service_callback(result, cb_token)
+
+    async def init_boot_time(self):
+        """Fill in the boot time of the node by running the appropriate command"""
+        await self.exec_cmd(self._parse_boottime_hostname, ["cat /proc/uptime",
+                                                            "hostname"], None)
+
+    def post_commands(self, service_callback, svc_defn: dict,
+                      cb_token: RsltToken):
+        if cb_token:
+            cb_token.nodeQsize = self._service_queue.qsize()
+        self._service_queue.put_nowait([service_callback, svc_defn, cb_token])
+
+    async def run(self):
+        tasks = []
+        while True:
+            if self.sigend:
+                self._terminate()
+                return
+
+            while (len(tasks) < self.batch_size):
+                request = await self._service_queue.get()
+                if self.sigend:
+                    await self._terminate()
+                    return
+                if request:
+                    tasks.append(self.exec_service(
+                        request[0], request[1], request[2]))
+                    self.logger.debug(
+                        f"Scheduling {request[2].service} for execution")
+                if self._service_queue.empty():
+                    break
+
+            if tasks:
+                done, pending = await asyncio.wait(
+                    tasks, return_when=asyncio.FIRST_COMPLETED)
+
+                tasks = list(pending)
+
+    async def ssh_gather(self, service_callback, cmd_list, cb_token, timeout):
+        """Given a dictionary of commands, run ssh and place output on service callback"""
+
+        result = []
+
+        if cmd_list is None:
+            await service_callback({}, cb_token)
+
+        if not self._conn:
+            await self._init_ssh()
+            if not self._conn:
+                for cmd in cmd_list:
+                    self.logger.error(
+                        "Unable to connect to node {} cmd {}".format(
+                            self.hostname, cmd))
+                    result.append(self._create_error(cmd))
+                await service_callback(result, cb_token)
+                return
+
+        if isinstance(cb_token, RsltToken):
+            cb_token.node_token = self.bootupTimestamp
+
+        timeout = timeout or self.cmd_timeout
+        for cmd in cmd_list:
+            try:
+                output = await asyncio.wait_for(self._conn.run(cmd),
+                                                timeout=timeout)
+                result.append(self._create_result(
+                    cmd, output.exit_status, output.stdout))
+            except Exception as e:
+                if self.sigend:
+                    self._terminate()
+                    return
+                self.last_exception = e
+                result.append(self._create_error(cmd))
+                if not isinstance(e, asyncio.TimeoutError):
+                    self.logger.error(
+                        f"Unable to connect to {self.hostname} for {cmd} "
+                        f"due to {str(e)}")
+                    await self._close_connection()
+                else:
+                    self.logger.error(
+                        f"Unable to connect to {self.hostname} {cmd} "
+                        "due to timeout")
+
+                break
+
+        await service_callback(result, cb_token)
+
+    async def _close_connection(self):
+        if self._conn:
+            self._conn.close()
+            await self._conn.wait_closed()
+        if self._tunnel:
+            self._tunnel.close()
+            await self._tunnel.wait_closed()
+
+        self._conn = None
+        self._tunnel = None
+
+    async def _terminate(self):
+        self.logger.warning(
+            f'Node: {self.hostname} received signal to terminate')
+        await self._close_connection()
+        return
+
+    def _init_service_queue(self):
+        if not self._service_queue:
+            self._service_queue = asyncio.Queue()
+
+    async def _init_ssh(self, init_boot_time=True) -> None:
+        await self.ssh_ready.wait()
+        if not self._conn:
+            self.ssh_ready.clear()
+            if self.ignore_known_hosts:
+                options = asyncssh.SSHClientConnectionOptions(
+                    client_keys=self.pvtkey if self.pvtkey else None,
+                    login_timeout=self.cmd_timeout,
+                    password=self.password if not self.pvtkey else None,
+                    known_hosts=None,
+                    config=self.ssh_config_file
+                )
+            else:
+                options = asyncssh.SSHClientConnectionOptions(
+                    client_keys=self.pvtkey if self.pvtkey else None,
+                    login_timeout=self.cmd_timeout,
+                    password=self.password if not self.pvtkey else None,
+                    config=self.ssh_config_file,
+                )
+
+            if self.jump_host_key_file:
+                if self.ignore_known_hosts:
+                    jump_host_options = asyncssh.SSHClientConnectionOptions(
+                        client_keys=self.jump_host_key_file,
+                        login_timeout=self.cmd_timeout,
+                        known_hosts=None,
+                        config=self.ssh_config_file,
+                    )
+                else:
+                    jump_host_options = asyncssh.SSHClientConnectionOptions(
+                        client_keys=self.jump_host_key_file,
+                        login_timeout=self.cmd_timeout,
+                        config=self.ssh_config_file,
                     )
             else:
+                jump_host_options = options
+
+            try:
+                if self.jump_host:
+                    self.logger.info(
+                        'Using jump host: {}, with username: {}, and port: {}'
+                        .format(self.jump_host, self.jump_user, self.jump_port)
+                    )
+                    self._tunnel = await asyncssh.connect(
+                        self.jump_host, port=self.jump_port,
+                        options=jump_host_options, username=self.jump_user)
+                    self.logger.info(
+                        f'Connection to jump host {self.jump_host} succeeded')
+
+            except Exception as e:
+                if self.sigend:
+                    self._terminate()
+                    return
                 self.logger.error(
-                    "%s: No normalization/textfsm function for device %s",
-                    self.name, data["hostname"])
+                    f"ERROR: Cannot connect to jump host: {self.jump_host}, "
+                    f" {str(e)}")
+                self.last_exception = e
+                self._conn = None
+                self._tunnel = None
+                self.ssh_ready.set()
+                return
 
+            try:
+                self._conn = await asyncssh.connect(
+                    self.address,
+                    tunnel=self._tunnel,
+                    username=self.username,
+                    port=self.port,
+                    options=options)
+
+                self.logger.info(
+                    f"Connected to {self.address} at {time.time()}")
+                self.ssh_ready.set()
+                if init_boot_time:
+                    await self.init_boot_time()
+            except Exception as e:
+                if self.sigend:
+                    self._terminate()
+                    return
+                self.logger.error(f"ERROR: Unable to connect, {str(e)}")
+                self.last_exception = e
+                self._conn = None
+                self._tunnel = None
+                self.ssh_ready.set()
+        return
+
+    def _create_error(self, cmd) -> dict:
+        data = {'error': str(self.last_exception)}
+        if isinstance(self.last_exception, TimeoutError):
+            status = HTTPStatus.REQUEST_TIMEOUT
+        elif isinstance(self.last_exception, asyncssh.misc.ProtocolError):
+            status = HTTPStatus.FORBIDDEN
+        elif hasattr(self.last_exception, 'code'):
+            status = self.last_exception.code
+        else:
+            status = -1
+        return self._create_result(cmd, status, data)
+
+    def _create_result(self, cmd, status, data) -> dict:
+        result = {
+            "status": status,
+            "timestamp": int(datetime.utcnow().timestamp() * 1000),
+            "cmd": cmd,
+            "devtype": self.devtype,
+            "namespace": self.nsname,
+            "hostname": self.hostname,
+            "address": self.address,
+            "version": self.version,
+            "data": data,
+        }
         return result
 
-    def process_data(self, data):
-        """Derive the data to be stored from the raw input"""
-        result_list = []
-        do_merge = True
-        for i, item in enumerate(data):
-            nfn = self._get_device_normalizer(item)
-            do_merge = do_merge and nfn and nfn.get('merge', True)
-            tmpres = self._process_each_output(i, item, nfn)
-            result_list.append(tmpres)
+    async def rest_gather(self, svc_dict, oformat="json"):
+        raise NotImplementedError
+
+    async def exec_cmd(self, service_callback, cmd_list, cb_token,
+                       oformat='json', timeout=None):
 
-        if do_merge:
-            result = self.merge_results(result_list, data)
+        if self.transport == "ssh":
+            await self.ssh_gather(service_callback, cmd_list, cb_token, timeout)
+        elif self.transport == "https":
+            await self.rest_gather(service_callback, cmd_list,
+                                   cb_token, oformat, timeout)
+        elif self.transport == "local":
+            await self.local_gather(service_callback, cmd_list,
+                                    cb_token, timeout)
         else:
-            result = [ele for sublist in result_list for ele in sublist]
-        return self.clean_data(result, data)
+            self.logger.error(
+                "Unsupported transport {} for node {}".format(
+                    self.transport, self.hostname
+                )
+            )
 
-    def get_key_flds(self):
-        """Get the key fields associated with this service.
-        Its a function because we want to override it.
-        """
-        return list(filter(lambda x: x not in ['namespace', 'hostname'],
-                           self.keys))
-
-    def merge_results(self, result_list, _):
-        '''Merge the results from multiple commands into a single result'''
-
-        int_res = {}
-        keyflds = self.get_key_flds()
-
-        for result in result_list:
-            for entry in result:
-                keyvals = []
-                for kfld in keyflds:
-                    if not entry.get(kfld, None):
-                        keyvals.append('_default')
-                    else:
-                        val = entry.get(kfld, '')
-                        if not isinstance(val, str):
-                            val = str(val)
-                        keyvals.append(val)
+        return
+
+    async def exec_service(self, service_callback, svc_defn: dict,
+                           cb_token: RsltToken):
 
-                if entry.get('_entryType', ''):
-                    keyvals.append(entry['_entryType'])
+        result = []  # same type as gather function
+        cmd = None
+        if not svc_defn:
+            return result
+
+        if self._status == "init":
+            if self.init_again_at < time.time():
+                await self.init_node()
+
+        if self._status == "init":
+            result.append(self._create_error(svc_defn.get("service", "-")))
+            return await service_callback(result, cb_token)
+
+        # Update our boot time value into the callback token
+        if cb_token:
+            cb_token.bootupTimestamp = self.bootupTimestamp
+
+        self.svcs_proc.add(svc_defn.get("service"))
+        use = svc_defn.get(self.hostname, None)
+        if not use:
+            use = svc_defn.get(self.devtype, {})
+        if not use:
+            if svc_defn.get("service") not in self.error_svcs_proc:
+                result.append(self._create_result(
+                    svc_defn, HTTPStatus.NOT_FOUND, "No service definition"))
+                self.error_svcs_proc.add(svc_defn.get("service"))
+            return await service_callback(result, cb_token)
+
+        # TODO This kind of logic should be encoded in config and node shouldn't have to know about it
+        if "copy" in use:
+            use = svc_defn.get(use.get("copy"))
+
+        if use:
+            if isinstance(use, list):
+                # There's more than one version here, we have to pick ours
+                for item in use:
+                    if (item["version"] == "all" or
+                            item["version"] == self.version):
+                        cmd = item.get("command", None)
+                        break
+            else:
+                cmd = use.get("command", None)
 
-                key = '-'.join(keyvals)
+        oformat = svc_defn.get(self.devtype, {}).get("format", "json")
 
-                if key not in int_res:
-                    int_res[key] = entry
-                else:
-                    existing = int_res[key]
-                    for fld in entry:
-                        if entry[fld] and not existing.get(fld, None):
-                            existing[fld] = entry[fld]
-                        elif entry[fld]:
-                            # cleanup routine specific to service can resolve
-                            existing[fld+"-_2nd"] = entry[fld]
-
-        final_res = list(int_res.values())
-
-        return (final_res)
-
-    def _get_devtype_from_input(self, input_data):
-        if isinstance(input_data, list):
-            return input_data[0].get('devtype', None)
+        if not cmd:
+            return result
+
+        if type(cmd) is not list:
+            cmdlist = [cmd]
         else:
-            return input_data.get('devtype', None)
+            cmdlist = [x.get('command', '') for x in cmd]
 
-    def clean_data(self, processed_data, raw_data):
-        """Massage the extracted data to match record specified by schema"""
+        await self.exec_cmd(service_callback, cmdlist, cb_token,
+                            oformat=oformat, timeout=cb_token.timeout)
 
-        dev_clean_fn = self.dev_clean_fn.get(self._get_devtype_from_input(
-            raw_data), None)
-        if dev_clean_fn:
-            processed_data = dev_clean_fn(processed_data, raw_data)
-
-        return self.clean_data_common(processed_data, raw_data)
-
-    def clean_data_common(self, processed_data, raw_data):
-        """Fix the type and default value of of each extracted field
-
-        This routine is common to all services. It ensures that all the missing
-        fields, as defined by the schema, are added to the records extracted.
-        Furthermore, each field is set to the specified type.
-        """
-
-        # Build default data structure
-        schema_rec = {}
-        def_vals = get_default_per_vals()
-
-        ptype_map = {
-            pa.string(): str,
-            pa.int32(): int,
-            pa.int64(): int,
-            pa.float32(): float,
-            pa.float64(): float,
-            pa.date64(): float,
-            pa.list_(pa.string()): list,
-            pa.list_(pa.int64()): list,
-            pa.bool_(): bool,
-        }
 
-        for fld in self.schema:
-            default = def_vals[fld.type]
-            schema_rec.update({fld.name: default})
+class EosNode(Node):
+    def _init(self, **kwargs):
+        super()._init(kwargs)
+        self.devtype = "eos"
+
+    async def init_node(self):
+        try:
+            await self.get_device_boottime_hostname()
+        except Exception as e:
+            if self.sigend:
+                self._terminate()
+                return
+            self.last_exception = e
 
-        if isinstance(raw_data, list):
-            read_from = raw_data[0]
-        else:
-            read_from = raw_data
+    async def get_device_type_hostname(self):
+        raise NotImplementedError
 
-        # pylint: disable=too-many-nested-blocks
-        for entry in processed_data or []:
-            entry.update({
-                "hostname": read_from["hostname"],
-                "namespace": read_from["namespace"],
-                "timestamp": read_from["timestamp"],
-                "sqvers": self.version
-            })
-            for fld, val in schema_rec.items():
-                if fld not in entry:
-                    if fld == "active":
-                        entry.update({fld: True})
-                    else:
-                        entry.update({fld: val})
-                else:
-                    fld_type = self.schema.field(fld).type
-                    if not isinstance(entry[fld], ptype_map[fld_type]):
-                        try:
-                            entry[fld] = ptype_map[fld_type](entry[fld])
-                        except (ValueError, TypeError):
-                            entry[fld] = val
-                    elif isinstance(entry[fld], list):
-                        for i, ele in enumerate(entry[fld]):
-                            if not isinstance(ele,
-                                              ptype_map[fld_type.value_type]):
-                                try:
-                                    if ptype_map[fld_type.value_type] == int:
-                                        entry[fld][i] = int(entry[fld][i])
-                                    elif ptype_map[fld_type.value_type] == str:
-                                        entry[fld][i] = str(entry[fld][i])
-                                    else:
-                                        raise ValueError
-                                except (ValueError, TypeError):
-                                    entry[fld][i] = val
-        return processed_data
-
-    async def commit_data(self, result: Dict, namespace: str, hostname: str,
-                          boot_timestamp: int):
-        """Write the result data out"""
-        records = []
-        key = f'{namespace}.{hostname}'
-        prev_res = self.previous_results.get(key, None)
-        last_device_session = self._node_boot_timestamps.get(key, 0)
-        # No data previously polled with this service from the the
-        # current namespace and hostname. Check if the datastore contains some
-        # information about
-        filter_df = f"hostname.str.match('{hostname}') and " \
-                    f"namespace.str.match('{namespace}')"
-        if prev_res is None:
-            df = self._db_access.read(
-                self.schema_table._table,
-                'pandas',
-                start_time='',
-                end_time='',
-                columns=self.schema_table.fields,
-                view='latest',
-                key_fields=self.schema_table.key_fields(),
-                add_filter=filter_df,
-                hostname=[hostname],
-                namespace=[namespace]).query('active')
-            # Get the latest device session we have written with this service
-            if not df.empty:
-                # If we are dealing with old data then the value of
-                # deviceSession will be unset, if this is the case, set the
-                # value to 0 so that we force write. We need to check only
-                # the first value of deviceSession as it is equal for all the
-                # latest record, as in case of reboot we rewrite everything.
-                if not df['deviceSession'].iloc[:1].isnull().any():
-                    last_device_session = df['deviceSession'].iloc[0] or 0
-                else:
-                    last_device_session = 0
+    async def get_device_boottime_hostname(self):
+        """Determine the type of device we are talking to"""
 
-                self._node_boot_timestamps[key] = int(last_device_session)
+        if self.transport == 'https':
+            cmdlist = ["show version", "show hostname"]
+        else:
+            cmdlist = ["show version|json", "show hostname|json"]
+        await self.exec_cmd(self._parse_boottime_hostname, cmdlist, None)
 
-            prev_res = df.to_dict('records')
-            self.previous_results[key] = prev_res
+    async def _parse_boottime_hostname(self, output, cb_token) -> None:
 
-        if result or prev_res:
-            # Check whether there has been a node reboot and in this case
-            # write everything
-            write_all = abs(boot_timestamp -
-                            last_device_session) > TIME_DRIFT_TOLERANCE
-            if write_all:
-                last_device_session = int(boot_timestamp)
-                self._node_boot_timestamps[key] = boot_timestamp
-
-            adds, dels = self.get_diff(prev_res, result, write_all)
-            if adds or dels:
-                self.previous_results[key] = copy.deepcopy(result)
-                for entry in adds:
-                    entry['deviceSession'] = last_device_session
-                    records.append(entry)
-                # make sure to use the same timestamp for all the deleted
-                # records. If the result is not empty, use that to get the
-                # timestamp. If the result is empty, use the current timestamp
-                if result:
-                    del_ts = result[0]['timestamp']
-                else:
-                    del_ts = int(datetime.now(
-                        tz=timezone.utc).timestamp() * 1000)
+        if output[0]["status"] == 0 or output[0]["status"] == 200:
+            data = output[0]["data"]
+            self.bootupTimestamp = data["bootupTimestamp"]
+
+        if output[1]["status"] == 0 or output[1]["status"] == 200:
+            data = output[1]["data"]
+            self.hostname = data["hostname"]
+            self._status = "good"
 
-                for entry in dels:
-                    if entry.get("active", True):
-                        # If there's already an entry marked as deleted
-                        # No point in adding one more
-                        entry.update({
-                            "active": False,
-                            "timestamp": del_ts
-                        })
-                        records.append(entry)
-
-                self._post_work_to_writer(records)
-
-    def _post_work_to_writer(self, records: dict):
-        """This posts the data to be written to the worker queue"""
-        if records:
-            self.writer_queue.put_nowait(
-                {
-                    "records": records,
-                    "topic": self.name,
-                    "schema": self.schema,
-                    "partition_cols": self.partition_cols
-                }
-            )
+    async def rest_gather(self, service_callback, cmd_list, cb_token,
+                          oformat="json", timeout=None):
 
-    def reset_stats(self, stats: ServiceStats) -> None:
-        """Reset the stats arrays.
-        """
-        stats.total_time = []
-        stats.gather_time = []
-        stats.svcQsize = []
-        stats.nodeQsize = []
-        stats.wrQsize = []
-        stats.rxBytes = []
-        stats.empty_count = 0
-        stats.time_excd_count = 0
-
-    def compute_basic_stats(self, statsList, newval: int) -> None:
-        """Compute min/max/avg for given stats with the new value
-
-        :param statsList: list consisting of 3 values in order: min, max, avg
-        :type statsList: list_
-
-        :param newval: The newval to update the list with
-        :type newval: int
-        """
-        if not statsList:
-            statsList = [newval, newval, newval]
-            return statsList
-
-        if newval < statsList[0]:
-            statsList[0] = newval
-        if newval > statsList[1]:
-            statsList[1] = newval
-        statsList[2] = (statsList[2]+newval)/2
-        if statsList[2] < 0.001:
-            statsList[2] = 0
-
-        return statsList
-
-    def update_stats(self, stats: ServiceStats, total_time: int,
-                     gather_time: int, qsize: int, wrQsize: int,
-                     nodeQsize: int, rxBytes) -> bool:
-        """Update per-node stats"""
-        write_stat = False
-        now = int(time.time()*1000)
-
-        stats.total_time = self.compute_basic_stats(stats.total_time,
-                                                    total_time)
-        stats.gather_time = self.compute_basic_stats(stats.gather_time,
-                                                     gather_time)
-        stats.svcQsize = self.compute_basic_stats(stats.svcQsize, qsize)
-        stats.wrQsize = self.compute_basic_stats(stats.wrQsize, wrQsize)
-        stats.nodeQsize = self.compute_basic_stats(stats.nodeQsize, nodeQsize)
-        stats.rxBytes = self.compute_basic_stats(stats.rxBytes, rxBytes)
-
-        if total_time > self.period*1000:
-            stats.time_excd_count += 1
-            write_stat = True
-
-        if now > stats.next_update_time:
-            stats.next_update_time = now + 5*60*1000  # 5 mins
-            write_stat = True
-
-        return write_stat
-
-    def is_first_run(self, key: str) -> bool:
-        '''Boolean indicating wether the current run
-           is the first since the service is running.
-        '''
-        return not self.previous_results.get(key, None)
+        result = []
+        if not cmd_list:
+            return result
 
-    # pylint: disable=too-many-statements
-    async def run(self):
-        """Start the service"""
-        self.logger.info(f"running service {self.name} ")
+        timeout = timeout or self.cmd_timeout
 
-        if self.run_once:
-            total_nodes = len(self.node_postcall_list)
+        now = int(datetime.utcnow().timestamp() * 1000)
+        auth = aiohttp.BasicAuth(self.username, password=self.password)
+        data = {
+            "jsonrpc": "2.0",
+            "method": "runCmds",
+            "id": int(now),
+            "params": {"version": 1, "format": oformat, "cmds": cmd_list},
+        }
+        headers = {"Content-Type": "application/json"}
+        if self.port:
+            url = "https://{}:{}/command-api".format(self.address, self.port)
         else:
-            total_nodes = 0
-        # Fire up the initial posts
-        await self.start_data_gather()
-        loop = asyncio.get_running_loop()
-        # pylint: disable=unnecessary-lambda
-        pernode_stats = defaultdict(lambda: ServiceStats())
+            url = "https://{}:{}/command-api".format(self.address, self.port)
 
-        while True:
-            try:
-                token, output = await self.result_queue.get()
-            except asyncio.CancelledError:
-                self.logger.warning(
-                    f'Service: {self.name}: Received signal to terminate')
-                return
-            qsize = self.result_queue.qsize()
+        output = []
+        status = 200  # status OK
 
-            self.logger.debug(f"Extracted response for {self.name} service")
-            if isinstance(token, list):
-                token = token[0]
-            gather_time = int(time.time()*1000) - token.start_time
-
-            status = HTTPStatus.NO_CONTENT        # Empty content
-            write_poller_stat = False
-            rxBytes = 0
-
-            if output:
-                ostatus = [x.get('status', -1) for x in output]
-
-                should_commit = True
-
-                # we should always commit during the first run of the service
-                # for each node regardless their status.
-                if not self.is_first_run(token.nodename):
-                    # If it's not the first run and some command did fail,
-                    # increment the count to be used in hysteresis.
-                    # The info will be committed in a future run.
-                    if any((not Service.is_status_ok(x) for x in ostatus)):
-                        self._consecutive_failures[token.nodename] += 1
-                    # otherwise reset the counter.
+        try:
+            async with aiohttp.ClientSession(
+                    auth=auth,
+                    conn_timeout=self.connect_timeout,
+                    read_timeout=timeout,
+                    connector=aiohttp.TCPConnector(ssl=False),
+            ) as session:
+                async with session.post(url, json=data, headers=headers) as response:
+                    status, json_out = response.status, await response.json()
+                    if "result" in json_out:
+                        output.extend(json_out["result"])
                     else:
-                        self._consecutive_failures[token.nodename] = 0
+                        output.extend(json_out["error"])
 
-                if 0 < self._consecutive_failures[token.nodename] < \
-                        HYSTERESIS_FAILURE_CNT:
-                    self.logger.info(
-                        f"{self.name} {token.nodename} node failure hysteresis"
-                        ", skipping data commit")
-                    should_commit = False
-
-                # pylint: disable=use-a-generator
-                write_poller_stat = not all([Service.is_status_ok(x)
-                                             for x in ostatus])
-                status = ostatus[0]
-                if (status in [0, 200]):
-                    rxBytes = len(str(output))
-
-                # We don't expect the output from two different hostnames
-                nodename = output[0]["hostname"]
-                self.logger.debug(f"Extracted response from {nodename} for "
-                                  f"{self.name} service")
-                # We can terminate processing if we've no data returned
-                # and we're reading inputs from a file
-                if nodename == '_filedata' and status == HTTPStatus.NO_CONTENT:
-                    return
+            for i, cmd in enumerate(cmd_list):
+                result.append(
+                    {
+                        "status": status,
+                        "timestamp": now,
+                        "cmd": cmd,
+                        "devtype": self.devtype,
+                        "namespace": self.nsname,
+                        "hostname": self.hostname,
+                        "address": self.address,
+                        "data": output[i] if type(output) is list else output,
+                    }
+                )
+        except Exception as e:
+            if self.sigend:
+                self._terminate()
+                return
+            self.last_exception = e
+            for cmd in cmd_list:
+                result.append(self._create_error(cmd))
+            self._status = "init"  # Recheck everything
+            self.logger.error("ERROR: (REST) Unable to communicate with node "
+                              "{} due to {}".format(self.address, str(e)))
+
+        await service_callback(result, cb_token)
+
+    async def _parse_hostname(self, output, cb_token) -> None:
+        """Parse the hostname command output"""
+        if not output:
+            self.hostname = "-"
+            return
 
-                # Process data independent of status to return an empty list
-                # so that the output can be updated. For example, if a service
-                #  is disabled, this can be the condition.
-                if self.run_once == "gather":
-                    if self.is_status_ok(status):
-                        self._post_work_to_writer(json.dumps(output, indent=4))
-                    total_nodes -= 1
-                    if total_nodes <= 0:
-                        self.logger.warning(
-                            f'Service: {self.name}: Finished gathering data')
-                        return
-                    continue
-
-                try:
-                    result = self.process_data(output)
-                except Exception:  # pylint: disable=broad-except
-                    result = []
-                    status = HTTPStatus.BAD_GATEWAY
-                    write_poller_stat = True
-                    self.logger.exception(
-                        f'Processing data failed for service '
-                        f'{self.name} on node {nodename}')
-
-                # Don't write the error every time the failure happens
-                if write_poller_stat:
-                    if nodename in self._failed_node_set:
-                        write_poller_stat = False
-                    else:
-                        self._failed_node_set.add(nodename)
-                elif nodename in self._failed_node_set:
-                    # So there was no error in this command that had failed b4
-                    self._failed_node_set.remove(nodename)
-
-                # If a node from init state to good state, hostname will change
-                # So fix that in the node list
-                if self.run_once == "process":
-                    if self.is_status_ok(status):
-                        self._post_work_to_writer(json.dumps(result, indent=4))
-                    total_nodes -= 1
-                    if total_nodes <= 0:
-                        return
-                    continue
-
-                if should_commit:
-                    await self.commit_data(result, output[0]["namespace"],
-                                           output[0]["hostname"],
-                                           token.bootupTimestamp)
-            elif self.run_once in ["gather", "process", "update"]:
-                total_nodes -= 1
-                if total_nodes <= 0:
-                    self.logger.info(f'Service: {self.name}: Finished '
-                                     f'{self.run_once}ing data')
-                    return
-                continue
+        if output[0]["status"] == 0:
+            data = output[1]["data"]
+            try:
+                jout = json.loads(data)
+                self.hostname = jout["hostname"]
+            except:
+                self.hostname = "-"
+
+
+class CumulusNode(Node):
+    def _init(self, **kwargs):
+        if "username" not in kwargs:
+            kwargs["username"] = "cumulus"
+        if "password" not in kwargs:
+            kwargs["password"] = "CumulusLinux!"
 
-            total_time = int(time.time()*1000) - token.start_time
+        super()._init(kwargs)
+        self.devtype = "cumulus"
 
-            if output:
+    async def rest_gather(self, service_callback, cmd_list, cb_token,
+                          oformat='json', timeout=None):
 
-                stats = pernode_stats[token.nodename]
-                write_poller_stat = (self.update_stats(
-                    stats, total_time, gather_time, qsize,
-                    self.writer_queue.qsize(), token.nodeQsize, rxBytes) or
-                    write_poller_stat or
-                    self.is_first_run(token.nodename))
-                pernode_stats[token.nodename] = stats
-                if write_poller_stat:
-                    poller_stat = [
-                        {"hostname": (output[0]["hostname"] or
-                                      output[0]['address']),
-                         "sqvers": self.poller_schema_version,
-                         "namespace": output[0]["namespace"],
-                         "active": True,
-                         "service": self.name,
-                         "status": status,
-                         "svcQsize": stats.svcQsize,
-                         "wrQsize": stats.wrQsize,
-                         "nodeQsize": stats.nodeQsize,
-                         "rxBytes": stats.rxBytes,
-                         "pollExcdPeriodCount": stats.time_excd_count,
-                         "gatherTime": stats.gather_time,
-                         "totalTime": stats.total_time,
-                         "version": SUZIEQ_VERSION,
-                         "nodesPolledCnt": len(self.node_postcall_list),
-                         "nodesFailedCnt": len(self._failed_node_set),
-                         "timestamp": int(datetime.now(tz=timezone.utc)
-                                          .timestamp() * 1000)}]
-
-                    self.writer_queue.put_nowait(
-                        {
-                            "records": poller_stat,
-                            "topic": "sqPoller",
-                            "schema": self.poller_schema,
-                            "partition_cols": self.partition_cols
-                        })
-                    self.reset_stats(pernode_stats[token.nodename])
-
-            # Post a cmd to fire up the next poll after the specified period
-            if self.run_once == "update":
-                total_nodes -= 1
-                if total_nodes <= 0:
-                    self.logger.info(
-                        f'Service: {self.name}: Finished updating data')
-                    return
-                continue
-            self.logger.debug(
-                f"Rescheduling service for {self.name} service")
-            loop.call_later(self.period, self.call_node_postcmd,
-                            self.node_postcall_list.get(token.nodename),
-                            token.nodename)
+        result = []
+        if not cmd_list:
+            return result
+
+        auth = aiohttp.BasicAuth(self.username, password=self.password)
+        url = "https://{0}:{1}/nclu/v1/rpc".format(self.address, self.port)
+        headers = {"Content-Type": "application/json"}
+
+        try:
+            async with aiohttp.ClientSession(
+                    auth=auth,
+                    timeout=timeout or self.cmd_timeout,
+                    connector=aiohttp.TCPConnector(ssl=False),
+            ) as session:
+                for cmd in cmd_list:
+                    data = {"cmd": cmd}
+                    async with session.post(
+                            url, json=data, headers=headers
+                    ) as response:
+                        result.append(
+                            {
+                                "status": response.status,
+                                "timestamp": int(datetime.utcnow().timestamp() * 1000),
+                                "cmd": cmd,
+                                "devtype": self.devtype,
+                                "namespace": self.nsname,
+                                "hostname": self.hostname,
+                                "address": self.address,
+                                "data": await response.text(),
+                            }
+                        )
+        except Exception as e:
+            if self.sigend:
+                self._terminate()
+                return
+            self.last_exception = e
+            result.append(self._create_error(cmd))
+            self.logger.error("ERROR: (REST) Unable to communicate with node "
+                              "{} due to {}".format(self.address, str(e)))
+
+        await service_callback(result, cb_token)
+
+
+class JunosNode(Node):
+
+    async def init_boot_time(self):
+        """Fill in the boot time of the node by running requisite cmd"""
+        await self.exec_cmd(self._parse_boottime_hostname,
+                            ["show system uptime|display json",
+                             "show version"], None)
+
+    async def _parse_boottime_hostname(self, output, cb_token) -> None:
+        """Parse the uptime command output"""
+        if output[0]["status"] == 0:
+            data = output[0]["data"]
+            try:
+                jdata = json.loads(data.replace('\n', '').strip())
+                if self.devtype == 'junos-qfx' or 'juniper-ex':
+                    jdata = jdata['multi-routing-engine-results'][0]['multi-routing-engine-item'][0]
+
+                timestr = jdata['system-uptime-information'][0]['system-booted-time'][0]['time-length'][0]['attributes']
+            except Exception:
+                self.logger.warning(
+                    f'Unable to parse junos boot time from {data}')
+                timestr = '{"junos:seconds": "0"}'
+            self.bootupTimestamp = (get_timestamp_from_junos_time(
+                timestr, output[0]['timestamp']/1000)/1000)
+
+        if output[1]["status"] == 0:
+            data = output[0]["data"]
+            hmatch = re.search(r'\nHostname:\s+(\S+)\n', data)
+            if hmatch:
+                self.set_hostname(hmatch.group(1))
+
+
+class NxosNode(Node):
+
+    async def init_boot_time(self):
+        """Fill in the boot time of the node by running requisite cmd"""
+        await self.exec_cmd(self._parse_boottime_hostname,
+                            ["show version|json", "show hostname"], None)
+
+    async def _parse_boottime_hostname(self, output, cb_token) -> None:
+        """Parse the uptime command output"""
+
+        if output[0]["status"] == 0:
+            data = json.loads(output[0]["data"])
+            upsecs = (24*3600*int(data.get('kern_uptm_days', 0)) +
+                      3600*int(data.get('kern_uptm_hrs', 0)) +
+                      60*int(data.get('kern_uptm_mins', 0)) +
+                      int(data.get('kern_uptm_secs', 0)))
+            if upsecs:
+                self.bootupTimestamp = int(int(time.time()*1000)
+                                           - float(upsecs)*1000)
+
+        if output[1]["status"] == 0:
+            hostname = output[1]["data"].strip()
+            if hostname:
+                self.set_hostname(hostname)
+
+
+class SonicNode(Node):
+
+    async def init_boot_time(self):
+        """Fill in the boot time of the node by running requisite cmd"""
+        await self.exec_cmd(self._parse_boottime_hostname, ["cat /proc/uptime",
+                                                            "hostname"], None)
+
+    async def _parse_boottime_hostname(self, output, cb_token) -> None:
+        """Parse the uptime command output"""
+
+        if output[0]["status"] == 0:
+            upsecs = output[0]["data"].split()[0]
+            self.bootupTimestamp = int(int(time.time()*1000)
+                                       - float(upsecs)*1000)
+        if output[1]["status"] == 0:
+            self.hostname = output[1]["data"].strip()
```

### Comparing `suzieq-0.22.0rc1/suzieq/poller/worker/services/svcparser.py` & `suzieq-0.8.0/suzieq/poller/services/svcparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import re
 import ast
 import logging
 import operator as op
 
-# pylint: disable=too-many-nested-blocks, too-many-statements
-
 
 def _stepdown_rest(entry) -> list:
     '''move the elements one level down into the existing JSON hierarchy.
 
     if `entry` has the structure {'vrfs': {'routes'...} on invocation,
     it'll be {'routes'...} on exit. It makes no sense to move down them
     hierarchy when you have only a list.
@@ -21,121 +19,14 @@
             entry += [{"rest": data[key]}]
     else:
         entry = [entry]
 
     return entry
 
 
-def parse_subtree(subflds, tmpval, maybe_list, defval):
-    '''Parse a nested subtree'''
-
-    value = []
-    useval = False
-
-    for i, subfld in enumerate(subflds):
-        subfld = subfld.strip()
-        if ':_sqstore' in subfld:
-            storekey = True
-            subfld = '*'
-        else:
-            storekey = False
-        if subfld == "*":
-            tmp = tmpval
-            for subele in tmp:
-                if storekey:
-                    storeval = subele
-                for ele in subflds[i+1:]:
-                    if isinstance(tmp, list):
-                        subele = subele.get(ele, None)
-                    else:
-                        subele = tmp[subele].get(ele, None)
-                    if subele is None:
-                        tmpval = None
-                        break
-                if subele:
-                    if storekey:
-                        value.append(storeval)
-                    else:
-                        value.append(subele)
-                    useval = True
-            break
-        if subfld.startswith('['):
-            # handle specific array index or dict key
-            # This additional handling of * is because of JUNOS
-            # interface address which is many levels deep and mixes
-            # IPv4/v6 address in a way that we can't entirely fix
-            # Post processing cleanup has to handle that part
-            if subfld.endswith('?'):
-                # This was added thanks to NXOS which provides
-                # nexthops as a list if ECMP, else a dictionary
-                if not isinstance(tmpval, list):
-                    continue
-                subfld = subfld[:-1]  # lose the final "?" char
-            if subfld == '[*]':
-                for item in tmpval:
-                    newval = parse_subtree(subflds[i+1:], item, maybe_list,
-                                           defval)
-                    if newval is not None:
-                        if isinstance(newval, list):
-                            value += newval
-                        else:
-                            value.append(newval)
-                useval = True
-                break
-            if tmpval:
-                tmpval = tmpval[eval_expr(subfld)]
-        elif isinstance(tmpval, dict):
-            tmpval = tmpval.get(subfld, None)
-        else:
-            tmpval = None
-
-        if not tmpval:
-            break
-
-    if useval:
-        if value:
-            return value
-        else:
-            return defval
-    else:
-        return tmpval
-
-
-def copy_keys_into_each_ele(result):
-    '''Copy key values into each element of sublist
-    Handle output like EOS OSPF output with the starting string
-    vrfs/*:vrf/instList/*:instance/ospfNeighborEntries/*/[
-    Move the keys into each element of the lists we need to pop
-    out these keys at the very end
-    '''
-    for entry in result:
-        elekeys = entry[0].keys() - set(['rest'])
-        if not elekeys:
-            # this happens when NXOS routes returns
-            # half-baked data when there are no routes
-            # in a VRF.
-            continue
-        for rstentry in entry[0]['rest']:
-            if isinstance(rstentry, list):
-                for entry2 in rstentry:
-                    entry2['sq-addnl-keys'] = []
-                    for key in elekeys:
-                        entry2['sq-addnl-keys'].append({
-                            key: entry[0][key]})
-            else:
-                rstentry['sq-addnl-keys'] = []
-                for key in elekeys:
-                    rstentry['sq-addnl-keys'].append({
-                        key: entry[0][key]})
-        for key in elekeys:
-            del entry[0][key]
-
-    return result
-
-
 def cons_recs_from_json_template(tmplt_str, in_data):
     ''' Return an array of records given the template and input data.
 
     This uses an XPATH-like template string to create a list of records
     matching the template. It also normalizes the key fields so that we
     can create records with keys that are agnostic of the source.
 
@@ -187,71 +78,55 @@
     except ValueError:
         ppos = 0                # completely flat JSON struct
     while ppos > 0:
         xstr = tmplt_str[0:pos]
 
         if ":" not in xstr:
             if not result:
-                if xstr not in ['*', '*?']:
+                if xstr != '*' and xstr != '*?':
                     if not data or not data.get(xstr, None):
                         # Some outputs contain just the main key with a null
                         # body such as ospfNbr from EOS: {'vrfs': {}}.
-                        logging.info(
-                            f"Unnatural return from svcparser. xstr is {xstr}.\
-                             Result is {result}")
+                        logging.error(
+                            f"Unnatural return from svcparser. xstr is {xstr}. \
+                            Result is {result}")
                         return cleanup_and_return(result)
                     result = [{"rest": data[xstr]}]
                 else:
                     if isinstance(data, dict):
                         result = [{"rest": []}]
                         for key in data.keys():
                             result[0]["rest"].append(data[key])
                     else:
                         result = [{"rest": data}]
             else:
-                if xstr not in ["*", '*?']:
+                if xstr != "*" and xstr != '*?':
                     # Handle xstr being a specific array index or dict key
                     if xstr.startswith('['):
                         if len(result[0]['rest']):
-                            result[0]["rest"] = result[0]["rest"][eval_expr(
-                                xstr)]
+                            result[0]["rest"] = result[0]["rest"][eval_expr(xstr)]
                         else:
                             # Handling the JUNOS EVPN pfx DB entry
-                            logging.info(
+                            logging.error(
                                 f'Unnatural return from svcparser. '
                                 f'xstr is {xstr}. Result is {result}')
                             return []
 
                     else:
                         tmpval = []
                         for ele in result:
                             # EOS routes case: vrfs/*:vrf/routes/*:prefix
                             # Otherwise there's usually one element here
-                            if isinstance(ele["rest"], list) and ele['rest']:
-                                # We need to check for empty rest because in
-                                # older NXOS, where there are OSPF neighbors
-                                # defined in a VRF, we can end up in this
-                                # if clause and miss out on good data thats
-                                # actually present in the else clause of this.
-                                for subidx, subele in enumerate(ele["rest"]):
+                            if isinstance(ele["rest"], list):
+                                for subele in ele["rest"]:
                                     if xstr in subele:
-                                        if nokeys:
-                                            tmpval.append(
-                                                {"rest": subele[xstr]})
-                                        else:
-                                            ele['rest'][subidx] = subele[xstr]
-                                if not nokeys:
-                                    if len(ele['rest']) == 1:
-                                        ele['rest'] = ele['rest'][0]
-
-                                    tmpval.append(ele)
+                                        tmpval.append({"rest": subele[xstr]})
                             else:
-                                if xstr in (ele['rest'] or {}):
+                                if xstr in ele['rest']:
                                     ele["rest"] = ele["rest"][xstr]
-
                         if tmpval:
                             result = tmpval
                 else:
                     if (xstr == '*?'):
                         # Massaging the format to handle cases like NXOS that
                         # provide dict when there's a single element and a list
                         # if there's more than one element
@@ -270,26 +145,36 @@
                         tmpres = result[0]
                         if tmpres[0].keys() != set(['rest']):
                             # Handle output like EOS OSPF output with the
                             # starting string:
                             # vrfs/*:vrf/instList/*:instance/ospfNeighborEntries/*/[
                             # Move the keys into each element of the lists
                             # we need to pop out these keys at the very end
-                            result = copy_keys_into_each_ele(result)
-                            tmpres = result[0]
-                            nokeys = True  # We've moved all the external keys
+                            for entry in result:
+                                elekeys = entry[0].keys() - set(['rest'])
+                                if not elekeys:
+                                    # this happens when NXOS routes returns
+                                    # half-baked data when there are no routes
+                                    # in a VRF.
+                                    continue
+                                for rstentry in entry[0]['rest']:
+                                    rstentry['sq-addnl-keys'] = []
+                                    for key in elekeys:
+                                        rstentry['sq-addnl-keys'].append({
+                                            key: entry[0][key]})
+                                for key in elekeys:
+                                    del entry[0][key]
+                                # We should only have 'rest' entries now
+                            nokeys = True  # We've moved all the external keys in
 
                         # Handle the output of the likes of EOS' BGP with
                         # starting string: 'vrfs/*/peerList/*/[ by
                         # merging the rest lists
                         for entry in result[1:]:
-                            # in case of junos routes, we sometimes end up with
-                            # {'rest': 'keepalive'} as an element. Ignore that
-                            if isinstance(tmpres[0]['rest'], list):
-                                tmpres[0]['rest'].extend(entry[0]['rest'])
+                            tmpres[0]['rest'].extend(entry[0]['rest'])
                         result = tmpres
 
             tmplt_str = tmplt_str[pos + 1:]
             if re.match(r'^\[\s+"', tmplt_str):
                 ppos = 0
                 continue
             try:
@@ -331,19 +216,19 @@
                             intres = [{rval: x.get(lval[1], ''),
                                        "rest": x.get(nxtfld, [])}
                                       for x in ele["rest"]]
                         else:
                             intres = [{rval: x.get(lval[1], ''), "rest": x}
                                       for x in ele["rest"]]
 
-                for oldkey, val in ele.items():
+                for oldkey in ele.keys():
                     if oldkey == "rest":
                         continue
                     for newele in intres:
-                        newele.update({oldkey: val})
+                        newele.update({oldkey: ele[oldkey]})
                 tmpres += intres
             result = tmpres
         else:
             if lval == ["*"]:
                 ks = list(data.keys())
 
             result = [{rval: x,
@@ -359,39 +244,40 @@
 
     # Now for the rest of the fields
     # if we only have 'rest' as the key, break out into individual mbrs
     if nokeys:
         if not result:
             result = [{"rest": data}]
         elif len(result) == 1:
-            if isinstance(result[0], list):
-                tmpval = []
-                for x in result[0]["rest"]:
-                    tmpval.append({"rest": x})
-                result = tmpval
+            tmpval = []
+            for x in result[0]["rest"]:
+                tmpval.append({"rest": x})
+            result = tmpval
 
     # In some cases such as FRR's BGP, you need to eliminate elements which
     # have no useful 'rest' field, for example the elements with vrfId and
     # vrfName. If at this point, you have nn element in result with rest
     # that is not a list or a dict, remove it
 
-    result = list(filter(lambda x: isinstance(x["rest"], (dict, list)),
+    result = list(filter(lambda x: isinstance(x["rest"], list) or
+                         isinstance(x["rest"], dict),
                          result))
 
     # At this point, we're expecting result to contain a list where each
     # entry contains the "rest' key with the fields from which further data
     # is to be extracted, and a series of keys which represent what has already
     # been extracted from the header string. If the format of result isn't
     # this, fix it
     if len(result) == 1 and isinstance(result[0]['rest'], list):
         tmpres = []
         entry = result[0]
         elekeys = entry.keys() - set(['rest'])
         for elem in entry['rest']:
-            newentry = {x: entry[x] for x in elekeys}
+            newentry = {}
+            [newentry.update({x: entry[x]}) for x in elekeys]
             newentry['rest'] = elem
             tmpres.append(newentry)
         result = tmpres
 
     # The if handles cases of flat JSON data such as evpnVni
     if tmplt_str.startswith('/['):
         tmplt_str = tmplt_str[2:-1]
@@ -402,23 +288,19 @@
         def_val = None
         # every element here MUST have the form lval:rval
         selem = selem.replace('"', '').strip()
         if not selem:
             # dealing with trailing "."
             continue
 
-        try:
-            lval, rval = selem.split(": ")
-        except ValueError:
-            logging.error(f"Unable to parse JSON field entry {selem}")
-            continue
+        lval, rval = selem.split(":")
 
         # Process default value processing of the form <key>?|<def_val> or
         # <key>?<expected_val>|<def_val>
-        op = None  # pylint: disable=redefined-outer-name
+        op = None
         if "?" in rval:
             rval, op = rval.split("?")
             exp_val, def_val = op.split("|")
 
             # Handle the case that the values are not strings
             if def_val.isdigit():
                 def_val = int(def_val)
@@ -445,50 +327,94 @@
         # Process for every element in result so far
         # Handles entries such as "vias/*/nexthopIps" and returns
         # a list of all nexthopIps.
         for x in result:
 
             loopdef_val = def_val
             if per_entry_defval and def_val is not None:
-                loopdef_val = x.get(def_val, '')
+                if def_val in x:
+                    loopdef_val = x[def_val]
+                else:
+                    loopdef_val = ''  # this shouldn't happen
 
             if "/" in lval:
                 subflds = lval.split("/")
                 tmpval = x["rest"]
                 value = None
-                if any(x in subflds for x in ["*", "*?", "[*]?", "[*]",
-                                              '*:_sqstore']):
+                if any(x in subflds for x in ["*", "*?", "[*]?", "[*]"]):
                     # Returning a list is the only supported option for now
                     value = []
                     maybe_list = True
                 else:
                     maybe_list = False
 
-                value = parse_subtree(
-                    subflds, tmpval, maybe_list, loopdef_val)
-                subflds = []
+                while subflds:
+                    subfld = subflds.pop(0).strip()
+                    if subfld == "*":
+                        tmp = tmpval
+                        for subele in tmp:
+                            for ele in subflds:
+                                if isinstance(tmp, list):
+                                    subele = subele.get(ele, None)
+                                else:
+                                    subele = tmp[subele].get(ele, None)
+                                if subele is None:
+                                    tmpval = None
+                                    break
+                            if subele:
+                                value.append(subele)
+                        subflds = []
+                    elif subfld.startswith('['):
+                        # handle specific array index or dict key
+                        # This additional handling of * is because of JUNOS
+                        # interface address which is many levels deep and mixes
+                        # IPv4/v6 address in a way that we can't entirely fix
+                        # Post processing cleanup has to handle that part
+                        if subfld.endswith('?'):
+                            # This was added thanks to NXOS which provides
+                            # nexthops as a list if ECMP, else a dictionary
+                            if type(tmpval) != list:
+                                continue
+                            subfld = subfld[:-1]  # lose the final "?" char
+                        if subfld == '[*]':
+                            tmp = tmpval
+                            for subele in tmp:
+                                for subfld in subflds:
+                                    if not subele:
+                                        break
+                                    if subfld == '*' or subfld == '[*]':
+                                        # We stop the recursive madness here
+                                        value.append(subele)
+                                        break
+                                    if subfld.startswith('['):
+                                        subele = subele[eval_expr(subfld)]
+                                    else:
+                                        subele = subele.get(subfld)
+                                value.append(subele)
+                            subflds = []
+                        elif tmpval:
+                            tmpval = tmpval[eval_expr(subfld)]
+                    else:
+                        tmpval = tmpval.get(subfld, None)
+                    if not tmpval:
+                        break
+
+                if value is None:
+                    value = tmpval
+                elif maybe_list and value == []:
+                    if tmpval:
+                        value = [tmpval]
             else:
-                if isinstance(x['rest'], dict):
-                    value = x["rest"].get(lval.strip(), None)
+                value = x["rest"].get(lval.strip(), None)
 
             if op:
                 if exp_val and value != exp_val:
                     value = loopdef_val
-                elif not exp_val:
-                    if (isinstance(value, list) and not
-                            any(x or (x == loopdef_val) for x in value)):
-                        if not isinstance(loopdef_val, list) and maybe_list:
-                            if loopdef_val == '':
-                                value = []
-                            else:
-                                value = [loopdef_val]
-                        else:
-                            value = loopdef_val
-                    elif not value:
-                        value = loopdef_val
+                elif not exp_val and not value:
+                    value = loopdef_val
 
             # Handle any operation on string
             rval = rval.strip()
             rval1 = re.split(r"([+/*-])", rval)
             if len(rval1) > 1:
                 iop = rval1[1]
                 if value is not None:
@@ -509,15 +435,14 @@
             else:
                 x.update({rval: value})
 
     return cleanup_and_return(result)
 
 
 def cleanup_and_return(result):
-    '''What it says: cleanup the result and return it'''
     for entry in result:
         # To handle entries like EOS' ospfNbr, we had saved the multiple keys
         # extracted from the initial part of the JSON string and saved it in
         # sq-addnl-keys. Now pop them out into the appropriate spot before
         # eliminating the 'rest' field which contains the unused fields
         rest = entry.pop('rest', {})
         if 'sq-addnl-keys' in rest:
@@ -529,15 +454,14 @@
 
 def eval_expr(expr):
     """Evaluate numerical expression without eval or other packages"""
     return num_eval(ast.parse(expr, mode='eval').body)
 
 
 def num_eval(node):
-    '''Numerical eval'''
     # supported arithmetic operators
     operators = {ast.Add: op.add, ast.Sub: op.sub, ast.Mult: op.mul,
                  ast.Div: op.truediv, ast.Pow: op.pow}
 
     if isinstance(node, ast.Num):  # <number>
         return node.n
     elif isinstance(node, ast.BinOp):  # <left> <operator> <right>
```

### Comparing `suzieq-0.22.0rc1/suzieq/poller/worker/services/topcpu.py` & `suzieq-0.8.0/suzieq/poller/services/topmem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from suzieq.poller.worker.services.service import Service
+from suzieq.poller.services.service import Service
 
 
-class TopCpuService(Service):
-    '''TopCpu service class'''
+class TopMemService(Service):
 
-    def _common_data_cleaner(self, processed_data, _):
+    def _common_data_cleaner(self, processed_data, raw_data):
 
         for entry in processed_data:
             for i in ["virtualMem", "residentMem", "cacheMem", "usedMem",
                       "totalMem", "freeMem"]:
                 try:
                     entry[i] = int(entry[i])
                 except ValueError:
                     if entry[i].endswith("g"):
                         val = float(entry[i].split("g")[0])*1000000
                         entry[i] = int(val)
-
         return processed_data
```

### Comparing `suzieq-0.22.0rc1/suzieq/poller/worker/services/topmem.py` & `suzieq-0.8.0/suzieq/poller/services/topcpu.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from suzieq.poller.worker.services.service import Service
+from suzieq.poller.services.service import Service
 
 
-class TopMemService(Service):
-    '''Top with focus on memory usage service'''
+class TopCpuService(Service):
 
-    def _common_data_cleaner(self, processed_data, _):
+    def _common_data_cleaner(self, processed_data, raw_data):
 
         for entry in processed_data:
             for i in ["virtualMem", "residentMem", "cacheMem", "usedMem",
                       "totalMem", "freeMem"]:
                 try:
                     entry[i] = int(entry[i])
                 except ValueError:
                     if entry[i].endswith("g"):
                         val = float(entry[i].split("g")[0])*1000000
                         entry[i] = int(val)
+
         return processed_data
```

### Comparing `suzieq-0.22.0rc1/suzieq/poller/worker/writers/parquet.py` & `suzieq-0.8.0/suzieq/poller/writer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,117 @@
-"""
-This module contains the logic of the writer for the 'parquet' mode
-"""
-import logging
 import os
-from typing import Dict
+import logging
+import json
 
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
-from suzieq.db.parquet.parquetdb import PARQUET_VERSION
-from suzieq.poller.worker.writers.output_worker import OutputWorker
-from suzieq.shared.exceptions import SqPollerConfError
 
-logger = logging.getLogger(__name__)
-
-
-class ParquetOutputWorker(OutputWorker):
-    """ParquetOutputWorker writes the data retrived by
-    the poller in a parquet output directory
-    """
+class OutputWorker(object):
 
     def __init__(self, **kwargs):
-        data_directory = kwargs.get('data_dir')
-
-        if not data_directory:
-            output_dir = '/tmp/suzieq/parquet-out/'
-            logger.warning(
-                'No output directory for parquet specified, using '
-                '/tmp/suzieq/parquet-out'
-            )
+        self.type = kwargs.get("type", None)
+        self.logger = logging.getLogger(__name__)
+        self.sigend = False
+
+        output_dir = kwargs.get("output_dir", None)
+        if output_dir:
+            self.root_output_dir = output_dir
+            if not os.path.isdir(output_dir):
+                os.makedirs(output_dir)
         else:
-            output_dir = data_directory
+            # TBD: The right error to raise here since this is a required
+            # keyword
+            self.logger.error("Need mandatory keyword arg: output_dir")
+            raise ValueError
+
+    def write_data(self, data):
+        raise NotImplementedError
 
-        if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
 
-        if not os.path.isdir(output_dir):
-            raise SqPollerConfError(
-                f'Output directory {output_dir} is not a directory'
-            )
-
-        logger.info(f'Parquet outputs will be under {output_dir}')
-        self.root_output_dir = output_dir
-
-    def write_data(self, data: Dict):
-        """Write the data into the Parquet output directory
-
-        Args:
-            data (Dict): dictionary containing the data to store.
-        """
-        cdir = os.path.join(self.root_output_dir, data['topic'])
+class ParquetOutputWorker(OutputWorker):
+
+    def write_data(self, data):
+        cdir = "{}/{}/".format(self.root_output_dir, data["topic"])
         if not os.path.isdir(cdir):
             os.makedirs(cdir)
 
         # dtypes = {x: data['schema'].field(x).type.__str__()
         #           if 'list' not in data['schema'].field(x).type.__str__()
         #           else data['schema'].field(x).type.to_pandas_dtype()
         #           for x in data['schema'].names}
 
-        df = pd.DataFrame.from_dict(data['records'])
+        df = pd.DataFrame.from_dict(data["records"])
         # df.to_parquet(
         #     path=cdir,
         #     partition_cols=data['partition_cols'],
         #     index=True,
         #     engine='pyarrow')
         # pq.write_metadata(
         #     self.schema,'{}/_metadata'.format(cdir),
         #     version='2.0',
         #     coerce_timestamps='us')
 
-        table = pa.Table.from_pandas(df, schema=data['schema'],
+        table = pa.Table.from_pandas(df, schema=data["schema"],
                                      preserve_index=False)
 
         pq.write_to_dataset(
             table,
             root_path=cdir,
             partition_cols=data['partition_cols'],
-            version=PARQUET_VERSION,
+            version="2.0",
             compression='ZSTD',
             row_group_size=100000,
         )
+
+
+class GatherOutputWorker(OutputWorker):
+    """This is used to write output for the run-once data gather mode"""
+
+    def write_data(self, data):
+        file = f"{self.root_output_dir}/{data['topic']}.output"
+        with open(file, 'a') as f:
+            # Even though we use JSON dump, the output is not valid JSON
+            f.write(data['records'])
+
+
+async def run_output_worker(queue, output_workers):
+
+    while True:
+        data = await queue.get()
+
+        if not output_workers:
+            return
+
+        if output_workers[0].sigend:
+            output_workers[0].logger.warning(
+                "Writer: Received terminate signal")
+            return
+
+        for worker in output_workers:
+            worker.write_data(data)
+
+
+def init_output_workers(output_types, output_args):
+    """Create the appropriate output worker objects and return them"""
+
+    workers = []
+    for otype in output_types:
+        if otype == "parquet":
+            worker = ParquetOutputWorker(output_dir=output_args["output_dir"])
+            if worker:
+                workers.append(worker)
+        elif otype == "gather":
+            try:
+                worker = GatherOutputWorker(
+                    output_dir=output_args["output_dir"])
+                if worker:
+                    workers.append(worker)
+            except Exception as e:
+                logger = logging.getLogger(__name__)
+                logger.error(
+                    f"Unable to create {otype} worker, exception {str(e)}")
+        else:
+            raise NotImplementedError("Unknown type: {}".format(otype))
+
+    return workers
```

### Comparing `suzieq-0.22.0rc1/suzieq/sqobjects/bgp.py` & `suzieq-0.8.0/suzieq/sqobjects/ospf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,65 @@
-from typing import List
 import pandas as pd
-from pandas.core.dtypes.dtypes import DatetimeTZDtype
+import numpy as np
 
 from suzieq.sqobjects.basicobj import SqObject
-from suzieq.shared.utils import humanize_timestamp
+from suzieq.utils import SchemaForTable, humanize_timestamp
 
 
-class BgpObj(SqObject):
-    '''The object providing access to the bgp table'''
-
+class OspfObj(SqObject):
     def __init__(self, **kwargs):
-        super().__init__(table='bgp', **kwargs)
-        self._valid_get_args = ['namespace', 'hostname', 'columns', 'state',
-                                'vrf', 'peer', 'asn', 'afiSafi', 'query_str']
+        super().__init__(table='ospf', **kwargs)
+        self._addnl_fields = ['passive', 'area', 'state']
+        self._addnl_nbr_fields = ['state']
+        self._valid_get_args = ['namespace', 'hostname', 'columns',
+                                'vrf', 'ifname', 'state', 'query_str']
+        self._valid_assert_args = ['namespace', 'vrf', 'status']
         self._valid_arg_vals = {
-            'state': ['Established', 'NotEstd', 'dynamic', ''],
-            'result': ['all', 'pass', 'fail'],
+            'state': ['full', 'other', 'passive', ''],
+            'status': ['all', 'pass', 'fail'],
         }
-        self._valid_assert_args = self._valid_get_args + ['result']
 
-    def humanize_fields(self, df: pd.DataFrame, _=None) -> pd.DataFrame:
+    def aver(self, **kwargs):
+        """Assert that the OSPF state is OK"""
+
+        if not self.ctxt.engine:
+            raise AttributeError('No analysis engine specified')
+
+        try:
+            self.validate_assert_input(**kwargs)
+        except Exception as error:
+            df = pd.DataFrame({'error': [f'{error}']})
+            return df
+
+        return self.engine_obj.aver(**kwargs)
+
+    def top(self, what='', n=5, reverse=False, **kwargs) -> pd.DataFrame:
+        """Get the list of top/bottom entries of "what" field"""
+
+        if "columns" in kwargs:
+            columns = kwargs["columns"]
+            del kwargs["columns"]
+        else:
+            columns = ["default"]
+
+        table_schema = SchemaForTable(self._table, self.all_schemas)
+        columns = table_schema.get_display_fields(columns)
+
+        if what == "numChanges" and what not in columns:
+            self._addnl_nbr_fields.append(what)
+
+        return self.engine_obj.top(what=what, n=n, reverse=reverse, **kwargs)
+
+    def humanize_fields(self, df: pd.DataFrame, subset=None) -> pd.DataFrame:
         '''Humanize the timestamp and boot time fields'''
         if df.empty:
             return df
 
-        if 'estdTime' in df.columns:
-            if not isinstance(df.estdTime.dtype, DatetimeTZDtype):
-                df['estdTime'] = humanize_timestamp(
-                    df.estdTime, self.cfg.get('analyzer', {})
-                    .get('timezone', None))
-
-        return super().humanize_fields(df)
-
-    def _get_empty_cols(self, columns: List[str], fun: str, **kwargs) \
-            -> List[str]:
-        if fun == 'assert' and columns in [['default'], ['*']]:
-            return ['namespace', 'hostname', 'vrf', 'peer',
-                    'asn', 'peerAsn', 'state', 'peerHostname',
-                    'result', 'assertReason', 'timestamp']
-        return super()._get_empty_cols(columns, fun, **kwargs)
+        if 'lastChangeTime' in df.columns:
+            df['lastChangeTime'] = humanize_timestamp(
+                df.lastChangeTime.fillna(0))
+
+            if 'adjState' in df.columns:
+                df['lastChangeTime'] = np.where(df.adjState == "passive", "-",
+                                                df.lastChangeTime)
+
+        return df
```

### Comparing `suzieq-0.22.0rc1/suzieq/sqobjects/device.py` & `suzieq-0.8.0/suzieq/sqobjects/interfaces.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import pandas as pd
-from pandas.core.dtypes.dtypes import DatetimeTZDtype
 
 from suzieq.sqobjects.basicobj import SqObject
-from suzieq.shared.utils import humanize_timestamp
+from suzieq.utils import humanize_timestamp
 
 
-class DeviceObj(SqObject):
-    '''The object providing access to the device table'''
-
+class IfObj(SqObject):
     def __init__(self, **kwargs):
-        super().__init__(table='device', **kwargs)
-        self._valid_get_args = ['namespace', 'hostname', 'columns', 'os',
-                                'vendor', 'model', 'status', 'version',
-                                'query_str', 'ignore_neverpoll']
+        super().__init__(table='interfaces', **kwargs)
+        self._valid_get_args = ['namespace', 'hostname', 'ifname', 'columns',
+                                'state', 'type', 'mtu', 'query_str']
+        self._valid_assert_args = ['namespace', 'hostname', 'ifname',
+                                   'what', 'matchval', 'status']
         self._valid_arg_vals = {
-            'status': ['alive', 'dead', 'neverpoll',
-                       '!alive', '!dead', '!neverpoll']
+            'state': ['up', 'down', ''],
+            'status': ['all', 'pass', 'fail'],
         }
-        self._unique_def_column = ['model']
 
-    def humanize_fields(self, df: pd.DataFrame, _=None) -> pd.DataFrame:
+    def aver(self, what='mtu-match', **kwargs) -> pd.DataFrame:
+        """Assert that interfaces are in good state"""
+        try:
+            self.validate_assert_input(**kwargs)
+        except Exception as error:
+            df = pd.DataFrame({'error': [f'{error}']})
+            return df
+
+        return self.engine_obj.aver(what=what, **kwargs)
+
+    def humanize_fields(self, df: pd.DataFrame, subset=None) -> pd.DataFrame:
         '''Humanize the timestamp and boot time fields'''
         if df.empty:
             return df
 
-        # Convert the bootup timestamp into a time delta
-        if 'bootupTimestamp' in df.columns:
-            if not isinstance(df.bootupTimestamp.dtype, DatetimeTZDtype):
-                df['bootupTimestamp'] = humanize_timestamp(
-                    df['bootupTimestamp']*1000,
-                    self.cfg.get('analyzer', {}).get('timezone', None))
+        if 'statusChangeTimestamp' in df.columns:
+            df['statusChangeTimestamp'] = humanize_timestamp(
+                df.statusChangeTimestamp)
 
-        return super().humanize_fields(df)
+        return df
```

### Comparing `suzieq-0.22.0rc1/suzieq/sqobjects/evpnVni.py` & `suzieq-0.8.0/suzieq/sqobjects/bgp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,38 @@
-from typing import List
 from suzieq.sqobjects.basicobj import SqObject
+import pandas as pd
+from suzieq.utils import humanize_timestamp
 
 
-class EvpnvniObj(SqObject):
-    '''The object providing access to the evpnVni table'''
-
+class BgpObj(SqObject):
     def __init__(self, **kwargs):
-        super().__init__(table='evpnVni', **kwargs)
-        self._valid_get_args = ['namespace', 'hostname', 'columns', 'vni',
-                                'priVtepIp', 'query_str']
-        self._valid_assert_args = self._valid_get_args + ['result']
+        super().__init__(table='bgp', **kwargs)
+        self._valid_get_args = ['namespace', 'hostname', 'columns', 'state',
+                                'vrf', 'peer', 'query_str']
         self._valid_arg_vals = {
-            'result': ['all', 'pass', 'fail'],
+            'state': ['Established', 'NotEstd', ''],
+            'status': ['all', 'pass', 'fail'],
         }
+        self._valid_assert_args = ['namespace', 'hostname', 'vrf', 'status']
+
+    def aver(self, **kwargs):
+        """Assert that the BGP state is OK"""
+
+        if not self.ctxt.engine:
+            raise AttributeError('No analysis engine specified')
+        try:
+            self.validate_assert_input(**kwargs)
+        except Exception as error:
+            df = pd.DataFrame({'error': [f'{error}']})
+            return df
+
+        return self.engine_obj.aver(**kwargs)
+
+    def humanize_fields(self, df: pd.DataFrame, subset=None) -> pd.DataFrame:
+        '''Humanize the timestamp and boot time fields'''
+        if df.empty:
+            return df
+
+        if 'estdTime' in df.columns:
+            df['estdTime'] = humanize_timestamp(df.estdTime)
 
-    def _get_empty_cols(self, columns: List[str], fun: str, **kwargs) \
-            -> List[str]:
-        if fun == 'assert':
-            if columns in [['default'], ['*']]:
-                # this is the copy of engine/pandas/self._assert_result_cols
-                return ['namespace', 'hostname', 'vni', 'type', 'vrf',
-                        'macaddr', 'timestamp', 'result', 'assertReason']
-        return super()._get_empty_cols(columns, fun, **kwargs)
+        return df
```

### Comparing `suzieq-0.22.0rc1/suzieq/sqobjects/macs.py` & `suzieq-0.8.0/suzieq/sqobjects/macs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 import re
-
 from suzieq.sqobjects.basicobj import SqObject
-from suzieq.shared.utils import convert_macaddr_format_to_colon
 
 
 class MacsObj(SqObject):
-    '''The object providing access to the MAC table'''
-
     def __init__(self, **kwargs):
         super().__init__(table='macs', **kwargs)
         self._valid_get_args = ['namespace', 'hostname', 'columns', 'macaddr',
-                                'remoteVtepIp', 'vlan', 'local', 'bd',
-                                'moveCount', 'query_str']
-        self._convert_args = {
-            'macaddr': convert_macaddr_format_to_colon
-        }
-        self._unique_def_column = ['macaddr']
+                                'remoteVtepIp', 'vlan', 'localOnly', 'bd',
+                                'query_str']
 
     def validate_get_input(self, **kwargs):
-        for key, val in kwargs.items():
+        for key in kwargs:
             if key == 'vlan':
-                for ele in val:
-                    if isinstance(ele, (int, float)):
-                        continue
+                for ele in kwargs[key]:
                     if (ele.startswith(('<', '>', '!')) and (
                             ele in ['<', '<=', '>', '>=', '!=', '!'])):
                         raise ValueError('operator must not be separated by '
                                          'space, as in "<20"')
                     words = re.split(r'<|<=|>|>=|!', ele)
                     try:
                         int(words[-1])
                     except Exception:
-                        raise ValueError(f'Invalid VLAN value: {val}')
-        return super().validate_get_input(**kwargs)
+                        raise ValueError(f'Invalid VLAN value: {kwargs[key]}')
+        super().validate_get_input(**kwargs)
```

### Comparing `suzieq-0.22.0rc1/suzieq/sqobjects/namespace.py` & `suzieq-0.8.0/suzieq/sqobjects/topology.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+import typing
+from collections import OrderedDict, defaultdict
+from itertools import repeat
+from dataclasses import dataclass
+
+import numpy as np
 import pandas as pd
+import networkx as nx
+import matplotlib.pyplot as plt
 
+from suzieq.sqobjects import interfaces, lldp, bgp, ospf, basicobj, address, evpnVni
 from suzieq.sqobjects.basicobj import SqObject
-from suzieq.shared.utils import humanize_timestamp
-
+from suzieq.exceptions import NoLLdpError, EmptyDataframeError, PathLoopError
 
-class NamespaceObj(SqObject):
-    '''The object providing access to the virtual table: namespace'''
 
+class TopologyObj(basicobj.SqObject):
     def __init__(self, **kwargs):
-        super().__init__(table='namespace', **kwargs)
-        self._valid_get_args = ['namespace', 'hostname', 'version', 'os',
-                                'model', 'vendor', 'columns', 'query_str']
-        self._unique_def_column = ['namespace']
-
-    def get(self, **kwargs) -> pd.DataFrame:
-        view = kwargs.get('view', self.view)
-        if view == 'all':
-            raise AttributeError("Cannot use 'view=all' with this table")
-        return super().get(**kwargs)
-
-    def humanize_fields(self, df: pd.DataFrame, _=None) -> pd.DataFrame:
-        '''Humanize the timestamp fields'''
-        if df.empty:
-            return df
-
-        if 'lastUpdate' in df.columns:
-            df['lastUpdate'] = humanize_timestamp(df.lastUpdate,
-                                                  self.cfg.get('analyzer', {})
-                                                  .get('timezone', None))
-
-        return super().humanize_fields(df)
+        super().__init__(table='topology', **kwargs)
+        self._sort_fields = ["namespace", "hostname", 'columns', ]
+        self._cat_fields = []
+        self._valid_get_args = ['namespace', 'hostname', 'columns',
+                                'polled_neighbor', 'query_str']
+
+    # overriding parent because we want to take more arguments than the standard
+    def summarize(self, namespace: typing.List[str] = [],
+                  hostname: typing.List[str] = [],
+                  polled_neighbor=None, query_str: str = '') -> pd.DataFrame:
+        if self.columns != ["default"]:
+            self.summarize_df = pd.DataFrame(
+                {'error': ['ERROR: You cannot specify columns with summarize']})
+            return self.summarize_df
+        return self.engine_obj.summarize(namespace=namespace, hostname=hostname,
+                                         query_str=query_str,
+                                         polled_neighbor=polled_neighbor)
```

### Comparing `suzieq-0.22.0rc1/suzieq/utilities/convert_legacy_dataset.py` & `suzieq-0.8.0/suzieq/utilities/convert_legacy_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 
 import sys
 import pyarrow.parquet as pq
 import pyarrow as pa
-from suzieq.shared.schema import Schema, SchemaForTable
+from suzieq.utils import Schema, SchemaForTable
 import logging
+import argparse
 import pandas as pd
 from pathlib import Path
 
 
 def convert_dir(input_dir: str, output_dir: str, svcschema: SchemaForTable):
     """Convert the data into a single file and write it out"""
```

### Comparing `suzieq-0.22.0rc1/suzieq/utilities/find_invalid_parquet.py` & `suzieq-0.8.0/suzieq/utilities/find_invalid_parquet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-""" searches the provided parquet-out directory to find any invalid files
+""" searches the provided parquet-out directory to find any invalid files 
     it just finds all the parquet files and tries to load them as valid files
     if there is an exception, then we know it's a bad file
 """
 
 # TODO
 #  figure out how to break the files into multiple processes, otherwise
 #  it gets stuck behind a single core
 
+from suzieq.utils import get_latest_files
 import argparse
 import os
 import pyarrow.parquet as pa
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     parser.add_argument('-p', '--parquet_dir', type=str, required=True,
                         help="parquet directory")
     userargs = parser.parse_args()
 
     # this doesn't work, it's broken and doesn't return all the files
-    # files = get_latest_files(f"{userargs.parquet_dir}/{table}", view='all')
+    #files = get_latest_files(f"{userargs.parquet_dir}/{table}", view='all')
 
     all_files = []
     broken_files = []
     for root, dirs, files in os.walk(f"{userargs.parquet_dir}"):
-        if ('_archived' not in root and '_broken' not in root and
-                '.sq-coalescer.pid' not in files):
-            all_files.extend(list(map(lambda x: f"{root}/{x}", files)))
+        all_files.extend(list(map(lambda x: f"{root}/{x}", files)))
     print(f"{len(all_files)} files")
 
+    
     for file in all_files:
         try:
             parquet_file = pa.ParquetFile(file)
-        except pa.lib.ArrowInvalid:
+        except pa.lib.ArrowInvalid as e:
             broken_files.append(file)
 
     print(f"Broken files: {broken_files}")
```

### Comparing `suzieq-0.22.0rc1/suzieq/utilities/gen_schema.py` & `suzieq-0.8.0/suzieq/gen_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,19 @@
 """
 Generate AVRO schema files from the service definition and textfsm files
 """
 
 import sys
 import os
 import re
+import yaml
 import json
 import ast
 from pathlib import Path
 
-import yaml
-
-# pylint: disable=redefined-outer-name
-
 
 def get_field_set(svc_def, textfsm_dir):
     """Return the dict of fields with types given a service definition file"""
 
     field_set = set()
     defn_list = svc_def.get('apply', [])
 
@@ -27,26 +24,25 @@
             plist = re.split('''/(?=(?:[^'"]|'[^']*'|"[^"]*")*$)''', nfn)
             for elem in plist:
                 try:
                     nfn_fld_list = ast.literal_eval(elem)
                     nfn_flds = [
                         re.match(r'\s*(?:add\(|div\(|mul\(|sub\()*(\w+)',
                                  fld.split(':')[1]).group(1)
-                        for fld in nfn_fld_list if isinstance(fld, str)
-                    ]
+                        for fld in nfn_fld_list if type(fld) is str
+                        ]
                     field_set.update(nfn_flds)
                 except (ValueError, SyntaxError):
                     words = elem.split(':')
                     if len(words) > 1:
                         field_set.add(re.match(r'\s*(\w+)',
                                                words[1]).group(1))
         else:
             nfn = defn_list[entry].get('textfsm', None)
             if nfn:
-                # pylint: disable=redefined-outer-name
                 with open(textfsm_dir + '/' + nfn, 'r') as f:
                     lines = f.readlines()
                 for line in lines:
                     if line.startswith('Value'):
                         g = re.match(r'Value\s+(\w+)\s*(\w*)', line).groups()
                         if g[-1]:
                             fldname = g[-1]
@@ -123,21 +119,19 @@
         oldflds = {v['name']: i
                    for i, v in enumerate(old_schema['fields'])}
         newflds = {v['name']: i
                    for i, v in enumerate(schema['fields'])}
 
         for fld in oldflds.keys():
             if fld in newflds:
-                schema['fields'][newflds[fld]]['type'] = \
-                    old_schema['fields'][oldflds[fld]]['type']
+                schema['fields'][newflds[fld]]['type'] = old_schema['fields'][oldflds[fld]]['type']
                 if (old_schema['fields'][oldflds[fld]].get('default', None)
                     and not schema['fields'][newflds[fld]].get('default',
                                                                None)):
-                    schema['fields'][newflds[fld]]['default'] = \
-                        old_schema['fields'][oldflds[fld]]['default']
+                    schema['fields'][newflds[fld]]['default'] = old_schema['fields'][oldflds[fld]]['default']
 
     with open(filename, 'w') as f:
         f.write(json.dumps(schema, indent=4))
 
     return
```

### Comparing `suzieq-0.22.0rc1/suzieq/utilities/migrate_data.py` & `suzieq-0.8.0/suzieq/utilities/migrate_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import sys
 import typing
 import pyarrow.parquet as pq
 import pyarrow as pa
 from pathlib import Path, PosixPath
-from suzieq.shared.schema import Schema, SchemaForTable
+from suzieq.utils import Schema, SchemaForTable
 import concurrent.futures
 import logging
 
 
 def convert_file(file: PosixPath, output_dir: str, schema: SchemaForTable,
                  defaults: typing.List,
                  arrow_schema: pa.lib.Schema,
```

