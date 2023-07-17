# Comparing `tmp/flux-burst-compute-engine-0.0.1.tar.gz` & `tmp/flux-burst-compute-engine-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-compute-engine-0.0.1.tar", last modified: Mon Jul 10 03:06:47 2023, max compression
+gzip compressed data, was "flux-burst-compute-engine-0.0.11.tar", last modified: Mon Jul 17 01:15:48 2023, max compression
```

## Comparing `flux-burst-compute-engine-0.0.1.tar` & `flux-burst-compute-engine-0.0.11.tar`

### file list

```diff
@@ -1,36 +1,30 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-10 03:06:47.922928 flux-burst-compute-engine-0.0.1/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.1/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.1/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      237 2023-07-02 19:33:43.000000 flux-burst-compute-engine-0.0.1/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.1/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2697 2023-07-10 03:06:47.922928 flux-burst-compute-engine-0.0.1/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1830 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-10 03:06:47.922928 flux-burst-compute-engine-0.0.1/flux_burst_compute_engine.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2697 2023-07-10 03:06:47.000000 flux-burst-compute-engine-0.0.1/flux_burst_compute_engine.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1026 2023-07-10 03:06:47.000000 flux-burst-compute-engine-0.0.1/flux_burst_compute_engine.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-10 03:06:47.000000 flux-burst-compute-engine-0.0.1/flux_burst_compute_engine.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-02 20:45:41.000000 flux-burst-compute-engine-0.0.1/flux_burst_compute_engine.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       95 2023-07-10 03:06:47.000000 flux-burst-compute-engine-0.0.1/flux_burst_compute_engine.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       25 2023-07-10 03:06:47.000000 flux-burst-compute-engine-0.0.1/flux_burst_compute_engine.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-10 03:06:47.922928 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      655 2023-07-02 20:46:03.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13191 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/plugin.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10917 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/templates.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1937 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/terraform.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-10 03:06:47.918928 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-10 03:06:47.922928 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/basic/
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      328 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/basic/boot_script.sh
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4496 2023-07-07 23:03:59.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/basic/foundation.tf
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      328 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/basic/install_nfs.sh
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1908 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/basic/main.tf
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4073 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/basic/variables.tf
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-10 03:06:47.922928 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/burst/
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      328 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/burst/boot_script.sh
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4496 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/burst/foundation.tf
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      328 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/burst/install_nfs.sh
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1398 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/burst/main.tf
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2190 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/burst/variables.tf
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1140 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.1/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      168 2023-07-10 03:06:47.922928 flux-burst-compute-engine-0.0.1/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3173 2023-07-02 19:33:43.000000 flux-burst-compute-engine-0.0.1/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:15:48.529450 flux-burst-compute-engine-0.0.11/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.11/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.11/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      237 2023-07-02 19:33:43.000000 flux-burst-compute-engine-0.0.11/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.11/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2698 2023-07-17 01:15:48.529450 flux-burst-compute-engine-0.0.11/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1830 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:15:48.525449 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2698 2023-07-17 01:15:48.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      791 2023-07-17 01:15:48.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-17 01:15:48.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-02 20:45:41.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       95 2023-07-17 01:15:48.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       25 2023-07-17 01:15:48.000000 flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:15:48.525449 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      655 2023-07-02 20:46:03.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12994 2023-07-17 01:15:45.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/plugin.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10593 2023-07-17 01:15:45.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/templates.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1937 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/terraform.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:15:48.525449 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-17 01:15:48.529450 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/
+-rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      328 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/boot_script.sh
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4496 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/foundation.tf
+-rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      328 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/install_nfs.sh
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1398 2023-07-16 20:17:40.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/main.tf
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2190 2023-07-10 03:06:17.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/variables.tf
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1141 2023-07-17 01:15:45.000000 flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-07-02 19:32:46.000000 flux-burst-compute-engine-0.0.11/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      168 2023-07-17 01:15:48.529450 flux-burst-compute-engine-0.0.11/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3173 2023-07-02 19:33:43.000000 flux-burst-compute-engine-0.0.11/setup.py
```

### Comparing `flux-burst-compute-engine-0.0.1/LICENSE` & `flux-burst-compute-engine-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.1/NOTICE` & `flux-burst-compute-engine-0.0.11/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.1/PKG-INFO` & `flux-burst-compute-engine-0.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-compute-engine
-Version: 0.0.1
+Version: 0.0.11
 Summary: A bursting plugin for Flux and Compute Engine on Google Cloud
 Home-page: https://github.com/converged-computing/flux-burst-compute-engine
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
```

### Comparing `flux-burst-compute-engine-0.0.1/README.md` & `flux-burst-compute-engine-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.1/flux_burst_compute_engine.egg-info/PKG-INFO` & `flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-compute-engine
-Version: 0.0.1
+Version: 0.0.11
 Summary: A bursting plugin for Flux and Compute Engine on Google Cloud
 Home-page: https://github.com/converged-computing/flux-burst-compute-engine
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
```

### Comparing `flux-burst-compute-engine-0.0.1/flux_burst_compute_engine.egg-info/SOURCES.txt` & `flux-burst-compute-engine-0.0.11/flux_burst_compute_engine.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,17 +13,12 @@
 flux_burst_compute_engine.egg-info/requires.txt
 flux_burst_compute_engine.egg-info/top_level.txt
 fluxburst_compute_engine/__init__.py
 fluxburst_compute_engine/plugin.py
 fluxburst_compute_engine/templates.py
 fluxburst_compute_engine/terraform.py
 fluxburst_compute_engine/version.py
-fluxburst_compute_engine/tf/basic/boot_script.sh
-fluxburst_compute_engine/tf/basic/foundation.tf
-fluxburst_compute_engine/tf/basic/install_nfs.sh
-fluxburst_compute_engine/tf/basic/main.tf
-fluxburst_compute_engine/tf/basic/variables.tf
 fluxburst_compute_engine/tf/burst/boot_script.sh
 fluxburst_compute_engine/tf/burst/foundation.tf
 fluxburst_compute_engine/tf/burst/install_nfs.sh
 fluxburst_compute_engine/tf/burst/main.tf
 fluxburst_compute_engine/tf/burst/variables.tf
```

### Comparing `flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/__init__.py` & `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/plugin.py` & `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     network_name: Optional[str] = "foundation-net"
     region: Optional[str] = "us-central1"
     zone: Optional[str] = "us-central1-a"
 
     # An isolated burst brings up an independent cluster
     isolated_burst: Optional[bool] = False
 
-    # Lead broker service hostname or ip address
+    # Lead broker service hostname or ip addressf
     lead_host: Optional[str] = None
 
     # Lead broker service port (e.g, 30093)
     lead_port: Optional[str] = None
 
     # Host names on the main cluster excluding the lead_host
     # and additional login hosts. E.g.,
@@ -61,15 +61,17 @@
     cluster_name: Optional[str] = "flux-bursted-cluster"
 
     # Compute node specs
     compute_scopes: List = field(default_factory=lambda: ["cloud-platform"])
     compute_name_prefix: Optional[str] = "gffw-compute-a"
     compute_machine_arch: Optional[str] = "x86-64"
     compute_machine_type: Optional[str] = "c2-standard-8"
-    compute_family: Optional[str] = "flux-bursted-compute-x86-64"
+
+    # This builds from converged-computing/flux-terraform-gcp/build-images/bursted
+    compute_family: Optional[str] = "flux-fw-bursted-x86-64"
 
     # Compact mode
     compute_compact: Optional[bool] = False
 
     # GPUS (not added yet)
     gpu_type: Optional[str] = None
     gpu_count: Optional[int] = 0
@@ -173,25 +175,18 @@
         """
         # hosts are the lead broker address plus the original node names.
         # TODO need to have NODELIST just be here
         # hosts = [{ host = "gffw-manager-001,gffw-login-001,gffw-compute-a-[001-004]" },]
         # Except gffw-manager-001 should be an ip address (typically)
         return f"{self.params.lead_host},{self.params.lead_hostnames}"
 
-    def run(self, request_burst=False, nodes=None, tasks=None):
+    def run(self, request_burst=False, nodes=None, **kwargs):
         """
         Given some set of scheduled jobs, run bursting.
         """
-        # Don't support this yet - not enough time to develop / ensure working
-        if self.params.isolated_burst:
-            logger.warning(
-                "Isolated burst is not fully tested yet, please open an issue if you want it."
-            )
-            return
-
         # Exit early if no jobs to burst
         if not self.jobs and not request_burst:
             logger.info(f"Plugin {self.name} has no jobs to burst.")
             return
 
         # If we have requested a burst, nodes are required
         if request_burst and not nodes:
```

### Comparing `flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/templates.py` & `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 default_boot_script = """#!/bin/sh
 
 set -eEu -o pipefail
 
 # This is already built into the image
 fluxuser=flux
-fluxuid=$(id -u ${fluxuser})
+fluxuid=$(id -u $fluxuser)
 
 # IMPORTANT - this needs to match the local cluster
 fluxroot=/usr
 
-echo "Flux username: ${fluxuser}"
-echo "Flux install root: ${fluxroot}"
+echo "Flux username: $fluxuser"
+echo "Flux install root: $fluxroot"
 export fluxroot
 
 # Prepare NFS
 dnf install nfs-utils -y
 
 mkdir -p /var/nfs/home
 chown nobody:nobody /var/nfs/home
@@ -30,145 +30,137 @@
 echo "/var/nfs/home *(rw,no_subtree_check,no_root_squash)" >> /etc/exports
 
 firewall-cmd --add-service={nfs,nfs3,mountd,rpc-bind} --permanent
 firewall-cmd --reload
 
 systemctl enable --now nfs-server rpcbind
 
-# commands to be run as root
-asFlux="sudo -u ${fluxuser} -E HOME=/home/${fluxuser} -E PATH=$PATH"
-
 # TODO we can allow custom logic here if needed
 
-echo "${fluxuser} ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers
-printf "${fluxuser} user identifiers:\n$(id ${fluxuser})\n"
-printf "\nAs Flux prefix for flux commands: ${asFlux}\n"
+echo "$fluxuser ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers
+printf "$fluxuser user identifiers:\n$(id $fluxuser)\n"
 
 export STATE_DIR=/var/lib/flux
 mkdir -p ${STATE_DIR}
-mkdir -p ${fluxroot}/etc/flux/system/conf.d
+mkdir -p $fluxroot/etc/flux/system/conf.d
 
 # --cores=IDS Assign cores with IDS to each rank in R, so we  assign 0-(N-1) to each host
 echo "flux R encode --hosts=NODELIST"
-flux R encode --hosts=NODELIST --local > ${fluxroot}/etc/flux/system/R
+flux R encode --hosts=NODELIST --local > $fluxroot/etc/flux/system/R
 printf "\n📦 Resources\n"
-cat ${fluxroot}/etc/flux/system/R
+cat $fluxroot/etc/flux/system/R
 
 mkdir -p /etc/flux/imp/conf.d/
 cat <<EOT >> /etc/flux/imp/conf.d/imp.toml
 [exec]
-allowed-users = [ "${fluxuser}", "root" ]
-allowed-shells = [ "${fluxroot}/libexec/flux/flux-shell" ]
+allowed-users = [ "$fluxuser", "root" ]
+allowed-shells = [ "$fluxroot/libexec/flux/flux-shell" ]
 EOT
 
 printf "\n🦊 Independent Minister of Privilege\n"
 cat /etc/flux/imp/conf.d/imp.toml
 
 cat <<EOT >> /tmp/system.toml
 [exec]
-imp = "${fluxroot}/libexec/flux/flux-imp"
+imp = "$fluxroot/libexec/flux/flux-imp"
 
 # Allow users other than the instance owner (guests) to connect to Flux
 # Optionally, root may be given "owner privileges" for convenience
 [access]
 allow-guest-user = true
 allow-root-owner = true
 
 # Point to shared network certificate generated flux-keygen(1).
 # Define the network endpoints for Flux's tree based overlay network
 # and inform Flux of the hostnames that will start flux-broker(1).
 [bootstrap]
-curve_cert = "${fluxroot}/etc/flux/system/curve.cert"
+curve_cert = "$fluxroot/etc/flux/system/curve.cert"
 
 default_port = 8050
 default_bind = "tcp://eth0:%p"
 default_connect = "tcp://%h:%p"
 
 hosts = [{host="NODELIST"}]
 
 # Speed up detection of crashed network peers (system default is around 20m)
 [tbon]
 tcp_user_timeout = "2m"
 
 # Point to resource definition generated with flux-R(1).
 # Uncomment to exclude nodes (e.g. mgmt, login), from eligibility to run jobs.
 [resource]
-path = "${fluxroot}/etc/flux/system/R"
+path = "$fluxroot/etc/flux/system/R"
 
 # Remove inactive jobs from the KVS after one week.
 [job-manager]
 inactive-age-limit = "7d"
 EOT
 
-mv /tmp/system.toml ${fluxroot}/etc/flux/system/conf.d/system.toml
+mv /tmp/system.toml $fluxroot/etc/flux/system/conf.d/system.toml
 
 echo "🐸 Broker Configuration"
-cat ${fluxroot}/etc/flux/system/conf.d/system.toml
+cat $fluxroot/etc/flux/system/conf.d/system.toml
 
 # If we are communicating via the flux uri this service needs to be started
-chmod u+s ${fluxroot}/libexec/flux/flux-imp
-chmod 4755 ${fluxroot}/libexec/flux/flux-imp
+chmod u+s $fluxroot/libexec/flux/flux-imp
+chmod 4755 $fluxroot/libexec/flux/flux-imp
 chmod 0644 /etc/flux/imp/conf.d/imp.toml
-sudo chown -R ${fluxuser}:${fluxuser} ${fluxroot}/etc/flux/system/conf.d
+# sudo chown -R $fluxuser:$fluxuser $fluxroot/etc/flux/system/conf.d
 
 cat << "PYTHON_DECODING_SCRIPT" > /tmp/convert_curve_cert.py
 #!/usr/bin/env python3
 import sys
 import base64
 
 string = sys.argv[1]
 dest = sys.argv[2]
 with open(dest, 'w') as fd:
     fd.write(base64.b64decode(string).decode('utf-8'))
 PYTHON_DECODING_SCRIPT
 
 python3 /tmp/convert_curve_cert.py "CURVECERT" /tmp/curve.cert
 
-mv /tmp/curve.cert ${fluxroot}/etc/flux/system/curve.cert
-chmod u=r,g=,o= ${fluxroot}/etc/flux/system/curve.cert
-chown ${fluxuser}:${fluxuser} ${fluxroot}/etc/flux/system/curve.cert
-service munge start > /dev/null 2>&1
+mv /tmp/curve.cert $fluxroot/etc/flux/system/curve.cert
+chmod u=r,g=,o= $fluxroot/etc/flux/system/curve.cert
+chown $fluxuser:$fluxuser $fluxroot/etc/flux/system/curve.cert
+# munge.key gets shipped with image, needs to be same / shared
+# /usr/sbin/create-munge-key
+service munge start
 
 # The rundir needs to be created first, and owned by user flux
 # Along with the state directory and curve certificate
 mkdir -p /run/flux
-sudo chown -R ${fluxuser}:${fluxuser} /run/flux
+sudo chown -R $fluxuser:$fluxuser /run/flux
 
 # Remove group and other read
-chmod o-r ${fluxroot}/etc/flux/system/curve.cert
-chmod g-r ${fluxroot}/etc/flux/system/curve.cert
-chown -R ${fluxuid} /run/flux ${STATE_DIR} ${fluxroot}/etc/flux/system/curve.cert
+chmod o-r $fluxroot/etc/flux/system/curve.cert
+chmod g-r $fluxroot/etc/flux/system/curve.cert
+chown -R $fluxuid /run/flux ${STATE_DIR} $fluxroot/etc/flux/system/curve.cert
 
 printf "\n✨ Curve certificate generated by helper pod\n"
-cat ${fluxroot}/etc/flux/system/curve.cert
-
-mkdir -p /etc/flux/manager
+cat $fluxroot/etc/flux/system/curve.cert
 
 cat << "FIRST_BOOT_UNIT" > /etc/systemd/system/flux-start.service
 [Unit]
 Description=Flux message broker
 Wants=munge.service
 
 [Service]
 Type=simple
 NotifyAccess=main
 TimeoutStopSec=90
 KillMode=mixed
-ExecStart=/bin/bash -c '/usr/bin/flux broker --config-path /usr/etc/flux/system/conf.d -Scron.directory=/usr/etc/flux/system/conf.d -Stbon.fanout=256  -Srundir=/run/flux -Sbroker.rc2_none -Sstatedir=/var/lib/flux -Slocal-uri=local:///run/flux/local -Stbon.connect_timeout=5s -Stbon.zmqdebug=1  -Slog-stderr-level=LOGLEVEL -Slog-stderr-mode=local'
+ExecStart=/usr/bin/flux start --broker-opts --config /usr/etc/flux/system/conf.d -Stbon.fanout=256  -Srundir=/run/flux -Sbroker.rc2_none -Sstatedir=/var/lib/flux -Slocal-uri=local:///run/flux/local -Stbon.connect_timeout=5s -Stbon.zmqdebug=1  -Slog-stderr-level=7 -Slog-stderr-mode=local
 SyslogIdentifier=flux
 Restart=always
 RestartSec=5s
 RestartPreventExitStatus=42
 SuccessExitStatus=42
 User=flux
 Group=flux
-RuntimeDirectory=flux
-RuntimeDirectoryMode=0755
-StateDirectory=flux
-StateDirectoryMode=0700
 PermissionsStartOnly=true
 Delegate=yes
 
 [Install]
 WantedBy=multi-user.target
 FIRST_BOOT_UNIT
```

### Comparing `flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/terraform.py` & `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/terraform.py`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/basic/foundation.tf` & `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/foundation.tf`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/basic/main.tf` & `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/main.tf`

 * *Files 22% similar despite different names*

```diff
@@ -9,40 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 module "cluster" {
-    source = "github.com/converged-computing/flux-terraform-gcp//tf?ref=test-bursted"
+    source = "github.com/converged-computing/flux-terraform-gcp//burst"
     project_id           = var.project_id
     region               = var.region
 
     service_account_emails = {
         manager = data.google_compute_default_service_account.default.email
         login   = data.google_compute_default_service_account.default.email
         compute = data.google_compute_default_service_account.default.email
     }
 
     subnetwork           = module.network.subnets_self_links[0]
     cluster_storage      = {
         mountpoint = "/home"
         share      = "${module.nfs_server_instance.instances_details.0.network_interface.0.network_ip}:/var/nfs/home"
     }
-
-    manager_name_prefix  = var.manager_name_prefix
-    manager_machine_type = var.manager_machine_type
-    manager_scopes       = var.manager_scopes
-    manager_family       = var.manager_family
-    broker_config        = var.broker_config
-    resource_hosts       = var.resource_hosts
-    curve_cert           = var.curve_cert
-    munge_key            = var.munge_key
-
-    login_node_specs = var.login_node_specs
-    login_scopes     = var.login_scopes
-    login_family     = var.login_family
-
     compute_node_specs = var.compute_node_specs
     compute_scopes     = var.compute_scopes
-    compute_family     = var.compute_family
+    family             = var.compute_family
 }
```

### Comparing `flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/tf/burst/variables.tf` & `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/tf/burst/variables.tf`

 * *Files identical despite different names*

### Comparing `flux-burst-compute-engine-0.0.1/fluxburst_compute_engine/version.py` & `flux-burst-compute-engine-0.0.11/fluxburst_compute_engine/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.1"
+__version__ = "0.0.11"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-burst-compute-engine"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst-compute-engine"
 KEYWORDS = "flux, flux-framework, workflow, example, plugin"
 DESCRIPTION = "A bursting plugin for Flux and Compute Engine on Google Cloud"
 LICENSE = "LICENSE"
```

### Comparing `flux-burst-compute-engine-0.0.1/setup.py` & `flux-burst-compute-engine-0.0.11/setup.py`

 * *Files identical despite different names*

