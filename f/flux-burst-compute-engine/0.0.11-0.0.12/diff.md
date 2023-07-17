# Comparing `tmp/flux-burst-compute-engine-0.0.11.tar.gz` & `tmp/flux-burst-compute-engine-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-compute-engine-0.0.11.tar", last modified: Mon Jul 17 01:15:48 2023, max compression
+gzip compressed data, was "flux-burst-compute-engine-0.0.12.tar", last modified: Mon Jul 17 01:58:22 2023, max compression
```

## Comparing `flux-burst-compute-engine-0.0.11.tar` & `flux-burst-compute-engine-0.0.12.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:15:48.529450 flux-burst-compute-engine-0.0.11/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.11/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.11/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      237 2023-07-02 19:33:43.000000 flux-burst-compute-engine-0.0.11/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.11/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2698 2023-07-17 01:15:48.529450 flux-burst-compute-engine-0.0.11/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1830 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:15:48.525449 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2698 2023-07-17 01:15:48.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      791 2023-07-17 01:15:48.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-17 01:15:48.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-02 20:45:41.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       95 2023-07-17 01:15:48.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       25 2023-07-17 01:15:48.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:15:48.525449 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      655 2023-07-02 20:46:03.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12994 2023-07-17 01:15:45.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/plugin.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10593 2023-07-17 01:15:45.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/templates.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1937 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/terraform.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:15:48.525449 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:15:48.529450 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      328 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/boot_script.sh
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4496 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/foundation.tf
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      328 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/install_nfs.sh
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1398 2023-07-16 20:17:40.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/main.tf
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2190 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/variables.tf
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1141 2023-07-17 01:15:45.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.11/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      168 2023-07-17 01:15:48.529450 flux-burst-compute-engine-0.0.11/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3173 2023-07-02 19:33:43.000000 flux-burst-compute-engine-0.0.11/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:58:22.897951 flux-burst-compute-engine-0.0.12/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.12/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.12/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      237 2023-07-02 19:33:43.000000 flux-burst-compute-engine-0.0.12/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.12/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2698 2023-07-17 01:58:22.897951 flux-burst-compute-engine-0.0.12/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1830 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.12/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:58:22.897951 flux-burst-compute-engine-0.0.12/flux_burst_compute_engine.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2698 2023-07-17 01:58:22.000000 flux-burst-compute-engine-0.0.12/flux_burst_compute_engine.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      900 2023-07-17 01:58:22.000000 flux-burst-compute-engine-0.0.12/flux_burst_compute_engine.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-17 01:58:22.000000 flux-burst-compute-engine-0.0.12/flux_burst_compute_engine.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-02 20:45:41.000000 flux-burst-compute-engine-0.0.12/flux_burst_compute_engine.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       95 2023-07-17 01:58:22.000000 flux-burst-compute-engine-0.0.12/flux_burst_compute_engine.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       25 2023-07-17 01:58:22.000000 flux-burst-compute-engine-0.0.12/flux_burst_compute_engine.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:58:22.897951 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      655 2023-07-02 20:46:03.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12838 2023-07-17 01:58:19.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/plugin.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:58:22.897951 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/templates/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      685 2023-07-17 01:58:19.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/templates/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5870 2023-07-17 01:58:19.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/templates/burst_boot.sh
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4944 2023-07-17 01:58:19.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/templates/default_boot.sh
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1937 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/terraform.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:58:22.897951 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/tf/
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:58:22.897951 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/tf/burst/
+-rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      328 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/tf/burst/boot_script.sh
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4496 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/tf/burst/foundation.tf
+-rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      328 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/tf/burst/install_nfs.sh
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1398 2023-07-16 20:17:40.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/tf/burst/main.tf
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2190 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/tf/burst/variables.tf
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1141 2023-07-17 01:58:19.000000 flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.12/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      168 2023-07-17 01:58:22.897951 flux-burst-compute-engine-0.0.12/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3173 2023-07-02 19:33:43.000000 flux-burst-compute-engine-0.0.12/setup.py
```

### Comparing `flux-burst-compute-engine-0.0.11/LICENSE` & `flux-burst-compute-engine-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.11/NOTICE` & `flux-burst-compute-engine-0.0.12/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.11/PKG-INFO` & `flux-burst-compute-engine-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-compute-engine
-Version: 0.0.11
+Version: 0.0.12
 Summary: A bursting plugin for Flux and Compute Engine on Google Cloud
 Home-page: https://github.com/converged-computing/flux-burst-compute-engine
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
```

### Comparing `flux-burst-compute-engine-0.0.11/README.md` & `flux-burst-compute-engine-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/PKG-INFO` & `flux-burst-compute-engine-0.0.12/flux_burst_compute_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-compute-engine
-Version: 0.0.11
+Version: 0.0.12
 Summary: A bursting plugin for Flux and Compute Engine on Google Cloud
 Home-page: https://github.com/converged-computing/flux-burst-compute-engine
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
```

### Comparing `flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/SOURCES.txt` & `flux-burst-compute-engine-0.0.12/flux_burst_compute_engine.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 flux_burst_compute_engine.egg-info/SOURCES.txt
 flux_burst_compute_engine.egg-info/dependency_links.txt
 flux_burst_compute_engine.egg-info/not-zip-safe
 flux_burst_compute_engine.egg-info/requires.txt
 flux_burst_compute_engine.egg-info/top_level.txt
 fluxburst_compute_engine/__init__.py
 fluxburst_compute_engine/plugin.py
-fluxburst_compute_engine/templates.py
 fluxburst_compute_engine/terraform.py
 fluxburst_compute_engine/version.py
+fluxburst_compute_engine/templates/__init__.py
+fluxburst_compute_engine/templates/burst_boot.sh
+fluxburst_compute_engine/templates/default_boot.sh
 fluxburst_compute_engine/tf/burst/boot_script.sh
 fluxburst_compute_engine/tf/burst/foundation.tf
 fluxburst_compute_engine/tf/burst/install_nfs.sh
 fluxburst_compute_engine/tf/burst/main.tf
 fluxburst_compute_engine/tf/burst/variables.tf
```

### Comparing `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/__init__.py` & `flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/plugin.py` & `flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,15 +98,14 @@
             return "0"
         return f"0-{size-1}"
 
     def generate_bursted_boot_script(self, hosts):
         """
         Generate a bursted broked config.
         """
-        template = templates.bursting_boot_script
         with open(self.params.munge_key, "rb") as fd:
             content = fd.read()
         bytes_string = base64.b64encode(content).decode("utf-8")
 
         # Also encode curve-cert in case there are illegal characters
         curve_cert = self.load_encoded_curve_cert()
 
@@ -115,16 +114,15 @@
             "NODELIST": hosts,
             "LOGLEVEL": str(self.params.log_level),
             "CURVECERT": curve_cert,
             "MUNGEKEY": bytes_string,
             "LEAD_BROKER_ADDRESS": self.params.lead_host,
             "LEAD_BROKER_PORT": str(self.params.lead_port),
         }
-        for key, value in replace.items():
-            template = template.replace(key, value)
+        template = templates.get_script("burst_boot.sh", replace)
         self.params.compute_boot_script = template
 
     def load_encoded_curve_cert(self):
         """
         Determine if we are given a path or string verbatim
 
         Return encoded for the start script to handle.
@@ -138,16 +136,14 @@
             )
         return base64.b64encode(curve_cert.encode("utf-8")).decode("utf-8")
 
     def generate_default_boot_script(self, node_count):
         """
         Generate a bursted broked config.
         """
-        template = templates.default_boot_script
-
         # Generate range of hosts, numbered 1-N
         hostrange = "001"
         if node_count > 1:
             # zfill 3 will produce 4 -> 004
             end = str(node_count).zfill(3)
             hostrange = f"[001-{end}]"
 
@@ -157,16 +153,15 @@
 
         # We call this a poor man's jinja2!
         replace = {
             "LOGLEVEL": str(self.params.log_level),
             "NODELIST": hosts,
             "CURVECERT": curve_cert,
         }
-        for key, value in replace.items():
-            template = template.replace(key, value)
+        template = templates.get_script("default_boot.sh", replace)
         self.params.compute_boot_script = template
 
     def generate_resource_hostlist(self):
         """
         Generate the hostlist for the resource spec and the broker.toml.
 
         The hostnames need to line up, index wise, for the bursting to work.
```

### Comparing `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/templates.py` & `flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/templates/burst_boot.sh`

 * *Files 25% similar despite different names*

```diff
@@ -1,178 +1,16 @@
-# Copyright 2023 Lawrence Livermore National Security, LLC and other
-# HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
-#
-# SPDX-License-Identifier: (MIT)
+#!/bin/sh
 
-
-default_boot_script = """#!/bin/sh
-
-set -eEu -o pipefail
-
-# This is already built into the image
-fluxuser=flux
-fluxuid=$(id -u $fluxuser)
-
-# IMPORTANT - this needs to match the local cluster
-fluxroot=/usr
-
-echo "Flux username: $fluxuser"
-echo "Flux install root: $fluxroot"
-export fluxroot
-
-# Prepare NFS
-dnf install nfs-utils -y
-
-mkdir -p /var/nfs/home
-chown nobody:nobody /var/nfs/home
-
-ip_addr=$(hostname -I)
-
-echo "/var/nfs/home *(rw,no_subtree_check,no_root_squash)" >> /etc/exports
-
-firewall-cmd --add-service={nfs,nfs3,mountd,rpc-bind} --permanent
-firewall-cmd --reload
-
-systemctl enable --now nfs-server rpcbind
-
-# TODO we can allow custom logic here if needed
-
-echo "$fluxuser ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers
-printf "$fluxuser user identifiers:\n$(id $fluxuser)\n"
-
-export STATE_DIR=/var/lib/flux
-mkdir -p ${STATE_DIR}
-mkdir -p $fluxroot/etc/flux/system/conf.d
-
-# --cores=IDS Assign cores with IDS to each rank in R, so we  assign 0-(N-1) to each host
-echo "flux R encode --hosts=NODELIST"
-flux R encode --hosts=NODELIST --local > $fluxroot/etc/flux/system/R
-printf "\n📦 Resources\n"
-cat $fluxroot/etc/flux/system/R
-
-mkdir -p /etc/flux/imp/conf.d/
-cat <<EOT >> /etc/flux/imp/conf.d/imp.toml
-[exec]
-allowed-users = [ "$fluxuser", "root" ]
-allowed-shells = [ "$fluxroot/libexec/flux/flux-shell" ]
-EOT
-
-printf "\n🦊 Independent Minister of Privilege\n"
-cat /etc/flux/imp/conf.d/imp.toml
-
-cat <<EOT >> /tmp/system.toml
-[exec]
-imp = "$fluxroot/libexec/flux/flux-imp"
-
-# Allow users other than the instance owner (guests) to connect to Flux
-# Optionally, root may be given "owner privileges" for convenience
-[access]
-allow-guest-user = true
-allow-root-owner = true
-
-# Point to shared network certificate generated flux-keygen(1).
-# Define the network endpoints for Flux's tree based overlay network
-# and inform Flux of the hostnames that will start flux-broker(1).
-[bootstrap]
-curve_cert = "$fluxroot/etc/flux/system/curve.cert"
-
-default_port = 8050
-default_bind = "tcp://eth0:%p"
-default_connect = "tcp://%h:%p"
-
-hosts = [{host="NODELIST"}]
-
-# Speed up detection of crashed network peers (system default is around 20m)
-[tbon]
-tcp_user_timeout = "2m"
-
-# Point to resource definition generated with flux-R(1).
-# Uncomment to exclude nodes (e.g. mgmt, login), from eligibility to run jobs.
-[resource]
-path = "$fluxroot/etc/flux/system/R"
-
-# Remove inactive jobs from the KVS after one week.
-[job-manager]
-inactive-age-limit = "7d"
-EOT
-
-mv /tmp/system.toml $fluxroot/etc/flux/system/conf.d/system.toml
-
-echo "🐸 Broker Configuration"
-cat $fluxroot/etc/flux/system/conf.d/system.toml
-
-# If we are communicating via the flux uri this service needs to be started
-chmod u+s $fluxroot/libexec/flux/flux-imp
-chmod 4755 $fluxroot/libexec/flux/flux-imp
-chmod 0644 /etc/flux/imp/conf.d/imp.toml
-# sudo chown -R $fluxuser:$fluxuser $fluxroot/etc/flux/system/conf.d
-
-cat << "PYTHON_DECODING_SCRIPT" > /tmp/convert_curve_cert.py
-#!/usr/bin/env python3
-import sys
-import base64
-
-string = sys.argv[1]
-dest = sys.argv[2]
-with open(dest, 'w') as fd:
-    fd.write(base64.b64decode(string).decode('utf-8'))
-PYTHON_DECODING_SCRIPT
-
-python3 /tmp/convert_curve_cert.py "CURVECERT" /tmp/curve.cert
-
-mv /tmp/curve.cert $fluxroot/etc/flux/system/curve.cert
-chmod u=r,g=,o= $fluxroot/etc/flux/system/curve.cert
-chown $fluxuser:$fluxuser $fluxroot/etc/flux/system/curve.cert
-# munge.key gets shipped with image, needs to be same / shared
-# /usr/sbin/create-munge-key
-service munge start
-
-# The rundir needs to be created first, and owned by user flux
-# Along with the state directory and curve certificate
-mkdir -p /run/flux
-sudo chown -R $fluxuser:$fluxuser /run/flux
-
-# Remove group and other read
-chmod o-r $fluxroot/etc/flux/system/curve.cert
-chmod g-r $fluxroot/etc/flux/system/curve.cert
-chown -R $fluxuid /run/flux ${STATE_DIR} $fluxroot/etc/flux/system/curve.cert
-
-printf "\n✨ Curve certificate generated by helper pod\n"
-cat $fluxroot/etc/flux/system/curve.cert
-
-cat << "FIRST_BOOT_UNIT" > /etc/systemd/system/flux-start.service
-[Unit]
-Description=Flux message broker
-Wants=munge.service
-
-[Service]
-Type=simple
-NotifyAccess=main
-TimeoutStopSec=90
-KillMode=mixed
-ExecStart=/usr/bin/flux start --broker-opts --config /usr/etc/flux/system/conf.d -Stbon.fanout=256  -Srundir=/run/flux -Sbroker.rc2_none -Sstatedir=/var/lib/flux -Slocal-uri=local:///run/flux/local -Stbon.connect_timeout=5s -Stbon.zmqdebug=1  -Slog-stderr-level=7 -Slog-stderr-mode=local
-SyslogIdentifier=flux
-Restart=always
-RestartSec=5s
-RestartPreventExitStatus=42
-SuccessExitStatus=42
-User=flux
-Group=flux
-PermissionsStartOnly=true
-Delegate=yes
-
-[Install]
-WantedBy=multi-user.target
-FIRST_BOOT_UNIT
-
-systemctl enable flux-start.service
-systemctl start flux-start.service
-"""
-
-bursting_boot_script = """#!/bin/sh
+# Burst boot, requires:
+# CURVECERT: base64 encoded curve certificate
+# NODELIST: with complete list of nodes
+# LOGLEVEL: desireed flux log level
+# MUNGEKEY: bytes string for the munge key
+# LEAD_BROKER_ADDRESS
+# LEAD_BROKER_PORT
 
 set -eEu -o pipefail
 
 # This is already built into the image
 fluxuser=flux
 fluxuid=$(id -u ${fluxuser})
 
@@ -354,8 +192,7 @@
 
 [Install]
 WantedBy=multi-user.target
 FIRST_BOOT_UNIT
 
 systemctl enable flux-start.service
 systemctl start flux-start.service
-"""
```

### Comparing `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/terraform.py` & `flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/terraform.py`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/foundation.tf` & `flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/tf/burst/foundation.tf`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/main.tf` & `flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/tf/burst/main.tf`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/variables.tf` & `flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/tf/burst/variables.tf`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/version.py` & `flux-burst-compute-engine-0.0.12/fluxburst_compute_engine/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.11"
+__version__ = "0.0.12"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-burst-compute-engine"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst-compute-engine"
 KEYWORDS = "flux, flux-framework, workflow, example, plugin"
 DESCRIPTION = "A bursting plugin for Flux and Compute Engine on Google Cloud"
 LICENSE = "LICENSE"
```

### Comparing `flux-burst-compute-engine-0.0.11/setup.py` & `flux-burst-compute-engine-0.0.12/setup.py`

 * *Files identical despite different names*

