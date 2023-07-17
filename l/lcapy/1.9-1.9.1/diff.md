# Comparing `tmp/lcapy-1.9.tar.gz` & `tmp/lcapy-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcapy-1.9.tar", last modified: Tue Nov  8 19:32:15 2022, max compression
+gzip compressed data, was "lcapy-1.9.1.tar", last modified: Wed Nov  9 02:03:59 2022, max compression
```

## Comparing `lcapy-1.9.tar` & `lcapy-1.9.1.tar`

### file list

```diff
@@ -1,398 +1,398 @@
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.849318 lcapy-1.9/
--rw-rw-r--   0 mph       (1000) mph       (1000)    26530 2022-11-08 19:28:45.000000 lcapy-1.9/LICENCE
--rw-rw-r--   0 mph       (1000) mph       (1000)      114 2022-11-08 19:28:45.000000 lcapy-1.9/MANIFEST.in
--rw-rw-r--   0 mph       (1000) mph       (1000)     9369 2022-11-08 19:32:15.849318 lcapy-1.9/PKG-INFO
--rw-rw-r--   0 mph       (1000) mph       (1000)     6937 2022-11-08 19:28:45.000000 lcapy-1.9/README.md
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.809319 lcapy-1.9/doc/
--rw-rw-r--   0 mph       (1000) mph       (1000)      755 2022-11-08 19:28:45.000000 lcapy-1.9/doc/DFTs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1249 2022-11-08 19:28:45.000000 lcapy-1.9/doc/DFTs.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)      721 2022-11-08 19:28:45.000000 lcapy-1.9/doc/DTFTs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3303 2022-11-08 19:28:45.000000 lcapy-1.9/doc/DTFTs.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)      694 2022-11-08 19:28:45.000000 lcapy-1.9/doc/ODTFTs.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3639 2022-11-08 19:28:45.000000 lcapy-1.9/doc/ODTFTs.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)     1553 2022-11-08 19:28:45.000000 lcapy-1.9/doc/about.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    18477 2022-11-08 19:28:45.000000 lcapy-1.9/doc/advanced.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)      473 2022-11-08 19:28:45.000000 lcapy-1.9/doc/applications.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    35680 2022-11-08 19:28:45.000000 lcapy-1.9/doc/circuits.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)     7926 2022-11-08 19:28:45.000000 lcapy-1.9/doc/conf.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1261 2022-11-08 19:28:45.000000 lcapy-1.9/doc/config.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)      751 2022-11-08 19:28:45.000000 lcapy-1.9/doc/development.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    20084 2022-11-08 19:28:45.000000 lcapy-1.9/doc/discretetime.rst
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.805319 lcapy-1.9/doc/examples/
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.813319 lcapy-1.9/doc/examples/discretetime/
--rw-rw-r--   0 mph       (1000) mph       (1000)      168 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/discretetime/cdt1-plot1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      875 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/discretetime/discretize1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      238 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/discretetime/dt1-DTFT-plot1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      143 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/discretetime/dt1-plot1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      181 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/discretetime/dt1-pole-zero-plot1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      911 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/discretetime/pade-step-delay.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1095 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/discretetime/pade-step-delay2.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.813319 lcapy-1.9/doc/examples/functions/
--rw-rw-r--   0 mph       (1000) mph       (1000)      189 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/crect.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      201 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/ctrap.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      183 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/ctri.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      186 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/dtrect4.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      186 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/dtrect5.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      178 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/dtsign.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      172 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/heaviside.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      186 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/psinc4.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      186 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/psinc8.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      177 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/ramp.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      185 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/rampstep.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      178 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/rect.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      178 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/sign.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      180 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/sincn.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      180 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/sincu.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      188 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/trapa.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      176 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/tri.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      180 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/unitimpulse.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      172 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/functions/unitstep.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.813319 lcapy-1.9/doc/examples/netlists/
--rw-rw-r--   0 mph       (1000) mph       (1000)      370 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/circuit-VRC1-vc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      272 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/circuit-VRC2-vc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      443 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/circuit-VRLC1-vr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      442 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/circuit-VRLC2-vr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      393 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/circuit-VRLC2b-vr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      444 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/circuit-VRLC3-vr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      403 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/circuit-series-VRC1-vc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      157 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/circuitgraph1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      157 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/circuitgraph2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      157 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/circuitgraph4.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      359 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/tf1-bode-plot.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      182 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/netlists/tf1-pole-zero-plot.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.821318 lcapy-1.9/doc/examples/networks/
--rw-rw-r--   0 mph       (1000) mph       (1000)       73 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/RLC-parallel.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       71 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/RLC-series.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       82 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/RLC2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       64 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/VRseries.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       88 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/colors.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      212 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladder1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      126 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladder2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      126 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladder3.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      126 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladder4.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      124 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladderCRCR1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      151 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladderRC1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      139 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladderRC2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      163 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladderRC3.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      124 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladderRCRC1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      151 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladderRL1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      190 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladderRLC1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      180 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladderRLC2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      200 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/ladderRLC3.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       99 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/net1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      132 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/net2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      158 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/net3.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       76 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/par3.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       87 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/par4.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      368 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/parallel-IRLC1-voc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      368 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/parallel-RLC3-Z.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/parallelseriesLC1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/parallelseriesRC1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/parallelseriesRL1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       81 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/pickup-s.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       69 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/pickup.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       89 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/pickupv.py
--rw-rw-r--   0 mph       (1000) mph       (1000)       81 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/rseries.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      354 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/series-RC1-Z.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      354 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/series-RL1-Z.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      202 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/series-RLC3-Z.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      212 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/series-VRC1-Isc-f.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      201 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/series-VRC1-isc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      201 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/series-VRL1-isc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      225 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/series-VRLC1-isc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/seriesparallelLC1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/seriesparallelRC1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/seriesparallelRL1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      160 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/twoport-chain1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      134 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/twoport-chain2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      161 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/twoport-hybrid1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      169 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/twoport-inverse-hybrid1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      162 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/twoport-parallel1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      161 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/twoport-series1.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.821318 lcapy-1.9/doc/examples/networks/twoports/
--rw-rw-r--   0 mph       (1000) mph       (1000)      848 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/networks/twoports/matrices.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.821318 lcapy-1.9/doc/examples/plotting/
--rw-rw-r--   0 mph       (1000) mph       (1000)      177 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/bode1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      141 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/cos1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      148 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/cos2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      196 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/cos3.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      188 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/deltas.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      147 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/lollipop1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      166 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/lollipop2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      200 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/nichols1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      201 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/nyquist1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      143 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/phasor1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      274 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/sincos1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      279 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/plotting/sincos2.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.825318 lcapy-1.9/doc/examples/simulation/
--rw-rw-r--   0 mph       (1000) mph       (1000)      287 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/simulation/sim1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      318 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/simulation/sim1be.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      287 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/simulation/sim2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      318 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/simulation/sim2be.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      288 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/simulation/sim3.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.805319 lcapy-1.9/doc/examples/tutorials/
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.825318 lcapy-1.9/doc/examples/tutorials/RCnoise/
--rw-rw-r--   0 mph       (1000) mph       (1000)      421 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/RCnoise/RCparallel1noise.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      432 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/RCnoise/RCparallel1noiseplot1.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.825318 lcapy-1.9/doc/examples/tutorials/annotations/
--rw-rw-r--   0 mph       (1000) mph       (1000)      165 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/annotations/circuit1_component_currents1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      176 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/annotations/circuit1_component_currents2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      189 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/annotations/circuit1_component_currents3.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      165 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/annotations/circuit1_component_voltages1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      142 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/annotations/circuit1_node_voltages1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      179 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/annotations/circuit1_node_voltages2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      197 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/annotations/circuit1_node_voltages3.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.825318 lcapy-1.9/doc/examples/tutorials/basic/
--rw-rw-r--   0 mph       (1000) mph       (1000)      201 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/basic/VRC1plot.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      189 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/basic/VRC1stepplot.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      222 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/basic/VRC2HdBplot.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      207 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/basic/VRC2Hmagplot.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      211 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/basic/VRC2Hphaseplot.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      351 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/basic/VRC2plot.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      351 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/basic/VRC2plot2.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.825318 lcapy-1.9/doc/examples/tutorials/discretetime/
--rw-rw-r--   0 mph       (1000) mph       (1000)      268 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/discretetime/filter1-response.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.825318 lcapy-1.9/doc/examples/tutorials/ivp/
--rw-rw-r--   0 mph       (1000) mph       (1000)      131 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/ivp/circuit-RLC-ivp1-solve.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.825318 lcapy-1.9/doc/examples/tutorials/opampnoise/
--rw-rw-r--   0 mph       (1000) mph       (1000)     1184 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opampnoise/opamp-noninverting-amplifier-noise1.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.825318 lcapy-1.9/doc/examples/tutorials/opamps/
--rw-rw-r--   0 mph       (1000) mph       (1000)      313 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/inoise1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      139 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-noninverting-amplifier1-gain.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      112 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-noninverting-amplifier1-gain1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      139 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-noninverting-amplifier1-gain2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      324 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-open-loop1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      466 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-piezo-amplifier1-asd1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      466 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-piezo-amplifier1-asd2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      466 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-piezo-amplifier2-asd1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      897 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-piezo-amplifier2-asd2.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      862 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-piezo-amplifier2-frequency-response1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      114 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-transimpedance-amplifier1-gain1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      413 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-voltage-follower-C-load-closed-loop-pole-plot1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      515 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-voltage-follower-C-load-open-loop1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      429 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-voltage-follower-RC-load-closed-loop-pole-plot1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      531 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/opamp-voltage-follower-RC-load-open-loop1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      310 2022-11-08 19:28:45.000000 lcapy-1.9/doc/examples/tutorials/opamps/vnoise1.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    91508 2022-11-08 19:28:45.000000 lcapy-1.9/doc/expressions.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)      609 2022-11-08 19:28:45.000000 lcapy-1.9/doc/fourier_transforms.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1997 2022-11-08 19:28:45.000000 lcapy-1.9/doc/fourier_transforms.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)     4380 2022-11-08 19:28:45.000000 lcapy-1.9/doc/gallery.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    31014 2022-11-08 19:28:45.000000 lcapy-1.9/doc/gallery.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)     2055 2022-11-08 19:28:45.000000 lcapy-1.9/doc/index.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)     3395 2022-11-08 19:28:45.000000 lcapy-1.9/doc/install.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    10749 2022-11-08 19:28:45.000000 lcapy-1.9/doc/internals.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)      742 2022-11-08 19:28:45.000000 lcapy-1.9/doc/laplace_transforms.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1851 2022-11-08 19:28:45.000000 lcapy-1.9/doc/laplace_transforms.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)      641 2022-11-08 19:28:45.000000 lcapy-1.9/doc/latex.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)     5993 2022-11-08 19:28:45.000000 lcapy-1.9/doc/modules.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    38222 2022-11-08 19:28:45.000000 lcapy-1.9/doc/netlists.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    24733 2022-11-08 19:28:45.000000 lcapy-1.9/doc/networks.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)     4147 2022-11-08 19:28:45.000000 lcapy-1.9/doc/novice.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    44241 2022-11-08 19:28:45.000000 lcapy-1.9/doc/overview.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    10151 2022-11-08 19:28:45.000000 lcapy-1.9/doc/problems.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    25075 2022-11-08 19:28:45.000000 lcapy-1.9/doc/releases.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    50397 2022-11-08 19:28:45.000000 lcapy-1.9/doc/schematics.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    13768 2022-11-08 19:28:45.000000 lcapy-1.9/doc/systems.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)     1391 2022-11-08 19:28:45.000000 lcapy-1.9/doc/transforms.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)    82326 2022-11-08 19:28:45.000000 lcapy-1.9/doc/tutorials.rst
--rw-rw-r--   0 mph       (1000) mph       (1000)      496 2022-11-08 19:28:45.000000 lcapy-1.9/doc/ztransforms.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1233 2022-11-08 19:28:45.000000 lcapy-1.9/doc/ztransforms.rst
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.845318 lcapy-1.9/lcapy/
--rw-rw-r--   0 mph       (1000) mph       (1000)     3256 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/__init__.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1042 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/abc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     5488 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/acdc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      747 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/admittance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1578 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/admittancemixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      191 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/admittancesquaredmixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2325 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/analysis.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4593 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/approximate.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     6302 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/assumptions.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      150 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/attrdict.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      258 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/cache.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      262 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/capacitance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     5943 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/cexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3814 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/circuit.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    12680 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/circuitgraph.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1882 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/classmap.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      772 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/cnodes.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      973 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/componentnamer.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1380 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/components.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      683 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/conductance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3222 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/config.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      269 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/context.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1887 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/current.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      419 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/currentmixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      214 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/currentsquaredmixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1822 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/deprecation.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      319 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/dexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    53439 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/dft.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3170 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/differenceequation.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2631 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/differentialequation.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      634 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/discretetime.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     7417 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/dltifilter.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4157 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/domains.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    12526 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/dtft.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     8181 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/dtstatespace.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2418 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/engformatter.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1045 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/equipotentialnodes.py
--rw-rw-r--   0 mph       (1000) mph       (1000)   134173 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/expr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     5564 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/expressionclasses.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     7119 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/extrafunctions.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     7372 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/fexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    13942 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/fourier.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     7226 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/functions.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    10158 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/grammar.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2289 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/immittancemixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      741 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/impedance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1581 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/impedancemixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      189 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/impedancesquaredmixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      259 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/inductance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1881 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/inverse_dft.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4369 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/inverse_dtft.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1620 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/inverse_fourier.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    22139 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/inverse_laplace.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    18216 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/inverse_ztransform.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     5900 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/jfexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     6061 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/jomegaexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4860 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/kexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1901 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/kseq.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3802 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/laddermaker.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    11483 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/laplace.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3056 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/latex.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     7359 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/loopanalysis.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     5481 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/ltifilter.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     8558 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/matrix.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    10879 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/mna.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    59174 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/mnacpts.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     5021 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/netfile.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     8629 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/netlist.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1911 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/netlisthelper.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      707 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/netlistmaker.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    76039 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/netlistmixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4292 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/netlistnamespace.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    15161 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/netlistsimplifymixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2375 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/nettransform.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    10303 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/network.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     9115 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/nexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      483 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/nmatrix.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     6627 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/nodalanalysis.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3474 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/node.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     8000 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/noiseexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4818 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/noisefexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     5122 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/noiseomegaexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     7243 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/normfexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     7545 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/normomegaexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2268 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/nseq.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     6733 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/omegaexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    43979 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/oneport.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3047 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/opts.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    11628 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/parser.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    15970 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/phasor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    26864 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/plot.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     8575 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/polyphase.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3624 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/polytwoport.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      394 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/powermixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    13650 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/printing.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      958 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/printing_config.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      923 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/quantity.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4037 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/randomnetwork.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    27942 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/ratfun.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      819 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/reactance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      676 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/resistance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    23576 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/schematic.py
--rw-rw-r--   0 mph       (1000) mph       (1000)   112834 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/schemcpts.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    25434 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/schemgraph.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1429 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/schemgraphplacer.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     6703 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/schemlineqplacer.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2622 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/schemmisc.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4932 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/schemnode.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      543 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/schemplacer.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3363 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/schemplacerbase.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.845318 lcapy-1.9/lcapy/scripts/
--rw-rw-r--   0 mph       (1000) mph       (1000)       38 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/scripts/__init__.py
--rwxrwxr-x   0 mph       (1000) mph       (1000)    11861 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/scripts/schtex.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1592 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/seq.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3918 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/seqexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    15244 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/sequence.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    27126 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/sexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     9514 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/simplify.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    11689 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/simulator.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1075 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/smatrix.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4217 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/state.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     8379 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/statespace.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    16078 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/statespacebase.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     9884 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/statespacemaker.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1799 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/subnetlist.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    24131 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/super.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3626 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/superpositioncurrent.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3623 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/superpositionvoltage.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      834 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/susceptance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    13559 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/sym.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4031 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/symbolregistry.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1034 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/symbols.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     9031 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/synthesis.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     8393 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/system.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1564 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/systemequations.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.849318 lcapy-1.9/lcapy/tests/
--rw-rw-r--   0 mph       (1000) mph       (1000)     1105 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_approximate.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2114 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_circuitgraph.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    26025 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_circuits.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    28529 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_core.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1993 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_dft.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3980 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_discretetime.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      562 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_dltifilter.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1836 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_dtft.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2141 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_dtstatespace.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4416 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_fourier.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2458 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_functions.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2248 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_immitance.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      582 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_jomega.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     7347 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_laplace.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1205 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_latex.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1309 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_loop_analysis.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4598 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_networks.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      593 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_nodal_analysis.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4945 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_noise.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    11423 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_oneport.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     7087 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_ops.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2062 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_parser.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2650 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_phasor.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1593 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_plot.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      330 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_polyphase.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4099 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_schematic.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     2603 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_simplify.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      668 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_simulation.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4670 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_statespace.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     8619 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_super.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3004 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_synthesis.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     4234 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_transform.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    15157 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_twoport.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     7174 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_units.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    12282 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tests/test_ztransform.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    11181 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/texpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    10312 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/threeport.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      469 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/tmatrix.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      808 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/transfer.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      340 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/transfermixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     6634 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/transform.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     6364 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/transformer.py
--rw-rw-r--   0 mph       (1000) mph       (1000)   103446 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/twoport.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     3709 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/units.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     9087 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/utils.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      565 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/vector.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1887 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/voltage.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      419 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/voltagemixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)      214 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/voltagesquaredmixin.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    15058 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/zexpr.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1439 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/zmatrix.py
--rw-rw-r--   0 mph       (1000) mph       (1000)     1594 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/zseq.py
--rw-rw-r--   0 mph       (1000) mph       (1000)    14499 2022-11-08 19:28:45.000000 lcapy-1.9/lcapy/ztransform.py
-drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-08 19:32:15.845318 lcapy-1.9/lcapy.egg-info/
--rw-rw-r--   0 mph       (1000) mph       (1000)     9369 2022-11-08 19:32:15.000000 lcapy-1.9/lcapy.egg-info/PKG-INFO
--rw-rw-r--   0 mph       (1000) mph       (1000)    10811 2022-11-08 19:32:15.000000 lcapy-1.9/lcapy.egg-info/SOURCES.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)        1 2022-11-08 19:32:15.000000 lcapy-1.9/lcapy.egg-info/dependency_links.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)       54 2022-11-08 19:32:15.000000 lcapy-1.9/lcapy.egg-info/entry_points.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)      209 2022-11-08 19:32:15.000000 lcapy-1.9/lcapy.egg-info/requires.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)        6 2022-11-08 19:32:15.000000 lcapy-1.9/lcapy.egg-info/top_level.txt
--rw-rw-r--   0 mph       (1000) mph       (1000)      287 2022-11-08 19:32:15.849318 lcapy-1.9/setup.cfg
--rw-rw-r--   0 mph       (1000) mph       (1000)     1698 2022-11-08 19:28:45.000000 lcapy-1.9/setup.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.562755 lcapy-1.9.1/
+-rw-rw-r--   0 mph       (1000) mph       (1000)    26530 2022-11-09 02:02:50.000000 lcapy-1.9.1/LICENCE
+-rw-rw-r--   0 mph       (1000) mph       (1000)      114 2022-11-09 02:02:50.000000 lcapy-1.9.1/MANIFEST.in
+-rw-rw-r--   0 mph       (1000) mph       (1000)     9371 2022-11-09 02:03:59.562755 lcapy-1.9.1/PKG-INFO
+-rw-rw-r--   0 mph       (1000) mph       (1000)     6937 2022-11-09 02:02:50.000000 lcapy-1.9.1/README.md
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.522754 lcapy-1.9.1/doc/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      755 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/DFTs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1249 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/DFTs.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)      721 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/DTFTs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3303 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/DTFTs.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)      694 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/ODTFTs.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3639 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/ODTFTs.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1553 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/about.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    18477 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/advanced.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)      473 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/applications.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    35680 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/circuits.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)     7926 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/conf.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1261 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/config.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)      751 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/development.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    20084 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/discretetime.rst
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.514754 lcapy-1.9.1/doc/examples/
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.522754 lcapy-1.9.1/doc/examples/discretetime/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      168 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/discretetime/cdt1-plot1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      875 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/discretetime/discretize1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      238 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/discretetime/dt1-DTFT-plot1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      143 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/discretetime/dt1-plot1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      181 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/discretetime/dt1-pole-zero-plot1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      911 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/discretetime/pade-step-delay.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1095 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/discretetime/pade-step-delay2.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.522754 lcapy-1.9.1/doc/examples/functions/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      189 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/crect.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      201 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/ctrap.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      183 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/ctri.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      186 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/dtrect4.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      186 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/dtrect5.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      178 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/dtsign.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      172 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/heaviside.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      186 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/psinc4.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      186 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/psinc8.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      177 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/ramp.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      185 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/rampstep.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      178 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/rect.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      178 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/sign.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      180 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/sincn.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      180 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/sincu.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      188 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/trapa.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      176 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/tri.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      180 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/unitimpulse.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      172 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/functions/unitstep.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.526754 lcapy-1.9.1/doc/examples/netlists/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      370 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/circuit-VRC1-vc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      272 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/circuit-VRC2-vc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      443 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/circuit-VRLC1-vr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      442 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/circuit-VRLC2-vr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      393 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/circuit-VRLC2b-vr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      444 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/circuit-VRLC3-vr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      403 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/circuit-series-VRC1-vc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      157 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/circuitgraph1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      157 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/circuitgraph2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      157 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/circuitgraph4.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      359 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/tf1-bode-plot.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      182 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/netlists/tf1-pole-zero-plot.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.530754 lcapy-1.9.1/doc/examples/networks/
+-rw-rw-r--   0 mph       (1000) mph       (1000)       73 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/RLC-parallel.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       71 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/RLC-series.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       82 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/RLC2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       64 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/VRseries.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       88 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/colors.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      212 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladder1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      126 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladder2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      126 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladder3.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      126 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladder4.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      124 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladderCRCR1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      151 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladderRC1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      139 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladderRC2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      163 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladderRC3.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      124 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladderRCRC1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      151 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladderRL1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      190 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladderRLC1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      180 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladderRLC2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      200 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/ladderRLC3.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       99 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/net1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      132 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/net2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      158 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/net3.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       76 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/par3.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       87 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/par4.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      368 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/parallel-IRLC1-voc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      368 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/parallel-RLC3-Z.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/parallelseriesLC1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/parallelseriesRC1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/parallelseriesRL1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       81 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/pickup-s.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       69 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/pickup.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       89 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/pickupv.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)       81 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/rseries.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      354 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/series-RC1-Z.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      354 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/series-RL1-Z.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      202 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/series-RLC3-Z.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      212 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/series-VRC1-Isc-f.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      201 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/series-VRC1-isc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      201 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/series-VRL1-isc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      225 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/series-VRLC1-isc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/seriesparallelLC1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/seriesparallelRC1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      110 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/seriesparallelRL1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      160 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/twoport-chain1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      134 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/twoport-chain2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      161 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/twoport-hybrid1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      169 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/twoport-inverse-hybrid1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      162 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/twoport-parallel1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      161 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/twoport-series1.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.530754 lcapy-1.9.1/doc/examples/networks/twoports/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      848 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/networks/twoports/matrices.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.530754 lcapy-1.9.1/doc/examples/plotting/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      177 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/bode1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      141 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/cos1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      148 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/cos2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      196 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/cos3.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      188 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/deltas.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      147 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/lollipop1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      166 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/lollipop2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      200 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/nichols1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      201 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/nyquist1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      143 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/phasor1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      274 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/sincos1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      279 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/plotting/sincos2.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.534755 lcapy-1.9.1/doc/examples/simulation/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      287 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/simulation/sim1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      318 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/simulation/sim1be.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      287 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/simulation/sim2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      318 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/simulation/sim2be.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      288 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/simulation/sim3.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.514754 lcapy-1.9.1/doc/examples/tutorials/
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.534755 lcapy-1.9.1/doc/examples/tutorials/RCnoise/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      421 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/RCnoise/RCparallel1noise.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      432 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/RCnoise/RCparallel1noiseplot1.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.534755 lcapy-1.9.1/doc/examples/tutorials/annotations/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      165 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/annotations/circuit1_component_currents1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      176 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/annotations/circuit1_component_currents2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      189 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/annotations/circuit1_component_currents3.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      165 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/annotations/circuit1_component_voltages1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      142 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/annotations/circuit1_node_voltages1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      179 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/annotations/circuit1_node_voltages2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      197 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/annotations/circuit1_node_voltages3.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.534755 lcapy-1.9.1/doc/examples/tutorials/basic/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      201 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/basic/VRC1plot.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      189 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/basic/VRC1stepplot.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      222 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/basic/VRC2HdBplot.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      207 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/basic/VRC2Hmagplot.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      211 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/basic/VRC2Hphaseplot.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      351 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/basic/VRC2plot.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      351 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/basic/VRC2plot2.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.534755 lcapy-1.9.1/doc/examples/tutorials/discretetime/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      268 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/discretetime/filter1-response.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.534755 lcapy-1.9.1/doc/examples/tutorials/ivp/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      131 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/ivp/circuit-RLC-ivp1-solve.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.534755 lcapy-1.9.1/doc/examples/tutorials/opampnoise/
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1184 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opampnoise/opamp-noninverting-amplifier-noise1.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.538755 lcapy-1.9.1/doc/examples/tutorials/opamps/
+-rw-rw-r--   0 mph       (1000) mph       (1000)      313 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/inoise1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      139 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-noninverting-amplifier1-gain.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      112 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-noninverting-amplifier1-gain1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      139 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-noninverting-amplifier1-gain2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      324 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-open-loop1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      466 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-piezo-amplifier1-asd1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      466 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-piezo-amplifier1-asd2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      466 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-piezo-amplifier2-asd1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      897 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-piezo-amplifier2-asd2.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      862 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-piezo-amplifier2-frequency-response1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      114 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-transimpedance-amplifier1-gain1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      413 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-voltage-follower-C-load-closed-loop-pole-plot1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      515 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-voltage-follower-C-load-open-loop1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      429 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-voltage-follower-RC-load-closed-loop-pole-plot1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      531 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-voltage-follower-RC-load-open-loop1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      310 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/examples/tutorials/opamps/vnoise1.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    91508 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/expressions.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)      609 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/fourier_transforms.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1997 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/fourier_transforms.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4380 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/gallery.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    31014 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/gallery.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2055 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/index.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3395 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/install.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    10749 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/internals.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)      742 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/laplace_transforms.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1851 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/laplace_transforms.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)      641 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/latex.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)     5993 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/modules.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    38222 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/netlists.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    24733 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/networks.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4147 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/novice.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    44899 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/overview.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    10151 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/problems.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    25075 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/releases.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    50397 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/schematics.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    13768 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/systems.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1391 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/transforms.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)    82326 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/tutorials.rst
+-rw-rw-r--   0 mph       (1000) mph       (1000)      496 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/ztransforms.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1233 2022-11-09 02:02:50.000000 lcapy-1.9.1/doc/ztransforms.rst
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.558755 lcapy-1.9.1/lcapy/
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3256 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/__init__.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1042 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/abc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     5488 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/acdc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      747 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/admittance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1578 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/admittancemixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      191 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/admittancesquaredmixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2325 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/analysis.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4593 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/approximate.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     6302 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/assumptions.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      150 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/attrdict.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      258 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/cache.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      262 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/capacitance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     5943 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/cexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3814 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/circuit.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    12680 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/circuitgraph.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1882 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/classmap.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      772 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/cnodes.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      973 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/componentnamer.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1380 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/components.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      683 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/conductance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3222 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/config.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      269 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/context.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1887 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/current.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      419 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/currentmixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      214 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/currentsquaredmixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1822 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/deprecation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      319 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/dexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    53439 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/dft.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3170 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/differenceequation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2631 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/differentialequation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      634 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/discretetime.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     7417 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/dltifilter.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4157 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/domains.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    12526 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/dtft.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     8181 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/dtstatespace.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2418 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/engformatter.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1045 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/equipotentialnodes.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)   134173 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/expr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     5564 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/expressionclasses.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     7119 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/extrafunctions.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     7372 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/fexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    13942 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/fourier.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     7226 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/functions.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    10158 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/grammar.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2289 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/immittancemixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      741 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/impedance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1581 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/impedancemixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      189 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/impedancesquaredmixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      259 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/inductance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1881 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/inverse_dft.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4369 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/inverse_dtft.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1620 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/inverse_fourier.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    22139 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/inverse_laplace.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    18216 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/inverse_ztransform.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     5900 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/jfexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     6061 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/jomegaexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4860 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/kexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1901 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/kseq.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3802 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/laddermaker.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    11483 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/laplace.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3056 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/latex.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     7359 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/loopanalysis.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     5481 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/ltifilter.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     8558 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/matrix.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    10879 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/mna.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    59174 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/mnacpts.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     5021 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/netfile.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     8629 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/netlist.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1911 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/netlisthelper.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      707 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/netlistmaker.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    76039 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/netlistmixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4292 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/netlistnamespace.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    15161 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/netlistsimplifymixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2375 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/nettransform.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    10303 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/network.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     9115 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/nexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      483 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/nmatrix.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     6627 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/nodalanalysis.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3474 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/node.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     8000 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/noiseexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4818 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/noisefexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     5122 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/noiseomegaexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     7243 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/normfexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     7545 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/normomegaexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2268 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/nseq.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     6733 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/omegaexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    43979 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/oneport.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3047 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/opts.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    11628 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/parser.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    15970 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/phasor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    26864 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/plot.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     8575 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/polyphase.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3624 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/polytwoport.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      394 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/powermixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    13650 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/printing.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      958 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/printing_config.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      923 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/quantity.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4037 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/randomnetwork.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    27942 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/ratfun.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      819 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/reactance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      676 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/resistance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    23576 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/schematic.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)   112834 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/schemcpts.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    25434 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/schemgraph.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1429 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/schemgraphplacer.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     6703 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/schemlineqplacer.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2622 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/schemmisc.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4932 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/schemnode.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      543 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/schemplacer.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3363 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/schemplacerbase.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.558755 lcapy-1.9.1/lcapy/scripts/
+-rw-rw-r--   0 mph       (1000) mph       (1000)       38 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/scripts/__init__.py
+-rwxrwxr-x   0 mph       (1000) mph       (1000)    11861 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/scripts/schtex.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1592 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/seq.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3918 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/seqexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    15244 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/sequence.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    27126 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/sexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     9514 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/simplify.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    11689 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/simulator.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1075 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/smatrix.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4217 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/state.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     8379 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/statespace.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    16078 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/statespacebase.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     9884 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/statespacemaker.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1799 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/subnetlist.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    24131 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/super.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3626 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/superpositioncurrent.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3623 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/superpositionvoltage.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      834 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/susceptance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    13559 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/sym.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4031 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/symbolregistry.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1034 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/symbols.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     9031 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/synthesis.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     8393 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/system.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1564 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/systemequations.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.562755 lcapy-1.9.1/lcapy/tests/
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1105 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_approximate.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2114 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_circuitgraph.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    26025 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_circuits.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    28529 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_core.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1993 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_dft.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3980 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_discretetime.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      562 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_dltifilter.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1836 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_dtft.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2141 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_dtstatespace.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4416 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_fourier.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2458 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_functions.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2248 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_immitance.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      582 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_jomega.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     7347 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_laplace.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1205 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_latex.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1309 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_loop_analysis.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4598 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_networks.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      593 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_nodal_analysis.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4945 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_noise.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    11423 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_oneport.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     7087 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_ops.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2062 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_parser.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2650 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_phasor.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1593 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_plot.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      330 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_polyphase.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4099 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_schematic.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     2603 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_simplify.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      668 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_simulation.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4670 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_statespace.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     8619 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_super.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3004 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_synthesis.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     4234 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_transform.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    15157 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_twoport.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     7174 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_units.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    12282 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tests/test_ztransform.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    11181 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/texpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    10312 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/threeport.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      469 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/tmatrix.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      808 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/transfer.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      340 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/transfermixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     6634 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/transform.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     6364 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/transformer.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)   103446 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/twoport.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     3709 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/units.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     9087 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/utils.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      565 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/vector.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1887 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/voltage.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      419 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/voltagemixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)      214 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/voltagesquaredmixin.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    15058 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/zexpr.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1439 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/zmatrix.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1594 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/zseq.py
+-rw-rw-r--   0 mph       (1000) mph       (1000)    14499 2022-11-09 02:02:50.000000 lcapy-1.9.1/lcapy/ztransform.py
+drwxrwxr-x   0 mph       (1000) mph       (1000)        0 2022-11-09 02:03:59.558755 lcapy-1.9.1/lcapy.egg-info/
+-rw-rw-r--   0 mph       (1000) mph       (1000)     9371 2022-11-09 02:03:59.000000 lcapy-1.9.1/lcapy.egg-info/PKG-INFO
+-rw-rw-r--   0 mph       (1000) mph       (1000)    10811 2022-11-09 02:03:59.000000 lcapy-1.9.1/lcapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)        1 2022-11-09 02:03:59.000000 lcapy-1.9.1/lcapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)       54 2022-11-09 02:03:59.000000 lcapy-1.9.1/lcapy.egg-info/entry_points.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)      209 2022-11-09 02:03:59.000000 lcapy-1.9.1/lcapy.egg-info/requires.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)        6 2022-11-09 02:03:59.000000 lcapy-1.9.1/lcapy.egg-info/top_level.txt
+-rw-rw-r--   0 mph       (1000) mph       (1000)      287 2022-11-09 02:03:59.566755 lcapy-1.9.1/setup.cfg
+-rw-rw-r--   0 mph       (1000) mph       (1000)     1700 2022-11-09 02:02:50.000000 lcapy-1.9.1/setup.py
```

### Comparing `lcapy-1.9/LICENCE` & `lcapy-1.9.1/LICENCE`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/PKG-INFO` & `lcapy-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcapy
-Version: 1.9
+Version: 1.9.1
 Summary: Symbolic linear circuit analysis
 Home-page: https://github.com/mph-/lcapy
 Author: Michael Hayes
 Author-email: michael.hayes@canterbury.ac.nz
 License: UNKNOWN
 Download-URL: https://github.com/mph-/lcapy
 Description: Lcapy is a Python package for linear circuit analysis.  It uses SymPy
```

### Comparing `lcapy-1.9/README.md` & `lcapy-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/DFTs.py` & `lcapy-1.9.1/doc/DFTs.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/DFTs.rst` & `lcapy-1.9.1/doc/DFTs.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/DTFTs.py` & `lcapy-1.9.1/doc/DTFTs.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/DTFTs.rst` & `lcapy-1.9.1/doc/DTFTs.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/ODTFTs.py` & `lcapy-1.9.1/doc/ODTFTs.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/ODTFTs.rst` & `lcapy-1.9.1/doc/ODTFTs.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/about.rst` & `lcapy-1.9.1/doc/about.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/advanced.rst` & `lcapy-1.9.1/doc/advanced.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/circuits.rst` & `lcapy-1.9.1/doc/circuits.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/conf.py` & `lcapy-1.9.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/config.rst` & `lcapy-1.9.1/doc/config.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/development.rst` & `lcapy-1.9.1/doc/development.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/discretetime.rst` & `lcapy-1.9.1/doc/discretetime.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/examples/discretetime/discretize1.py` & `lcapy-1.9.1/doc/examples/discretetime/discretize1.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/examples/discretetime/pade-step-delay.py` & `lcapy-1.9.1/doc/examples/discretetime/pade-step-delay.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/examples/discretetime/pade-step-delay2.py` & `lcapy-1.9.1/doc/examples/discretetime/pade-step-delay2.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/examples/networks/twoports/matrices.py` & `lcapy-1.9.1/doc/examples/networks/twoports/matrices.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/examples/tutorials/opampnoise/opamp-noninverting-amplifier-noise1.py` & `lcapy-1.9.1/doc/examples/tutorials/opampnoise/opamp-noninverting-amplifier-noise1.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/examples/tutorials/opamps/opamp-piezo-amplifier2-asd2.py` & `lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-piezo-amplifier2-asd2.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/examples/tutorials/opamps/opamp-piezo-amplifier2-frequency-response1.py` & `lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-piezo-amplifier2-frequency-response1.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/examples/tutorials/opamps/opamp-voltage-follower-C-load-open-loop1.py` & `lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-voltage-follower-C-load-open-loop1.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/examples/tutorials/opamps/opamp-voltage-follower-RC-load-open-loop1.py` & `lcapy-1.9.1/doc/examples/tutorials/opamps/opamp-voltage-follower-RC-load-open-loop1.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/expressions.rst` & `lcapy-1.9.1/doc/expressions.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/fourier_transforms.py` & `lcapy-1.9.1/doc/fourier_transforms.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/fourier_transforms.rst` & `lcapy-1.9.1/doc/fourier_transforms.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/gallery.py` & `lcapy-1.9.1/doc/gallery.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/gallery.rst` & `lcapy-1.9.1/doc/gallery.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/index.rst` & `lcapy-1.9.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/install.rst` & `lcapy-1.9.1/doc/install.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/internals.rst` & `lcapy-1.9.1/doc/internals.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/laplace_transforms.py` & `lcapy-1.9.1/doc/laplace_transforms.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/laplace_transforms.rst` & `lcapy-1.9.1/doc/laplace_transforms.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/latex.rst` & `lcapy-1.9.1/doc/latex.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/modules.rst` & `lcapy-1.9.1/doc/modules.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/netlists.rst` & `lcapy-1.9.1/doc/netlists.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/networks.rst` & `lcapy-1.9.1/doc/networks.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/novice.rst` & `lcapy-1.9.1/doc/novice.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/overview.rst` & `lcapy-1.9.1/doc/overview.rst`

 * *Files 1% similar despite different names*

```diff
@@ -28,36 +28,45 @@
 Lcapy cannot directly analyse non-linear devices such as diodes or
 transistors although it does support simple opamps without saturation.
 Nevertheless, it can draw them!  Lcapy can generate text-book quality schematics using vector graphics (unlike the bit-mapped graphics used in this document).
 
 Lcapy uses SymPy (symbolic Python) for its values and expressions
 and thus the circuit analysis can be performed symbolically.  See http://docs.sympy.org/latest/tutorial/index.html for the SymPy tutorial.
 
-Lcapy can perform many other linear circuit analysis operations, including:
+Lcapy can perform many linear circuit analysis operations, including:
 
-1. Two-port parameters (A, B, G, H, S, T, Y, and Z)
+1. Solve linear circuits and networks symbolically (including time-variant circuits with switches)
 
-2. Norton/Thevenin transforms
+2. Generate high-quality semi-automated schematics from netlists
 
-3. Wye-delta transforms
+3. Generate systems of equations for nodal, modified nodal, and mesh analysis
 
-4. Polyphase transforms
+4. Perform state-space analysis
 
-5. Laplace transforms
+5. Perform Laplace, Fourier, Z, discrete-time Fourier, and discrete Fourier transforms
 
-6. Fourier transforms
+6. Track units of expressions for dimensional analysis
 
-7. Discrete-time Fourier transforms
+7. Analyse two-port networks (A, B, G, H, S, T, Y, and Z)
 
-8. Discrete Fourier transforms
+8. Perform Norton/Thevenin and wye/delta transforms
 
-9. z-transforms
+9. Analyse poly-phase systems
 
-10. Time-stepping simulation (see :ref:`simulation`)
+10. Perform time-stepping simulation for numerical circuit analysis (see :ref:`simulation`)
 
+11. Generate many forms of plot (Bode, Nichols, Nyquist, pole-zero, etc.) with automatic axis labelling
+
+12. Perform network synthesis given an immitance expression
+
+13. Approximate continuous-time systems as discrete-time
+
+14. Convert expressions into many forms (ZPK, partial fraction, etc.)
+
+15. Parameterize an expression
 
 If you need to model a non-linear circuit numerically using Python, see PySpice (https://pypi.org/project/PySpice/).
 
 
 
 Preliminaries
 =============
```

### Comparing `lcapy-1.9/doc/problems.rst` & `lcapy-1.9.1/doc/problems.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/releases.rst` & `lcapy-1.9.1/doc/releases.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/schematics.rst` & `lcapy-1.9.1/doc/schematics.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/systems.rst` & `lcapy-1.9.1/doc/systems.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/transforms.rst` & `lcapy-1.9.1/doc/transforms.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/tutorials.rst` & `lcapy-1.9.1/doc/tutorials.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/doc/ztransforms.rst` & `lcapy-1.9.1/doc/ztransforms.rst`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/__init__.py` & `lcapy-1.9.1/lcapy/__init__.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/abc.py` & `lcapy-1.9.1/lcapy/abc.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/acdc.py` & `lcapy-1.9.1/lcapy/acdc.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/admittance.py` & `lcapy-1.9.1/lcapy/admittance.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/admittancemixin.py` & `lcapy-1.9.1/lcapy/admittancemixin.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/analysis.py` & `lcapy-1.9.1/lcapy/analysis.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/approximate.py` & `lcapy-1.9.1/lcapy/approximate.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/assumptions.py` & `lcapy-1.9.1/lcapy/assumptions.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/cexpr.py` & `lcapy-1.9.1/lcapy/cexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/circuit.py` & `lcapy-1.9.1/lcapy/circuit.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/circuitgraph.py` & `lcapy-1.9.1/lcapy/circuitgraph.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/classmap.py` & `lcapy-1.9.1/lcapy/classmap.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/cnodes.py` & `lcapy-1.9.1/lcapy/cnodes.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/componentnamer.py` & `lcapy-1.9.1/lcapy/componentnamer.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/components.py` & `lcapy-1.9.1/lcapy/components.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/conductance.py` & `lcapy-1.9.1/lcapy/conductance.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/config.py` & `lcapy-1.9.1/lcapy/config.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/current.py` & `lcapy-1.9.1/lcapy/current.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/deprecation.py` & `lcapy-1.9.1/lcapy/deprecation.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/dft.py` & `lcapy-1.9.1/lcapy/dft.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/differenceequation.py` & `lcapy-1.9.1/lcapy/differenceequation.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/differentialequation.py` & `lcapy-1.9.1/lcapy/differentialequation.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/discretetime.py` & `lcapy-1.9.1/lcapy/discretetime.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/dltifilter.py` & `lcapy-1.9.1/lcapy/dltifilter.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/domains.py` & `lcapy-1.9.1/lcapy/domains.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/dtft.py` & `lcapy-1.9.1/lcapy/dtft.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/dtstatespace.py` & `lcapy-1.9.1/lcapy/dtstatespace.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/engformatter.py` & `lcapy-1.9.1/lcapy/engformatter.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/equipotentialnodes.py` & `lcapy-1.9.1/lcapy/equipotentialnodes.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/expr.py` & `lcapy-1.9.1/lcapy/expr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/expressionclasses.py` & `lcapy-1.9.1/lcapy/expressionclasses.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/extrafunctions.py` & `lcapy-1.9.1/lcapy/extrafunctions.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/fexpr.py` & `lcapy-1.9.1/lcapy/fexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/fourier.py` & `lcapy-1.9.1/lcapy/fourier.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/functions.py` & `lcapy-1.9.1/lcapy/functions.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/grammar.py` & `lcapy-1.9.1/lcapy/grammar.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/immittancemixin.py` & `lcapy-1.9.1/lcapy/immittancemixin.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/impedance.py` & `lcapy-1.9.1/lcapy/impedance.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/impedancemixin.py` & `lcapy-1.9.1/lcapy/impedancemixin.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/inverse_dft.py` & `lcapy-1.9.1/lcapy/inverse_dft.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/inverse_dtft.py` & `lcapy-1.9.1/lcapy/inverse_dtft.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/inverse_fourier.py` & `lcapy-1.9.1/lcapy/inverse_fourier.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/inverse_laplace.py` & `lcapy-1.9.1/lcapy/inverse_laplace.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/inverse_ztransform.py` & `lcapy-1.9.1/lcapy/inverse_ztransform.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/jfexpr.py` & `lcapy-1.9.1/lcapy/jfexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/jomegaexpr.py` & `lcapy-1.9.1/lcapy/jomegaexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/kexpr.py` & `lcapy-1.9.1/lcapy/kexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/kseq.py` & `lcapy-1.9.1/lcapy/kseq.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/laddermaker.py` & `lcapy-1.9.1/lcapy/laddermaker.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/laplace.py` & `lcapy-1.9.1/lcapy/laplace.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/latex.py` & `lcapy-1.9.1/lcapy/latex.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/loopanalysis.py` & `lcapy-1.9.1/lcapy/loopanalysis.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/ltifilter.py` & `lcapy-1.9.1/lcapy/ltifilter.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/matrix.py` & `lcapy-1.9.1/lcapy/matrix.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/mna.py` & `lcapy-1.9.1/lcapy/mna.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/mnacpts.py` & `lcapy-1.9.1/lcapy/mnacpts.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/netfile.py` & `lcapy-1.9.1/lcapy/netfile.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/netlist.py` & `lcapy-1.9.1/lcapy/netlist.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/netlisthelper.py` & `lcapy-1.9.1/lcapy/netlisthelper.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/netlistmaker.py` & `lcapy-1.9.1/lcapy/netlistmaker.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/netlistmixin.py` & `lcapy-1.9.1/lcapy/netlistmixin.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/netlistnamespace.py` & `lcapy-1.9.1/lcapy/netlistnamespace.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/netlistsimplifymixin.py` & `lcapy-1.9.1/lcapy/netlistsimplifymixin.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/nettransform.py` & `lcapy-1.9.1/lcapy/nettransform.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/network.py` & `lcapy-1.9.1/lcapy/network.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/nexpr.py` & `lcapy-1.9.1/lcapy/nexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/nodalanalysis.py` & `lcapy-1.9.1/lcapy/nodalanalysis.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/node.py` & `lcapy-1.9.1/lcapy/node.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/noiseexpr.py` & `lcapy-1.9.1/lcapy/noiseexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/noisefexpr.py` & `lcapy-1.9.1/lcapy/noisefexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/noiseomegaexpr.py` & `lcapy-1.9.1/lcapy/noiseomegaexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/normfexpr.py` & `lcapy-1.9.1/lcapy/normfexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/normomegaexpr.py` & `lcapy-1.9.1/lcapy/normomegaexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/nseq.py` & `lcapy-1.9.1/lcapy/nseq.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/omegaexpr.py` & `lcapy-1.9.1/lcapy/omegaexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/oneport.py` & `lcapy-1.9.1/lcapy/oneport.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/opts.py` & `lcapy-1.9.1/lcapy/opts.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/parser.py` & `lcapy-1.9.1/lcapy/parser.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/phasor.py` & `lcapy-1.9.1/lcapy/phasor.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/plot.py` & `lcapy-1.9.1/lcapy/plot.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/polyphase.py` & `lcapy-1.9.1/lcapy/polyphase.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/polytwoport.py` & `lcapy-1.9.1/lcapy/polytwoport.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/printing.py` & `lcapy-1.9.1/lcapy/printing.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/printing_config.py` & `lcapy-1.9.1/lcapy/printing_config.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/quantity.py` & `lcapy-1.9.1/lcapy/quantity.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/randomnetwork.py` & `lcapy-1.9.1/lcapy/randomnetwork.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/ratfun.py` & `lcapy-1.9.1/lcapy/ratfun.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/reactance.py` & `lcapy-1.9.1/lcapy/reactance.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/resistance.py` & `lcapy-1.9.1/lcapy/resistance.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/schematic.py` & `lcapy-1.9.1/lcapy/schematic.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/schemcpts.py` & `lcapy-1.9.1/lcapy/schemcpts.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/schemgraph.py` & `lcapy-1.9.1/lcapy/schemgraph.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/schemgraphplacer.py` & `lcapy-1.9.1/lcapy/schemgraphplacer.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/schemlineqplacer.py` & `lcapy-1.9.1/lcapy/schemlineqplacer.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/schemmisc.py` & `lcapy-1.9.1/lcapy/schemmisc.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/schemnode.py` & `lcapy-1.9.1/lcapy/schemnode.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/schemplacer.py` & `lcapy-1.9.1/lcapy/schemplacer.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/schemplacerbase.py` & `lcapy-1.9.1/lcapy/schemplacerbase.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/scripts/schtex.py` & `lcapy-1.9.1/lcapy/scripts/schtex.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/seq.py` & `lcapy-1.9.1/lcapy/seq.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/seqexpr.py` & `lcapy-1.9.1/lcapy/seqexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/sequence.py` & `lcapy-1.9.1/lcapy/sequence.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/sexpr.py` & `lcapy-1.9.1/lcapy/sexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/simplify.py` & `lcapy-1.9.1/lcapy/simplify.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/simulator.py` & `lcapy-1.9.1/lcapy/simulator.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/smatrix.py` & `lcapy-1.9.1/lcapy/smatrix.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/state.py` & `lcapy-1.9.1/lcapy/state.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/statespace.py` & `lcapy-1.9.1/lcapy/statespace.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/statespacebase.py` & `lcapy-1.9.1/lcapy/statespacebase.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/statespacemaker.py` & `lcapy-1.9.1/lcapy/statespacemaker.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/subnetlist.py` & `lcapy-1.9.1/lcapy/subnetlist.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/super.py` & `lcapy-1.9.1/lcapy/super.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/superpositioncurrent.py` & `lcapy-1.9.1/lcapy/superpositioncurrent.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/superpositionvoltage.py` & `lcapy-1.9.1/lcapy/superpositionvoltage.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/susceptance.py` & `lcapy-1.9.1/lcapy/susceptance.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/sym.py` & `lcapy-1.9.1/lcapy/sym.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/symbolregistry.py` & `lcapy-1.9.1/lcapy/symbolregistry.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/symbols.py` & `lcapy-1.9.1/lcapy/symbols.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/synthesis.py` & `lcapy-1.9.1/lcapy/synthesis.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/system.py` & `lcapy-1.9.1/lcapy/system.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/systemequations.py` & `lcapy-1.9.1/lcapy/systemequations.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_approximate.py` & `lcapy-1.9.1/lcapy/tests/test_approximate.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_circuitgraph.py` & `lcapy-1.9.1/lcapy/tests/test_circuitgraph.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_circuits.py` & `lcapy-1.9.1/lcapy/tests/test_circuits.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_core.py` & `lcapy-1.9.1/lcapy/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_dft.py` & `lcapy-1.9.1/lcapy/tests/test_dft.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_discretetime.py` & `lcapy-1.9.1/lcapy/tests/test_discretetime.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_dltifilter.py` & `lcapy-1.9.1/lcapy/tests/test_dltifilter.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_dtft.py` & `lcapy-1.9.1/lcapy/tests/test_dtft.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_dtstatespace.py` & `lcapy-1.9.1/lcapy/tests/test_dtstatespace.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_fourier.py` & `lcapy-1.9.1/lcapy/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_functions.py` & `lcapy-1.9.1/lcapy/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_immitance.py` & `lcapy-1.9.1/lcapy/tests/test_immitance.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_jomega.py` & `lcapy-1.9.1/lcapy/tests/test_jomega.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_laplace.py` & `lcapy-1.9.1/lcapy/tests/test_laplace.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_latex.py` & `lcapy-1.9.1/lcapy/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_loop_analysis.py` & `lcapy-1.9.1/lcapy/tests/test_loop_analysis.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_networks.py` & `lcapy-1.9.1/lcapy/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_nodal_analysis.py` & `lcapy-1.9.1/lcapy/tests/test_nodal_analysis.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_noise.py` & `lcapy-1.9.1/lcapy/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_oneport.py` & `lcapy-1.9.1/lcapy/tests/test_oneport.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_ops.py` & `lcapy-1.9.1/lcapy/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_parser.py` & `lcapy-1.9.1/lcapy/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_phasor.py` & `lcapy-1.9.1/lcapy/tests/test_phasor.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_plot.py` & `lcapy-1.9.1/lcapy/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_schematic.py` & `lcapy-1.9.1/lcapy/tests/test_schematic.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_simplify.py` & `lcapy-1.9.1/lcapy/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_simulation.py` & `lcapy-1.9.1/lcapy/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_statespace.py` & `lcapy-1.9.1/lcapy/tests/test_statespace.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_super.py` & `lcapy-1.9.1/lcapy/tests/test_super.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_synthesis.py` & `lcapy-1.9.1/lcapy/tests/test_synthesis.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_transform.py` & `lcapy-1.9.1/lcapy/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_twoport.py` & `lcapy-1.9.1/lcapy/tests/test_twoport.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_units.py` & `lcapy-1.9.1/lcapy/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/tests/test_ztransform.py` & `lcapy-1.9.1/lcapy/tests/test_ztransform.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/texpr.py` & `lcapy-1.9.1/lcapy/texpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/threeport.py` & `lcapy-1.9.1/lcapy/threeport.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/transfer.py` & `lcapy-1.9.1/lcapy/transfer.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/transform.py` & `lcapy-1.9.1/lcapy/transform.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/transformer.py` & `lcapy-1.9.1/lcapy/transformer.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/twoport.py` & `lcapy-1.9.1/lcapy/twoport.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/units.py` & `lcapy-1.9.1/lcapy/units.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/utils.py` & `lcapy-1.9.1/lcapy/utils.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/vector.py` & `lcapy-1.9.1/lcapy/vector.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/voltage.py` & `lcapy-1.9.1/lcapy/voltage.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/zexpr.py` & `lcapy-1.9.1/lcapy/zexpr.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/zmatrix.py` & `lcapy-1.9.1/lcapy/zmatrix.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/zseq.py` & `lcapy-1.9.1/lcapy/zseq.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy/ztransform.py` & `lcapy-1.9.1/lcapy/ztransform.py`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/lcapy.egg-info/PKG-INFO` & `lcapy-1.9.1/lcapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcapy
-Version: 1.9
+Version: 1.9.1
 Summary: Symbolic linear circuit analysis
 Home-page: https://github.com/mph-/lcapy
 Author: Michael Hayes
 Author-email: michael.hayes@canterbury.ac.nz
 License: UNKNOWN
 Download-URL: https://github.com/mph-/lcapy
 Description: Lcapy is a Python package for linear circuit analysis.  It uses SymPy
```

### Comparing `lcapy-1.9/lcapy.egg-info/SOURCES.txt` & `lcapy-1.9.1/lcapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lcapy-1.9/setup.py` & `lcapy-1.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 
-__version__ = '1.9'
+__version__ = '1.9.1'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 tests_require = ['nose', 'flake8', 'flake8-bugbear',
                  'flake8-comprehensions', 'flake8-requirements']
```

