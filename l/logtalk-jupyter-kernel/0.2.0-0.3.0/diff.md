# Comparing `tmp/logtalk-jupyter-kernel-0.2.0.tar.gz` & `tmp/logtalk-jupyter-kernel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logtalk-jupyter-kernel-0.2.0.tar", last modified: Wed Feb 15 22:10:47 2023, max compression
+gzip compressed data, was "logtalk-jupyter-kernel-0.3.0.tar", last modified: Mon Jul 17 09:31:32 2023, max compression
```

## Comparing `logtalk-jupyter-kernel-0.2.0.tar` & `logtalk-jupyter-kernel-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,38 @@
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-02-15 22:10:47.364340 logtalk-jupyter-kernel-0.2.0/
--rw-r--r--   0 pmoura     (501) staff       (20)     1129 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/LICENSE
--rw-r--r--   0 pmoura     (501) staff       (20)      164 2023-02-15 15:11:09.000000 logtalk-jupyter-kernel-0.2.0/MANIFEST.in
--rw-r--r--   0 pmoura     (501) staff       (20)    16304 2023-02-15 22:10:47.364616 logtalk-jupyter-kernel-0.2.0/PKG-INFO
--rw-r--r--   0 pmoura     (501) staff       (20)    14127 2023-02-15 20:04:42.000000 logtalk-jupyter-kernel-0.2.0/README.md
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-02-15 22:10:47.349118 logtalk-jupyter-kernel-0.2.0/logtalk_jupyter_kernel.egg-info/
--rw-r--r--   0 pmoura     (501) staff       (20)    16304 2023-02-15 22:10:47.000000 logtalk-jupyter-kernel-0.2.0/logtalk_jupyter_kernel.egg-info/PKG-INFO
--rw-r--r--   0 pmoura     (501) staff       (20)     1281 2023-02-15 22:10:47.000000 logtalk-jupyter-kernel-0.2.0/logtalk_jupyter_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 pmoura     (501) staff       (20)        1 2023-02-15 22:10:47.000000 logtalk-jupyter-kernel-0.2.0/logtalk_jupyter_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 pmoura     (501) staff       (20)       97 2023-02-15 22:10:47.000000 logtalk-jupyter-kernel-0.2.0/logtalk_jupyter_kernel.egg-info/requires.txt
--rw-r--r--   0 pmoura     (501) staff       (20)       20 2023-02-15 22:10:47.000000 logtalk-jupyter-kernel-0.2.0/logtalk_jupyter_kernel.egg-info/top_level.txt
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-02-15 22:10:47.352741 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/
--rw-r--r--   0 pmoura     (501) staff       (20)     1497 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/__init__.py
--rw-r--r--   0 pmoura     (501) staff       (20)     1526 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/__main__.py
--rw-r--r--   0 pmoura     (501) staff       (20)     3388 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/install.py
--rw-r--r--   0 pmoura     (501) staff       (20)    29462 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/kernel.py
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-02-15 22:10:47.353091 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/kernelspec/
--rw-r--r--   0 pmoura     (501) staff       (20)     4957 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/kernelspec/kernel.js
--rw-r--r--   0 pmoura     (501) staff       (20)    30599 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_kernel_base_implementation.py
--rw-r--r--   0 pmoura     (501) staff       (20)     8218 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_kernel_config.py
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-02-15 22:10:47.357704 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/
--rw-r--r--   0 pmoura     (501) staff       (20)    16216 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)    14513 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_jsonrpc.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     2733 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_logging.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     4393 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_preferences.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)    13945 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_query_handling.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)    13816 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_request_handling.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     5875 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_server.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)    62311 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_term_handling.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     7583 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_variable_bindings.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     2111 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/loader.lgt
--rw-r--r--   0 pmoura     (501) staff       (20)     8264 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/sicstus_kernel_implementation.py
--rw-r--r--   0 pmoura     (501) staff       (20)     3854 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.2.0/logtalk_kernel/swi_kernel_implementation.py
-drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-02-15 22:10:47.362797 logtalk-jupyter-kernel-0.2.0/notebooks/
--rw-r--r--   0 pmoura     (501) staff       (20)    44781 2022-12-21 14:27:08.000000 logtalk-jupyter-kernel-0.2.0/notebooks/JupyterKernelForLogtalkOverview.ipynb
--rw-r--r--   0 pmoura     (501) staff       (20)    44419 2023-02-09 20:56:59.000000 logtalk-jupyter-kernel-0.2.0/notebooks/LogtalkTutorial.ipynb
--rw-r--r--   0 pmoura     (501) staff       (20)   225124 2022-11-07 13:48:42.000000 logtalk-jupyter-kernel-0.2.0/notebooks/architecture_diagram.png
--rw-r--r--   0 pmoura     (501) staff       (20)   142829 2022-11-07 13:48:42.000000 logtalk-jupyter-kernel-0.2.0/notebooks/user_interaction_diagram.png
--rw-r--r--   0 pmoura     (501) staff       (20)     1144 2023-02-15 20:15:36.000000 logtalk-jupyter-kernel-0.2.0/pyproject.toml
--rw-r--r--   0 pmoura     (501) staff       (20)      200 2023-02-15 22:10:47.365352 logtalk-jupyter-kernel-0.2.0/setup.cfg
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.638483 logtalk-jupyter-kernel-0.3.0/
+-rw-r--r--   0 pmoura     (501) staff       (20)     1129 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/LICENSE
+-rw-r--r--   0 pmoura     (501) staff       (20)      164 2023-02-15 15:11:09.000000 logtalk-jupyter-kernel-0.3.0/MANIFEST.in
+-rw-r--r--   0 pmoura     (501) staff       (20)    16472 2023-07-17 09:31:32.638671 logtalk-jupyter-kernel-0.3.0/PKG-INFO
+-rw-r--r--   0 pmoura     (501) staff       (20)    14295 2023-07-15 19:06:11.000000 logtalk-jupyter-kernel-0.3.0/README.md
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.626451 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/
+-rw-r--r--   0 pmoura     (501) staff       (20)    16472 2023-07-17 09:31:32.000000 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 pmoura     (501) staff       (20)     1207 2023-07-17 09:31:32.000000 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 pmoura     (501) staff       (20)        1 2023-07-17 09:31:32.000000 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 pmoura     (501) staff       (20)       97 2023-07-17 09:31:32.000000 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/requires.txt
+-rw-r--r--   0 pmoura     (501) staff       (20)       32 2023-07-17 09:31:32.000000 logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/top_level.txt
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.629099 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/
+-rw-r--r--   0 pmoura     (501) staff       (20)     1497 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/__init__.py
+-rw-r--r--   0 pmoura     (501) staff       (20)     1526 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/__main__.py
+-rw-r--r--   0 pmoura     (501) staff       (20)     3388 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/install.py
+-rw-r--r--   0 pmoura     (501) staff       (20)    29462 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/kernel.py
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.629486 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/kernelspec/
+-rw-r--r--   0 pmoura     (501) staff       (20)     4957 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/kernelspec/kernel.js
+-rw-r--r--   0 pmoura     (501) staff       (20)    30599 2023-02-15 16:44:31.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_kernel_base_implementation.py
+-rw-r--r--   0 pmoura     (501) staff       (20)     8218 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_kernel_config.py
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.635172 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/
+-rw-r--r--   0 pmoura     (501) staff       (20)    16216 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)    14513 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_jsonrpc.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     2733 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_logging.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     4393 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_preferences.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)    13945 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_query_handling.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)    13816 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_request_handling.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     5875 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_server.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)    62311 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_term_handling.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     7583 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_variable_bindings.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     2111 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/loader.lgt
+-rw-r--r--   0 pmoura     (501) staff       (20)     8264 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/sicstus_kernel_implementation.py
+-rw-r--r--   0 pmoura     (501) staff       (20)     3854 2023-02-15 16:44:25.000000 logtalk-jupyter-kernel-0.3.0/logtalk_kernel/swi_kernel_implementation.py
+drwxr-xr-x   0 pmoura     (501) staff       (20)        0 2023-07-17 09:31:32.636977 logtalk-jupyter-kernel-0.3.0/notebooks/
+-rw-r--r--   0 pmoura     (501) staff       (20)    45691 2023-07-17 09:09:11.000000 logtalk-jupyter-kernel-0.3.0/notebooks/JupyterKernelForLogtalkOverview.ipynb
+-rw-r--r--   0 pmoura     (501) staff       (20)    44419 2023-02-09 20:56:59.000000 logtalk-jupyter-kernel-0.3.0/notebooks/LogtalkTutorial.ipynb
+-rw-r--r--   0 pmoura     (501) staff       (20)     1156 2023-07-17 09:23:37.000000 logtalk-jupyter-kernel-0.3.0/pyproject.toml
+-rw-r--r--   0 pmoura     (501) staff       (20)      200 2023-07-17 09:31:32.639206 logtalk-jupyter-kernel-0.3.0/setup.cfg
```

### Comparing `logtalk-jupyter-kernel-0.2.0/LICENSE` & `logtalk-jupyter-kernel-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/PKG-INFO` & `logtalk-jupyter-kernel-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logtalk-jupyter-kernel
-Version: 0.2.0
+Version: 0.3.0
 Summary: Hercutalk - A Jupyter Kernel for Logtalk
 Author: Paulo Moura, Anne Brecklinghaus, Michael Leuschel, dgelessus
 License: Copyright (c) 2022-2023 Paulo Moura  
         Copyright (c) 2022 Anne Brecklinghaus, Michael Leuschel, dgelessus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -48,21 +48,23 @@
 
 This project is a fork of the [prolog-jupyter-kernel](https://github.com/hhu-stups/prolog-jupyter-kernel) project (developed by Anne Brecklinghaus in her Master's thesis at the University of Düsseldorf under the supervision of Michael Leuschel and Philipp Körner) and still under development. It includes back-ports of recent patches and improvements by Michael Leuschel, dgelessus, and Silas Kraume. Major changes are committed and more are expected. Furthermore, no liability is accepted for correctness and completeness (see the [LICENSE](LICENSE) file).
 
 
 ## Supported Prolog backends
 
 - [ECLiPSe 7.0 #57 or later](http://eclipseclp.org/)
-- [GNU Prolog 1.5.1 or later](http://www.gprolog.org/) (use git version until 1.5.1 is released)
-- [LVM 5.0.0 or later](https://graphstax.ai/)
+- [GNU Prolog 1.6.0 or later](http://www.gprolog.org/) (use git version until 1.6.0 is released)
+- [LVM 6.3.0 or later](https://permion.ai/)
 - [SICStus Prolog 4.5.1 or later](https://sicstus.sics.se/)
 - [SWI-Prolog 8.4.3 or later](https://www.swi-prolog.org/) (default)
-- [Trealla Prolog 2.6.9 or later](https://github.com/trealla-prolog/trealla)
+- [Trealla Prolog 2.18.7 or later](https://github.com/trealla-prolog/trealla)
 - [YAP 7.2.1 or later](https://github.com/vscosta)
 
+Note that an online use of this kernel (instead of local) may be restricted to a subset of these backends (notably, due to some systems requiring commercial licenses).
+
 The kernel is implemented in a way that basically all functionality except the loading of configuration files can easily be overridden. This is especially useful for **extending the kernel for further Prolog backends** or running code with a different version of a backend. For further information about this, see [Configuration](#configuration).
 
 Also see the [JupyterLab Logtalk CodeMirror Extension](https://github.com/LogtalkDotOrg/jupyterlab-logtalk-codemirror-extension) for *syntax highlighting* of Logtalk code in JupyterLab (forked from the [JupyterLab Prolog CodeMirror Extension](https://github.com/hhu-stups/jupyterlab-prolog-codemirror-extension)).
 
 
 ## Prolog backend requirements
```

### Comparing `logtalk-jupyter-kernel-0.2.0/README.md` & `logtalk-jupyter-kernel-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 
 This project is a fork of the [prolog-jupyter-kernel](https://github.com/hhu-stups/prolog-jupyter-kernel) project (developed by Anne Brecklinghaus in her Master's thesis at the University of Düsseldorf under the supervision of Michael Leuschel and Philipp Körner) and still under development. It includes back-ports of recent patches and improvements by Michael Leuschel, dgelessus, and Silas Kraume. Major changes are committed and more are expected. Furthermore, no liability is accepted for correctness and completeness (see the [LICENSE](LICENSE) file).
 
 
 ## Supported Prolog backends
 
 - [ECLiPSe 7.0 #57 or later](http://eclipseclp.org/)
-- [GNU Prolog 1.5.1 or later](http://www.gprolog.org/) (use git version until 1.5.1 is released)
-- [LVM 5.0.0 or later](https://graphstax.ai/)
+- [GNU Prolog 1.6.0 or later](http://www.gprolog.org/) (use git version until 1.6.0 is released)
+- [LVM 6.3.0 or later](https://permion.ai/)
 - [SICStus Prolog 4.5.1 or later](https://sicstus.sics.se/)
 - [SWI-Prolog 8.4.3 or later](https://www.swi-prolog.org/) (default)
-- [Trealla Prolog 2.6.9 or later](https://github.com/trealla-prolog/trealla)
+- [Trealla Prolog 2.18.7 or later](https://github.com/trealla-prolog/trealla)
 - [YAP 7.2.1 or later](https://github.com/vscosta)
 
+Note that an online use of this kernel (instead of local) may be restricted to a subset of these backends (notably, due to some systems requiring commercial licenses).
+
 The kernel is implemented in a way that basically all functionality except the loading of configuration files can easily be overridden. This is especially useful for **extending the kernel for further Prolog backends** or running code with a different version of a backend. For further information about this, see [Configuration](#configuration).
 
 Also see the [JupyterLab Logtalk CodeMirror Extension](https://github.com/LogtalkDotOrg/jupyterlab-logtalk-codemirror-extension) for *syntax highlighting* of Logtalk code in JupyterLab (forked from the [JupyterLab Prolog CodeMirror Extension](https://github.com/hhu-stups/jupyterlab-prolog-codemirror-extension)).
 
 
 ## Prolog backend requirements
```

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_jupyter_kernel.egg-info/PKG-INFO` & `logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logtalk-jupyter-kernel
-Version: 0.2.0
+Version: 0.3.0
 Summary: Hercutalk - A Jupyter Kernel for Logtalk
 Author: Paulo Moura, Anne Brecklinghaus, Michael Leuschel, dgelessus
 License: Copyright (c) 2022-2023 Paulo Moura  
         Copyright (c) 2022 Anne Brecklinghaus, Michael Leuschel, dgelessus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -48,21 +48,23 @@
 
 This project is a fork of the [prolog-jupyter-kernel](https://github.com/hhu-stups/prolog-jupyter-kernel) project (developed by Anne Brecklinghaus in her Master's thesis at the University of Düsseldorf under the supervision of Michael Leuschel and Philipp Körner) and still under development. It includes back-ports of recent patches and improvements by Michael Leuschel, dgelessus, and Silas Kraume. Major changes are committed and more are expected. Furthermore, no liability is accepted for correctness and completeness (see the [LICENSE](LICENSE) file).
 
 
 ## Supported Prolog backends
 
 - [ECLiPSe 7.0 #57 or later](http://eclipseclp.org/)
-- [GNU Prolog 1.5.1 or later](http://www.gprolog.org/) (use git version until 1.5.1 is released)
-- [LVM 5.0.0 or later](https://graphstax.ai/)
+- [GNU Prolog 1.6.0 or later](http://www.gprolog.org/) (use git version until 1.6.0 is released)
+- [LVM 6.3.0 or later](https://permion.ai/)
 - [SICStus Prolog 4.5.1 or later](https://sicstus.sics.se/)
 - [SWI-Prolog 8.4.3 or later](https://www.swi-prolog.org/) (default)
-- [Trealla Prolog 2.6.9 or later](https://github.com/trealla-prolog/trealla)
+- [Trealla Prolog 2.18.7 or later](https://github.com/trealla-prolog/trealla)
 - [YAP 7.2.1 or later](https://github.com/vscosta)
 
+Note that an online use of this kernel (instead of local) may be restricted to a subset of these backends (notably, due to some systems requiring commercial licenses).
+
 The kernel is implemented in a way that basically all functionality except the loading of configuration files can easily be overridden. This is especially useful for **extending the kernel for further Prolog backends** or running code with a different version of a backend. For further information about this, see [Configuration](#configuration).
 
 Also see the [JupyterLab Logtalk CodeMirror Extension](https://github.com/LogtalkDotOrg/jupyterlab-logtalk-codemirror-extension) for *syntax highlighting* of Logtalk code in JupyterLab (forked from the [JupyterLab Prolog CodeMirror Extension](https://github.com/hhu-stups/jupyterlab-prolog-codemirror-extension)).
 
 
 ## Prolog backend requirements
```

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_jupyter_kernel.egg-info/SOURCES.txt` & `logtalk-jupyter-kernel-0.3.0/logtalk_jupyter_kernel.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,10 +24,8 @@
 logtalk_kernel/logtalk_server/jupyter_query_handling.lgt
 logtalk_kernel/logtalk_server/jupyter_request_handling.lgt
 logtalk_kernel/logtalk_server/jupyter_server.lgt
 logtalk_kernel/logtalk_server/jupyter_term_handling.lgt
 logtalk_kernel/logtalk_server/jupyter_variable_bindings.lgt
 logtalk_kernel/logtalk_server/loader.lgt
 notebooks/JupyterKernelForLogtalkOverview.ipynb
-notebooks/LogtalkTutorial.ipynb
-notebooks/architecture_diagram.png
-notebooks/user_interaction_diagram.png
+notebooks/LogtalkTutorial.ipynb
```

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/__init__.py` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/__main__.py` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/__main__.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/install.py` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/install.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/kernel.py` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/kernelspec/kernel.js` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/kernelspec/kernel.js`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_kernel_base_implementation.py` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_kernel_base_implementation.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_kernel_config.py` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_kernel_config.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter.lgt` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_jsonrpc.lgt` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_jsonrpc.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_logging.lgt` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_logging.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_preferences.lgt` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_preferences.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_query_handling.lgt` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_query_handling.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_request_handling.lgt` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_request_handling.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_server.lgt` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_server.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_term_handling.lgt` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_term_handling.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/jupyter_variable_bindings.lgt` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/jupyter_variable_bindings.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/logtalk_server/loader.lgt` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/logtalk_server/loader.lgt`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/sicstus_kernel_implementation.py` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/sicstus_kernel_implementation.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/logtalk_kernel/swi_kernel_implementation.py` & `logtalk-jupyter-kernel-0.3.0/logtalk_kernel/swi_kernel_implementation.py`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/notebooks/JupyterKernelForLogtalkOverview.ipynb` & `logtalk-jupyter-kernel-0.3.0/notebooks/JupyterKernelForLogtalkOverview.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998134190544905%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'data': {'text/plain': ['\\x1b[1mVersionData = "*

 * *            "logtalk(3,68,0,b02)']}}}}, 5: {'outputs': {1: {'data': {'text/plain': "*

 * *            "['\\x1b[1mVersion = v(9,1,11)']}}}}, 34: {'outputs': {0: {'data': {'text/plain': "*

 * *            "{insert: [(1, '   Call: (1) fred::number_of_legs(_24368)\\n'), (2, '   Call: (2) "*

 * *            "number_of_legs(_24368)\\n')], delete: [2, 1]}}}}}, 36: {'outputs': {0: {'data': "*

 * *            "{'text/plain': ['   Debugger tracing switche […]*

```diff
@@ -34,15 +34,15 @@
                     "languageId": "logtalk"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "\u001b[1mVersionData = logtalk(3,61,0,stable)"
+                            "\u001b[1mVersionData = logtalk(3,68,0,b02)"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
@@ -101,15 +101,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "\u001b[1mVersion = v(9,1,2)"
+                            "\u001b[1mVersion = v(9,1,11)"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
@@ -721,16 +721,16 @@
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "   Debugger switched on: tracing everything for all objects compiled in debug mode.\n",
-                            "   Call: (1) fred::number_of_legs(_15550)\n",
-                            "   Call: (2) number_of_legs(_15550)\n",
+                            "   Call: (1) fred::number_of_legs(_24368)\n",
+                            "   Call: (2) number_of_legs(_24368)\n",
                             "   Fact: (2) number_of_legs(4)\n",
                             "   Exit: (2) number_of_legs(4)\n",
                             "   Exit: (1) fred::number_of_legs(4)"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -766,15 +766,15 @@
                     "languageId": "logtalk"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "   Debugger switched off."
+                            "   Debugger tracing switched off."
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
@@ -810,37 +810,37 @@
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "% \n",
-                            "% tests started at 2022-12-21, 14:27:01\n",
+                            "% tests started at 2023-07-17, 10:08:41\n",
                             "% \n",
                             "% running tests from object tests\n",
                             "% file: /Users/pmoura/logtalk/examples/ack/tests.lgt\n",
                             "% \n",
-                            "% ack_1: success (in 0.0008719999999999839 seconds)\n",
-                            "% ack_2: success (in 0.1536439999999999 seconds)\n",
-                            "% ack_3: success (in 0.8019719999999999 seconds)\n",
+                            "% ack_1: success (in 0.001569000 seconds)\n",
+                            "% ack_2: success (in 0.055794000 seconds)\n",
+                            "% ack_3: success (in 0.238780000 seconds)\n",
                             "% \n",
                             "% 3 tests: 0 skipped, 3 passed, 0 failed (0 flaky)\n",
                             "% completed tests from object tests\n",
                             "% \n",
                             "% \n",
                             "% clause coverage ratio and covered clauses per entity predicate\n",
                             "% \n",
                             "% ack: ack/3 - 3/3 - (all)\n",
                             "% ack: 3 out of 3 clauses covered, 100.000000% coverage\n",
                             "% \n",
                             "% 1 entity declared as covered containing 3 clauses\n",
                             "% 1 out of 1 entity covered, 100.000000% entity coverage\n",
                             "% 3 out of 3 clauses covered, 100.000000% clause coverage\n",
                             "% \n",
-                            "% tests ended at 2022-12-21, 14:27:02\n",
+                            "% tests ended at 2023-07-17, 10:08:42\n",
                             "% "
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
@@ -1059,15 +1059,112 @@
                 "vscode": {
                     "languageId": "logtalk"
                 }
             },
             "outputs": [
                 {
                     "data": {
-                        "image/svg+xml": "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n<!-- Generated by graphviz version 7.0.1 (20221109.1506)\n -->\n<!-- Pages: 1 -->\n<svg width=\"216pt\" height=\"305pt\"\n viewBox=\"0.00 0.00 216.00 305.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 301)\">\n<polygon fill=\"white\" stroke=\"none\" points=\"-4,4 -4,-301 212,-301 212,4 -4,4\"/>\n<!-- 1 -->\n<g id=\"node1\" class=\"node\">\n<title>1</title>\n<ellipse fill=\"none\" stroke=\"black\" cx=\"27\" cy=\"-192\" rx=\"27\" ry=\"18\"/>\n<text text-anchor=\"middle\" x=\"27\" y=\"-188.3\" font-family=\"Times,serif\" font-size=\"14.00\">1</text>\n</g>\n<!-- 2 -->\n<g id=\"node2\" class=\"node\">\n<title>2</title>\n<ellipse fill=\"none\" stroke=\"black\" cx=\"73\" cy=\"-105\" rx=\"27\" ry=\"18\"/>\n<text text-anchor=\"middle\" x=\"73\" y=\"-101.3\" font-family=\"Times,serif\" font-size=\"14.00\">2</text>\n</g>\n<!-- 3 -->\n<g id=\"node3\" class=\"node\">\n<title>3</title>\n<ellipse fill=\"none\" stroke=\"black\" cx=\"109\" cy=\"-18\" rx=\"27\" ry=\"18\"/>\n<text text-anchor=\"middle\" x=\"109\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">3</text>\n</g>\n<!-- 4 -->\n<g id=\"node4\" class=\"node\">\n<title>4</title>\n<ellipse fill=\"none\" stroke=\"black\" cx=\"181\" cy=\"-18\" rx=\"27\" ry=\"18\"/>\n<text text-anchor=\"middle\" x=\"181\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">4</text>\n</g>\n<!-- a(1,b(2,c(3,4))) -->\n<g id=\"node5\" class=\"node\">\n<title>a(1,b(2,c(3,4)))</title>\n<polygon fill=\"none\" stroke=\"black\" points=\"79,-297 25,-297 25,-261 79,-261 79,-297\"/>\n<text text-anchor=\"middle\" x=\"52\" y=\"-275.3\" font-family=\"Times,serif\" font-size=\"14.00\">a</text>\n</g>\n<!-- a(1,b(2,c(3,4)))&#45;&gt;1 -->\n<g id=\"edge1\" class=\"edge\">\n<title>a(1,b(2,c(3,4)))&#45;&gt;1</title>\n<path fill=\"none\" stroke=\"black\" d=\"M46.94,-260.8C43.59,-249.39 39.11,-234.16 35.24,-221.03\"/>\n<polygon fill=\"black\" stroke=\"black\" points=\"38.66,-220.23 32.48,-211.63 31.94,-222.21 38.66,-220.23\"/>\n<text text-anchor=\"middle\" x=\"44.5\" y=\"-231.8\" font-family=\"Times,serif\" font-size=\"14.00\">1</text>\n</g>\n<!-- b(2,c(3,4)) -->\n<g id=\"node6\" class=\"node\">\n<title>b(2,c(3,4))</title>\n<polygon fill=\"none\" stroke=\"black\" points=\"126,-210 72,-210 72,-174 126,-174 126,-210\"/>\n<text text-anchor=\"middle\" x=\"99\" y=\"-188.3\" font-family=\"Times,serif\" font-size=\"14.00\">b</text>\n</g>\n<!-- a(1,b(2,c(3,4)))&#45;&gt;b(2,c(3,4)) -->\n<g id=\"edge2\" class=\"edge\">\n<title>a(1,b(2,c(3,4)))&#45;&gt;b(2,c(3,4))</title>\n<path fill=\"none\" stroke=\"black\" d=\"M61.51,-260.8C67.9,-249.24 76.47,-233.75 83.79,-220.5\"/>\n<polygon fill=\"black\" stroke=\"black\" points=\"86.83,-222.24 88.61,-211.79 80.71,-218.85 86.83,-222.24\"/>\n<text text-anchor=\"middle\" x=\"82.5\" y=\"-231.8\" font-family=\"Times,serif\" font-size=\"14.00\">2</text>\n</g>\n<!-- b(2,c(3,4))&#45;&gt;2 -->\n<g id=\"edge3\" class=\"edge\">\n<title>b(2,c(3,4))&#45;&gt;2</title>\n<path fill=\"none\" stroke=\"black\" d=\"M93.74,-173.8C90.23,-162.32 85.53,-146.96 81.49,-133.77\"/>\n<polygon fill=\"black\" stroke=\"black\" points=\"84.88,-132.87 78.61,-124.33 78.19,-134.92 84.88,-132.87\"/>\n<text text-anchor=\"middle\" x=\"91.5\" y=\"-144.8\" font-family=\"Times,serif\" font-size=\"14.00\">1</text>\n</g>\n<!-- c(3,4) -->\n<g id=\"node7\" class=\"node\">\n<title>c(3,4)</title>\n<polygon fill=\"none\" stroke=\"black\" points=\"172,-123 118,-123 118,-87 172,-87 172,-123\"/>\n<text text-anchor=\"middle\" x=\"145\" y=\"-101.3\" font-family=\"Times,serif\" font-size=\"14.00\">c</text>\n</g>\n<!-- b(2,c(3,4))&#45;&gt;c(3,4) -->\n<g id=\"edge4\" class=\"edge\">\n<title>b(2,c(3,4))&#45;&gt;c(3,4)</title>\n<path fill=\"none\" stroke=\"black\" d=\"M108.31,-173.8C114.56,-162.24 122.95,-146.75 130.12,-133.5\"/>\n<polygon fill=\"black\" stroke=\"black\" points=\"133.15,-135.26 134.83,-124.8 126.99,-131.93 133.15,-135.26\"/>\n<text text-anchor=\"middle\" x=\"127.5\" y=\"-144.8\" font-family=\"Times,serif\" font-size=\"14.00\">2</text>\n</g>\n<!-- c(3,4)&#45;&gt;3 -->\n<g id=\"edge5\" class=\"edge\">\n<title>c(3,4)&#45;&gt;3</title>\n<path fill=\"none\" stroke=\"black\" d=\"M137.71,-86.8C132.77,-75.13 126.13,-59.45 120.48,-46.11\"/>\n<polygon fill=\"black\" stroke=\"black\" points=\"123.74,-44.83 116.62,-36.99 117.3,-47.56 123.74,-44.83\"/>\n<text text-anchor=\"middle\" x=\"132.5\" y=\"-57.8\" font-family=\"Times,serif\" font-size=\"14.00\">1</text>\n</g>\n<!-- c(3,4)&#45;&gt;4 -->\n<g id=\"edge6\" class=\"edge\">\n<title>c(3,4)&#45;&gt;4</title>\n<path fill=\"none\" stroke=\"black\" d=\"M152.29,-86.8C157.23,-75.13 163.87,-59.45 169.52,-46.11\"/>\n<polygon fill=\"black\" stroke=\"black\" points=\"172.7,-47.56 173.38,-36.99 166.26,-44.83 172.7,-47.56\"/>\n<text text-anchor=\"middle\" x=\"168.5\" y=\"-57.8\" font-family=\"Times,serif\" font-size=\"14.00\">2</text>\n</g>\n</g>\n</svg>\n",
+                        "image/svg+xml": [
+                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
+                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
+                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
+                            "<!-- Generated by graphviz version 8.1.0 (20230707.0739)\n",
+                            " -->\n",
+                            "<!-- Pages: 1 -->\n",
+                            "<svg width=\"216pt\" height=\"310pt\"\n",
+                            " viewBox=\"0.00 0.00 216.00 309.50\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
+                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 305.5)\">\n",
+                            "<polygon fill=\"white\" stroke=\"none\" points=\"-4,4 -4,-305.5 212,-305.5 212,4 -4,4\"/>\n",
+                            "<!-- 1 -->\n",
+                            "<g id=\"node1\" class=\"node\">\n",
+                            "<title>1</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"27\" cy=\"-195\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"27\" y=\"-189.95\" font-family=\"Times,serif\" font-size=\"14.00\">1</text>\n",
+                            "</g>\n",
+                            "<!-- 2 -->\n",
+                            "<g id=\"node2\" class=\"node\">\n",
+                            "<title>2</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"73\" cy=\"-106.5\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"73\" y=\"-101.45\" font-family=\"Times,serif\" font-size=\"14.00\">2</text>\n",
+                            "</g>\n",
+                            "<!-- 3 -->\n",
+                            "<g id=\"node3\" class=\"node\">\n",
+                            "<title>3</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"109\" cy=\"-18\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"109\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">3</text>\n",
+                            "</g>\n",
+                            "<!-- 4 -->\n",
+                            "<g id=\"node4\" class=\"node\">\n",
+                            "<title>4</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"181\" cy=\"-18\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"181\" y=\"-12.95\" font-family=\"Times,serif\" font-size=\"14.00\">4</text>\n",
+                            "</g>\n",
+                            "<!-- a(1,b(2,c(3,4))) -->\n",
+                            "<g id=\"node5\" class=\"node\">\n",
+                            "<title>a(1,b(2,c(3,4)))</title>\n",
+                            "<polygon fill=\"none\" stroke=\"black\" points=\"69,-301.5 15,-301.5 15,-265.5 69,-265.5 69,-301.5\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"42\" y=\"-278.45\" font-family=\"Times,serif\" font-size=\"14.00\">a</text>\n",
+                            "</g>\n",
+                            "<!-- a(1,b(2,c(3,4)))&#45;&gt;1 -->\n",
+                            "<g id=\"edge1\" class=\"edge\">\n",
+                            "<title>a(1,b(2,c(3,4)))&#45;&gt;1</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M39.04,-265.41C37,-253.64 34.24,-237.73 31.87,-224.11\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"35.17,-223.61 30.01,-214.35 28.27,-224.8 35.17,-223.61\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"39.38\" y=\"-234.2\" font-family=\"Times,serif\" font-size=\"14.00\">1</text>\n",
+                            "</g>\n",
+                            "<!-- b(2,c(3,4)) -->\n",
+                            "<g id=\"node6\" class=\"node\">\n",
+                            "<title>b(2,c(3,4))</title>\n",
+                            "<polygon fill=\"none\" stroke=\"black\" points=\"126,-213 72,-213 72,-177 126,-177 126,-213\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"99\" y=\"-189.95\" font-family=\"Times,serif\" font-size=\"14.00\">b</text>\n",
+                            "</g>\n",
+                            "<!-- a(1,b(2,c(3,4)))&#45;&gt;b(2,c(3,4)) -->\n",
+                            "<g id=\"edge2\" class=\"edge\">\n",
+                            "<title>a(1,b(2,c(3,4)))&#45;&gt;b(2,c(3,4))</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M53.26,-265.41C61.33,-253.17 72.35,-236.45 81.55,-222.49\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"84.99,-224.63 87.57,-214.35 79.14,-220.77 84.99,-224.63\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"79.38\" y=\"-234.2\" font-family=\"Times,serif\" font-size=\"14.00\">2</text>\n",
+                            "</g>\n",
+                            "<!-- b(2,c(3,4))&#45;&gt;2 -->\n",
+                            "<g id=\"edge3\" class=\"edge\">\n",
+                            "<title>b(2,c(3,4))&#45;&gt;2</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M93.86,-176.91C90.27,-164.94 85.38,-148.7 81.25,-134.93\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"84.36,-134.12 78.13,-125.55 77.65,-136.14 84.36,-134.12\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"92.38\" y=\"-145.7\" font-family=\"Times,serif\" font-size=\"14.00\">1</text>\n",
+                            "</g>\n",
+                            "<!-- c(3,4) -->\n",
+                            "<g id=\"node7\" class=\"node\">\n",
+                            "<title>c(3,4)</title>\n",
+                            "<polygon fill=\"none\" stroke=\"black\" points=\"172,-124.5 118,-124.5 118,-88.5 172,-88.5 172,-124.5\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"145\" y=\"-101.45\" font-family=\"Times,serif\" font-size=\"14.00\">c</text>\n",
+                            "</g>\n",
+                            "<!-- b(2,c(3,4))&#45;&gt;c(3,4) -->\n",
+                            "<g id=\"edge4\" class=\"edge\">\n",
+                            "<title>b(2,c(3,4))&#45;&gt;c(3,4)</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M108.09,-176.91C114.54,-164.79 123.32,-148.27 130.7,-134.39\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"134.17,-136.32 135.77,-125.85 127.99,-133.04 134.17,-136.32\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"130.38\" y=\"-145.7\" font-family=\"Times,serif\" font-size=\"14.00\">2</text>\n",
+                            "</g>\n",
+                            "<!-- c(3,4)&#45;&gt;3 -->\n",
+                            "<g id=\"edge5\" class=\"edge\">\n",
+                            "<title>c(3,4)&#45;&gt;3</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M137.89,-88.41C132.83,-76.25 125.92,-59.66 120.14,-45.76\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"123.05,-44.65 115.98,-36.76 116.59,-47.34 123.05,-44.65\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"134.38\" y=\"-57.2\" font-family=\"Times,serif\" font-size=\"14.00\">1</text>\n",
+                            "</g>\n",
+                            "<!-- c(3,4)&#45;&gt;4 -->\n",
+                            "<g id=\"edge6\" class=\"edge\">\n",
+                            "<title>c(3,4)&#45;&gt;4</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M152.11,-88.41C157.17,-76.25 164.08,-59.66 169.86,-45.76\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"173.41,-47.34 174.02,-36.76 166.95,-44.65 173.41,-47.34\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"169.38\" y=\"-57.2\" font-family=\"Times,serif\" font-size=\"14.00\">2</text>\n",
+                            "</g>\n",
+                            "</g>\n",
+                            "</svg>\n"
+                        ],
                         "text/plain": [
                             "digraph {\n",
                             "\"1\" [shape=\"oval\", label=\"1\"]\n",
                             "\"2\" [shape=\"oval\", label=\"2\"]\n",
                             "\"3\" [shape=\"oval\", label=\"3\"]\n",
                             "\"4\" [shape=\"oval\", label=\"4\"]\n",
                             "\"a(1,b(2,c(3,4)))\" [shape=\"rect\", label=\"a\"]\n",
@@ -1376,31 +1473,28 @@
         },
         {
             "cell_type": "markdown",
             "id": "65ec5ff2",
             "metadata": {},
             "source": [
                 "- *Two-process model*:\n",
-                "<img style=\"float: right; max-width: 40%;\" src=\"user_interaction_diagram.png\">\n",
                 "\n",
                 "    - Client process: responsible for user interaction\n",
                 "    - Kernel process: handles code execution"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ad708ac3-8d47-4ee8-8171-7c786550c288",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "## Architecture\n",
                 "\n",
-                "<img style=\"max-width: 80%;\" src=\"architecture_diagram.png\">\n",
-                "\n",
                 "\n",
                 "\n",
                 "\n"
             ]
         },
         {
             "cell_type": "markdown",
@@ -1409,15 +1503,15 @@
                 "tags": []
             },
             "source": [
                 "Kernel split in three:\n",
                 "- Extends IPython kernel: **inherits** the communication with a frontend via the ZeroMQ protocol\n",
                 "\n",
                 "\n",
-                "- Does not interpret Prolog itself\n",
+                "- Does not interpret Logtalk itself\n",
                 "    - Starts an existing Logtalk instance in a **subprocess**\n",
                 "        - Communicates with it according to the JSON-RPC 2.0 protocol\n",
                 "    - For any code execution **request**:\n",
                 "        - Sends a request message to the Logtalk server containing the **code**\n",
                 "        - Terms are read from the code and handled\n",
                 "    \n",
                 "    \n",
@@ -1433,15 +1527,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8323263c",
             "metadata": {},
             "source": [
-                "## Changing the Prolog Implementation\n",
+                "## Changing the Prolog Backend\n",
                 "\n",
                 "- Switch between Prolog backends on the fly\n",
                 "- The previous server process is kept running\n",
                 "    - When switching back, the database state has not changed\n",
                 "\n",
                 "Several Prolog backends are supported and shortcuts are provided to switch to them if installed:\n",
                 "\n",
```

### Comparing `logtalk-jupyter-kernel-0.2.0/notebooks/LogtalkTutorial.ipynb` & `logtalk-jupyter-kernel-0.3.0/notebooks/LogtalkTutorial.ipynb`

 * *Files identical despite different names*

### Comparing `logtalk-jupyter-kernel-0.2.0/pyproject.toml` & `logtalk-jupyter-kernel-0.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=61.0"
 ]
 
 [project]
 name = "logtalk-jupyter-kernel"
-version = "0.2.0"
+version = "0.3.0"
 authors = [ {name="Paulo Moura"}, { name="Anne Brecklinghaus" }, { name="Michael Leuschel" }, { name="dgelessus" } ]
 description = "Hercutalk - A Jupyter Kernel for Logtalk"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
-	"Development Status :: 4 - Beta",
-	"Framework :: Jupyter",
+  "Development Status :: 4 - Beta",
+  "Framework :: Jupyter",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Intended Audience :: Developers",
-	"Intended Audience :: Education",
-	"Topic :: Scientific/Engineering",
-	"Topic :: System :: Shells",
-	"Natural Language :: English",
+  "Intended Audience :: Education",
+  "Topic :: Scientific/Engineering",
+  "Topic :: System :: Shells",
+  "Natural Language :: English",
 ]
 keywords = [
-	"logtalk",
-	"prolog",
-	"logic-programming",
+  "logtalk",
+  "prolog",
+  "logic-programming",
 ]
 dependencies = [
   "jupyter_client",
   "IPython",
   "ipykernel",
   "graphviz",
   "beautifulsoup4",
@@ -38,11 +38,11 @@
 
 [project.urls]
 "Source" = "https://github.com/LogtalkDotOrg/logtalk-jupyter-kernel"
 "Issues" = "https://github.com/LogtalkDotOrg/logtalk-jupyter-kernel/issues"
 
 [project.optional-dependencies]
 dev = [
-	"jupyter_core",
-	"jupyterlab",
-	"notebook",
+  "jupyter_core",
+  "jupyterlab",
+  "notebook",
 ]
```

