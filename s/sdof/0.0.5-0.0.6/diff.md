# Comparing `tmp/sdof-0.0.5.tar.gz` & `tmp/sdof-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdof-0.0.5.tar", last modified: Sat Feb 25 09:09:39 2023, max compression
+gzip compressed data, was "sdof-0.0.6.tar", last modified: Sun Jul 16 22:48:27 2023, max compression
```

## Comparing `sdof-0.0.5.tar` & `sdof-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 09:09:39.363819 sdof-0.0.5/
--rw-rw-rw-   0        0        0     5749 2023-02-25 09:09:39.362040 sdof-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5427 2023-02-25 09:07:15.000000 sdof-0.0.5/README.md
--rw-rw-rw-   0        0        0      658 2023-02-25 09:07:15.000000 sdof-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-25 09:09:39.364815 sdof-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      214 2023-02-25 09:07:15.000000 sdof-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-25 09:09:39.268058 sdof-0.0.5/src/
--rw-rw-rw-   0        0        0     6004 2023-02-25 09:07:15.000000 sdof-0.0.5/src/fsdof.c
-drwxrwxrwx   0        0        0        0 2023-02-25 09:09:39.291299 sdof-0.0.5/src/sdof/
--rw-rw-rw-   0        0        0     2509 2023-02-25 09:07:15.000000 sdof-0.0.5/src/sdof/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-25 09:09:39.338955 sdof-0.0.5/src/sdof.egg-info/
--rw-rw-rw-   0        0        0     5749 2023-02-25 09:09:39.000000 sdof-0.0.5/src/sdof.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-02-25 09:09:39.000000 sdof-0.0.5/src/sdof.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 09:09:39.000000 sdof-0.0.5/src/sdof.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-02-25 09:09:39.000000 sdof-0.0.5/src/sdof.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-25 09:09:39.356641 sdof-0.0.5/tests/
--rw-rw-rw-   0        0        0     1034 2023-02-25 09:07:15.000000 sdof-0.0.5/tests/test.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       62 2023-02-10 17:50:46.000000 sdof-0.0.6/.gitignore
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      748 2023-07-16 22:46:57.000000 sdof-0.0.6/Makefile
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     6235 2023-07-16 22:48:26.996706 sdof-0.0.6/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     5889 2023-07-16 22:46:27.000000 sdof-0.0.6/README.md
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/data/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)    16031 2022-04-04 01:35:00.000000 sdof-0.0.6/data/elCentro.AT2
+-rw-r--r--   0 claudio   (1001) claudio   (1001)    17878 2022-04-04 01:36:22.000000 sdof-0.0.6/data/elCentro.txt
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/dist/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)   185034 2022-04-06 02:05:30.000000 sdof-0.0.6/dist/alpha.js
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    16284 2022-04-06 02:05:30.000000 sdof-0.0.6/dist/alpha.wasm
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      718 2023-07-16 22:48:09.000000 sdof-0.0.6/pyproject.toml
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-07-16 22:48:26.996706 sdof-0.0.6/setup.cfg
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      203 2023-02-10 17:57:42.000000 sdof-0.0.6/setup.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/src/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3001 2023-01-09 19:17:41.000000 sdof-0.0.6/src/alpha.c
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     7687 2023-07-16 21:09:24.000000 sdof-0.0.6/src/fsdof.c
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2654 2022-04-06 02:09:45.000000 sdof-0.0.6/src/modal.c
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/src/sdof/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     5244 2023-07-16 22:47:36.000000 sdof-0.0.6/src/sdof/__init__.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1313 2023-07-16 22:46:57.000000 sdof-0.0.6/src/sdof/__main__.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/src/sdof.egg-info/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     6235 2023-07-16 22:48:26.000000 sdof-0.0.6/src/sdof.egg-info/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      379 2023-07-16 22:48:26.000000 sdof-0.0.6/src/sdof.egg-info/SOURCES.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-07-16 22:48:26.000000 sdof-0.0.6/src/sdof.egg-info/dependency_links.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       25 2023-07-16 22:48:26.000000 sdof-0.0.6/src/sdof.egg-info/top_level.txt
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/tests/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      966 2023-01-09 19:21:13.000000 sdof-0.0.6/tests/chopra.sh
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      975 2023-01-11 21:44:56.000000 sdof-0.0.6/tests/test.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3400 2023-07-16 05:13:02.000000 sdof-0.0.6/theory.md
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-16 22:48:26.996706 sdof-0.0.6/wasm/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2305 2023-02-12 03:13:03.000000 sdof-0.0.6/wasm/index.js
```

### Comparing `sdof-0.0.5/PKG-INFO` & `sdof-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,201 +1,221 @@
-Metadata-Version: 2.1
-Name: sdof
-Version: 0.0.5
-Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>
-Project-URL: repository, http://github.com/BRACE2/sdof
-Project-URL: documentation, https://brace2.github.io/sdof
-Keywords: seismic,earthquake
-Description-Content-Type: text/markdown
-
-# `sdof`
-
-Fast integration of single degree-of-freedom systems.
-
-This package solves scalar problems of the form
-
-$$
-m \ddot{u} + c \dot{u} + k u = f(t)
-$$
-
-Integration is carried out using the Generalized - $\alpha$ method. This is an
-implicit method that like the HHT method allows for high frequency energy
-dissipation and second order accuracy.
-
-<hr />
-
-<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg" alt="NPM version" /></a></span>
-
-
-## Compile
-
-### Python
-
-```
-pip install .
-```
-
-### Javascript
-
-- Install `emscripten` from [here](https://emscripten.org/)
-- run `make`. This creates the following files:
-  - `dist/fsdof.wasm` - Web assembly - compiled library,
-  - `dist/fsdof.js` - interface to binary `fsdof.wasm`
-
-- to test, you can use Python to start an HTTP server in the current directory
-  as follows:
-  ```shell
-  python -m http.server .
-  ```
-
-## Python API
-
-```python
-def peaks(m, c, k, f, dt): ...
-```
-
-## Integrator (Reproduced from OpenSees docs)
-
-<table>
-<tbody>
-<tr class="odd">
-<td><p><code class="parameter-table-variable">alphaM</code></p></td>
-<td><p>$\alpha_M$ factor</p></td>
-</tr>
-<tr class="even">
-<td><p><code class="parameter-table-variable">alphaF</code></p></td>
-<td><p>$\alpha_F$ factor</p></td>
-</tr>
-<tr class="odd">
-<td><p><code class="parameter-table-variable">gamma</code></p></td>
-<td><p>$\gamma$ factor</p></td>
-</tr>
-<tr class="even">
-<td><p><code class="parameter-table-variable">beta</code></p></td>
-<td><p>$\beta$ factor</p></td>
-</tr>
-</tbody>
-</table>
-
-<ol>
-<li>$\alpha_F$ and
-  $\alpha_M$ are defined differently that in the
-  paper, we use $\alpha_F = (1-\alpha_f)$ and
-  $\alpha_M=(1-\gamma_m)$ where
-  $\alpha_f$ and $\alpha_m$
-  are those used in the paper.</li>
-
-<li>Like Newmark and other implicit schemes, the unconditional
-  stability of this method applies to linear problems. There are no
-  results showing stability of this method over the wide range of
-  nonlinear problems that potentially exist. Experience indicates that the
-  time step for implicit schemes in nonlinear situations can be much
-  greater than those for explicit schemes.</li>
-
-<li>$\alpha_M = 1.0, \alpha_F = 1.0$ produces the Newmark Method.</li>
-<li>$\alpha_M = 1.0$ corresponds to the HHT method.</li>
-<li>The method is second-order accurate provided $\gamma = \dfrac{1}{2} + \alpha_M - \alpha_F$</li>
-<li>The method is unconditionally stable provided $\alpha_M \ge \alpha_F \ge \dfrac{1}{2}, \quad \beta \ge \dfrac{1}{4} +\dfrac{1}{2}(\gamma_M - \gamma_F)$</li>
-
-<li>$\gamma$ and $\beta$
-  are optional. The default values ensure the method is unconditionally
-  stable, second order accurate and high frequency dissipation is
-  maximized.</li>
-</ol>
-<p>The defaults are:</p>
-<dl>
-<dt></dt>
-<dd>
-
-$$\gamma = \dfrac{1}{2} + \gamma_M - \gamma_F$$
-
-</dd>
-</dl>
-<p>and</p>
-<dl>
-<dt></dt>
-<dd>
-
-$$\beta = \dfrac{1}{4}(1 + \gamma_M - \gamma_F)^2$$
-
-</dd>
-</dl>
-
-### Theory
-
-The generalized $\alpha$ method is a one
-step implicit method for solving the transient problem which attempts to
-increase the amount of numerical damping present without degrading the order of
-accuracy. In the HHT method, the same Newmark approximations are used:
-
-<dl>
-<dt></dt>
-<dd>
-
-$$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta)
-\Delta t^2] \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
-
-</dd>
-</dl>
-<dl>
-<dt></dt>
-<dd>
-
-$$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot
-U_t + [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
-
-</dd>
-</dl>
-<p>but the time-discrete momentum equation is modified:</p>
-
-$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot
-U_{t + \alpha_M \Delta t} - C \dot U_{t+\alpha_F \Delta t} -
-F^{int}(U_{t + \alpha_F \Delta t})
-$$
-
-where the displacements and velocities at the intermediate point are
-given by:
-
-$$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F
-U_{t + \Delta t}$$
-
-$$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t +
-\alpha_F \dot U_{t + \Delta t}$$
-
-$$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
-\alpha_M \ddot U_{t + \Delta t}$$
-
-<p>Following the methods outlined for Newmarks method, linearization of
-the nonlinear momentum equation results in the following linear
-equations:</p>
-
-$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta
-t}^i$$
-
-$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \frac{\alpha_F
-\gamma}{\beta \Delta t} C_t + \frac{\alpha_M}{\beta \Delta t^2}
-M$$
-
-<p>and</p>
-
-$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha
-F \Delta t}^{i-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M
-\ddot U_{t+ \alpha M \Delta t}^{i-1}$$
-
-The linear equations are used to solve for 
-
-$$U_{t+\alpha_F \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$
-
-Once convergence has been achieved the displacements,
-velocities and accelerations at time $t + \Delta t$ can be computed.
-
-## References
-
-<p>J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural
-   Dynamics with Improved Numerical Dissipation: The
-   Generalized - $\alpha$ Method" ASME Journal of
-   Applied Mechanics, 60, 371:375, 1993.</p>
-
-<hr />
-
-<p>Code Developed by: <span style="color:blue">fmk</span></p>
-
+Metadata-Version: 2.1
+Name: sdof
+Version: 0.0.6
+Summary: Lightning-fast integration of single degree-of-freedom systems.
+Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>
+Project-URL: repository, http://github.com/claudioperez/sdof
+Keywords: seismic,earthquake-engineering
+Description-Content-Type: text/markdown
+
+# `sdof`
+
+Lightning-fast integration of single degree-of-freedom systems.
+
+This package solves scalar differential equations of the form
+
+$$
+m \ddot{u} + c \dot{u} + k u = f(t)
+$$
+
+Integration is carried out using a Generalized - $\alpha$ integrator that
+is implemented under the hood in highly optimized multi-threaded C code. 
+
+Generalized - $\alpha$ is an implicit method that allows for high frequency energy
+dissipation and second order accuracy. With the right selection of parameters,
+the method can be specialized to the Hibert-Hughes-Taylor (HHT), or Newmark
+families of integration schemes.
+
+<hr />
+
+<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg" alt="NPM version" /></a></span>
+
+
+## Python API
+
+```python
+from sdof import integrate, peaks, spectrum
+
+m  = 1.0
+c  = 1.0
+k  = 2.0
+f  = np.sin(np.linspace(0, 5*np.pi, 100))
+dt = 5*np.pi/100
+
+u_max, v_max, a_max =  peaks(m, c, k, f, dt)
+
+u, v, a    = integrate(m, c, k, f, dt)
+
+Su, Sv, Sa =  spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02, 3.0, 100))
+```
+
+## Integrator (Reproduced from OpenSees docs)
+
+<table>
+<tbody>
+<tr class="odd">
+<td><p><code class="parameter-table-variable">alphaM</code></p></td>
+<td><p>$\alpha_M$ factor</p></td>
+</tr>
+<tr class="even">
+<td><p><code class="parameter-table-variable">alphaF</code></p></td>
+<td><p>$\alpha_F$ factor</p></td>
+</tr>
+<tr class="odd">
+<td><p><code class="parameter-table-variable">gamma</code></p></td>
+<td><p>$\gamma$ factor</p></td>
+</tr>
+<tr class="even">
+<td><p><code class="parameter-table-variable">beta</code></p></td>
+<td><p>$\beta$ factor</p></td>
+</tr>
+</tbody>
+</table>
+
+<ol>
+<li>$\alpha_F$ and
+  $\alpha_M$ are defined differently that in the
+  paper, we use $\alpha_F = (1-\alpha_f)$ and
+  $\alpha_M=(1-\gamma_m)$ where
+  $\alpha_f$ and $\alpha_m$
+  are those used in the paper.</li>
+
+<li>Like Newmark and other implicit schemes, the unconditional
+  stability of this method applies to linear problems. There are no
+  results showing stability of this method over the wide range of
+  nonlinear problems that potentially exist. Experience indicates that the
+  time step for implicit schemes in nonlinear situations can be much
+  greater than those for explicit schemes.</li>
+
+<li>$\alpha_M = 1.0, \alpha_F = 1.0$ produces the Newmark Method.</li>
+<li>$\alpha_M = 1.0$ corresponds to the HHT method.</li>
+<li>The method is second-order accurate provided $\gamma = \dfrac{1}{2} + \alpha_M - \alpha_F$</li>
+<li>The method is unconditionally stable provided $\alpha_M \ge \alpha_F \ge \dfrac{1}{2}, \quad \beta \ge \dfrac{1}{4} +\dfrac{1}{2}(\gamma_M - \gamma_F)$</li>
+
+<li>$\gamma$ and $\beta$
+  are optional. The default values ensure the method is unconditionally
+  stable, second order accurate and high frequency dissipation is
+  maximized.</li>
+</ol>
+<p>The defaults are:</p>
+<dl>
+<dt></dt>
+<dd>
+
+$$\gamma = \dfrac{1}{2} + \gamma_M - \gamma_F$$
+
+</dd>
+</dl>
+<p>and</p>
+<dl>
+<dt></dt>
+<dd>
+
+$$\beta = \dfrac{1}{4}(1 + \gamma_M - \gamma_F)^2$$
+
+</dd>
+</dl>
+
+### Theory
+
+The generalized $\alpha$ method is a one
+step implicit method for solving the transient problem which attempts to
+increase the amount of numerical damping present without degrading the order of
+accuracy. In the HHT method, the same Newmark approximations are used:
+
+<dl>
+<dt></dt>
+<dd>
+
+$$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta)
+\Delta t^2] \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
+
+</dd>
+</dl>
+<dl>
+<dt></dt>
+<dd>
+
+$$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot
+U_t + [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
+
+</dd>
+</dl>
+<p>but the time-discrete momentum equation is modified:</p>
+
+$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot
+U_{t + \alpha_M \Delta t} - C \dot U_{t+\alpha_F \Delta t} -
+F^{int}(U_{t + \alpha_F \Delta t})
+$$
+
+where the displacements and velocities at the intermediate point are
+given by:
+
+$$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F
+U_{t + \Delta t}$$
+
+$$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t +
+\alpha_F \dot U_{t + \Delta t}$$
+
+$$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
+\alpha_M \ddot U_{t + \Delta t}$$
+
+<p>Following the methods outlined for Newmarks method, linearization of
+the nonlinear momentum equation results in the following linear
+equations:</p>
+
+$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta
+t}^i$$
+
+$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \frac{\alpha_F
+\gamma}{\beta \Delta t} C_t + \frac{\alpha_M}{\beta \Delta t^2}
+M$$
+
+<p>and</p>
+
+$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha
+F \Delta t}^{i-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M
+\ddot U_{t+ \alpha M \Delta t}^{i-1}$$
+
+The linear equations are used to solve for 
+
+$$U_{t+\alpha_F \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$
+
+Once convergence has been achieved the displacements,
+velocities and accelerations at time $t + \Delta t$ can be computed.
+
+## Compiling
+
+The main integrator is implemented in standard C and can be compiled
+as either a Python extension, or Javascript library (via WASM).
+
+### Python
+
+```
+pip install .
+```
+
+### Javascript
+
+- Install `emscripten` from [here](https://emscripten.org/)
+- run `make`. This creates the following files:
+  - `dist/fsdof.wasm` - Web assembly - compiled library,
+  - `dist/fsdof.js` - interface to binary `fsdof.wasm`
+
+- to test, you can use Python to start an HTTP server in the current directory
+  as follows:
+  ```shell
+  python -m http.server .
+  ```
+
+
+## References
+
+<p>J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural
+   Dynamics with Improved Numerical Dissipation: The
+   Generalized - $\alpha$ Method" ASME Journal of
+   Applied Mechanics, 60, 371:375, 1993.</p>
+
+<hr />
+
+<p>Code Developed by: <span style="color:blue">fmk</span></p>
+
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: sdof Version: 0.0.5 Author-email: "Claudio M.
+Metadata-Version: 2.1 Name: sdof Version: 0.0.6 Summary: Lightning-fast
+integration of single degree-of-freedom systems. Author-email: "Claudio M.
 Perez" <50180406+claudioperez@users.noreply.github.com> Project-URL:
-repository, http://github.com/BRACE2/sdof Project-URL: documentation, https://
-brace2.github.io/sdof Keywords: seismic,earthquake Description-Content-Type:
-text/markdown # `sdof` Fast integration of single degree-of-freedom systems.
-This package solves scalar problems of the form $$ m \ddot{u} + c \dot{u} + k u
-= f(t) $$ Integration is carried out using the Generalized - $\alpha$ method.
-This is an implicit method that like the HHT method allows for high frequency
-energy dissipation and second order accuracy.
+repository, http://github.com/claudioperez/sdof Keywords: seismic,earthquake-
+engineering Description-Content-Type: text/markdown # `sdof` Lightning-fast
+integration of single degree-of-freedom systems. This package solves scalar
+differential equations of the form $$ m \ddot{u} + c \dot{u} + k u = f(t) $$
+Integration is carried out using a Generalized - $\alpha$ integrator that is
+implemented under the hood in highly optimized multi-threaded C code.
+Generalized - $\alpha$ is an implicit method that allows for high frequency
+energy dissipation and second order accuracy. With the right selection of
+parameters, the method can be specialized to the Hibert-Hughes-Taylor (HHT), or
+Newmark families of integration schemes.
 ===============================================================================
-[NPM_version] ## Compile ### Python ``` pip install . ``` ### Javascript -
-Install `emscripten` from [here](https://emscripten.org/) - run `make`. This
-creates the following files: - `dist/fsdof.wasm` - Web assembly - compiled
-library, - `dist/fsdof.js` - interface to binary `fsdof.wasm` - to test, you
-can use Python to start an HTTP server in the current directory as follows:
-```shell python -m http.server . ``` ## Python API ```python def peaks(m, c, k,
-f, dt): ... ``` ## Integrator (Reproduced from OpenSees docs)
+[NPM_version] ## Python API ```python from sdof import integrate, peaks,
+spectrum m = 1.0 c = 1.0 k = 2.0 f = np.sin(np.linspace(0, 5*np.pi, 100)) dt =
+5*np.pi/100 u_max, v_max, a_max = peaks(m, c, k, f, dt) u, v, a = integrate(m,
+c, k, f, dt) Su, Sv, Sa = spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02,
+3.0, 100)) ``` ## Integrator (Reproduced from OpenSees docs)
 alphaM $\alpha_M$ factor
 alphaF $\alpha_F$ factor
 gamma  $\gamma$ factor
 beta   $\beta$ factor
    1. $\alpha_F$ and $\alpha_M$ are defined differently that in the paper, we
       use $\alpha_F = (1-\alpha_f)$ and $\alpha_M=(1-\gamma_m)$ where
       $\alpha_f$ and $\alpha_m$ are those used in the paper.
@@ -65,13 +67,20 @@
 {\alpha_M}{\beta \Delta t^2} M$$
 and
 $$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha F \Delta t}^{i-
 1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M \ddot U_{t+ \alpha M
 \Delta t}^{i-1}$$ The linear equations are used to solve for $$U_{t+\alpha_F
 \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$ Once
 convergence has been achieved the displacements, velocities and accelerations
-at time $t + \Delta t$ can be computed. ## References
+at time $t + \Delta t$ can be computed. ## Compiling The main integrator is
+implemented in standard C and can be compiled as either a Python extension, or
+Javascript library (via WASM). ### Python ``` pip install . ``` ### Javascript
+- Install `emscripten` from [here](https://emscripten.org/) - run `make`. This
+creates the following files: - `dist/fsdof.wasm` - Web assembly - compiled
+library, - `dist/fsdof.js` - interface to binary `fsdof.wasm` - to test, you
+can use Python to start an HTTP server in the current directory as follows:
+```shell python -m http.server . ``` ## References
 J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural Dynamics
 with Improved Numerical Dissipation: The Generalized - $\alpha$ Method" ASME
 Journal of Applied Mechanics, 60, 371:375, 1993.
 ===============================================================================
 Code Developed by: fmk
```

### Comparing `sdof-0.0.5/README.md` & `sdof-0.0.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,192 +1,212 @@
-# `sdof`
-
-Fast integration of single degree-of-freedom systems.
-
-This package solves scalar problems of the form
-
-$$
-m \ddot{u} + c \dot{u} + k u = f(t)
-$$
-
-Integration is carried out using the Generalized - $\alpha$ method. This is an
-implicit method that like the HHT method allows for high frequency energy
-dissipation and second order accuracy.
-
-<hr />
-
-<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg" alt="NPM version" /></a></span>
-
-
-## Compile
-
-### Python
-
-```
-pip install .
-```
-
-### Javascript
-
-- Install `emscripten` from [here](https://emscripten.org/)
-- run `make`. This creates the following files:
-  - `dist/fsdof.wasm` - Web assembly - compiled library,
-  - `dist/fsdof.js` - interface to binary `fsdof.wasm`
-
-- to test, you can use Python to start an HTTP server in the current directory
-  as follows:
-  ```shell
-  python -m http.server .
-  ```
-
-## Python API
-
-```python
-def peaks(m, c, k, f, dt): ...
-```
-
-## Integrator (Reproduced from OpenSees docs)
-
-<table>
-<tbody>
-<tr class="odd">
-<td><p><code class="parameter-table-variable">alphaM</code></p></td>
-<td><p>$\alpha_M$ factor</p></td>
-</tr>
-<tr class="even">
-<td><p><code class="parameter-table-variable">alphaF</code></p></td>
-<td><p>$\alpha_F$ factor</p></td>
-</tr>
-<tr class="odd">
-<td><p><code class="parameter-table-variable">gamma</code></p></td>
-<td><p>$\gamma$ factor</p></td>
-</tr>
-<tr class="even">
-<td><p><code class="parameter-table-variable">beta</code></p></td>
-<td><p>$\beta$ factor</p></td>
-</tr>
-</tbody>
-</table>
-
-<ol>
-<li>$\alpha_F$ and
-  $\alpha_M$ are defined differently that in the
-  paper, we use $\alpha_F = (1-\alpha_f)$ and
-  $\alpha_M=(1-\gamma_m)$ where
-  $\alpha_f$ and $\alpha_m$
-  are those used in the paper.</li>
-
-<li>Like Newmark and other implicit schemes, the unconditional
-  stability of this method applies to linear problems. There are no
-  results showing stability of this method over the wide range of
-  nonlinear problems that potentially exist. Experience indicates that the
-  time step for implicit schemes in nonlinear situations can be much
-  greater than those for explicit schemes.</li>
-
-<li>$\alpha_M = 1.0, \alpha_F = 1.0$ produces the Newmark Method.</li>
-<li>$\alpha_M = 1.0$ corresponds to the HHT method.</li>
-<li>The method is second-order accurate provided $\gamma = \dfrac{1}{2} + \alpha_M - \alpha_F$</li>
-<li>The method is unconditionally stable provided $\alpha_M \ge \alpha_F \ge \dfrac{1}{2}, \quad \beta \ge \dfrac{1}{4} +\dfrac{1}{2}(\gamma_M - \gamma_F)$</li>
-
-<li>$\gamma$ and $\beta$
-  are optional. The default values ensure the method is unconditionally
-  stable, second order accurate and high frequency dissipation is
-  maximized.</li>
-</ol>
-<p>The defaults are:</p>
-<dl>
-<dt></dt>
-<dd>
-
-$$\gamma = \dfrac{1}{2} + \gamma_M - \gamma_F$$
-
-</dd>
-</dl>
-<p>and</p>
-<dl>
-<dt></dt>
-<dd>
-
-$$\beta = \dfrac{1}{4}(1 + \gamma_M - \gamma_F)^2$$
-
-</dd>
-</dl>
-
-### Theory
-
-The generalized $\alpha$ method is a one
-step implicit method for solving the transient problem which attempts to
-increase the amount of numerical damping present without degrading the order of
-accuracy. In the HHT method, the same Newmark approximations are used:
-
-<dl>
-<dt></dt>
-<dd>
-
-$$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta)
-\Delta t^2] \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
-
-</dd>
-</dl>
-<dl>
-<dt></dt>
-<dd>
-
-$$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot
-U_t + [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
-
-</dd>
-</dl>
-<p>but the time-discrete momentum equation is modified:</p>
-
-$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot
-U_{t + \alpha_M \Delta t} - C \dot U_{t+\alpha_F \Delta t} -
-F^{int}(U_{t + \alpha_F \Delta t})
-$$
-
-where the displacements and velocities at the intermediate point are
-given by:
-
-$$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F
-U_{t + \Delta t}$$
-
-$$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t +
-\alpha_F \dot U_{t + \Delta t}$$
-
-$$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
-\alpha_M \ddot U_{t + \Delta t}$$
-
-<p>Following the methods outlined for Newmarks method, linearization of
-the nonlinear momentum equation results in the following linear
-equations:</p>
-
-$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta
-t}^i$$
-
-$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \frac{\alpha_F
-\gamma}{\beta \Delta t} C_t + \frac{\alpha_M}{\beta \Delta t^2}
-M$$
-
-<p>and</p>
-
-$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha
-F \Delta t}^{i-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M
-\ddot U_{t+ \alpha M \Delta t}^{i-1}$$
-
-The linear equations are used to solve for 
-
-$$U_{t+\alpha_F \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$
-
-Once convergence has been achieved the displacements,
-velocities and accelerations at time $t + \Delta t$ can be computed.
-
-## References
-
-<p>J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural
-   Dynamics with Improved Numerical Dissipation: The
-   Generalized - $\alpha$ Method" ASME Journal of
-   Applied Mechanics, 60, 371:375, 1993.</p>
-
-<hr />
-
-<p>Code Developed by: <span style="color:blue">fmk</span></p>
-
+# `sdof`
+
+Lightning-fast integration of single degree-of-freedom systems.
+
+This package solves scalar differential equations of the form
+
+$$
+m \ddot{u} + c \dot{u} + k u = f(t)
+$$
+
+Integration is carried out using a Generalized - $\alpha$ integrator that
+is implemented under the hood in highly optimized multi-threaded C code. 
+
+Generalized - $\alpha$ is an implicit method that allows for high frequency energy
+dissipation and second order accuracy. With the right selection of parameters,
+the method can be specialized to the Hibert-Hughes-Taylor (HHT), or Newmark
+families of integration schemes.
+
+<hr />
+
+<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg" alt="NPM version" /></a></span>
+
+
+## Python API
+
+```python
+from sdof import integrate, peaks, spectrum
+
+m  = 1.0
+c  = 1.0
+k  = 2.0
+f  = np.sin(np.linspace(0, 5*np.pi, 100))
+dt = 5*np.pi/100
+
+u_max, v_max, a_max =  peaks(m, c, k, f, dt)
+
+u, v, a    = integrate(m, c, k, f, dt)
+
+Su, Sv, Sa =  spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02, 3.0, 100))
+```
+
+## Integrator (Reproduced from OpenSees docs)
+
+<table>
+<tbody>
+<tr class="odd">
+<td><p><code class="parameter-table-variable">alphaM</code></p></td>
+<td><p>$\alpha_M$ factor</p></td>
+</tr>
+<tr class="even">
+<td><p><code class="parameter-table-variable">alphaF</code></p></td>
+<td><p>$\alpha_F$ factor</p></td>
+</tr>
+<tr class="odd">
+<td><p><code class="parameter-table-variable">gamma</code></p></td>
+<td><p>$\gamma$ factor</p></td>
+</tr>
+<tr class="even">
+<td><p><code class="parameter-table-variable">beta</code></p></td>
+<td><p>$\beta$ factor</p></td>
+</tr>
+</tbody>
+</table>
+
+<ol>
+<li>$\alpha_F$ and
+  $\alpha_M$ are defined differently that in the
+  paper, we use $\alpha_F = (1-\alpha_f)$ and
+  $\alpha_M=(1-\gamma_m)$ where
+  $\alpha_f$ and $\alpha_m$
+  are those used in the paper.</li>
+
+<li>Like Newmark and other implicit schemes, the unconditional
+  stability of this method applies to linear problems. There are no
+  results showing stability of this method over the wide range of
+  nonlinear problems that potentially exist. Experience indicates that the
+  time step for implicit schemes in nonlinear situations can be much
+  greater than those for explicit schemes.</li>
+
+<li>$\alpha_M = 1.0, \alpha_F = 1.0$ produces the Newmark Method.</li>
+<li>$\alpha_M = 1.0$ corresponds to the HHT method.</li>
+<li>The method is second-order accurate provided $\gamma = \dfrac{1}{2} + \alpha_M - \alpha_F$</li>
+<li>The method is unconditionally stable provided $\alpha_M \ge \alpha_F \ge \dfrac{1}{2}, \quad \beta \ge \dfrac{1}{4} +\dfrac{1}{2}(\gamma_M - \gamma_F)$</li>
+
+<li>$\gamma$ and $\beta$
+  are optional. The default values ensure the method is unconditionally
+  stable, second order accurate and high frequency dissipation is
+  maximized.</li>
+</ol>
+<p>The defaults are:</p>
+<dl>
+<dt></dt>
+<dd>
+
+$$\gamma = \dfrac{1}{2} + \gamma_M - \gamma_F$$
+
+</dd>
+</dl>
+<p>and</p>
+<dl>
+<dt></dt>
+<dd>
+
+$$\beta = \dfrac{1}{4}(1 + \gamma_M - \gamma_F)^2$$
+
+</dd>
+</dl>
+
+### Theory
+
+The generalized $\alpha$ method is a one
+step implicit method for solving the transient problem which attempts to
+increase the amount of numerical damping present without degrading the order of
+accuracy. In the HHT method, the same Newmark approximations are used:
+
+<dl>
+<dt></dt>
+<dd>
+
+$$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta)
+\Delta t^2] \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
+
+</dd>
+</dl>
+<dl>
+<dt></dt>
+<dd>
+
+$$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot
+U_t + [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
+
+</dd>
+</dl>
+<p>but the time-discrete momentum equation is modified:</p>
+
+$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot
+U_{t + \alpha_M \Delta t} - C \dot U_{t+\alpha_F \Delta t} -
+F^{int}(U_{t + \alpha_F \Delta t})
+$$
+
+where the displacements and velocities at the intermediate point are
+given by:
+
+$$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F
+U_{t + \Delta t}$$
+
+$$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t +
+\alpha_F \dot U_{t + \Delta t}$$
+
+$$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
+\alpha_M \ddot U_{t + \Delta t}$$
+
+<p>Following the methods outlined for Newmarks method, linearization of
+the nonlinear momentum equation results in the following linear
+equations:</p>
+
+$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta
+t}^i$$
+
+$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \frac{\alpha_F
+\gamma}{\beta \Delta t} C_t + \frac{\alpha_M}{\beta \Delta t^2}
+M$$
+
+<p>and</p>
+
+$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha
+F \Delta t}^{i-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M
+\ddot U_{t+ \alpha M \Delta t}^{i-1}$$
+
+The linear equations are used to solve for 
+
+$$U_{t+\alpha_F \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$
+
+Once convergence has been achieved the displacements,
+velocities and accelerations at time $t + \Delta t$ can be computed.
+
+## Compiling
+
+The main integrator is implemented in standard C and can be compiled
+as either a Python extension, or Javascript library (via WASM).
+
+### Python
+
+```
+pip install .
+```
+
+### Javascript
+
+- Install `emscripten` from [here](https://emscripten.org/)
+- run `make`. This creates the following files:
+  - `dist/fsdof.wasm` - Web assembly - compiled library,
+  - `dist/fsdof.js` - interface to binary `fsdof.wasm`
+
+- to test, you can use Python to start an HTTP server in the current directory
+  as follows:
+  ```shell
+  python -m http.server .
+  ```
+
+
+## References
+
+<p>J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural
+   Dynamics with Improved Numerical Dissipation: The
+   Generalized - $\alpha$ Method" ASME Journal of
+   Applied Mechanics, 60, 371:375, 1993.</p>
+
+<hr />
+
+<p>Code Developed by: <span style="color:blue">fmk</span></p>
+
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-# `sdof` Fast integration of single degree-of-freedom systems. This package
-solves scalar problems of the form $$ m \ddot{u} + c \dot{u} + k u = f(t) $$
-Integration is carried out using the Generalized - $\alpha$ method. This is an
-implicit method that like the HHT method allows for high frequency energy
-dissipation and second order accuracy.
+# `sdof` Lightning-fast integration of single degree-of-freedom systems. This
+package solves scalar differential equations of the form $$ m \ddot{u} + c \dot
+{u} + k u = f(t) $$ Integration is carried out using a Generalized - $\alpha$
+integrator that is implemented under the hood in highly optimized multi-
+threaded C code. Generalized - $\alpha$ is an implicit method that allows for
+high frequency energy dissipation and second order accuracy. With the right
+selection of parameters, the method can be specialized to the Hibert-Hughes-
+Taylor (HHT), or Newmark families of integration schemes.
 ===============================================================================
-[NPM_version] ## Compile ### Python ``` pip install . ``` ### Javascript -
-Install `emscripten` from [here](https://emscripten.org/) - run `make`. This
-creates the following files: - `dist/fsdof.wasm` - Web assembly - compiled
-library, - `dist/fsdof.js` - interface to binary `fsdof.wasm` - to test, you
-can use Python to start an HTTP server in the current directory as follows:
-```shell python -m http.server . ``` ## Python API ```python def peaks(m, c, k,
-f, dt): ... ``` ## Integrator (Reproduced from OpenSees docs)
+[NPM_version] ## Python API ```python from sdof import integrate, peaks,
+spectrum m = 1.0 c = 1.0 k = 2.0 f = np.sin(np.linspace(0, 5*np.pi, 100)) dt =
+5*np.pi/100 u_max, v_max, a_max = peaks(m, c, k, f, dt) u, v, a = integrate(m,
+c, k, f, dt) Su, Sv, Sa = spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02,
+3.0, 100)) ``` ## Integrator (Reproduced from OpenSees docs)
 alphaM $\alpha_M$ factor
 alphaF $\alpha_F$ factor
 gamma  $\gamma$ factor
 beta   $\beta$ factor
    1. $\alpha_F$ and $\alpha_M$ are defined differently that in the paper, we
       use $\alpha_F = (1-\alpha_f)$ and $\alpha_M=(1-\gamma_m)$ where
       $\alpha_f$ and $\alpha_m$ are those used in the paper.
@@ -61,13 +62,20 @@
 {\alpha_M}{\beta \Delta t^2} M$$
 and
 $$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha F \Delta t}^{i-
 1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M \ddot U_{t+ \alpha M
 \Delta t}^{i-1}$$ The linear equations are used to solve for $$U_{t+\alpha_F
 \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$ Once
 convergence has been achieved the displacements, velocities and accelerations
-at time $t + \Delta t$ can be computed. ## References
+at time $t + \Delta t$ can be computed. ## Compiling The main integrator is
+implemented in standard C and can be compiled as either a Python extension, or
+Javascript library (via WASM). ### Python ``` pip install . ``` ### Javascript
+- Install `emscripten` from [here](https://emscripten.org/) - run `make`. This
+creates the following files: - `dist/fsdof.wasm` - Web assembly - compiled
+library, - `dist/fsdof.js` - interface to binary `fsdof.wasm` - to test, you
+can use Python to start an HTTP server in the current directory as follows:
+```shell python -m http.server . ``` ## References
 J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural Dynamics
 with Improved Numerical Dissipation: The Generalized - $\alpha$ Method" ASME
 Journal of Applied Mechanics, 60, 371:375, 1993.
 ===============================================================================
 Code Developed by: fmk
```

### Comparing `sdof-0.0.5/src/sdof.egg-info/PKG-INFO` & `sdof-0.0.6/src/sdof.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,201 +1,221 @@
-Metadata-Version: 2.1
-Name: sdof
-Version: 0.0.5
-Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>
-Project-URL: repository, http://github.com/BRACE2/sdof
-Project-URL: documentation, https://brace2.github.io/sdof
-Keywords: seismic,earthquake
-Description-Content-Type: text/markdown
-
-# `sdof`
-
-Fast integration of single degree-of-freedom systems.
-
-This package solves scalar problems of the form
-
-$$
-m \ddot{u} + c \dot{u} + k u = f(t)
-$$
-
-Integration is carried out using the Generalized - $\alpha$ method. This is an
-implicit method that like the HHT method allows for high frequency energy
-dissipation and second order accuracy.
-
-<hr />
-
-<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg" alt="NPM version" /></a></span>
-
-
-## Compile
-
-### Python
-
-```
-pip install .
-```
-
-### Javascript
-
-- Install `emscripten` from [here](https://emscripten.org/)
-- run `make`. This creates the following files:
-  - `dist/fsdof.wasm` - Web assembly - compiled library,
-  - `dist/fsdof.js` - interface to binary `fsdof.wasm`
-
-- to test, you can use Python to start an HTTP server in the current directory
-  as follows:
-  ```shell
-  python -m http.server .
-  ```
-
-## Python API
-
-```python
-def peaks(m, c, k, f, dt): ...
-```
-
-## Integrator (Reproduced from OpenSees docs)
-
-<table>
-<tbody>
-<tr class="odd">
-<td><p><code class="parameter-table-variable">alphaM</code></p></td>
-<td><p>$\alpha_M$ factor</p></td>
-</tr>
-<tr class="even">
-<td><p><code class="parameter-table-variable">alphaF</code></p></td>
-<td><p>$\alpha_F$ factor</p></td>
-</tr>
-<tr class="odd">
-<td><p><code class="parameter-table-variable">gamma</code></p></td>
-<td><p>$\gamma$ factor</p></td>
-</tr>
-<tr class="even">
-<td><p><code class="parameter-table-variable">beta</code></p></td>
-<td><p>$\beta$ factor</p></td>
-</tr>
-</tbody>
-</table>
-
-<ol>
-<li>$\alpha_F$ and
-  $\alpha_M$ are defined differently that in the
-  paper, we use $\alpha_F = (1-\alpha_f)$ and
-  $\alpha_M=(1-\gamma_m)$ where
-  $\alpha_f$ and $\alpha_m$
-  are those used in the paper.</li>
-
-<li>Like Newmark and other implicit schemes, the unconditional
-  stability of this method applies to linear problems. There are no
-  results showing stability of this method over the wide range of
-  nonlinear problems that potentially exist. Experience indicates that the
-  time step for implicit schemes in nonlinear situations can be much
-  greater than those for explicit schemes.</li>
-
-<li>$\alpha_M = 1.0, \alpha_F = 1.0$ produces the Newmark Method.</li>
-<li>$\alpha_M = 1.0$ corresponds to the HHT method.</li>
-<li>The method is second-order accurate provided $\gamma = \dfrac{1}{2} + \alpha_M - \alpha_F$</li>
-<li>The method is unconditionally stable provided $\alpha_M \ge \alpha_F \ge \dfrac{1}{2}, \quad \beta \ge \dfrac{1}{4} +\dfrac{1}{2}(\gamma_M - \gamma_F)$</li>
-
-<li>$\gamma$ and $\beta$
-  are optional. The default values ensure the method is unconditionally
-  stable, second order accurate and high frequency dissipation is
-  maximized.</li>
-</ol>
-<p>The defaults are:</p>
-<dl>
-<dt></dt>
-<dd>
-
-$$\gamma = \dfrac{1}{2} + \gamma_M - \gamma_F$$
-
-</dd>
-</dl>
-<p>and</p>
-<dl>
-<dt></dt>
-<dd>
-
-$$\beta = \dfrac{1}{4}(1 + \gamma_M - \gamma_F)^2$$
-
-</dd>
-</dl>
-
-### Theory
-
-The generalized $\alpha$ method is a one
-step implicit method for solving the transient problem which attempts to
-increase the amount of numerical damping present without degrading the order of
-accuracy. In the HHT method, the same Newmark approximations are used:
-
-<dl>
-<dt></dt>
-<dd>
-
-$$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta)
-\Delta t^2] \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
-
-</dd>
-</dl>
-<dl>
-<dt></dt>
-<dd>
-
-$$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot
-U_t + [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
-
-</dd>
-</dl>
-<p>but the time-discrete momentum equation is modified:</p>
-
-$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot
-U_{t + \alpha_M \Delta t} - C \dot U_{t+\alpha_F \Delta t} -
-F^{int}(U_{t + \alpha_F \Delta t})
-$$
-
-where the displacements and velocities at the intermediate point are
-given by:
-
-$$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F
-U_{t + \Delta t}$$
-
-$$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t +
-\alpha_F \dot U_{t + \Delta t}$$
-
-$$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
-\alpha_M \ddot U_{t + \Delta t}$$
-
-<p>Following the methods outlined for Newmarks method, linearization of
-the nonlinear momentum equation results in the following linear
-equations:</p>
-
-$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta
-t}^i$$
-
-$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \frac{\alpha_F
-\gamma}{\beta \Delta t} C_t + \frac{\alpha_M}{\beta \Delta t^2}
-M$$
-
-<p>and</p>
-
-$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha
-F \Delta t}^{i-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M
-\ddot U_{t+ \alpha M \Delta t}^{i-1}$$
-
-The linear equations are used to solve for 
-
-$$U_{t+\alpha_F \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$
-
-Once convergence has been achieved the displacements,
-velocities and accelerations at time $t + \Delta t$ can be computed.
-
-## References
-
-<p>J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural
-   Dynamics with Improved Numerical Dissipation: The
-   Generalized - $\alpha$ Method" ASME Journal of
-   Applied Mechanics, 60, 371:375, 1993.</p>
-
-<hr />
-
-<p>Code Developed by: <span style="color:blue">fmk</span></p>
-
+Metadata-Version: 2.1
+Name: sdof
+Version: 0.0.6
+Summary: Lightning-fast integration of single degree-of-freedom systems.
+Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>
+Project-URL: repository, http://github.com/claudioperez/sdof
+Keywords: seismic,earthquake-engineering
+Description-Content-Type: text/markdown
+
+# `sdof`
+
+Lightning-fast integration of single degree-of-freedom systems.
+
+This package solves scalar differential equations of the form
+
+$$
+m \ddot{u} + c \dot{u} + k u = f(t)
+$$
+
+Integration is carried out using a Generalized - $\alpha$ integrator that
+is implemented under the hood in highly optimized multi-threaded C code. 
+
+Generalized - $\alpha$ is an implicit method that allows for high frequency energy
+dissipation and second order accuracy. With the right selection of parameters,
+the method can be specialized to the Hibert-Hughes-Taylor (HHT), or Newmark
+families of integration schemes.
+
+<hr />
+
+<span class="badge-npmversion"><a href="https://npmjs.org/package/sdof" title="View this project on NPM"><img src="https://img.shields.io/npm/v/sdof.svg" alt="NPM version" /></a></span>
+
+
+## Python API
+
+```python
+from sdof import integrate, peaks, spectrum
+
+m  = 1.0
+c  = 1.0
+k  = 2.0
+f  = np.sin(np.linspace(0, 5*np.pi, 100))
+dt = 5*np.pi/100
+
+u_max, v_max, a_max =  peaks(m, c, k, f, dt)
+
+u, v, a    = integrate(m, c, k, f, dt)
+
+Su, Sv, Sa =  spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02, 3.0, 100))
+```
+
+## Integrator (Reproduced from OpenSees docs)
+
+<table>
+<tbody>
+<tr class="odd">
+<td><p><code class="parameter-table-variable">alphaM</code></p></td>
+<td><p>$\alpha_M$ factor</p></td>
+</tr>
+<tr class="even">
+<td><p><code class="parameter-table-variable">alphaF</code></p></td>
+<td><p>$\alpha_F$ factor</p></td>
+</tr>
+<tr class="odd">
+<td><p><code class="parameter-table-variable">gamma</code></p></td>
+<td><p>$\gamma$ factor</p></td>
+</tr>
+<tr class="even">
+<td><p><code class="parameter-table-variable">beta</code></p></td>
+<td><p>$\beta$ factor</p></td>
+</tr>
+</tbody>
+</table>
+
+<ol>
+<li>$\alpha_F$ and
+  $\alpha_M$ are defined differently that in the
+  paper, we use $\alpha_F = (1-\alpha_f)$ and
+  $\alpha_M=(1-\gamma_m)$ where
+  $\alpha_f$ and $\alpha_m$
+  are those used in the paper.</li>
+
+<li>Like Newmark and other implicit schemes, the unconditional
+  stability of this method applies to linear problems. There are no
+  results showing stability of this method over the wide range of
+  nonlinear problems that potentially exist. Experience indicates that the
+  time step for implicit schemes in nonlinear situations can be much
+  greater than those for explicit schemes.</li>
+
+<li>$\alpha_M = 1.0, \alpha_F = 1.0$ produces the Newmark Method.</li>
+<li>$\alpha_M = 1.0$ corresponds to the HHT method.</li>
+<li>The method is second-order accurate provided $\gamma = \dfrac{1}{2} + \alpha_M - \alpha_F$</li>
+<li>The method is unconditionally stable provided $\alpha_M \ge \alpha_F \ge \dfrac{1}{2}, \quad \beta \ge \dfrac{1}{4} +\dfrac{1}{2}(\gamma_M - \gamma_F)$</li>
+
+<li>$\gamma$ and $\beta$
+  are optional. The default values ensure the method is unconditionally
+  stable, second order accurate and high frequency dissipation is
+  maximized.</li>
+</ol>
+<p>The defaults are:</p>
+<dl>
+<dt></dt>
+<dd>
+
+$$\gamma = \dfrac{1}{2} + \gamma_M - \gamma_F$$
+
+</dd>
+</dl>
+<p>and</p>
+<dl>
+<dt></dt>
+<dd>
+
+$$\beta = \dfrac{1}{4}(1 + \gamma_M - \gamma_F)^2$$
+
+</dd>
+</dl>
+
+### Theory
+
+The generalized $\alpha$ method is a one
+step implicit method for solving the transient problem which attempts to
+increase the amount of numerical damping present without degrading the order of
+accuracy. In the HHT method, the same Newmark approximations are used:
+
+<dl>
+<dt></dt>
+<dd>
+
+$$U_{t+\Delta t} = U_t + \Delta t \dot U_t + [(0.5 - \beta)
+\Delta t^2] \ddot U_t + [\beta \Delta t^2] \ddot U_{t+\Delta t}$$
+
+</dd>
+</dl>
+<dl>
+<dt></dt>
+<dd>
+
+$$\dot U_{t+\Delta t} = \dot U_t + [(1-\gamma)\Delta t] \ddot
+U_t + [\gamma \Delta t ] \ddot U_{t+\Delta t} $$
+
+</dd>
+</dl>
+<p>but the time-discrete momentum equation is modified:</p>
+
+$$R_{t + \alpha_M \Delta t} = F_{t+\Delta t}^{ext} - M \ddot
+U_{t + \alpha_M \Delta t} - C \dot U_{t+\alpha_F \Delta t} -
+F^{int}(U_{t + \alpha_F \Delta t})
+$$
+
+where the displacements and velocities at the intermediate point are
+given by:
+
+$$U_{t+ \alpha_F \Delta t} = (1 - \alpha_F) U_t + \alpha_F
+U_{t + \Delta t}$$
+
+$$\dot U_{t+\alpha_F \Delta t} = (1-\alpha_F) \dot U_t +
+\alpha_F \dot U_{t + \Delta t}$$
+
+$$\ddot U_{t+\alpha_M \Delta t} = (1-\alpha_M) \ddot U_t +
+\alpha_M \ddot U_{t + \Delta t}$$
+
+<p>Following the methods outlined for Newmarks method, linearization of
+the nonlinear momentum equation results in the following linear
+equations:</p>
+
+$$K_{t+\Delta t}^{*i} d U_{t+\Delta t}^{i+1} = R_{t+\Delta
+t}^i$$
+
+$$K_{t+\Delta t}^{*i} = \alpha_F K_t + \frac{\alpha_F
+\gamma}{\beta \Delta t} C_t + \frac{\alpha_M}{\beta \Delta t^2}
+M$$
+
+<p>and</p>
+
+$$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha
+F \Delta t}^{i-1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M
+\ddot U_{t+ \alpha M \Delta t}^{i-1}$$
+
+The linear equations are used to solve for 
+
+$$U_{t+\alpha_F \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$
+
+Once convergence has been achieved the displacements,
+velocities and accelerations at time $t + \Delta t$ can be computed.
+
+## Compiling
+
+The main integrator is implemented in standard C and can be compiled
+as either a Python extension, or Javascript library (via WASM).
+
+### Python
+
+```
+pip install .
+```
+
+### Javascript
+
+- Install `emscripten` from [here](https://emscripten.org/)
+- run `make`. This creates the following files:
+  - `dist/fsdof.wasm` - Web assembly - compiled library,
+  - `dist/fsdof.js` - interface to binary `fsdof.wasm`
+
+- to test, you can use Python to start an HTTP server in the current directory
+  as follows:
+  ```shell
+  python -m http.server .
+  ```
+
+
+## References
+
+<p>J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural
+   Dynamics with Improved Numerical Dissipation: The
+   Generalized - $\alpha$ Method" ASME Journal of
+   Applied Mechanics, 60, 371:375, 1993.</p>
+
+<hr />
+
+<p>Code Developed by: <span style="color:blue">fmk</span></p>
+
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: sdof Version: 0.0.5 Author-email: "Claudio M.
+Metadata-Version: 2.1 Name: sdof Version: 0.0.6 Summary: Lightning-fast
+integration of single degree-of-freedom systems. Author-email: "Claudio M.
 Perez" <50180406+claudioperez@users.noreply.github.com> Project-URL:
-repository, http://github.com/BRACE2/sdof Project-URL: documentation, https://
-brace2.github.io/sdof Keywords: seismic,earthquake Description-Content-Type:
-text/markdown # `sdof` Fast integration of single degree-of-freedom systems.
-This package solves scalar problems of the form $$ m \ddot{u} + c \dot{u} + k u
-= f(t) $$ Integration is carried out using the Generalized - $\alpha$ method.
-This is an implicit method that like the HHT method allows for high frequency
-energy dissipation and second order accuracy.
+repository, http://github.com/claudioperez/sdof Keywords: seismic,earthquake-
+engineering Description-Content-Type: text/markdown # `sdof` Lightning-fast
+integration of single degree-of-freedom systems. This package solves scalar
+differential equations of the form $$ m \ddot{u} + c \dot{u} + k u = f(t) $$
+Integration is carried out using a Generalized - $\alpha$ integrator that is
+implemented under the hood in highly optimized multi-threaded C code.
+Generalized - $\alpha$ is an implicit method that allows for high frequency
+energy dissipation and second order accuracy. With the right selection of
+parameters, the method can be specialized to the Hibert-Hughes-Taylor (HHT), or
+Newmark families of integration schemes.
 ===============================================================================
-[NPM_version] ## Compile ### Python ``` pip install . ``` ### Javascript -
-Install `emscripten` from [here](https://emscripten.org/) - run `make`. This
-creates the following files: - `dist/fsdof.wasm` - Web assembly - compiled
-library, - `dist/fsdof.js` - interface to binary `fsdof.wasm` - to test, you
-can use Python to start an HTTP server in the current directory as follows:
-```shell python -m http.server . ``` ## Python API ```python def peaks(m, c, k,
-f, dt): ... ``` ## Integrator (Reproduced from OpenSees docs)
+[NPM_version] ## Python API ```python from sdof import integrate, peaks,
+spectrum m = 1.0 c = 1.0 k = 2.0 f = np.sin(np.linspace(0, 5*np.pi, 100)) dt =
+5*np.pi/100 u_max, v_max, a_max = peaks(m, c, k, f, dt) u, v, a = integrate(m,
+c, k, f, dt) Su, Sv, Sa = spectrum(f, dt, damping=[0.02, 0.05], periods=(0.02,
+3.0, 100)) ``` ## Integrator (Reproduced from OpenSees docs)
 alphaM $\alpha_M$ factor
 alphaF $\alpha_F$ factor
 gamma  $\gamma$ factor
 beta   $\beta$ factor
    1. $\alpha_F$ and $\alpha_M$ are defined differently that in the paper, we
       use $\alpha_F = (1-\alpha_f)$ and $\alpha_M=(1-\gamma_m)$ where
       $\alpha_f$ and $\alpha_m$ are those used in the paper.
@@ -65,13 +67,20 @@
 {\alpha_M}{\beta \Delta t^2} M$$
 and
 $$R_{t+\Delta t}^i = F_{t + \Delta t}^{ext} - F(U_{t + \alpha F \Delta t}^{i-
 1})^{int} - C \dot U_{t+\alpha F \Delta t}^{i-1} - M \ddot U_{t+ \alpha M
 \Delta t}^{i-1}$$ The linear equations are used to solve for $$U_{t+\alpha_F
 \Delta t}, \dot U_{t + \alpha_F \Delta t} \ddot U_{t+ \alpha M \Delta t}$$ Once
 convergence has been achieved the displacements, velocities and accelerations
-at time $t + \Delta t$ can be computed. ## References
+at time $t + \Delta t$ can be computed. ## Compiling The main integrator is
+implemented in standard C and can be compiled as either a Python extension, or
+Javascript library (via WASM). ### Python ``` pip install . ``` ### Javascript
+- Install `emscripten` from [here](https://emscripten.org/) - run `make`. This
+creates the following files: - `dist/fsdof.wasm` - Web assembly - compiled
+library, - `dist/fsdof.js` - interface to binary `fsdof.wasm` - to test, you
+can use Python to start an HTTP server in the current directory as follows:
+```shell python -m http.server . ``` ## References
 J. Chung, G.M.Hubert. "A Time Integration Algorithm for Structural Dynamics
 with Improved Numerical Dissipation: The Generalized - $\alpha$ Method" ASME
 Journal of Applied Mechanics, 60, 371:375, 1993.
 ===============================================================================
 Code Developed by: fmk
```

