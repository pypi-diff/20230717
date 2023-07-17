# Comparing `tmp/sdof-0.0.6.tar.gz` & `tmp/sdof-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdof-0.0.6.tar", last modified: Sun Jul 16 22:48:27 2023, max compression
+gzip compressed data, was "sdof-0.0.7.tar", last modified: Mon Jul 17 01:21:08 2023, max compression
```

## Comparing `sdof-0.0.6.tar` & `sdof-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/
--rw-r--r--   0 claudio   (1001) claudio   (1001)       62 2023-02-10 17:50:46.000000 sdof-0.0.6/.gitignore
--rw-r--r--   0 claudio   (1001) claudio   (1001)      748 2023-07-16 22:46:57.000000 sdof-0.0.6/Makefile
--rw-r--r--   0 claudio   (1001) claudio   (1001)     6235 2023-07-16 22:48:26.996706 sdof-0.0.6/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)     5889 2023-07-16 22:46:27.000000 sdof-0.0.6/README.md
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/data/
--rw-r--r--   0 claudio   (1001) claudio   (1001)    16031 2022-04-04 01:35:00.000000 sdof-0.0.6/data/elCentro.AT2
--rw-r--r--   0 claudio   (1001) claudio   (1001)    17878 2022-04-04 01:36:22.000000 sdof-0.0.6/data/elCentro.txt
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/dist/
--rw-r--r--   0 claudio   (1001) claudio   (1001)   185034 2022-04-06 02:05:30.000000 sdof-0.0.6/dist/alpha.js
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)    16284 2022-04-06 02:05:30.000000 sdof-0.0.6/dist/alpha.wasm
--rw-r--r--   0 claudio   (1001) claudio   (1001)      718 2023-07-16 22:48:09.000000 sdof-0.0.6/pyproject.toml
--rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-07-16 22:48:26.996706 sdof-0.0.6/setup.cfg
--rw-r--r--   0 claudio   (1001) claudio   (1001)      203 2023-02-10 17:57:42.000000 sdof-0.0.6/setup.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/src/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3001 2023-01-09 19:17:41.000000 sdof-0.0.6/src/alpha.c
--rw-r--r--   0 claudio   (1001) claudio   (1001)     7687 2023-07-16 21:09:24.000000 sdof-0.0.6/src/fsdof.c
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2654 2022-04-06 02:09:45.000000 sdof-0.0.6/src/modal.c
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/src/sdof/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     5244 2023-07-16 22:47:36.000000 sdof-0.0.6/src/sdof/__init__.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1313 2023-07-16 22:46:57.000000 sdof-0.0.6/src/sdof/__main__.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/src/sdof.egg-info/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     6235 2023-07-16 22:48:26.000000 sdof-0.0.6/src/sdof.egg-info/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)      379 2023-07-16 22:48:26.000000 sdof-0.0.6/src/sdof.egg-info/SOURCES.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-07-16 22:48:26.000000 sdof-0.0.6/src/sdof.egg-info/dependency_links.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)       25 2023-07-16 22:48:26.000000 sdof-0.0.6/src/sdof.egg-info/top_level.txt
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/tests/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      966 2023-01-09 19:21:13.000000 sdof-0.0.6/tests/chopra.sh
--rw-r--r--   0 claudio   (1001) claudio   (1001)      975 2023-01-11 21:44:56.000000 sdof-0.0.6/tests/test.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3400 2023-07-16 05:13:02.000000 sdof-0.0.6/theory.md
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/wasm/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2305 2023-02-12 03:13:03.000000 sdof-0.0.6/wasm/index.js
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 01:21:08.806706 sdof-0.0.7/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       62 2023-02-10 17:50:46.000000 sdof-0.0.7/.gitignore
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      748 2023-07-16 22:46:57.000000 sdof-0.0.7/Makefile
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     6737 2023-07-17 01:21:08.806706 sdof-0.0.7/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     6325 2023-07-17 01:13:43.000000 sdof-0.0.7/README.md
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 01:21:08.806706 sdof-0.0.7/data/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)    16031 2022-04-04 01:35:00.000000 sdof-0.0.7/data/elCentro.AT2
+-rw-r--r--   0 claudio   (1001) claudio   (1001)    17878 2022-04-04 01:36:22.000000 sdof-0.0.7/data/elCentro.txt
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 01:21:08.806706 sdof-0.0.7/dist/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)   185034 2022-04-06 02:05:30.000000 sdof-0.0.7/dist/alpha.js
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    16284 2022-04-06 02:05:30.000000 sdof-0.0.7/dist/alpha.wasm
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      804 2023-07-17 01:20:58.000000 sdof-0.0.7/pyproject.toml
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-07-17 01:21:08.806706 sdof-0.0.7/setup.cfg
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      203 2023-02-10 17:57:42.000000 sdof-0.0.7/setup.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 01:21:08.806706 sdof-0.0.7/src/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3001 2023-01-09 19:17:41.000000 sdof-0.0.7/src/alpha.c
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     7687 2023-07-16 21:09:24.000000 sdof-0.0.7/src/fsdof.c
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2654 2022-04-06 02:09:45.000000 sdof-0.0.7/src/modal.c
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 01:21:08.806706 sdof-0.0.7/src/sdof/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     5232 2023-07-17 00:25:32.000000 sdof-0.0.7/src/sdof/__init__.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1313 2023-07-16 22:46:57.000000 sdof-0.0.7/src/sdof/__main__.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 01:21:08.806706 sdof-0.0.7/src/sdof.egg-info/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     6737 2023-07-17 01:21:08.000000 sdof-0.0.7/src/sdof.egg-info/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      379 2023-07-17 01:21:08.000000 sdof-0.0.7/src/sdof.egg-info/SOURCES.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-07-17 01:21:08.000000 sdof-0.0.7/src/sdof.egg-info/dependency_links.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       25 2023-07-17 01:21:08.000000 sdof-0.0.7/src/sdof.egg-info/top_level.txt
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 01:21:08.806706 sdof-0.0.7/tests/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      966 2023-01-09 19:21:13.000000 sdof-0.0.7/tests/chopra.sh
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      975 2023-01-11 21:44:56.000000 sdof-0.0.7/tests/test.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3400 2023-07-16 05:13:02.000000 sdof-0.0.7/theory.md
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 01:21:08.806706 sdof-0.0.7/wasm/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2305 2023-02-12 03:13:03.000000 sdof-0.0.7/wasm/index.js
```

### Comparing `sdof-0.0.6/Makefile` & `sdof-0.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/PKG-INFO` & `sdof-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 Metadata-Version: 2.1
 Name: sdof
-Version: 0.0.6
+Version: 0.0.7
 Summary: Lightning-fast integration of single degree-of-freedom systems.
-Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>
+Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>, Chrystal Chern <52893467+chrystalchern@users.noreply.github.com>
 Project-URL: repository, http://github.com/claudioperez/sdof
 Keywords: seismic,earthquake-engineering
 Description-Content-Type: text/markdown
 
 # `sdof`
 
+<img align="left" src="https://raw.githubusercontent.com/BRACE2/OpenSeesRT/master/docs/figures/spectrum.svg" width="250px" alt="PEER Logo">
+
 Lightning-fast integration of single degree-of-freedom systems.
 
+<br>
+
+<div style="align:center">
+
+[![Latest PyPI version](https://img.shields.io/pypi/v/sdof?logo=pypi&style=for-the-badge)](https://pypi.python.org/pypi/sdof)
+<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg?logo=npm&style=for-the-badge" alt="NPM version" /></a></span>
+
+</div>
+
+-------------------------------------------------
+
 This package solves scalar differential equations of the form
 
 $$
 m \ddot{u} + c \dot{u} + k u = f(t)
 $$
 
 Integration is carried out using a Generalized - $\alpha$ integrator that
@@ -23,36 +36,36 @@
 Generalized - $\alpha$ is an implicit method that allows for high frequency energy
 dissipation and second order accuracy. With the right selection of parameters,
 the method can be specialized to the Hibert-Hughes-Taylor (HHT), or Newmark
 families of integration schemes.
 
 <hr />
 
-<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg" alt="NPM version" /></a></span>
 
 
 ## Python API
 
 ```python
+import numpy as np
 from sdof import integrate, peaks, spectrum
 
 m  = 1.0
 c  = 1.0
 k  = 2.0
 f  = np.sin(np.linspace(0, 5*np.pi, 100))
 dt = 5*np.pi/100
 
 u_max, v_max, a_max =  peaks(m, c, k, f, dt)
 
-u, v, a    = integrate(m, c, k, f, dt)
+u, v, a = integrate(m, c, k, f, dt)
 
-Su, Sv, Sa =  spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02, 3.0, 100))
+D, V, A =  spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02, 3.0, 100))
 ```
 
-## Integrator (Reproduced from OpenSees docs)
+## Integrator (Adapted from OpenSees docs)
 
 <table>
 <tbody>
 <tr class="odd">
 <td><p><code class="parameter-table-variable">alphaM</code></p></td>
 <td><p>$\alpha_M$ factor</p></td>
 </tr>
@@ -122,67 +135,65 @@
 increase the amount of numerical damping present without degrading the order of
 accuracy. In the HHT method, the same Newmark approximations are used:
 
 <dl>
 <dt></dt>
 <dd>
 
-$$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta)
-\Delta t^2] \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
+$$u_{t+\Delta t} = u_t + \Delta t \dot u_t + [(0.5 - \beta)
+\Delta t^2] \ddot u_t + [\beta \Delta t^2] \ddot u_{t+\Delta t}$$
 
 </dd>
 </dl>
 <dl>
 <dt></dt>
 <dd>
 
-$$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot
-U_t + [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
+$$\dot u_{t+\Delta t} = \dot u_t + [(1-\gamma)\Delta t] \ddot
+u_t + [\gamma \Delta t ] \ddot u_{t+\Delta t} $$
 
 </dd>
 </dl>
 <p>but the time-discrete momentum equation is modified:</p>
 
-$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot
-U_{t + \alpha_M \Delta t} - C \dot U_{t+\alpha_F \Delta t} -
-F^{int}(U_{t + \alpha_F \Delta t})
+$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{\mathrm{ext}} - M \ddot
+u_{t + \alpha_M \Delta t} - C \dot u_{t+\alpha_F \Delta t} -
+F^{\mathrm{int}}(u_{t + \alpha_F \Delta t})
 $$
 
 where the displacements and velocities at the intermediate point are
 given by:
 
-$$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F
-U_{t + \Delta t}$$
+$$u_{t+ \alpha_F \Delta t} = (1 - \alpha_F) u_t + \alpha_F
+u_{t + \Delta t}$$
 
-$$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t +
-\alpha_F \dot U_{t + \Delta t}$$
+$$\dot u_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot u_t +
+\alpha_F \dot u_{t + \Delta t}$$
 
-$$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
-\alpha_M \ddot U_{t + \Delta t}$$
+$$\ddot u_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot u_t +
+\alpha_M \ddot u_{t + \Delta t}$$
 
 <p>Following the methods outlined for Newmarks method, linearization of
 the nonlinear momentum equation results in the following linear
 equations:</p>
 
-$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta
+$$K_{t+\Delta t}^{*i} d u_{t+\Delta t}^{i+1} = R_{t+\Delta
 t}^i$$
 
-$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \frac{\alpha_F
-\gamma}{\beta \Delta t} C_t + \frac{\alpha_M}{\beta \Delta t^2}
-M$$
+$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \alpha_F \frac{\gamma}{\beta \Delta t} C_t + \alpha_M\frac{1}{\beta \Delta t^2}M$$
 
 <p>and</p>
 
-$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha
-F \Delta t}^{i-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M
-\ddot U_{t+ \alpha M \Delta t}^{i-1}$$
+$$R_{t+\Delta t}^i = F_{t + \Delta t}^{\mathrm{ext}} - F(u_{t + \alpha
+F \Delta t}^{i-1})^{\mathrm{int}} - C \dot u_{t+\alpha F \Delta t}^{i-1} - M
+\ddot u_{t+ \alpha M \Delta t}^{i-1}$$
 
 The linear equations are used to solve for 
 
-$$U_{t+\alpha_F \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$
+$$u_{t+\alpha_F \Delta t}, \dot u_{t + \alpha_F \Delta t} \ddot u_{t+ \alpha M \Delta t}$$
 
 Once convergence has been achieved the displacements,
 velocities and accelerations at time $t + \Delta t$ can be computed.
 
 ## Compiling
 
 The main integrator is implemented in standard C and can be compiled
```

#### html2text {}

```diff
@@ -1,26 +1,30 @@
-Metadata-Version: 2.1 Name: sdof Version: 0.0.6 Summary: Lightning-fast
+Metadata-Version: 2.1 Name: sdof Version: 0.0.7 Summary: Lightning-fast
 integration of single degree-of-freedom systems. Author-email: "Claudio M.
-Perez" <50180406+claudioperez@users.noreply.github.com> Project-URL:
-repository, http://github.com/claudioperez/sdof Keywords: seismic,earthquake-
-engineering Description-Content-Type: text/markdown # `sdof` Lightning-fast
-integration of single degree-of-freedom systems. This package solves scalar
+Perez" <50180406+claudioperez@users.noreply.github.com>, Chrystal Chern
+<52893467+chrystalchern@users.noreply.github.com> Project-URL: repository,
+http://github.com/claudioperez/sdof Keywords: seismic,earthquake-engineering
+Description-Content-Type: text/markdown # `sdof` [PEER Logo] Lightning-fast
+integration of single degree-of-freedom systems.
+[![Latest PyPI version](https://img.shields.io/pypi/v/sdof?logo=pypi&style=for-
+the-badge)](https://pypi.python.org/pypi/sdof) [NPM_version]
+------------------------------------------------- This package solves scalar
 differential equations of the form $$ m \ddot{u} + c \dot{u} + k u = f(t) $$
 Integration is carried out using a Generalized - $\alpha$ integrator that is
 implemented under the hood in highly optimized multi-threaded C code.
 Generalized - $\alpha$ is an implicit method that allows for high frequency
 energy dissipation and second order accuracy. With the right selection of
 parameters, the method can be specialized to the Hibert-Hughes-Taylor (HHT), or
 Newmark families of integration schemes.
 ===============================================================================
-[NPM_version] ## Python API ```python from sdof import integrate, peaks,
+## Python API ```python import numpy as np from sdof import integrate, peaks,
 spectrum m = 1.0 c = 1.0 k = 2.0 f = np.sin(np.linspace(0, 5*np.pi, 100)) dt =
 5*np.pi/100 u_max, v_max, a_max = peaks(m, c, k, f, dt) u, v, a = integrate(m,
-c, k, f, dt) Su, Sv, Sa = spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02,
-3.0, 100)) ``` ## Integrator (Reproduced from OpenSees docs)
+c, k, f, dt) D, V, A = spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02,
+3.0, 100)) ``` ## Integrator (Adapted from OpenSees docs)
 alphaM $\alpha_M$ factor
 alphaF $\alpha_F$ factor
 gamma  $\gamma$ factor
 beta   $\beta$ factor
    1. $\alpha_F$ and $\alpha_M$ are defined differently that in the paper, we
       use $\alpha_F = (1-\alpha_f)$ and $\alpha_M=(1-\gamma_m)$ where
       $\alpha_f$ and $\alpha_m$ are those used in the paper.
@@ -44,43 +48,44 @@
       $$\gamma = \dfrac{1}{2} + \gamma_M - \gamma_F$$
 and
       $$\beta = \dfrac{1}{4}(1 + \gamma_M - \gamma_F)^2$$
 ### Theory The generalized $\alpha$ method is a one step implicit method for
 solving the transient problem which attempts to increase the amount of
 numerical damping present without degrading the order of accuracy. In the HHT
 method, the same Newmark approximations are used:
-      $$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta) \Delta t^2]
-      \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
-      $$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot U_t +
-      [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
+      $$u_{t+\Delta t} = u_t + \Delta t \dot u_t + [(0.5 - \beta) \Delta t^2]
+      \ddot u_t + [\beta \Delta t^2] \ddot u_{t+\Delta t}$$
+      $$\dot u_{t+\Delta t} = \dot u_t + [(1-\gamma)\Delta t] \ddot u_t +
+      [\gamma \Delta t ] \ddot u_{t+\Delta t} $$
 but the time-discrete momentum equation is modified:
-$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot U_{t + \alpha_M
-\Delta t} - C \dot U_{t+\alpha_F \Delta t} - F^{int}(U_{t + \alpha_F \Delta t})
-$$ where the displacements and velocities at the intermediate point are given
-by: $$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F U_{t + \Delta
-t}$$ $$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t + \alpha_F \dot U_
-{t + \Delta t}$$ $$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
-\alpha_M \ddot U_{t + \Delta t}$$
+$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{\mathrm{ext}} - M \ddot u_{t +
+\alpha_M \Delta t} - C \dot u_{t+\alpha_F \Delta t} - F^{\mathrm{int}}(u_{t +
+\alpha_F \Delta t}) $$ where the displacements and velocities at the
+intermediate point are given by: $$u_{t+ \alpha_F \Delta t} = (1 - \alpha_F)
+u_t + \alpha_F u_{t + \Delta t}$$ $$\dot u_{t+\alpha_F \Delta t} = (1-\alpha_F)
+\dot u_t + \alpha_F \dot u_{t + \Delta t}$$ $$\ddot u_{t+\alpha_M \Delta t} =
+(1-\alpha_M) \ddot u_t + \alpha_M \ddot u_{t + \Delta t}$$
 Following the methods outlined for Newmarks method, linearization of the
 nonlinear momentum equation results in the following linear equations:
-$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta t}^i$$ $$K_{t+\Delta
-t}^{*i} = \alpha_F K_t + \frac{\alpha_F \gamma}{\beta \Delta t} C_t + \frac
-{\alpha_M}{\beta \Delta t^2} M$$
+$$K_{t+\Delta t}^{*i} d u_{t+\Delta t}^{i+1} = R_{t+\Delta t}^i$$ $$K_{t+\Delta
+t}^{*i} = \alpha_F K_t + \alpha_F \frac{\gamma}{\beta \Delta t} C_t +
+\alpha_M\frac{1}{\beta \Delta t^2}M$$
 and
-$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha F \Delta t}^{i-
-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M \ddot U_{t+ \alpha M
-\Delta t}^{i-1}$$ The linear equations are used to solve for $$U_{t+\alpha_F
-\Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$ Once
-convergence has been achieved the displacements, velocities and accelerations
-at time $t + \Delta t$ can be computed. ## Compiling The main integrator is
-implemented in standard C and can be compiled as either a Python extension, or
-Javascript library (via WASM). ### Python ``` pip install . ``` ### Javascript
-- Install `emscripten` from [here](https://emscripten.org/) - run `make`. This
-creates the following files: - `dist/fsdof.wasm` - Web assembly - compiled
-library, - `dist/fsdof.js` - interface to binary `fsdof.wasm` - to test, you
-can use Python to start an HTTP server in the current directory as follows:
-```shell python -m http.server . ``` ## References
+$$R_{t+\Delta t}^i = F_{t + \Delta t}^{\mathrm{ext}} - F(u_{t + \alpha F \Delta
+t}^{i-1})^{\mathrm{int}} - C \dot u_{t+\alpha F \Delta t}^{i-1} - M \ddot u_{t+
+\alpha M \Delta t}^{i-1}$$ The linear equations are used to solve for $$u_
+{t+\alpha_F \Delta t}, \dot u_{t + \alpha_F \Delta t} \ddot u_{t+ \alpha M
+\Delta t}$$ Once convergence has been achieved the displacements, velocities
+and accelerations at time $t + \Delta t$ can be computed. ## Compiling The main
+integrator is implemented in standard C and can be compiled as either a Python
+extension, or Javascript library (via WASM). ### Python ``` pip install . ```
+### Javascript - Install `emscripten` from [here](https://emscripten.org/) -
+run `make`. This creates the following files: - `dist/fsdof.wasm` - Web
+assembly - compiled library, - `dist/fsdof.js` - interface to binary
+`fsdof.wasm` - to test, you can use Python to start an HTTP server in the
+current directory as follows: ```shell python -m http.server . ``` ##
+References
 J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural Dynamics
 with Improved Numerical Dissipation: The Generalized - $\alpha$ Method" ASME
 Journal of Applied Mechanics, 60, 371:375, 1993.
 ===============================================================================
 Code Developed by: fmk
```

### Comparing `sdof-0.0.6/README.md` & `sdof-0.0.7/src/sdof.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,33 @@
+Metadata-Version: 2.1
+Name: sdof
+Version: 0.0.7
+Summary: Lightning-fast integration of single degree-of-freedom systems.
+Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>, Chrystal Chern <52893467+chrystalchern@users.noreply.github.com>
+Project-URL: repository, http://github.com/claudioperez/sdof
+Keywords: seismic,earthquake-engineering
+Description-Content-Type: text/markdown
+
 # `sdof`
 
+<img align="left" src="https://raw.githubusercontent.com/BRACE2/OpenSeesRT/master/docs/figures/spectrum.svg" width="250px" alt="PEER Logo">
+
 Lightning-fast integration of single degree-of-freedom systems.
 
+<br>
+
+<div style="align:center">
+
+[![Latest PyPI version](https://img.shields.io/pypi/v/sdof?logo=pypi&style=for-the-badge)](https://pypi.python.org/pypi/sdof)
+<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg?logo=npm&style=for-the-badge" alt="NPM version" /></a></span>
+
+</div>
+
+-------------------------------------------------
+
 This package solves scalar differential equations of the form
 
 $$
 m \ddot{u} + c \dot{u} + k u = f(t)
 $$
 
 Integration is carried out using a Generalized - $\alpha$ integrator that
@@ -14,36 +36,36 @@
 Generalized - $\alpha$ is an implicit method that allows for high frequency energy
 dissipation and second order accuracy. With the right selection of parameters,
 the method can be specialized to the Hibert-Hughes-Taylor (HHT), or Newmark
 families of integration schemes.
 
 <hr />
 
-<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg" alt="NPM version" /></a></span>
 
 
 ## Python API
 
 ```python
+import numpy as np
 from sdof import integrate, peaks, spectrum
 
 m  = 1.0
 c  = 1.0
 k  = 2.0
 f  = np.sin(np.linspace(0, 5*np.pi, 100))
 dt = 5*np.pi/100
 
 u_max, v_max, a_max =  peaks(m, c, k, f, dt)
 
-u, v, a    = integrate(m, c, k, f, dt)
+u, v, a = integrate(m, c, k, f, dt)
 
-Su, Sv, Sa =  spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02, 3.0, 100))
+D, V, A =  spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02, 3.0, 100))
 ```
 
-## Integrator (Reproduced from OpenSees docs)
+## Integrator (Adapted from OpenSees docs)
 
 <table>
 <tbody>
 <tr class="odd">
 <td><p><code class="parameter-table-variable">alphaM</code></p></td>
 <td><p>$\alpha_M$ factor</p></td>
 </tr>
@@ -113,67 +135,65 @@
 increase the amount of numerical damping present without degrading the order of
 accuracy. In the HHT method, the same Newmark approximations are used:
 
 <dl>
 <dt></dt>
 <dd>
 
-$$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta)
-\Delta t^2] \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
+$$u_{t+\Delta t} = u_t + \Delta t \dot u_t + [(0.5 - \beta)
+\Delta t^2] \ddot u_t + [\beta \Delta t^2] \ddot u_{t+\Delta t}$$
 
 </dd>
 </dl>
 <dl>
 <dt></dt>
 <dd>
 
-$$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot
-U_t + [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
+$$\dot u_{t+\Delta t} = \dot u_t + [(1-\gamma)\Delta t] \ddot
+u_t + [\gamma \Delta t ] \ddot u_{t+\Delta t} $$
 
 </dd>
 </dl>
 <p>but the time-discrete momentum equation is modified:</p>
 
-$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot
-U_{t + \alpha_M \Delta t} - C \dot U_{t+\alpha_F \Delta t} -
-F^{int}(U_{t + \alpha_F \Delta t})
+$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{\mathrm{ext}} - M \ddot
+u_{t + \alpha_M \Delta t} - C \dot u_{t+\alpha_F \Delta t} -
+F^{\mathrm{int}}(u_{t + \alpha_F \Delta t})
 $$
 
 where the displacements and velocities at the intermediate point are
 given by:
 
-$$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F
-U_{t + \Delta t}$$
+$$u_{t+ \alpha_F \Delta t} = (1 - \alpha_F) u_t + \alpha_F
+u_{t + \Delta t}$$
 
-$$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t +
-\alpha_F \dot U_{t + \Delta t}$$
+$$\dot u_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot u_t +
+\alpha_F \dot u_{t + \Delta t}$$
 
-$$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
-\alpha_M \ddot U_{t + \Delta t}$$
+$$\ddot u_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot u_t +
+\alpha_M \ddot u_{t + \Delta t}$$
 
 <p>Following the methods outlined for Newmarks method, linearization of
 the nonlinear momentum equation results in the following linear
 equations:</p>
 
-$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta
+$$K_{t+\Delta t}^{*i} d u_{t+\Delta t}^{i+1} = R_{t+\Delta
 t}^i$$
 
-$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \frac{\alpha_F
-\gamma}{\beta \Delta t} C_t + \frac{\alpha_M}{\beta \Delta t^2}
-M$$
+$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \alpha_F \frac{\gamma}{\beta \Delta t} C_t + \alpha_M\frac{1}{\beta \Delta t^2}M$$
 
 <p>and</p>
 
-$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha
-F \Delta t}^{i-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M
-\ddot U_{t+ \alpha M \Delta t}^{i-1}$$
+$$R_{t+\Delta t}^i = F_{t + \Delta t}^{\mathrm{ext}} - F(u_{t + \alpha
+F \Delta t}^{i-1})^{\mathrm{int}} - C \dot u_{t+\alpha F \Delta t}^{i-1} - M
+\ddot u_{t+ \alpha M \Delta t}^{i-1}$$
 
 The linear equations are used to solve for 
 
-$$U_{t+\alpha_F \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$
+$$u_{t+\alpha_F \Delta t}, \dot u_{t + \alpha_F \Delta t} \ddot u_{t+ \alpha M \Delta t}$$
 
 Once convergence has been achieved the displacements,
 velocities and accelerations at time $t + \Delta t$ can be computed.
 
 ## Compiling
 
 The main integrator is implemented in standard C and can be compiled
```

#### html2text {}

```diff
@@ -1,21 +1,30 @@
-# `sdof` Lightning-fast integration of single degree-of-freedom systems. This
-package solves scalar differential equations of the form $$ m \ddot{u} + c \dot
-{u} + k u = f(t) $$ Integration is carried out using a Generalized - $\alpha$
-integrator that is implemented under the hood in highly optimized multi-
-threaded C code. Generalized - $\alpha$ is an implicit method that allows for
-high frequency energy dissipation and second order accuracy. With the right
-selection of parameters, the method can be specialized to the Hibert-Hughes-
-Taylor (HHT), or Newmark families of integration schemes.
+Metadata-Version: 2.1 Name: sdof Version: 0.0.7 Summary: Lightning-fast
+integration of single degree-of-freedom systems. Author-email: "Claudio M.
+Perez" <50180406+claudioperez@users.noreply.github.com>, Chrystal Chern
+<52893467+chrystalchern@users.noreply.github.com> Project-URL: repository,
+http://github.com/claudioperez/sdof Keywords: seismic,earthquake-engineering
+Description-Content-Type: text/markdown # `sdof` [PEER Logo] Lightning-fast
+integration of single degree-of-freedom systems.
+[![Latest PyPI version](https://img.shields.io/pypi/v/sdof?logo=pypi&style=for-
+the-badge)](https://pypi.python.org/pypi/sdof) [NPM_version]
+------------------------------------------------- This package solves scalar
+differential equations of the form $$ m \ddot{u} + c \dot{u} + k u = f(t) $$
+Integration is carried out using a Generalized - $\alpha$ integrator that is
+implemented under the hood in highly optimized multi-threaded C code.
+Generalized - $\alpha$ is an implicit method that allows for high frequency
+energy dissipation and second order accuracy. With the right selection of
+parameters, the method can be specialized to the Hibert-Hughes-Taylor (HHT), or
+Newmark families of integration schemes.
 ===============================================================================
-[NPM_version] ## Python API ```python from sdof import integrate, peaks,
+## Python API ```python import numpy as np from sdof import integrate, peaks,
 spectrum m = 1.0 c = 1.0 k = 2.0 f = np.sin(np.linspace(0, 5*np.pi, 100)) dt =
 5*np.pi/100 u_max, v_max, a_max = peaks(m, c, k, f, dt) u, v, a = integrate(m,
-c, k, f, dt) Su, Sv, Sa = spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02,
-3.0, 100)) ``` ## Integrator (Reproduced from OpenSees docs)
+c, k, f, dt) D, V, A = spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02,
+3.0, 100)) ``` ## Integrator (Adapted from OpenSees docs)
 alphaM $\alpha_M$ factor
 alphaF $\alpha_F$ factor
 gamma  $\gamma$ factor
 beta   $\beta$ factor
    1. $\alpha_F$ and $\alpha_M$ are defined differently that in the paper, we
       use $\alpha_F = (1-\alpha_f)$ and $\alpha_M=(1-\gamma_m)$ where
       $\alpha_f$ and $\alpha_m$ are those used in the paper.
@@ -39,43 +48,44 @@
       $$\gamma = \dfrac{1}{2} + \gamma_M - \gamma_F$$
 and
       $$\beta = \dfrac{1}{4}(1 + \gamma_M - \gamma_F)^2$$
 ### Theory The generalized $\alpha$ method is a one step implicit method for
 solving the transient problem which attempts to increase the amount of
 numerical damping present without degrading the order of accuracy. In the HHT
 method, the same Newmark approximations are used:
-      $$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta) \Delta t^2]
-      \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
-      $$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot U_t +
-      [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
+      $$u_{t+\Delta t} = u_t + \Delta t \dot u_t + [(0.5 - \beta) \Delta t^2]
+      \ddot u_t + [\beta \Delta t^2] \ddot u_{t+\Delta t}$$
+      $$\dot u_{t+\Delta t} = \dot u_t + [(1-\gamma)\Delta t] \ddot u_t +
+      [\gamma \Delta t ] \ddot u_{t+\Delta t} $$
 but the time-discrete momentum equation is modified:
-$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot U_{t + \alpha_M
-\Delta t} - C \dot U_{t+\alpha_F \Delta t} - F^{int}(U_{t + \alpha_F \Delta t})
-$$ where the displacements and velocities at the intermediate point are given
-by: $$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F U_{t + \Delta
-t}$$ $$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t + \alpha_F \dot U_
-{t + \Delta t}$$ $$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
-\alpha_M \ddot U_{t + \Delta t}$$
+$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{\mathrm{ext}} - M \ddot u_{t +
+\alpha_M \Delta t} - C \dot u_{t+\alpha_F \Delta t} - F^{\mathrm{int}}(u_{t +
+\alpha_F \Delta t}) $$ where the displacements and velocities at the
+intermediate point are given by: $$u_{t+ \alpha_F \Delta t} = (1 - \alpha_F)
+u_t + \alpha_F u_{t + \Delta t}$$ $$\dot u_{t+\alpha_F \Delta t} = (1-\alpha_F)
+\dot u_t + \alpha_F \dot u_{t + \Delta t}$$ $$\ddot u_{t+\alpha_M \Delta t} =
+(1-\alpha_M) \ddot u_t + \alpha_M \ddot u_{t + \Delta t}$$
 Following the methods outlined for Newmarks method, linearization of the
 nonlinear momentum equation results in the following linear equations:
-$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta t}^i$$ $$K_{t+\Delta
-t}^{*i} = \alpha_F K_t + \frac{\alpha_F \gamma}{\beta \Delta t} C_t + \frac
-{\alpha_M}{\beta \Delta t^2} M$$
+$$K_{t+\Delta t}^{*i} d u_{t+\Delta t}^{i+1} = R_{t+\Delta t}^i$$ $$K_{t+\Delta
+t}^{*i} = \alpha_F K_t + \alpha_F \frac{\gamma}{\beta \Delta t} C_t +
+\alpha_M\frac{1}{\beta \Delta t^2}M$$
 and
-$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha F \Delta t}^{i-
-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M \ddot U_{t+ \alpha M
-\Delta t}^{i-1}$$ The linear equations are used to solve for $$U_{t+\alpha_F
-\Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$ Once
-convergence has been achieved the displacements, velocities and accelerations
-at time $t + \Delta t$ can be computed. ## Compiling The main integrator is
-implemented in standard C and can be compiled as either a Python extension, or
-Javascript library (via WASM). ### Python ``` pip install . ``` ### Javascript
-- Install `emscripten` from [here](https://emscripten.org/) - run `make`. This
-creates the following files: - `dist/fsdof.wasm` - Web assembly - compiled
-library, - `dist/fsdof.js` - interface to binary `fsdof.wasm` - to test, you
-can use Python to start an HTTP server in the current directory as follows:
-```shell python -m http.server . ``` ## References
+$$R_{t+\Delta t}^i = F_{t + \Delta t}^{\mathrm{ext}} - F(u_{t + \alpha F \Delta
+t}^{i-1})^{\mathrm{int}} - C \dot u_{t+\alpha F \Delta t}^{i-1} - M \ddot u_{t+
+\alpha M \Delta t}^{i-1}$$ The linear equations are used to solve for $$u_
+{t+\alpha_F \Delta t}, \dot u_{t + \alpha_F \Delta t} \ddot u_{t+ \alpha M
+\Delta t}$$ Once convergence has been achieved the displacements, velocities
+and accelerations at time $t + \Delta t$ can be computed. ## Compiling The main
+integrator is implemented in standard C and can be compiled as either a Python
+extension, or Javascript library (via WASM). ### Python ``` pip install . ```
+### Javascript - Install `emscripten` from [here](https://emscripten.org/) -
+run `make`. This creates the following files: - `dist/fsdof.wasm` - Web
+assembly - compiled library, - `dist/fsdof.js` - interface to binary
+`fsdof.wasm` - to test, you can use Python to start an HTTP server in the
+current directory as follows: ```shell python -m http.server . ``` ##
+References
 J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural Dynamics
 with Improved Numerical Dissipation: The Generalized - $\alpha$ Method" ASME
 Journal of Applied Mechanics, 60, 371:375, 1993.
 ===============================================================================
 Code Developed by: fmk
```

### Comparing `sdof-0.0.6/data/elCentro.AT2` & `sdof-0.0.7/data/elCentro.AT2`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/data/elCentro.txt` & `sdof-0.0.7/data/elCentro.txt`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/dist/alpha.js` & `sdof-0.0.7/dist/alpha.js`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/dist/alpha.wasm` & `sdof-0.0.7/dist/alpha.wasm`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/pyproject.toml` & `sdof-0.0.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [project]
 name = "sdof"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
-  {name="Claudio M. Perez", email="50180406+claudioperez@users.noreply.github.com"}
+  {name="Claudio M. Perez", email="50180406+claudioperez@users.noreply.github.com"},
+  {name="Chrystal Chern",   email="52893467+chrystalchern@users.noreply.github.com"}
 ]
 
 description="Lightning-fast integration of single degree-of-freedom systems."
 readme = "README.md"
 
 keywords = [
   "seismic",
```

### Comparing `sdof-0.0.6/src/alpha.c` & `sdof-0.0.7/src/alpha.c`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/src/fsdof.c` & `sdof-0.0.7/src/fsdof.c`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/src/modal.c` & `sdof-0.0.7/src/modal.c`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/src/sdof/__init__.py` & `sdof-0.0.7/src/sdof/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 beta   =beta,
                 gamma  =gamma
     )
 
     _fsdof_integrate2(CONFIG, m, c, k, 1.0, len(f), np.asarray(f).ctypes.data_as(POINTER(c_double)), dt, output)
     return output.T
 
-<<<<<<< HEAD
+
 
 def _thread_spectrum(n_threads=1):
     import threading
     threads = []
     for i in range(n_threads):
         threads.append(
                 threading.Thread(
```

### Comparing `sdof-0.0.6/src/sdof/__main__.py` & `sdof-0.0.7/src/sdof/__main__.py`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/src/sdof.egg-info/PKG-INFO` & `sdof-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-Metadata-Version: 2.1
-Name: sdof
-Version: 0.0.6
-Summary: Lightning-fast integration of single degree-of-freedom systems.
-Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>
-Project-URL: repository, http://github.com/claudioperez/sdof
-Keywords: seismic,earthquake-engineering
-Description-Content-Type: text/markdown
-
 # `sdof`
 
+<img align="left" src="https://raw.githubusercontent.com/BRACE2/OpenSeesRT/master/docs/figures/spectrum.svg" width="250px" alt="PEER Logo">
+
 Lightning-fast integration of single degree-of-freedom systems.
 
+<br>
+
+<div style="align:center">
+
+[![Latest PyPI version](https://img.shields.io/pypi/v/sdof?logo=pypi&style=for-the-badge)](https://pypi.python.org/pypi/sdof)
+<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg?logo=npm&style=for-the-badge" alt="NPM version" /></a></span>
+
+</div>
+
+-------------------------------------------------
+
 This package solves scalar differential equations of the form
 
 $$
 m \ddot{u} + c \dot{u} + k u = f(t)
 $$
 
 Integration is carried out using a Generalized - $\alpha$ integrator that
@@ -23,36 +27,36 @@
 Generalized - $\alpha$ is an implicit method that allows for high frequency energy
 dissipation and second order accuracy. With the right selection of parameters,
 the method can be specialized to the Hibert-Hughes-Taylor (HHT), or Newmark
 families of integration schemes.
 
 <hr />
 
-<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg" alt="NPM version" /></a></span>
 
 
 ## Python API
 
 ```python
+import numpy as np
 from sdof import integrate, peaks, spectrum
 
 m  = 1.0
 c  = 1.0
 k  = 2.0
 f  = np.sin(np.linspace(0, 5*np.pi, 100))
 dt = 5*np.pi/100
 
 u_max, v_max, a_max =  peaks(m, c, k, f, dt)
 
-u, v, a    = integrate(m, c, k, f, dt)
+u, v, a = integrate(m, c, k, f, dt)
 
-Su, Sv, Sa =  spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02, 3.0, 100))
+D, V, A =  spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02, 3.0, 100))
 ```
 
-## Integrator (Reproduced from OpenSees docs)
+## Integrator (Adapted from OpenSees docs)
 
 <table>
 <tbody>
 <tr class="odd">
 <td><p><code class="parameter-table-variable">alphaM</code></p></td>
 <td><p>$\alpha_M$ factor</p></td>
 </tr>
@@ -122,67 +126,65 @@
 increase the amount of numerical damping present without degrading the order of
 accuracy. In the HHT method, the same Newmark approximations are used:
 
 <dl>
 <dt></dt>
 <dd>
 
-$$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta)
-\Delta t^2] \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
+$$u_{t+\Delta t} = u_t + \Delta t \dot u_t + [(0.5 - \beta)
+\Delta t^2] \ddot u_t + [\beta \Delta t^2] \ddot u_{t+\Delta t}$$
 
 </dd>
 </dl>
 <dl>
 <dt></dt>
 <dd>
 
-$$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot
-U_t + [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
+$$\dot u_{t+\Delta t} = \dot u_t + [(1-\gamma)\Delta t] \ddot
+u_t + [\gamma \Delta t ] \ddot u_{t+\Delta t} $$
 
 </dd>
 </dl>
 <p>but the time-discrete momentum equation is modified:</p>
 
-$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot
-U_{t + \alpha_M \Delta t} - C \dot U_{t+\alpha_F \Delta t} -
-F^{int}(U_{t + \alpha_F \Delta t})
+$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{\mathrm{ext}} - M \ddot
+u_{t + \alpha_M \Delta t} - C \dot u_{t+\alpha_F \Delta t} -
+F^{\mathrm{int}}(u_{t + \alpha_F \Delta t})
 $$
 
 where the displacements and velocities at the intermediate point are
 given by:
 
-$$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F
-U_{t + \Delta t}$$
+$$u_{t+ \alpha_F \Delta t} = (1 - \alpha_F) u_t + \alpha_F
+u_{t + \Delta t}$$
 
-$$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t +
-\alpha_F \dot U_{t + \Delta t}$$
+$$\dot u_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot u_t +
+\alpha_F \dot u_{t + \Delta t}$$
 
-$$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
-\alpha_M \ddot U_{t + \Delta t}$$
+$$\ddot u_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot u_t +
+\alpha_M \ddot u_{t + \Delta t}$$
 
 <p>Following the methods outlined for Newmarks method, linearization of
 the nonlinear momentum equation results in the following linear
 equations:</p>
 
-$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta
+$$K_{t+\Delta t}^{*i} d u_{t+\Delta t}^{i+1} = R_{t+\Delta
 t}^i$$
 
-$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \frac{\alpha_F
-\gamma}{\beta \Delta t} C_t + \frac{\alpha_M}{\beta \Delta t^2}
-M$$
+$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \alpha_F \frac{\gamma}{\beta \Delta t} C_t + \alpha_M\frac{1}{\beta \Delta t^2}M$$
 
 <p>and</p>
 
-$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha
-F \Delta t}^{i-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M
-\ddot U_{t+ \alpha M \Delta t}^{i-1}$$
+$$R_{t+\Delta t}^i = F_{t + \Delta t}^{\mathrm{ext}} - F(u_{t + \alpha
+F \Delta t}^{i-1})^{\mathrm{int}} - C \dot u_{t+\alpha F \Delta t}^{i-1} - M
+\ddot u_{t+ \alpha M \Delta t}^{i-1}$$
 
 The linear equations are used to solve for 
 
-$$U_{t+\alpha_F \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$
+$$u_{t+\alpha_F \Delta t}, \dot u_{t + \alpha_F \Delta t} \ddot u_{t+ \alpha M \Delta t}$$
 
 Once convergence has been achieved the displacements,
 velocities and accelerations at time $t + \Delta t$ can be computed.
 
 ## Compiling
 
 The main integrator is implemented in standard C and can be compiled
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1 Name: sdof Version: 0.0.6 Summary: Lightning-fast
-integration of single degree-of-freedom systems. Author-email: "Claudio M.
-Perez" <50180406+claudioperez@users.noreply.github.com> Project-URL:
-repository, http://github.com/claudioperez/sdof Keywords: seismic,earthquake-
-engineering Description-Content-Type: text/markdown # `sdof` Lightning-fast
-integration of single degree-of-freedom systems. This package solves scalar
+# `sdof` [PEER Logo] Lightning-fast integration of single degree-of-freedom
+systems.
+[![Latest PyPI version](https://img.shields.io/pypi/v/sdof?logo=pypi&style=for-
+the-badge)](https://pypi.python.org/pypi/sdof) [NPM_version]
+------------------------------------------------- This package solves scalar
 differential equations of the form $$ m \ddot{u} + c \dot{u} + k u = f(t) $$
 Integration is carried out using a Generalized - $\alpha$ integrator that is
 implemented under the hood in highly optimized multi-threaded C code.
 Generalized - $\alpha$ is an implicit method that allows for high frequency
 energy dissipation and second order accuracy. With the right selection of
 parameters, the method can be specialized to the Hibert-Hughes-Taylor (HHT), or
 Newmark families of integration schemes.
 ===============================================================================
-[NPM_version] ## Python API ```python from sdof import integrate, peaks,
+## Python API ```python import numpy as np from sdof import integrate, peaks,
 spectrum m = 1.0 c = 1.0 k = 2.0 f = np.sin(np.linspace(0, 5*np.pi, 100)) dt =
 5*np.pi/100 u_max, v_max, a_max = peaks(m, c, k, f, dt) u, v, a = integrate(m,
-c, k, f, dt) Su, Sv, Sa = spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02,
-3.0, 100)) ``` ## Integrator (Reproduced from OpenSees docs)
+c, k, f, dt) D, V, A = spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02,
+3.0, 100)) ``` ## Integrator (Adapted from OpenSees docs)
 alphaM $\alpha_M$ factor
 alphaF $\alpha_F$ factor
 gamma  $\gamma$ factor
 beta   $\beta$ factor
    1. $\alpha_F$ and $\alpha_M$ are defined differently that in the paper, we
       use $\alpha_F = (1-\alpha_f)$ and $\alpha_M=(1-\gamma_m)$ where
       $\alpha_f$ and $\alpha_m$ are those used in the paper.
@@ -44,43 +43,44 @@
       $$\gamma = \dfrac{1}{2} + \gamma_M - \gamma_F$$
 and
       $$\beta = \dfrac{1}{4}(1 + \gamma_M - \gamma_F)^2$$
 ### Theory The generalized $\alpha$ method is a one step implicit method for
 solving the transient problem which attempts to increase the amount of
 numerical damping present without degrading the order of accuracy. In the HHT
 method, the same Newmark approximations are used:
-      $$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta) \Delta t^2]
-      \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
-      $$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot U_t +
-      [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
+      $$u_{t+\Delta t} = u_t + \Delta t \dot u_t + [(0.5 - \beta) \Delta t^2]
+      \ddot u_t + [\beta \Delta t^2] \ddot u_{t+\Delta t}$$
+      $$\dot u_{t+\Delta t} = \dot u_t + [(1-\gamma)\Delta t] \ddot u_t +
+      [\gamma \Delta t ] \ddot u_{t+\Delta t} $$
 but the time-discrete momentum equation is modified:
-$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot U_{t + \alpha_M
-\Delta t} - C \dot U_{t+\alpha_F \Delta t} - F^{int}(U_{t + \alpha_F \Delta t})
-$$ where the displacements and velocities at the intermediate point are given
-by: $$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F U_{t + \Delta
-t}$$ $$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t + \alpha_F \dot U_
-{t + \Delta t}$$ $$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
-\alpha_M \ddot U_{t + \Delta t}$$
+$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{\mathrm{ext}} - M \ddot u_{t +
+\alpha_M \Delta t} - C \dot u_{t+\alpha_F \Delta t} - F^{\mathrm{int}}(u_{t +
+\alpha_F \Delta t}) $$ where the displacements and velocities at the
+intermediate point are given by: $$u_{t+ \alpha_F \Delta t} = (1 - \alpha_F)
+u_t + \alpha_F u_{t + \Delta t}$$ $$\dot u_{t+\alpha_F \Delta t} = (1-\alpha_F)
+\dot u_t + \alpha_F \dot u_{t + \Delta t}$$ $$\ddot u_{t+\alpha_M \Delta t} =
+(1-\alpha_M) \ddot u_t + \alpha_M \ddot u_{t + \Delta t}$$
 Following the methods outlined for Newmarks method, linearization of the
 nonlinear momentum equation results in the following linear equations:
-$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta t}^i$$ $$K_{t+\Delta
-t}^{*i} = \alpha_F K_t + \frac{\alpha_F \gamma}{\beta \Delta t} C_t + \frac
-{\alpha_M}{\beta \Delta t^2} M$$
+$$K_{t+\Delta t}^{*i} d u_{t+\Delta t}^{i+1} = R_{t+\Delta t}^i$$ $$K_{t+\Delta
+t}^{*i} = \alpha_F K_t + \alpha_F \frac{\gamma}{\beta \Delta t} C_t +
+\alpha_M\frac{1}{\beta \Delta t^2}M$$
 and
-$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha F \Delta t}^{i-
-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M \ddot U_{t+ \alpha M
-\Delta t}^{i-1}$$ The linear equations are used to solve for $$U_{t+\alpha_F
-\Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$ Once
-convergence has been achieved the displacements, velocities and accelerations
-at time $t + \Delta t$ can be computed. ## Compiling The main integrator is
-implemented in standard C and can be compiled as either a Python extension, or
-Javascript library (via WASM). ### Python ``` pip install . ``` ### Javascript
-- Install `emscripten` from [here](https://emscripten.org/) - run `make`. This
-creates the following files: - `dist/fsdof.wasm` - Web assembly - compiled
-library, - `dist/fsdof.js` - interface to binary `fsdof.wasm` - to test, you
-can use Python to start an HTTP server in the current directory as follows:
-```shell python -m http.server . ``` ## References
+$$R_{t+\Delta t}^i = F_{t + \Delta t}^{\mathrm{ext}} - F(u_{t + \alpha F \Delta
+t}^{i-1})^{\mathrm{int}} - C \dot u_{t+\alpha F \Delta t}^{i-1} - M \ddot u_{t+
+\alpha M \Delta t}^{i-1}$$ The linear equations are used to solve for $$u_
+{t+\alpha_F \Delta t}, \dot u_{t + \alpha_F \Delta t} \ddot u_{t+ \alpha M
+\Delta t}$$ Once convergence has been achieved the displacements, velocities
+and accelerations at time $t + \Delta t$ can be computed. ## Compiling The main
+integrator is implemented in standard C and can be compiled as either a Python
+extension, or Javascript library (via WASM). ### Python ``` pip install . ```
+### Javascript - Install `emscripten` from [here](https://emscripten.org/) -
+run `make`. This creates the following files: - `dist/fsdof.wasm` - Web
+assembly - compiled library, - `dist/fsdof.js` - interface to binary
+`fsdof.wasm` - to test, you can use Python to start an HTTP server in the
+current directory as follows: ```shell python -m http.server . ``` ##
+References
 J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural Dynamics
 with Improved Numerical Dissipation: The Generalized - $\alpha$ Method" ASME
 Journal of Applied Mechanics, 60, 371:375, 1993.
 ===============================================================================
 Code Developed by: fmk
```

### Comparing `sdof-0.0.6/tests/chopra.sh` & `sdof-0.0.7/tests/chopra.sh`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/tests/test.py` & `sdof-0.0.7/tests/test.py`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/theory.md` & `sdof-0.0.7/theory.md`

 * *Files identical despite different names*

### Comparing `sdof-0.0.6/wasm/index.js` & `sdof-0.0.7/wasm/index.js`

 * *Files identical despite different names*

