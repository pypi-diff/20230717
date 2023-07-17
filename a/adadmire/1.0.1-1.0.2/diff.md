# Comparing `tmp/adadmire-1.0.1.tar.gz` & `tmp/adadmire-1.0.2.tar.gz`

## Comparing `adadmire-1.0.1.tar` & `adadmire-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 adadmire-1.0.1/ex.py
--rw-r--r--   0        0        0    63488 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Feist_et_al/data_raw.xlsx
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Feist_et_al/levels.npy
--rw-r--r--   0        0        0     9728 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Feist_et_al/pheno.npy
--rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Feist_et_al/pheno_with_stimulations.xlsx
--rw-r--r--   0        0        0    39328 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Feist_et_al/scaled_data_raw.npy
--rw-r--r--   0        0        0   217728 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/data_na_scaled.npy
--rw-r--r--   0        0        0   310332 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/data_raw.xlsx
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/levels.npy
--rw-r--r--   0        0        0    19328 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/pheno.npy
--rw-r--r--   0        0        0    20483 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/pheno.xlsx
--rw-r--r--   0        0        0    19328 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/pheno_na.npy
--rw-r--r--   0        0        0   217728 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/scaled_data_raw.npy
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 adadmire-1.0.1/doc/contribute.md
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 adadmire-1.0.1/src/adadmire/__init__.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 adadmire-1.0.1/src/adadmire/apgpy.py
--rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 adadmire-1.0.1/src/adadmire/main.py
--rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 adadmire-1.0.1/src/adadmire/mgm.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adadmire-1.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 adadmire-1.0.1/LICENSE
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 adadmire-1.0.1/README.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 adadmire-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 adadmire-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    63488 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Feist_et_al/data_raw.xlsx
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Feist_et_al/levels.npy
+-rw-r--r--   0        0        0     9728 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Feist_et_al/pheno.npy
+-rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Feist_et_al/pheno_with_stimulations.xlsx
+-rw-r--r--   0        0        0    39328 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Feist_et_al/scaled_data_raw.npy
+-rw-r--r--   0        0        0   217728 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Higuera_et_al/data_na_scaled.npy
+-rw-r--r--   0        0        0   310332 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Higuera_et_al/data_raw.xlsx
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Higuera_et_al/levels.npy
+-rw-r--r--   0        0        0    19328 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Higuera_et_al/pheno.npy
+-rw-r--r--   0        0        0    20483 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Higuera_et_al/pheno.xlsx
+-rw-r--r--   0        0        0    19328 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Higuera_et_al/pheno_na.npy
+-rw-r--r--   0        0        0   217728 2020-02-02 00:00:00.000000 adadmire-1.0.2/data/Higuera_et_al/scaled_data_raw.npy
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 adadmire-1.0.2/doc/contribute.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 adadmire-1.0.2/src/adadmire/__init__.py
+-rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 adadmire-1.0.2/src/adadmire/apgpy.py
+-rw-r--r--   0        0        0    15138 2020-02-02 00:00:00.000000 adadmire-1.0.2/src/adadmire/main.py
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 adadmire-1.0.2/src/adadmire/mgm.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 adadmire-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 adadmire-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 adadmire-1.0.2/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 adadmire-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 adadmire-1.0.2/PKG-INFO
```

### Comparing `adadmire-1.0.1/data/Feist_et_al/data_raw.xlsx` & `adadmire-1.0.2/data/Feist_et_al/data_raw.xlsx`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.1/data/Feist_et_al/pheno.npy` & `adadmire-1.0.2/data/Feist_et_al/pheno.npy`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.1/data/Feist_et_al/pheno_with_stimulations.xlsx` & `adadmire-1.0.2/data/Feist_et_al/pheno_with_stimulations.xlsx`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.1/data/Feist_et_al/scaled_data_raw.npy` & `adadmire-1.0.2/data/Feist_et_al/scaled_data_raw.npy`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.1/data/Higuera_et_al/data_na_scaled.npy` & `adadmire-1.0.2/data/Higuera_et_al/data_na_scaled.npy`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.1/data/Higuera_et_al/data_raw.xlsx` & `adadmire-1.0.2/data/Higuera_et_al/data_raw.xlsx`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.1/data/Higuera_et_al/pheno.npy` & `adadmire-1.0.2/data/Higuera_et_al/pheno.npy`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.1/data/Higuera_et_al/pheno.xlsx` & `adadmire-1.0.2/data/Higuera_et_al/pheno.xlsx`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.1/data/Higuera_et_al/pheno_na.npy` & `adadmire-1.0.2/data/Higuera_et_al/pheno_na.npy`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.1/data/Higuera_et_al/scaled_data_raw.npy` & `adadmire-1.0.2/data/Higuera_et_al/scaled_data_raw.npy`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.1/doc/contribute.md` & `adadmire-1.0.2/doc/contribute.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# Contribute
-
-In case you have **questions**, **feature requests** or find any **bugs** in adadmire, please create a corresponding issue at [gitlab.spang-lab.de/bul38390/admire/issues](https://github.com/spang-lab/adadmire/issues).
-
-In case you want to **write code** for this package, please also create an [Issue](https://github.com/spang-lab/adadmire/issues) first, in which you describe your planned code contribution. After acceptance of your proposal by an active maintainer of the repository you will get permissions to create branches for this repository. After this, please follow the steps outlined in the following to create new versions of adadmire.
-
-🗒️Note: all following steps are based on <https://packaging.python.org/en/latest/tutorials/packaging-projects/>.
-
-⚠️Important: all commands mentioned in the following should be run from the root folder of this repository.
-
-1. **Make your code changes**
-2. **Increase the version** in [pyproject.toml](../pyproject.toml)
-3. **Build the package**:
-   * Run command `python -m pip install --upgrade build twine` to install modules [build](https://pypi.org/project/build/) and [twine](https://pypi.org/project/twine/) (required for building and uploading of packages) 
-   * Run command `python -m build` to generate pre-built version of your package (`dist/adadmire*.whl`) as well as a source version of your package (`dist/adadmire*.tar.gz`)
-4. **Upload to PyPI Test Server**: this step is optional and only required if you want to try out the upload and following installation.
-   * Run command `python -m twine upload --repository testpypi dist/*` to upload your package to [test.pypi.org](https://test.pypi.org/). **Important**: for this to work, you need to create an account at [test.pypi.org](https://test.pypi.org/) first! Please also note, that you need two separate accounts for [test.pypi.org](https://test.pypi.org/) and [pypi.org](https://pypi.org/).
-   * Check that your new version is listed at [test.pypi.org/project/adadmire](https://test.pypi.org/project/adadmire)
-   * Run command `python -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps adadmire` to check that your new version can be installed via pip
-5. **Upload to PyPI Production Server**
-   * Run command `python -m twine upload dist/*` to upload your package to [test.pypi.org](https://test.pypi.org/). **Important**: for this to work, you need to create an account at [pypi.org](https://pypi.org/) first! Please also note, that you need two separate accounts for [pypi.org](https://pypi.org/) and [test.pypi.org](https://test.pypi.org/).
-   * Check that your new version is listed at [pypi.org/project/adadmire](https://pypi.org/project/adadmire)
-   * Run command `python -m pip install --upgrade adadmire` to check that your new version can be installed via pip
-
-All above commands in short
-
-```bash
-python -m pip install --upgrade build twine wheel # Update packages
-rm dist/* # Clean dist folder
-python -m build # Build package. IMPORTANT: version updated in pyproject.toml?
-# IF POWERSHELL
-$whl=$(ls ./dist/adadmire-*-py3-none-any.whl).FullName
-python -m pip install $whl # Test installation locally
-# ELSE
-python -m pip install ./dist/adadmire-*-py3-none-any.whl
-# END IF
-python -m twine upload --repository testpypi dist/* # Upload to test server
-python -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps adadmire
-python -m twine upload dist/* # Upload to production server
-python -m pip install --upgrade adadmire # Test installation from server
-# IMPORTANT: do not forget to push your changes to Github as well ;)
-```
-
-## Tips and Tricks
-
-### Create a .pypirc file
-
-Create a [.pypirc](https://packaging.python.org/en/latest/specifications/pypirc/) file in your local home directory. This way you don't have to type your PyPI username and password each time. Mine looks as follows:
-
-```
-[testpypi]
-repository = https://test.pypi.org/legacy/
-username = <my_test_pypi_username>
-password = <my_test_pypi_password>
-
-[pypi]
-repository = https://upload.pypi.org/legacy/
-username = <my_pypi_username>
-password = <my_pypi_password>
-```
+# Contribute
+
+In case you have **questions**, **feature requests** or find any **bugs** in adadmire, please create a corresponding issue at [gitlab.spang-lab.de/bul38390/admire/issues](https://github.com/spang-lab/adadmire/issues).
+
+In case you want to **write code** for this package, please also create an [Issue](https://github.com/spang-lab/adadmire/issues) first, in which you describe your planned code contribution. After acceptance of your proposal by an active maintainer of the repository you will get permissions to create branches for this repository. After this, please follow the steps outlined in the following to create new versions of adadmire.
+
+🗒️Note: all following steps are based on <https://packaging.python.org/en/latest/tutorials/packaging-projects/>.
+
+⚠️Important: all commands mentioned in the following should be run from the root folder of this repository.
+
+1. **Make your code changes**
+2. **Increase the version** in [pyproject.toml](../pyproject.toml)
+3. **Build the package**:
+   * Run command `python -m pip install --upgrade build twine` to install modules [build](https://pypi.org/project/build/) and [twine](https://pypi.org/project/twine/) (required for building and uploading of packages) 
+   * Run command `python -m build` to generate pre-built version of your package (`dist/adadmire*.whl`) as well as a source version of your package (`dist/adadmire*.tar.gz`)
+4. **Upload to PyPI Test Server**: this step is optional and only required if you want to try out the upload and following installation.
+   * Run command `python -m twine upload --repository testpypi dist/*` to upload your package to [test.pypi.org](https://test.pypi.org/). **Important**: for this to work, you need to create an account at [test.pypi.org](https://test.pypi.org/) first! Please also note, that you need two separate accounts for [test.pypi.org](https://test.pypi.org/) and [pypi.org](https://pypi.org/).
+   * Check that your new version is listed at [test.pypi.org/project/adadmire](https://test.pypi.org/project/adadmire)
+   * Run command `python -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps adadmire` to check that your new version can be installed via pip
+5. **Upload to PyPI Production Server**
+   * Run command `python -m twine upload dist/*` to upload your package to [test.pypi.org](https://test.pypi.org/). **Important**: for this to work, you need to create an account at [pypi.org](https://pypi.org/) first! Please also note, that you need two separate accounts for [pypi.org](https://pypi.org/) and [test.pypi.org](https://test.pypi.org/).
+   * Check that your new version is listed at [pypi.org/project/adadmire](https://pypi.org/project/adadmire)
+   * Run command `python -m pip install --upgrade adadmire` to check that your new version can be installed via pip
+
+All above commands in short
+
+```bash
+python -m pip install --upgrade build twine wheel # Update packages
+rm dist/* # Clean dist folder
+python -m build # Build package. IMPORTANT: version updated in pyproject.toml?
+# IF POWERSHELL
+$whl=$(ls ./dist/adadmire-*-py3-none-any.whl).FullName
+python -m pip install $whl # Test installation locally
+# ELSE
+python -m pip install ./dist/adadmire-*-py3-none-any.whl
+# END IF
+python -m twine upload --repository testpypi dist/* # Upload to test server
+python -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps adadmire
+python -m twine upload dist/* # Upload to production server
+python -m pip install --upgrade adadmire # Test installation from server
+# IMPORTANT: do not forget to push your changes to Github as well ;)
+```
+
+## Tips and Tricks
+
+### Create a .pypirc file
+
+Create a [.pypirc](https://packaging.python.org/en/latest/specifications/pypirc/) file in your local home directory. This way you don't have to type your PyPI username and password each time. Mine looks as follows:
+
+```
+[testpypi]
+repository = https://test.pypi.org/legacy/
+username = <my_test_pypi_username>
+password = <my_test_pypi_password>
+
+[pypi]
+repository = https://upload.pypi.org/legacy/
+username = <my_pypi_username>
+password = <my_pypi_password>
+```
```

### Comparing `adadmire-1.0.1/src/adadmire/apgpy.py` & `adadmire-1.0.2/src/adadmire/apgpy.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-# Copyright (c) 2012-2013, Brendan O'Donoghue (bodonoghue85@gmail.com)
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions are met:
-#
-# 1. Redistributions of source code must retain the above copyright notice, this
-#    list of conditions and the following disclaimer.
-# 2. Redistributions in binary form must reproduce the above copyright notice,
-#    this list of conditions and the following disclaimer in the documentation
-#    and/or other materials provided with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
-# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
-# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-# POSSIBILITY OF SUCH DAMAGE.
-#
-# The views and conclusions contained in the software and documentation are those
-# of the authors and should not be interpreted as representing official policies,
-# either expressed or implied, of the FreeBSD Project, the Air Force Research
-# Laboratory, or the U.S. Government.
-
-
-# Note from Tobias Schmidt: this file contains source code from the package
-# apgpy (https://github.com/bodono/apgpy). Package apgpy is not available via
-# PyPI (https://pypi.org) and therefore cannot be resolved automatically by
-# pip. We include its source code directly within this package to make
-# installation via pip possible. This is explicictly allowed by the license of
-# apgpy (see above).
-from __future__ import print_function
-import numpy as np
-from functools import partial
-
-class IWrapper:
-    def dot(self, other):
-        raise NotImplementedError("Implement in subclass")
-
-    def __add__(self, other):
-        raise NotImplementedError("Implement in subclass")
-
-    def __sub__(self, other):
-        raise NotImplementedError("Implement in subclass")
-
-    def __mul__(self, scalar):
-        raise NotImplementedError("Implement in subclass")
-
-    def copy(self):
-        raise NotImplementedError("Implement in subclass")
-
-    def norm(self):
-        raise NotImplementedError("Implement in subclass")
-
-    @property
-    def data(self):
-        return self
-
-    __rmul__ = __mul__
-
-
-class NumpyWrapper(IWrapper):
-    def __init__(self, nparray):
-        self._nparray = nparray
-
-    def dot(self, other):
-        return np.inner(self.data, other.data)
-
-    def __add__(self, other):
-        return NumpyWrapper(self.data + other.data)
-
-    def __sub__(self, other):
-        return NumpyWrapper(self.data - other.data)
-
-    def __mul__(self, scalar):
-        return NumpyWrapper(self.data * scalar)
-
-    def copy(self):
-        return NumpyWrapper(np.copy(self.data))
-
-    def norm(self):
-        return np.linalg.norm(self.data)
-
-    @property
-    def data(self):
-        return self._nparray
-
-    __rmul__ = __mul__
-
-
-def npwrap(x):
-    if isinstance(x, np.ndarray):
-        return NumpyWrapper(x)
-    return x
-
-
-def npwrapfunc(f, *args):
-    return npwrap(f(*args))
-
-
-def solve(grad_f, prox_h, x_init,
-          max_iters=2500,
-          eps=1e-6,
-          alpha=1.01,
-          beta=0.5,
-          use_restart=True,
-          gen_plots=False,
-          quiet=False,
-          use_gra=False,
-          step_size=False,
-          fixed_step_size=False,
-          debug=False):
-
-    df = partial(npwrapfunc, grad_f)
-    ph = partial(npwrapfunc, prox_h)
-
-    x_init = npwrap(x_init)
-
-    x = x_init.copy()
-    y = x.copy()
-    g = df(y.data)
-    theta = 1.
-
-    if not step_size:
-        # barzilai-borwein step-size initialization:
-        t = 1. / g.norm()
-        x_hat = x - t * g
-        g_hat = df(x_hat.data)
-        t = abs((x - x_hat).dot(g - g_hat) / (g - g_hat).norm() ** 2)
-    else:
-        t = step_size
-
-    if gen_plots:
-        errs = np.zeros(max_iters)
-
-    k = 0
-    err1 = np.nan
-    iter_str = 'iter num %i, norm(Gk)/(1+norm(xk)): %1.2e, step-size: %1.2e'
-    for k in range(max_iters):
-
-        if not quiet and k % 100 == 0:
-            print(iter_str % (k, err1, t))
-
-        x_old = x.copy()
-        y_old = y.copy()
-
-        x = y - t * g
-
-        if prox_h:
-            x = ph(x.data, t)
-
-        err1 = (y - x).norm() / (1 + x.norm()) / t
-
-        if gen_plots:
-            errs[k] = err1
-
-        if err1 < eps:
-            break
-
-        if not use_gra:
-            theta = 2. / (1 + np.sqrt(1 + 4 / (theta ** 2)))
-        else:
-            theta = 1.
-
-        if not use_gra and use_restart and (y - x).dot(x - x_old) > 0:
-            if debug:
-                print('restart, dg = %1.2e' % (y - x).dot(x - x_old))
-            x = x_old.copy()
-            y = x.copy()
-            theta = 1.
-        else:
-            y = x + (1 - theta) * (x - x_old)
-
-        g_old = g.copy()
-        g = df(y.data)
-
-        # tfocs-style backtracking:
-        if not fixed_step_size:
-            t_old = t
-            t_hat = 0.5 * ((y - y_old).norm() ** 2) / \
-                abs((y - y_old).dot(g_old - g))
-            t = min(alpha * t, max(beta * t, t_hat))
-            if debug:
-                if t_old > t:
-                    print('back-track, t = %1.2e, t_old = %1.2e, t_hat = %1.2e' %
-                          (t, t_old, t_hat))
-
-    if not quiet:
-        print(iter_str % (k, err1, t))
-        print('terminated')
-    if gen_plots:
-        import matplotlib.pyplot as plt
-        errs = errs[1:k]
-        plt.figure()
-        plt.semilogy(errs[1:k])
-        plt.xlabel('iters')
-        plt.title('||Gk||/(1+||xk||)')
-        plt.draw()
-
-    return x.data
+# Copyright (c) 2012-2013, Brendan O'Donoghue (bodonoghue85@gmail.com)
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are met:
+#
+# 1. Redistributions of source code must retain the above copyright notice, this
+#    list of conditions and the following disclaimer.
+# 2. Redistributions in binary form must reproduce the above copyright notice,
+#    this list of conditions and the following disclaimer in the documentation
+#    and/or other materials provided with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
+# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+# POSSIBILITY OF SUCH DAMAGE.
+#
+# The views and conclusions contained in the software and documentation are those
+# of the authors and should not be interpreted as representing official policies,
+# either expressed or implied, of the FreeBSD Project, the Air Force Research
+# Laboratory, or the U.S. Government.
+
+
+# Note from Tobias Schmidt: this file contains source code from the package
+# apgpy (https://github.com/bodono/apgpy). Package apgpy is not available via
+# PyPI (https://pypi.org) and therefore cannot be resolved automatically by
+# pip. We include its source code directly within this package to make
+# installation via pip possible. This is explicictly allowed by the license of
+# apgpy (see above).
+from __future__ import print_function
+import numpy as np
+from functools import partial
+
+class IWrapper:
+    def dot(self, other):
+        raise NotImplementedError("Implement in subclass")
+
+    def __add__(self, other):
+        raise NotImplementedError("Implement in subclass")
+
+    def __sub__(self, other):
+        raise NotImplementedError("Implement in subclass")
+
+    def __mul__(self, scalar):
+        raise NotImplementedError("Implement in subclass")
+
+    def copy(self):
+        raise NotImplementedError("Implement in subclass")
+
+    def norm(self):
+        raise NotImplementedError("Implement in subclass")
+
+    @property
+    def data(self):
+        return self
+
+    __rmul__ = __mul__
+
+
+class NumpyWrapper(IWrapper):
+    def __init__(self, nparray):
+        self._nparray = nparray
+
+    def dot(self, other):
+        return np.inner(self.data, other.data)
+
+    def __add__(self, other):
+        return NumpyWrapper(self.data + other.data)
+
+    def __sub__(self, other):
+        return NumpyWrapper(self.data - other.data)
+
+    def __mul__(self, scalar):
+        return NumpyWrapper(self.data * scalar)
+
+    def copy(self):
+        return NumpyWrapper(np.copy(self.data))
+
+    def norm(self):
+        return np.linalg.norm(self.data)
+
+    @property
+    def data(self):
+        return self._nparray
+
+    __rmul__ = __mul__
+
+
+def npwrap(x):
+    if isinstance(x, np.ndarray):
+        return NumpyWrapper(x)
+    return x
+
+
+def npwrapfunc(f, *args):
+    return npwrap(f(*args))
+
+
+def solve(grad_f, prox_h, x_init,
+          max_iters=2500,
+          eps=1e-6,
+          alpha=1.01,
+          beta=0.5,
+          use_restart=True,
+          gen_plots=False,
+          quiet=False,
+          use_gra=False,
+          step_size=False,
+          fixed_step_size=False,
+          debug=False):
+
+    df = partial(npwrapfunc, grad_f)
+    ph = partial(npwrapfunc, prox_h)
+
+    x_init = npwrap(x_init)
+
+    x = x_init.copy()
+    y = x.copy()
+    g = df(y.data)
+    theta = 1.
+
+    if not step_size:
+        # barzilai-borwein step-size initialization:
+        t = 1. / g.norm()
+        x_hat = x - t * g
+        g_hat = df(x_hat.data)
+        t = abs((x - x_hat).dot(g - g_hat) / (g - g_hat).norm() ** 2)
+    else:
+        t = step_size
+
+    if gen_plots:
+        errs = np.zeros(max_iters)
+
+    k = 0
+    err1 = np.nan
+    iter_str = 'iter num %i, norm(Gk)/(1+norm(xk)): %1.2e, step-size: %1.2e'
+    for k in range(max_iters):
+
+        if not quiet and k % 100 == 0:
+            print(iter_str % (k, err1, t))
+
+        x_old = x.copy()
+        y_old = y.copy()
+
+        x = y - t * g
+
+        if prox_h:
+            x = ph(x.data, t)
+
+        err1 = (y - x).norm() / (1 + x.norm()) / t
+
+        if gen_plots:
+            errs[k] = err1
+
+        if err1 < eps:
+            break
+
+        if not use_gra:
+            theta = 2. / (1 + np.sqrt(1 + 4 / (theta ** 2)))
+        else:
+            theta = 1.
+
+        if not use_gra and use_restart and (y - x).dot(x - x_old) > 0:
+            if debug:
+                print('restart, dg = %1.2e' % (y - x).dot(x - x_old))
+            x = x_old.copy()
+            y = x.copy()
+            theta = 1.
+        else:
+            y = x + (1 - theta) * (x - x_old)
+
+        g_old = g.copy()
+        g = df(y.data)
+
+        # tfocs-style backtracking:
+        if not fixed_step_size:
+            t_old = t
+            t_hat = 0.5 * ((y - y_old).norm() ** 2) / \
+                abs((y - y_old).dot(g_old - g))
+            t = min(alpha * t, max(beta * t, t_hat))
+            if debug:
+                if t_old > t:
+                    print('back-track, t = %1.2e, t_old = %1.2e, t_hat = %1.2e' %
+                          (t, t_old, t_hat))
+
+    if not quiet:
+        print(iter_str % (k, err1, t))
+        print('terminated')
+    if gen_plots:
+        import matplotlib.pyplot as plt
+        errs = errs[1:k]
+        plt.figure()
+        plt.semilogy(errs[1:k])
+        plt.xlabel('iters')
+        plt.title('||Gk||/(1+||xk||)')
+        plt.draw()
+
+    return x.data
```

### Comparing `adadmire-1.0.1/src/adadmire/main.py` & `adadmire-1.0.2/src/adadmire/main.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,394 +1,394 @@
-from scipy.stats import norm
-from adadmire.mgm import *
-import numpy as np
-import random
-from sklearn.metrics.pairwise import nan_euclidean_distances
-
-def pred_continuous(B, Rho, alphap, D_pred, X_pred):
-    ind = np.array(D_pred) == 1
-    # for all features sum over rho (sum rho_sj(y_j))
-    r_sum = np.array([])
-    for k in range(0, Rho.shape[1]):
-        tmp = sum(Rho[ind, k])
-        r_sum = np.append(r_sum, tmp)
-    # calculate scalar product beta*x
-    x_b = np.array([])
-    for k in range(0, B.shape[0]):
-        tmp = np.dot(B[k], X_pred)
-        tmp = tmp - B[k, k]*X_pred[k]
-        x_b = np.append(x_b, tmp)
-
-    x_hat = -(alphap + r_sum + x_b) / (0.5 * np.diag(B))
-    return (x_hat)
-
-
-def pred_discrete(Rho, X_pred, D_pred, alphaq, Phi, levels, p):
-    levels = levels.flatten()
-    lSum = [0]
-    lSum.extend(levels)
-    lSum = np.cumsum(lSum)
-    q = len(levels)
-    q0 = np.sum(levels)
-    prob_cat = np.array([])
-    for j in range(q):
-        D_del = np.array(D_pred)
-        D_del[lSum[j]:lSum[j + 1]] = 0.
-        t1 = Rho[lSum[j]:lSum[j + 1], :] @ X_pred.reshape((p, 1))
-        t2 = alphaq[lSum[j]:lSum[j + 1]].reshape((levels[j], 1))
-        t3 = Phi[lSum[j]:lSum[j + 1], :] @ D_del.reshape((q0, 1))
-        denom = np.sum(np.exp(t1 + t2 + t3))
-        numer = np.exp(t1 + t2 + t3)
-        tmp = numer.flatten() / denom
-        prob_cat = np.append(prob_cat, tmp)
-    return (prob_cat)
-
-
-def calc_mean(X, D):
-    mean = np.zeros(X.shape)
-    for i in range(X.shape[0]):
-        ind = np.where((D == D[i]).all(axis=1))
-        mean[i] = np.mean(X[ind], axis=0)
-    return (mean)
-
-
-def loo_cv_cor(X, D, levels, lam_seq, oIterations=10000, oTol=1e-6, t=0.05):
-    means = calc_mean(X, D)
-    MSE = 2e10
-    MSE_old = 2e10
-    j = 0
-    X_hat = np.zeros(shape=X.shape)
-    X_hat_cor_xp = np.zeros(shape=X.shape)
-    D_hat = np.zeros(shape=D.shape)
-    D_hat_cor_xp = np.zeros(shape=D.shape)
-    prob_cont = np.zeros(shape=X.shape)
-    Var = np.zeros(shape=X.shape)
-    MSE_seq = np.array([])
-    lam_opt = np.array([lam_seq[0]])
-    lam_opt_old = np.array([lam_seq[0]])
-    while ((MSE_old >= MSE) and (j < np.size(lam_seq))):
-        lam_opt_old = np.copy(lam_opt)
-        MSE_old = np.copy(MSE)
-        X_hat_cor_xp_old = np.copy(X_hat_cor_xp)
-        D_hat_old = np.copy(D_hat)
-        D_hat_cor_xp_old = np.copy(D_hat_cor_xp)
-        prob_cont_old = np.copy(prob_cont)
-        Var_old = np.copy(Var)
-        lambda_t = np.array([lam_seq[j]])
-        # loop over all samples
-        for i in range(X.shape[0]):
-            # sample which has to be predicted
-            print('Sample Nummer:', i)
-            X_pred = X[i]
-            D_pred = D[i]
-            # rest of the samples
-            X_red = np.delete(X, i, 0)
-            D_red = np.delete(D, i, 0)
-            # learn models for all other samples and current lambda
-            Res = Fit_MGM(X_red, D_red, levels, lambda_t,
-                          oIterations, eps=oTol)
-            Res = Res[0]
-            # predict sample which has been left out
-            B = Res[0][0]
-            B = B + np.transpose(B)
-            Phi = Res[0][2]
-            Phi = Phi + np.transpose(Phi)
-            alphap = Res[0][3]
-            Rho = Res[0][1]
-            alphaq = Res[0][4]
-            p = B.shape[0]
-            # predict sample
-            x_hat = pred_continuous(B, Rho, alphap, D_pred, X_pred)
-            # calculate probabilities
-            dev = 0.5 * abs(np.diag(B))
-            eps = abs(X_pred - x_hat)
-            p_val = 2 * norm.cdf(x_hat - eps, loc=x_hat,
-                                 scale=np.sqrt(1 / dev))
-            # if p_val for data point < t replace it in other predictions by mean of feature
-            x_cor = np.where(p_val < t, means[i], X_pred)
-            # get discrete predictions
-            d_hat = pred_discrete(Rho, X_pred, D_pred, alphaq, Phi, levels, p)
-            # if probability of discrete data point < t change state to most likely one
-            d_hat_cor = np.copy(d_hat)
-            levelSum = np.cumsum(levels)
-            levelSum = np.insert(levelSum, 0, 0)
-            d_var = 0
-            D_pred_cor = np.copy(D_pred)
-            for k in range(len(d_hat)):
-                if k == levelSum[d_var]:
-                    d_var = d_var + 1
-                if D_pred[k] == 1 and d_hat[k] < t:
-                    tmp = np.zeros(
-                        shape=len(d_hat[levelSum[d_var-1]:levelSum[d_var]]))
-                    tmp[np.where(d_hat[levelSum[d_var-1]:levelSum[d_var]]
-                                 == max(d_hat[levelSum[d_var-1]:levelSum[d_var]]))] = 1
-                    D_pred_cor[levelSum[d_var-1]:levelSum[d_var]] = tmp
-            # predict cat again using adjusted states
-
-            # predict continuous and discrete again using corrected states and values
-            x_hat_cor_xp = pred_continuous(B, Rho, alphap, D_pred_cor, x_cor)
-            d_hat_cor_xp = pred_discrete(
-                Rho, x_cor, D_pred_cor, alphaq, Phi, levels, p)
-            X_hat[i] = x_hat
-            X_hat_cor_xp[i] = x_hat_cor_xp
-            D_hat[i] = d_hat
-            D_hat_cor_xp[i] = d_hat_cor_xp
-            eps = abs(X_pred - x_hat)
-            p_val = 2 * norm.cdf(x_hat - eps, loc=x_hat,
-                                 scale=np.sqrt(1 / dev))
-            prob_cont[i] = p_val
-            Var[i] = dev
-        MSE = np.mean((X_hat - X)**2)
-        MSE_seq = np.append(MSE_seq, MSE)
-        lam_opt = lambda_t
-        j = j+1
-
-    if (MSE < MSE_old):
-        print('Minimum not found, choose smaller Lam sequence')
-    if (np.size(lam_seq) == 1): # in case only one lambda submitted
-        X_hat_cor_xp_old = np.copy(X_hat_cor_xp)
-        D_hat_cor_xp_old = np.copy(D_hat_cor_xp)
-        prob_cont_old = np.copy(prob_cont)
-        Var_old = np.copy(Var)
-
-    return (prob_cont_old, Var_old, lam_opt_old, X_hat_cor_xp_old, D_hat_cor_xp_old)
-
-
-def get_threshold_continuous(X, X_hat, dev):
-    random.seed(671)
-    # calculate random scores from estimated distribution
-    # first draw random realizations from estimated distribution with 100 repetitions
-    mu = X_hat.flatten(order='F')
-    dev = dev.flatten(order='F')
-    X_flat = X.flatten(order='F')
-    random_scores = np.zeros(shape=(mu.shape[0], 100))
-    for i in range(mu.shape[0]):
-        tmp = norm.rvs(loc=mu[i], scale=np.sqrt(1/dev[i]), size=100)
-        random_scores[i, ] = np.divide(np.abs(tmp - mu[i]), np.sqrt(1/dev[i]))
-
-    # rank random scores for each repetition separately
-    random_scores = np.sort(random_scores, axis=0)
-    # average over all repetitions
-    random_scores = np.flip(np.mean(random_scores, axis=1))
-    # get observed scores
-    observed_scores = np.abs(mu - X_flat)/np.sqrt(1/dev)
-    observed_scores_sorted = np.flip(np.sort(observed_scores))
-    # determine threshold
-    threshold = random_scores[np.where(
-        random_scores >= observed_scores_sorted)][0]
-    # and number of detected anomalies
-    n_ano = np.sum(observed_scores >= threshold)
-    # correct anomalies found in X with predictions X_hat
-    observed_scores = np.reshape(observed_scores, X.shape, 'F')
-    X_cor = np.where(observed_scores <= threshold, X, X_hat)
-    ano_index = np.transpose((observed_scores >= threshold).nonzero())
-
-    return (X_cor, threshold, n_ano, ano_index)
-
-
-def get_threshold_discrete(D, levels, D_hat):
-    random.seed(321)
-    # first calculate observed scores
-    # get index of "true" state
-    ind = np.where(D == 1)
-    p = D_hat[ind]
-    observed_scores = -np.log(p)
-    observed_scores_sorted = np.flip(np.sort(observed_scores))
-    # now sample states according to estimated distribution with 100 repetitions
-    random_scores = [np.zeros(shape=(D.shape[0], 100))
-                     for i in range(len(levels))]
-    start = 0
-    for i in range(len(levels)):
-        end = int(start + levels[i])
-        prob = D_hat[:, start:end]
-
-        state_index = np.arange(levels[i])
-        for j in range(D.shape[0]):
-            random_obs = np.random.choice(state_index, p=prob[j], size=100)
-            random_scores[i][j] = -np.log(prob[j, random_obs])
-        start = end
-
-    # concatenate and average random scores
-    random_scores = np.concatenate((random_scores), axis=0)
-    random_scores = np.sort(random_scores, axis=0)
-    random_scores = np.flip(np.mean(random_scores, axis=1))
-    # determine threshold
-    threshold = random_scores[np.where(
-        random_scores >= observed_scores_sorted)][0]
-    # and number of detected anomalies
-    n_ano = np.sum(observed_scores >= threshold)
-    # get position of detected anomalies
-    # first array corresponds to sample, second array to feature position
-    pos = np.array([ind[0][np.where(observed_scores >= threshold)],
-                   ind[1][np.where(observed_scores >= threshold)]])
-    return (n_ano, threshold, pos)
-
-def transform_data(
-        X
-):
-    X_trans  = (X-X.min(axis = 0))/(X.max(axis=0) - X.min(axis=0))
-    return(X_trans)
-
-def transform_back(
-        X,
-        X_scaled
-):
-    X_back = X_scaled * (X.max(axis=0) - X.min(axis=0)) + X.min(axis=0)
-    return(X_back)
-
-def rel_dev(
-        x, 
-        org):
-    return(abs((x-org)/org))
-
-def place_anomalies_continuous(
-        X,
-        n_ano,
-        epsilon,
-        positive = False
-):
-    random.seed(987)
-    # first transform data feature-wise to [0,1]
-    X_scaled = transform_data(X)
-    # Calculate 15% border
-    Z = (0.15*X) / (X.max(axis=0) - X.min(axis=0))
-    ano = [np.copy(X) for i in range(len(epsilon))]
-    change = np.copy(X)
-    dirm = np.copy(X)
-    # for each element in X sample shift
-    for i in range(X.shape[0]):
-        for j in range(X.shape[1]):
-            lc = random.uniform( Z[i,j],(Z[i,j]+X_scaled[i,j]))
-            uc = random.uniform( Z[i,j],(1+Z[i,j]-X_scaled[i,j]))
-            # decide whether lower or upper change
-            dir = random.randint(0,1)
-            if dir == 1:
-                for k in range(len(epsilon)):
-                    ano[k][i,j] = X_scaled[i,j] + epsilon[k]*uc
-                    change[i,j] = uc
-                    dirm[i,j] = 1
-            else:
-                for k in range(len(epsilon)):
-                    ano[k][i,j] = X_scaled[i,j] - epsilon[k] * lc
-                    change[i,j] = lc
-                    dirm[i,j] = 0
-    # transform anomalies back
-    ano_retrans = [transform_back(X, tmp) for tmp in ano]
-    # place anomalies
-    position = np.array([])
-    position.shape = (0,2)
-    X_ano = [np.copy(X) for i in range(len(epsilon))]
-    k = 0
-    while k < n_ano:
-        # sample position
-        row = random.randint(0, (X.shape[0]-1))
-        col = random.randint(0, (X.shape[1]-1))
-        # first check if anomaly already has been placed at that position
-        if sum((position == [[row,col]]).all(axis = 1)) == 0:
-            # check if introduced anomaly > 15% deviation (only for epsilon < 1 relevant) and anomaly still positiv 
-            if positive == True:
-                if rel_dev(ano_retrans[0][row,col],X[row,col]) > 0.15 and ano_retrans[(len(epsilon)-1)][row,col] > 0:
-                    k = k+1
-                    position = np.append(position, [[row, col]], axis = 0)
-                    for l in range(len(epsilon)):
-                        X_ano[l][row, col] = ano_retrans[l][row,col]
-            else :
-                if rel_dev(ano_retrans[0][row,col],X[row,col]) > 0.15:
-                    k = k+1
-                    position = np.append(position, [[row, col]], axis = 0)
-                    for l in range(len(epsilon)):
-                        X_ano[l][row, col] = ano_retrans[l][row,col]
-    return(X_ano, position)
-
-def impute(
-        X,
-        D,
-        levels, 
-        lam_seq,
-        oIterations = 10000, 
-        oTol = 1e-6 ):
-    # calculate Euclidean distance of all samples to each other
-    # ignore NaN values
-    dist = nan_euclidean_distances(X,X)
-    np.fill_diagonal(dist, np.inf)
-    X_preimp = np.copy(X)
-    D_preimp = np.copy(D)
-
-    for i in range(X.shape[0]):
-        ind_disc = np.where(np.isnan(D[i]))[0]
-        ind_cont = np.where(np.isnan(X[i]))[0]
-        # impute continuous with value of closest sample
-        for j in ind_cont:
-            sample = np.argmin(dist[i])
-            dist_new = np.copy(dist)
-            while np.isnan(X[sample,j]): # check if value for imputation is also nan
-                dist_new[i,sample] = np.inf
-                sample = np.argmin(dist_new[i]) # use second, third, .. closest sample
-            X_preimp[i,j] = X[sample,j]
-        # same for discrete 
-        for j in ind_disc:
-            sample = np.argmin(dist[i])
-            dist_new = np.copy(dist)
-            while np.isnan(D[sample,j]): # check if value for imputation is also nan
-                dist_new[i,sample] = np.inf
-                sample = np.argmin(dist_new[i]) # use second, third, .. closest sample
-            D_preimp[i,j] = D[sample,j]
-
-    # for each lam in lam_seq fit MGM on all data
-    # calculate MSE
-
-    MSE = 2e10
-    MSE_old = 2e10
-    j = 0
-    X_hat = np.zeros(shape=X.shape)
-    D_hat = np.zeros(shape=D.shape)
-    MSE_seq = np.array([])
-    lam_opt = np.array([lam_seq[0]])
-    lam_opt_old = np.array([lam_seq[0]])
-    while ((MSE_old >= MSE) and (j < np.size(lam_seq))):
-        lam_opt_old = np.copy(lam_opt)
-        MSE_old = np.copy(MSE)
-        X_hat_old = np.copy(X_hat)
-        D_hat_old = np.copy(D_hat)
-        lambda_t = np.array([lam_seq[j]])
-        # fit model on all samples
-        Res = Fit_MGM(X_preimp, D_preimp, levels, lambda_t, oIterations, eps=oTol)
-        Res = Res[0]
-        B = Res[0][0]
-        B = B + np.transpose(B)
-        Phi = Res[0][2]
-        Phi = Phi + np.transpose(Phi)
-        alphap = Res[0][3]
-        Rho = Res[0][1]
-        alphaq = Res[0][4]
-        p = B.shape[0]
-        # loop over all samples
-        for i in range(X.shape[0]):
-            X_pred = X_preimp[i]
-            D_pred = D_preimp[i]
-            # predict sample
-            x_hat = pred_continuous(B, Rho, alphap, D_pred, X_pred)
-            # get discrete predictions
-            d_hat = pred_discrete(Rho, X_pred, D_pred, alphaq, Phi, levels,p)
-            levelSum = np.cumsum(levels)
-            levelSum = np.insert(levelSum, 0, 0)
-            d_var = 0
-            d_hat_state = np.copy(D_pred)
-            for k in range(len(d_hat)):
-                if k == levelSum[d_var]:
-                    d_var = d_var + 1
-                    tmp = np.zeros(shape=len(d_hat[levelSum[d_var-1]:levelSum[d_var]]))
-                    tmp[np.where(d_hat[levelSum[d_var-1]:levelSum[d_var]] == max(d_hat[levelSum[d_var-1]:levelSum[d_var]]))] = 1
-                    d_hat_state[levelSum[d_var-1]:levelSum[d_var]] = tmp
-            X_hat[i] = x_hat
-            D_hat[i] = d_hat_state
-        MSE = np.mean((X_hat - X_preimp)**2)
-        MSE_seq = np.append(MSE_seq, MSE)
-        lam_opt = lambda_t
-        j = j+1
-    ind_cont = np.where(np.isnan(X))
-    ind_disc = np.where(np.isnan(D))
-    X_imp = np.copy(X)
-    X_imp[ind_cont] = X_hat_old[ind_cont]
-    D_imp = np.copy(D)
-    D_imp[ind_disc] = D_hat_old[ind_disc]
-    return(X_imp, D_imp, lam_opt_old)
+from scipy.stats import norm
+from adadmire.mgm import *
+import numpy as np
+import random
+from sklearn.metrics.pairwise import nan_euclidean_distances
+
+def pred_continuous(B, Rho, alphap, D_pred, X_pred):
+    ind = np.array(D_pred) == 1
+    # for all features sum over rho (sum rho_sj(y_j))
+    r_sum = np.array([])
+    for k in range(0, Rho.shape[1]):
+        tmp = sum(Rho[ind, k])
+        r_sum = np.append(r_sum, tmp)
+    # calculate scalar product beta*x
+    x_b = np.array([])
+    for k in range(0, B.shape[0]):
+        tmp = np.dot(B[k], X_pred)
+        tmp = tmp - B[k, k]*X_pred[k]
+        x_b = np.append(x_b, tmp)
+
+    x_hat = -(alphap + r_sum + x_b) / (0.5 * np.diag(B))
+    return (x_hat)
+
+
+def pred_discrete(Rho, X_pred, D_pred, alphaq, Phi, levels, p):
+    levels = levels.flatten()
+    lSum = [0]
+    lSum.extend(levels)
+    lSum = np.cumsum(lSum)
+    q = len(levels)
+    q0 = np.sum(levels)
+    prob_cat = np.array([])
+    for j in range(q):
+        D_del = np.array(D_pred)
+        D_del[lSum[j]:lSum[j + 1]] = 0.
+        t1 = Rho[lSum[j]:lSum[j + 1], :] @ X_pred.reshape((p, 1))
+        t2 = alphaq[lSum[j]:lSum[j + 1]].reshape((levels[j], 1))
+        t3 = Phi[lSum[j]:lSum[j + 1], :] @ D_del.reshape((q0, 1))
+        denom = np.sum(np.exp(t1 + t2 + t3))
+        numer = np.exp(t1 + t2 + t3)
+        tmp = numer.flatten() / denom
+        prob_cat = np.append(prob_cat, tmp)
+    return (prob_cat)
+
+
+def calc_mean(X, D):
+    mean = np.zeros(X.shape)
+    for i in range(X.shape[0]):
+        ind = np.where((D == D[i]).all(axis=1))
+        mean[i] = np.mean(X[ind], axis=0)
+    return (mean)
+
+
+def loo_cv_cor(X, D, levels, lam_seq, oIterations=10000, oTol=1e-6, t=0.05):
+    means = calc_mean(X, D)
+    MSE = 2e10
+    MSE_old = 2e10
+    j = 0
+    X_hat = np.zeros(shape=X.shape)
+    X_hat_cor_xp = np.zeros(shape=X.shape)
+    D_hat = np.zeros(shape=D.shape)
+    D_hat_cor_xp = np.zeros(shape=D.shape)
+    prob_cont = np.zeros(shape=X.shape)
+    Var = np.zeros(shape=X.shape)
+    MSE_seq = np.array([])
+    lam_opt = np.array([lam_seq[0]])
+    lam_opt_old = np.array([lam_seq[0]])
+    while ((MSE_old >= MSE) and (j < np.size(lam_seq))):
+        lam_opt_old = np.copy(lam_opt)
+        MSE_old = np.copy(MSE)
+        X_hat_cor_xp_old = np.copy(X_hat_cor_xp)
+        D_hat_old = np.copy(D_hat)
+        D_hat_cor_xp_old = np.copy(D_hat_cor_xp)
+        prob_cont_old = np.copy(prob_cont)
+        Var_old = np.copy(Var)
+        lambda_t = np.array([lam_seq[j]])
+        # loop over all samples
+        for i in range(X.shape[0]):
+            # sample which has to be predicted
+            print('Sample Nummer:', i)
+            X_pred = X[i]
+            D_pred = D[i]
+            # rest of the samples
+            X_red = np.delete(X, i, 0)
+            D_red = np.delete(D, i, 0)
+            # learn models for all other samples and current lambda
+            Res = Fit_MGM(X_red, D_red, levels, lambda_t,
+                          oIterations, eps=oTol)
+            Res = Res[0]
+            # predict sample which has been left out
+            B = Res[0][0]
+            B = B + np.transpose(B)
+            Phi = Res[0][2]
+            Phi = Phi + np.transpose(Phi)
+            alphap = Res[0][3]
+            Rho = Res[0][1]
+            alphaq = Res[0][4]
+            p = B.shape[0]
+            # predict sample
+            x_hat = pred_continuous(B, Rho, alphap, D_pred, X_pred)
+            # calculate probabilities
+            dev = 0.5 * abs(np.diag(B))
+            eps = abs(X_pred - x_hat)
+            p_val = 2 * norm.cdf(x_hat - eps, loc=x_hat,
+                                 scale=np.sqrt(1 / dev))
+            # if p_val for data point < t replace it in other predictions by mean of feature
+            x_cor = np.where(p_val < t, means[i], X_pred)
+            # get discrete predictions
+            d_hat = pred_discrete(Rho, X_pred, D_pred, alphaq, Phi, levels, p)
+            # if probability of discrete data point < t change state to most likely one
+            d_hat_cor = np.copy(d_hat)
+            levelSum = np.cumsum(levels)
+            levelSum = np.insert(levelSum, 0, 0)
+            d_var = 0
+            D_pred_cor = np.copy(D_pred)
+            for k in range(len(d_hat)):
+                if k == levelSum[d_var]:
+                    d_var = d_var + 1
+                if D_pred[k] == 1 and d_hat[k] < t:
+                    tmp = np.zeros(
+                        shape=len(d_hat[levelSum[d_var-1]:levelSum[d_var]]))
+                    tmp[np.where(d_hat[levelSum[d_var-1]:levelSum[d_var]]
+                                 == max(d_hat[levelSum[d_var-1]:levelSum[d_var]]))] = 1
+                    D_pred_cor[levelSum[d_var-1]:levelSum[d_var]] = tmp
+            # predict cat again using adjusted states
+
+            # predict continuous and discrete again using corrected states and values
+            x_hat_cor_xp = pred_continuous(B, Rho, alphap, D_pred_cor, x_cor)
+            d_hat_cor_xp = pred_discrete(
+                Rho, x_cor, D_pred_cor, alphaq, Phi, levels, p)
+            X_hat[i] = x_hat
+            X_hat_cor_xp[i] = x_hat_cor_xp
+            D_hat[i] = d_hat
+            D_hat_cor_xp[i] = d_hat_cor_xp
+            eps = abs(X_pred - x_hat)
+            p_val = 2 * norm.cdf(x_hat - eps, loc=x_hat,
+                                 scale=np.sqrt(1 / dev))
+            prob_cont[i] = p_val
+            Var[i] = dev
+        MSE = np.mean((X_hat - X)**2)
+        MSE_seq = np.append(MSE_seq, MSE)
+        lam_opt = lambda_t
+        j = j+1
+
+    if (MSE < MSE_old):
+        print('Minimum not found, choose smaller Lam sequence')
+    if (np.size(lam_seq) == 1): # in case only one lambda submitted
+        X_hat_cor_xp_old = np.copy(X_hat_cor_xp)
+        D_hat_cor_xp_old = np.copy(D_hat_cor_xp)
+        prob_cont_old = np.copy(prob_cont)
+        Var_old = np.copy(Var)
+
+    return (prob_cont_old, Var_old, lam_opt_old, X_hat_cor_xp_old, D_hat_cor_xp_old)
+
+
+def get_threshold_continuous(X, X_hat, dev):
+    random.seed(671)
+    # calculate random scores from estimated distribution
+    # first draw random realizations from estimated distribution with 100 repetitions
+    mu = X_hat.flatten(order='F')
+    dev = dev.flatten(order='F')
+    X_flat = X.flatten(order='F')
+    random_scores = np.zeros(shape=(mu.shape[0], 100))
+    for i in range(mu.shape[0]):
+        tmp = norm.rvs(loc=mu[i], scale=np.sqrt(1/dev[i]), size=100)
+        random_scores[i, ] = np.divide(np.abs(tmp - mu[i]), np.sqrt(1/dev[i]))
+
+    # rank random scores for each repetition separately
+    random_scores = np.sort(random_scores, axis=0)
+    # average over all repetitions
+    random_scores = np.flip(np.mean(random_scores, axis=1))
+    # get observed scores
+    observed_scores = np.abs(mu - X_flat)/np.sqrt(1/dev)
+    observed_scores_sorted = np.flip(np.sort(observed_scores))
+    # determine threshold
+    threshold = random_scores[np.where(
+        random_scores >= observed_scores_sorted)][0]
+    # and number of detected anomalies
+    n_ano = np.sum(observed_scores >= threshold)
+    # correct anomalies found in X with predictions X_hat
+    observed_scores = np.reshape(observed_scores, X.shape, 'F')
+    X_cor = np.where(observed_scores <= threshold, X, X_hat)
+    ano_index = np.transpose((observed_scores >= threshold).nonzero())
+
+    return (X_cor, threshold, n_ano, ano_index)
+
+
+def get_threshold_discrete(D, levels, D_hat):
+    random.seed(321)
+    # first calculate observed scores
+    # get index of "true" state
+    ind = np.where(D == 1)
+    p = D_hat[ind]
+    observed_scores = -np.log(p)
+    observed_scores_sorted = np.flip(np.sort(observed_scores))
+    # now sample states according to estimated distribution with 100 repetitions
+    random_scores = [np.zeros(shape=(D.shape[0], 100))
+                     for i in range(len(levels))]
+    start = 0
+    for i in range(len(levels)):
+        end = int(start + levels[i])
+        prob = D_hat[:, start:end]
+
+        state_index = np.arange(levels[i])
+        for j in range(D.shape[0]):
+            random_obs = np.random.choice(state_index, p=prob[j], size=100)
+            random_scores[i][j] = -np.log(prob[j, random_obs])
+        start = end
+
+    # concatenate and average random scores
+    random_scores = np.concatenate((random_scores), axis=0)
+    random_scores = np.sort(random_scores, axis=0)
+    random_scores = np.flip(np.mean(random_scores, axis=1))
+    # determine threshold
+    threshold = random_scores[np.where(
+        random_scores >= observed_scores_sorted)][0]
+    # and number of detected anomalies
+    n_ano = np.sum(observed_scores >= threshold)
+    # get position of detected anomalies
+    # first array corresponds to sample, second array to feature position
+    pos = np.array([ind[0][np.where(observed_scores >= threshold)],
+                   ind[1][np.where(observed_scores >= threshold)]])
+    return (n_ano, threshold, pos)
+
+def transform_data(
+        X
+):
+    X_trans  = (X-X.min(axis = 0))/(X.max(axis=0) - X.min(axis=0))
+    return(X_trans)
+
+def transform_back(
+        X,
+        X_scaled
+):
+    X_back = X_scaled * (X.max(axis=0) - X.min(axis=0)) + X.min(axis=0)
+    return(X_back)
+
+def rel_dev(
+        x, 
+        org):
+    return(abs((x-org)/org))
+
+def place_anomalies_continuous(
+        X,
+        n_ano,
+        epsilon,
+        positive = False
+):
+    random.seed(987)
+    # first transform data feature-wise to [0,1]
+    X_scaled = transform_data(X)
+    # Calculate 15% border
+    Z = (0.15*X) / (X.max(axis=0) - X.min(axis=0))
+    ano = [np.copy(X) for i in range(len(epsilon))]
+    change = np.copy(X)
+    dirm = np.copy(X)
+    # for each element in X sample shift
+    for i in range(X.shape[0]):
+        for j in range(X.shape[1]):
+            lc = random.uniform( Z[i,j],(Z[i,j]+X_scaled[i,j]))
+            uc = random.uniform( Z[i,j],(1+Z[i,j]-X_scaled[i,j]))
+            # decide whether lower or upper change
+            dir = random.randint(0,1)
+            if dir == 1:
+                for k in range(len(epsilon)):
+                    ano[k][i,j] = X_scaled[i,j] + epsilon[k]*uc
+                    change[i,j] = uc
+                    dirm[i,j] = 1
+            else:
+                for k in range(len(epsilon)):
+                    ano[k][i,j] = X_scaled[i,j] - epsilon[k] * lc
+                    change[i,j] = lc
+                    dirm[i,j] = 0
+    # transform anomalies back
+    ano_retrans = [transform_back(X, tmp) for tmp in ano]
+    # place anomalies
+    position = np.array([])
+    position.shape = (0,2)
+    X_ano = [np.copy(X) for i in range(len(epsilon))]
+    k = 0
+    while k < n_ano:
+        # sample position
+        row = random.randint(0, (X.shape[0]-1))
+        col = random.randint(0, (X.shape[1]-1))
+        # first check if anomaly already has been placed at that position
+        if sum((position == [[row,col]]).all(axis = 1)) == 0:
+            # check if introduced anomaly > 15% deviation (only for epsilon < 1 relevant) and anomaly still positiv 
+            if positive == True:
+                if rel_dev(ano_retrans[0][row,col],X[row,col]) > 0.15 and ano_retrans[(len(epsilon)-1)][row,col] > 0:
+                    k = k+1
+                    position = np.append(position, [[row, col]], axis = 0)
+                    for l in range(len(epsilon)):
+                        X_ano[l][row, col] = ano_retrans[l][row,col]
+            else :
+                if rel_dev(ano_retrans[0][row,col],X[row,col]) > 0.15:
+                    k = k+1
+                    position = np.append(position, [[row, col]], axis = 0)
+                    for l in range(len(epsilon)):
+                        X_ano[l][row, col] = ano_retrans[l][row,col]
+    return(X_ano, position)
+
+def impute(
+        X,
+        D,
+        levels, 
+        lam_seq,
+        oIterations = 10000, 
+        oTol = 1e-6 ):
+    # calculate Euclidean distance of all samples to each other
+    # ignore NaN values
+    dist = nan_euclidean_distances(X,X)
+    np.fill_diagonal(dist, np.inf)
+    X_preimp = np.copy(X)
+    D_preimp = np.copy(D)
+
+    for i in range(X.shape[0]):
+        ind_disc = np.where(np.isnan(D[i]))[0]
+        ind_cont = np.where(np.isnan(X[i]))[0]
+        # impute continuous with value of closest sample
+        for j in ind_cont:
+            sample = np.argmin(dist[i])
+            dist_new = np.copy(dist)
+            while np.isnan(X[sample,j]): # check if value for imputation is also nan
+                dist_new[i,sample] = np.inf
+                sample = np.argmin(dist_new[i]) # use second, third, .. closest sample
+            X_preimp[i,j] = X[sample,j]
+        # same for discrete 
+        for j in ind_disc:
+            sample = np.argmin(dist[i])
+            dist_new = np.copy(dist)
+            while np.isnan(D[sample,j]): # check if value for imputation is also nan
+                dist_new[i,sample] = np.inf
+                sample = np.argmin(dist_new[i]) # use second, third, .. closest sample
+            D_preimp[i,j] = D[sample,j]
+
+    # for each lam in lam_seq fit MGM on all data
+    # calculate MSE
+
+    MSE = 2e10
+    MSE_old = 2e10
+    j = 0
+    X_hat = np.zeros(shape=X.shape)
+    D_hat = np.zeros(shape=D.shape)
+    MSE_seq = np.array([])
+    lam_opt = np.array([lam_seq[0]])
+    lam_opt_old = np.array([lam_seq[0]])
+    while ((MSE_old >= MSE) and (j < np.size(lam_seq))):
+        lam_opt_old = np.copy(lam_opt)
+        MSE_old = np.copy(MSE)
+        X_hat_old = np.copy(X_hat)
+        D_hat_old = np.copy(D_hat)
+        lambda_t = np.array([lam_seq[j]])
+        # fit model on all samples
+        Res = Fit_MGM(X_preimp, D_preimp, levels, lambda_t, oIterations, eps=oTol)
+        Res = Res[0]
+        B = Res[0][0]
+        B = B + np.transpose(B)
+        Phi = Res[0][2]
+        Phi = Phi + np.transpose(Phi)
+        alphap = Res[0][3]
+        Rho = Res[0][1]
+        alphaq = Res[0][4]
+        p = B.shape[0]
+        # loop over all samples
+        for i in range(X.shape[0]):
+            X_pred = X_preimp[i]
+            D_pred = D_preimp[i]
+            # predict sample
+            x_hat = pred_continuous(B, Rho, alphap, D_pred, X_pred)
+            # get discrete predictions
+            d_hat = pred_discrete(Rho, X_pred, D_pred, alphaq, Phi, levels,p)
+            levelSum = np.cumsum(levels)
+            levelSum = np.insert(levelSum, 0, 0)
+            d_var = 0
+            d_hat_state = np.copy(D_pred)
+            for k in range(len(d_hat)):
+                if k == levelSum[d_var]:
+                    d_var = d_var + 1
+                    tmp = np.zeros(shape=len(d_hat[levelSum[d_var-1]:levelSum[d_var]]))
+                    tmp[np.where(d_hat[levelSum[d_var-1]:levelSum[d_var]] == max(d_hat[levelSum[d_var-1]:levelSum[d_var]]))] = 1
+                    d_hat_state[levelSum[d_var-1]:levelSum[d_var]] = tmp
+            X_hat[i] = x_hat
+            D_hat[i] = d_hat_state
+        MSE = np.mean((X_hat - X_preimp)**2)
+        MSE_seq = np.append(MSE_seq, MSE)
+        lam_opt = lambda_t
+        j = j+1
+    ind_cont = np.where(np.isnan(X))
+    ind_disc = np.where(np.isnan(D))
+    X_imp = np.copy(X)
+    X_imp[ind_cont] = X_hat_old[ind_cont]
+    D_imp = np.copy(D)
+    D_imp[ind_disc] = D_hat_old[ind_disc]
+    return(X_imp, D_imp, lam_opt_old)
```

### Comparing `adadmire-1.0.1/src/adadmire/mgm.py` & `adadmire-1.0.2/src/adadmire/mgm.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-# MIT License
-# Copyright (c) 2019 Michael Altenbuchinger and Helena Zacharias
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-import numpy as np
-import adadmire.apgpy as apg
-
-def grad_neglogli(B, Rho, Phi, alphap, alphaq, X, D, levels):
-    n = X.shape[0]
-    p = B.shape[0]
-    q = levels.shape[0]
-
-    levelSum = [0]
-    levelSum.extend(levels)
-    levelSum = np.cumsum(levelSum)
-    for r in range(0, q):
-        Phi[int(levelSum[r]):int(levelSum[r]+levels[r]),
-            int(levelSum[r]):int(levelSum[r]+levels[r])] = 0
-
-    Bd = np.diag(B)
-    B = B - np.diag(Bd)
-    B = np.triu(B)
-    B = B + np.transpose(B)
-    DRho = np.dot(D, Rho)
-    DRho = np.dot(DRho, np.diag(np.divide(np.repeat(1., p), Bd)))
-    XB = np.dot(X, B)
-    XB = np.dot(XB, np.diag(np.divide(np.repeat(1., p), Bd)))
-    consts = np.tile(alphap, (n, 1))
-    Xt = np.transpose(X)
-    res = consts + DRho + XB + X
-    gradBd = np.repeat(0., p)
-
-    for s in range(0, p):
-        gradBd[s] = - n/(2.*Bd[s]) - .5*np.dot(res[:, s], res[:, s]
-                                              ) + np.dot(res[:, s], XB[:, s] +
-                                                         DRho[:, s])
-
-    gradB = - np.dot(Xt, res)
-    gradB = gradB - np.diag(np.diag(gradB))
-    gradB = np.transpose(np.tril(gradB)) + np.triu(gradB)
-    gradalphap = - np.dot(np.diag(Bd), np.sum(res, axis=0)[:, np.newaxis])
-    gradalphap = gradalphap[:, 0]
-
-    gradRho = - np.dot(np.transpose(D), res)
-
-    Xt = np.transpose(X)
-    RhoX = np.dot(Rho, Xt)
-    Phi = Phi - np.diag(np.diag(Phi))
-    Phi = np.triu(Phi)
-    Phi = Phi + np.transpose(Phi)
-    Phirr = np.transpose(np.tile(alphaq, (n, 1)))
-    PhiD = np.dot(Phi, np.transpose(D))
-    discprod = np.transpose(RhoX+Phirr+PhiD)
-
-    for r in range(0, q):
-        disctemp = discprod[:, int(levelSum[r]):int(levelSum[r]+levels[r])]
-        denominator = np.logaddexp.reduce(disctemp, axis=1)
-        disctemp = disctemp - denominator[:, np.newaxis]
-        disctemp = np.exp(disctemp)
-        temp = disctemp - D[:, int(levelSum[r]):int(levelSum[r]+levels[r])]
-        discprod[:, int(levelSum[r]):int(levelSum[r]+levels[r])] = temp
-
-    gradalphaq = np.sum(discprod, axis=0)
-    gradw = np.dot(Xt, discprod)
-    gradRho = gradRho+np.transpose(gradw)
-    gradPhi = np.dot(np.transpose(D), discprod)
-
-    for r in range(0, q):
-        gradPhi[int(levelSum[r]):int(levelSum[r]+levels[r]),
-                int(levelSum[r]):int(levelSum[r]+levels[r])] = 0
-
-    gradPhi = np.transpose(np.tril(gradPhi))+np.triu(gradPhi)
-    gradB.flat[::p+1] = gradBd
-    gradB = gradB/n
-    gradRho = gradRho/n
-    gradPhi = gradPhi/n
-    gradalphap = gradalphap/n
-    gradalphaq = gradalphaq/n
-    return gradB, gradRho, gradPhi, gradalphap, gradalphaq
-
-
-def neglogli(B, Rho, Phi, alphap, alphaq, X, D, levels):
-    n = X.shape[0]
-    p = B.shape[0]
-    q = levels.shape[0]
-    Bd = np.diag(B)
-    B = B - np.diag(Bd)
-    B = np.triu(B)
-    B = B + np.transpose(B)
-    DRho = np.dot(D, Rho)
-    DRho = np.dot(DRho, np.diag(np.divide(np.repeat(1, p), Bd)))
-    XB = np.dot(X, B)
-    XB = np.dot(XB, np.diag(np.divide(np.repeat(1, p), Bd)))
-    Xt = np.transpose(X)
-    RhoX = np.dot(Rho, Xt)
-    Phi = Phi - np.diag(np.diag(Phi))
-    Phi = np.triu(Phi)
-    Phi = Phi + np.transpose(Phi)
-    Phirr = np.transpose(np.tile(alphaq, (n, 1)))
-    PhiD = np.dot(Phi, np.transpose(D))
-    levelSum = [0]
-    levelSum.extend(levels)
-    levelSum = np.cumsum(levelSum)
-    consts = np.tile(alphap, (n, 1))
-    PLcont1 = -n/2.*np.sum(np.log(-Bd)) #here, the constant term is neglected
-    PLcont2 = consts + DRho + XB + X
-    PLcont2 = np.dot(PLcont2, np.diag(np.sqrt(-Bd)))
-    PLcont2 = np.multiply(PLcont2, PLcont2)
-    PLcont2 = 0.5*np.sum(np.sum(PLcont2, axis=0))
-    temp = RhoX+Phirr+PhiD
-    PLdisc = 0
-    for r in range(0, q):
-        temp2 = temp[int(levelSum[r]):int(levelSum[r]+levels[r]), :]
-        denominator = np.sum(
-            np.exp(np.dot(np.identity(int(levels[r])), temp2)), axis=0)
-        numerator = np.sum(np.multiply(D[:, int(levelSum[r]):int(
-            levelSum[r]+levels[r])], np.transpose(temp2)), axis=1)
-        PLdisc = PLdisc-numerator+np.log(denominator)
-    PLdisc = np.sum(PLdisc)
-    return((PLcont1+PLcont2+PLdisc)/n)
-
-
-def neglogli_plain(B_Rho_Phi_alphap_alphaq, X, D, levels, p, q):
-    x2 = Inv_B_Rho_Phi_alphap_alphaq(B_Rho_Phi_alphap_alphaq, p, q)
-    x1 = neglogli(x2[0], x2[1], x2[2], x2[3], x2[4], X, D, levels)
-    return(x1)
-
-
-def B_Rho_Phi_alphap_alphaq(B, Rho, Phi, alphap, alphaq):
-    p = B.shape[0]
-    q = Phi.shape[0]
-    sizes = np.cumsum([p*p, p*q, q*q, p, q])
-    x = np.repeat(0., sizes[4])
-    x[0:sizes[0]] = np.reshape(B, (1, p*p))[0, :]
-    x[sizes[0]:sizes[1]] = np.reshape(Rho, (1, p*q))[0, :]
-    x[sizes[1]:sizes[2]] = np.reshape(Phi, (1, q*q))[0, :]
-    x[sizes[2]:sizes[3]] = alphap
-    x[sizes[3]:sizes[4]] = alphaq
-    return(x)
-
-
-def Inv_B_Rho_Phi_alphap_alphaq(x, p, q):
-    sizes = np.cumsum([p*p, p*q, q*q, p, q])
-    B = np.reshape(x[0:sizes[0]], (p, p))
-    Rho = np.reshape(x[sizes[0]:sizes[1]], (q, p))
-    Phi = np.reshape(x[sizes[1]:sizes[2]], (q, q))
-    alphap = x[sizes[2]:sizes[3]]
-    alphaq = x[sizes[3]:sizes[4]]
-    return(B, Rho, Phi, alphap, alphaq)
-
-
-def grad_neglogli_plain(B_Rho_Phi_alphap_alphaq, X, D, levels, p, q):
-    x2 = Inv_B_Rho_Phi_alphap_alphaq(B_Rho_Phi_alphap_alphaq, p, q)
-    x1 = grad_neglogli(x2[0], x2[1], x2[2], x2[3], x2[4], X, D, levels)
-    return(x1[0], x1[1], x1[2], x1[3], x1[4])
-
-
-def make_starting_parameters(X, D, levels):
-    p = X.shape[1]
-    q = D.shape[1]
-    B = -np.diag(np.repeat(1, p))
-    Rho = np.zeros((q, p))
-    Phi = np.zeros((q, q))
-    alphap = np.zeros(p)
-    alphaq = np.zeros(q)
-    return(B, Rho, Phi, alphap, alphaq, p, q)
-
-
-def grad_f_temp(x, X, D, levels, p, q):
-    x2 = grad_neglogli_plain(x, X, D, levels, p, q)
-    x3 = B_Rho_Phi_alphap_alphaq(x2[0], x2[1], x2[2], x2[3], x2[4])
-    return(x3)
-
-
-def prox_enet(x, l_l1, l_l2, t, pen, p0, tol0):
-    prox_l1 = np.sign(x) * np.maximum(abs(x) - t * l_l1 * pen, 0)
-    return prox_l1 / (1. + t * l_l2 * pen)
-
-
-def make_penalty_factors(X, D, levels):
-    levelSum = [0]
-    levelSum.extend(levels)
-    levelSum = np.cumsum(levelSum)
-    p = X.shape[1]
-    qL = len(levels)
-    q = np.sum(levels)
-    sds = np.reshape(np.std(X, axis=0), (p, 1))
-    ps = np.reshape(np.mean(D, axis=0), (q, 1))
-    B = np.ones((p, p)) - np.diag(np.repeat(1, p))
-    B = np.multiply(B, np.dot(sds, np.transpose(sds)))
-    Rho = np.ones((q, p))
-    Phi = np.ones((q, q))
-    alphap = np.zeros(p)
-    alphaq = np.zeros(q)
-    for r in range(0, qL):
-        Phi[int(levelSum[r]), :] = np.repeat(10, Phi.shape[1])
-        Phi[:, int(levelSum[r])] = np.repeat(10, Phi.shape[1])
-        ps_t = ps[int(levelSum[r]):int(levelSum[r]+levels[r])]
-        ps[int(levelSum[r]):int(levelSum[r]+levels[r])
-           ] = np.sqrt(np.sum(ps_t*(1-ps_t)))
-        Rho[int(levelSum[r]), :] = np.repeat(10, Rho.shape[1])
-    Rho = np.multiply(Rho, np.dot(ps, np.transpose(sds)))
-    Phi = np.multiply(Phi, np.dot(ps, np.transpose(ps)))
-    return(B, Rho, Phi, alphap, alphaq, p, q)
-
-
-def Fit_MGM(X, D, levels, lambda_seq, iterations, eps=1e-6):
-    p = X.shape[1]
-    q = D.shape[1]
-    start = make_starting_parameters(X, D, levels)
-    start = B_Rho_Phi_alphap_alphaq(
-        start[0], start[1], start[2], start[3], start[4])
-    penalty = make_penalty_factors(X, D, levels)
-    penalty = B_Rho_Phi_alphap_alphaq(
-        penalty[0], penalty[1], penalty[2], penalty[3], penalty[4])
-    x_start = np.zeros(penalty.shape[0])
-
-    def grad_f(x): return grad_f_temp(x + x_start, X, D, levels, p, q)
-
-    def fun(x): return neglogli_plain(x + x_start, X, D, levels, p, q)
-    x_list = [None]*lambda_seq.shape[0]
-    xtemp = start
-    for i in range(0, lambda_seq.shape[0]):
-        l_l1 = lambda_seq[i]
-        print("lambda =", l_l1)
-
-        def prox_g(x, l): return prox_enet(
-            x, l_l1, 0, t=l, pen=penalty, p0=p, tol0=eps)
-        x_fista = apg.solve(grad_f, prox_g, xtemp, eps=eps,
-                            max_iters=iterations, gen_plots=False,
-                            debug=False)
-        x_list[i] = Inv_B_Rho_Phi_alphap_alphaq(x_fista, p, q)
-        xtemp = x_fista
-    loss_list = []
-    k = 0
-    for j in range(0, len(x_list)):
-        k = k+1
-        loss_vec = neglogli(
-            x_list[j][0], x_list[j][1], x_list[j][2], x_list[j][3],
-            x_list[j][4], X, D, levels)
-        loss_list = np.append(loss_list, loss_vec)
-    return([x_list, loss_list])
+# MIT License
+# Copyright (c) 2019 Michael Altenbuchinger and Helena Zacharias
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import numpy as np
+import adadmire.apgpy as apg
+
+def grad_neglogli(B, Rho, Phi, alphap, alphaq, X, D, levels):
+    n = X.shape[0]
+    p = B.shape[0]
+    q = levels.shape[0]
+
+    levelSum = [0]
+    levelSum.extend(levels)
+    levelSum = np.cumsum(levelSum)
+    for r in range(0, q):
+        Phi[int(levelSum[r]):int(levelSum[r]+levels[r]),
+            int(levelSum[r]):int(levelSum[r]+levels[r])] = 0
+
+    Bd = np.diag(B)
+    B = B - np.diag(Bd)
+    B = np.triu(B)
+    B = B + np.transpose(B)
+    DRho = np.dot(D, Rho)
+    DRho = np.dot(DRho, np.diag(np.divide(np.repeat(1., p), Bd)))
+    XB = np.dot(X, B)
+    XB = np.dot(XB, np.diag(np.divide(np.repeat(1., p), Bd)))
+    consts = np.tile(alphap, (n, 1))
+    Xt = np.transpose(X)
+    res = consts + DRho + XB + X
+    gradBd = np.repeat(0., p)
+
+    for s in range(0, p):
+        gradBd[s] = - n/(2.*Bd[s]) - .5*np.dot(res[:, s], res[:, s]
+                                              ) + np.dot(res[:, s], XB[:, s] +
+                                                         DRho[:, s])
+
+    gradB = - np.dot(Xt, res)
+    gradB = gradB - np.diag(np.diag(gradB))
+    gradB = np.transpose(np.tril(gradB)) + np.triu(gradB)
+    gradalphap = - np.dot(np.diag(Bd), np.sum(res, axis=0)[:, np.newaxis])
+    gradalphap = gradalphap[:, 0]
+
+    gradRho = - np.dot(np.transpose(D), res)
+
+    Xt = np.transpose(X)
+    RhoX = np.dot(Rho, Xt)
+    Phi = Phi - np.diag(np.diag(Phi))
+    Phi = np.triu(Phi)
+    Phi = Phi + np.transpose(Phi)
+    Phirr = np.transpose(np.tile(alphaq, (n, 1)))
+    PhiD = np.dot(Phi, np.transpose(D))
+    discprod = np.transpose(RhoX+Phirr+PhiD)
+
+    for r in range(0, q):
+        disctemp = discprod[:, int(levelSum[r]):int(levelSum[r]+levels[r])]
+        denominator = np.logaddexp.reduce(disctemp, axis=1)
+        disctemp = disctemp - denominator[:, np.newaxis]
+        disctemp = np.exp(disctemp)
+        temp = disctemp - D[:, int(levelSum[r]):int(levelSum[r]+levels[r])]
+        discprod[:, int(levelSum[r]):int(levelSum[r]+levels[r])] = temp
+
+    gradalphaq = np.sum(discprod, axis=0)
+    gradw = np.dot(Xt, discprod)
+    gradRho = gradRho+np.transpose(gradw)
+    gradPhi = np.dot(np.transpose(D), discprod)
+
+    for r in range(0, q):
+        gradPhi[int(levelSum[r]):int(levelSum[r]+levels[r]),
+                int(levelSum[r]):int(levelSum[r]+levels[r])] = 0
+
+    gradPhi = np.transpose(np.tril(gradPhi))+np.triu(gradPhi)
+    gradB.flat[::p+1] = gradBd
+    gradB = gradB/n
+    gradRho = gradRho/n
+    gradPhi = gradPhi/n
+    gradalphap = gradalphap/n
+    gradalphaq = gradalphaq/n
+    return gradB, gradRho, gradPhi, gradalphap, gradalphaq
+
+
+def neglogli(B, Rho, Phi, alphap, alphaq, X, D, levels):
+    n = X.shape[0]
+    p = B.shape[0]
+    q = levels.shape[0]
+    Bd = np.diag(B)
+    B = B - np.diag(Bd)
+    B = np.triu(B)
+    B = B + np.transpose(B)
+    DRho = np.dot(D, Rho)
+    DRho = np.dot(DRho, np.diag(np.divide(np.repeat(1, p), Bd)))
+    XB = np.dot(X, B)
+    XB = np.dot(XB, np.diag(np.divide(np.repeat(1, p), Bd)))
+    Xt = np.transpose(X)
+    RhoX = np.dot(Rho, Xt)
+    Phi = Phi - np.diag(np.diag(Phi))
+    Phi = np.triu(Phi)
+    Phi = Phi + np.transpose(Phi)
+    Phirr = np.transpose(np.tile(alphaq, (n, 1)))
+    PhiD = np.dot(Phi, np.transpose(D))
+    levelSum = [0]
+    levelSum.extend(levels)
+    levelSum = np.cumsum(levelSum)
+    consts = np.tile(alphap, (n, 1))
+    PLcont1 = -n/2.*np.sum(np.log(-Bd)) #here, the constant term is neglected
+    PLcont2 = consts + DRho + XB + X
+    PLcont2 = np.dot(PLcont2, np.diag(np.sqrt(-Bd)))
+    PLcont2 = np.multiply(PLcont2, PLcont2)
+    PLcont2 = 0.5*np.sum(np.sum(PLcont2, axis=0))
+    temp = RhoX+Phirr+PhiD
+    PLdisc = 0
+    for r in range(0, q):
+        temp2 = temp[int(levelSum[r]):int(levelSum[r]+levels[r]), :]
+        denominator = np.sum(
+            np.exp(np.dot(np.identity(int(levels[r])), temp2)), axis=0)
+        numerator = np.sum(np.multiply(D[:, int(levelSum[r]):int(
+            levelSum[r]+levels[r])], np.transpose(temp2)), axis=1)
+        PLdisc = PLdisc-numerator+np.log(denominator)
+    PLdisc = np.sum(PLdisc)
+    return((PLcont1+PLcont2+PLdisc)/n)
+
+
+def neglogli_plain(B_Rho_Phi_alphap_alphaq, X, D, levels, p, q):
+    x2 = Inv_B_Rho_Phi_alphap_alphaq(B_Rho_Phi_alphap_alphaq, p, q)
+    x1 = neglogli(x2[0], x2[1], x2[2], x2[3], x2[4], X, D, levels)
+    return(x1)
+
+
+def B_Rho_Phi_alphap_alphaq(B, Rho, Phi, alphap, alphaq):
+    p = B.shape[0]
+    q = Phi.shape[0]
+    sizes = np.cumsum([p*p, p*q, q*q, p, q])
+    x = np.repeat(0., sizes[4])
+    x[0:sizes[0]] = np.reshape(B, (1, p*p))[0, :]
+    x[sizes[0]:sizes[1]] = np.reshape(Rho, (1, p*q))[0, :]
+    x[sizes[1]:sizes[2]] = np.reshape(Phi, (1, q*q))[0, :]
+    x[sizes[2]:sizes[3]] = alphap
+    x[sizes[3]:sizes[4]] = alphaq
+    return(x)
+
+
+def Inv_B_Rho_Phi_alphap_alphaq(x, p, q):
+    sizes = np.cumsum([p*p, p*q, q*q, p, q])
+    B = np.reshape(x[0:sizes[0]], (p, p))
+    Rho = np.reshape(x[sizes[0]:sizes[1]], (q, p))
+    Phi = np.reshape(x[sizes[1]:sizes[2]], (q, q))
+    alphap = x[sizes[2]:sizes[3]]
+    alphaq = x[sizes[3]:sizes[4]]
+    return(B, Rho, Phi, alphap, alphaq)
+
+
+def grad_neglogli_plain(B_Rho_Phi_alphap_alphaq, X, D, levels, p, q):
+    x2 = Inv_B_Rho_Phi_alphap_alphaq(B_Rho_Phi_alphap_alphaq, p, q)
+    x1 = grad_neglogli(x2[0], x2[1], x2[2], x2[3], x2[4], X, D, levels)
+    return(x1[0], x1[1], x1[2], x1[3], x1[4])
+
+
+def make_starting_parameters(X, D, levels):
+    p = X.shape[1]
+    q = D.shape[1]
+    B = -np.diag(np.repeat(1, p))
+    Rho = np.zeros((q, p))
+    Phi = np.zeros((q, q))
+    alphap = np.zeros(p)
+    alphaq = np.zeros(q)
+    return(B, Rho, Phi, alphap, alphaq, p, q)
+
+
+def grad_f_temp(x, X, D, levels, p, q):
+    x2 = grad_neglogli_plain(x, X, D, levels, p, q)
+    x3 = B_Rho_Phi_alphap_alphaq(x2[0], x2[1], x2[2], x2[3], x2[4])
+    return(x3)
+
+
+def prox_enet(x, l_l1, l_l2, t, pen, p0, tol0):
+    prox_l1 = np.sign(x) * np.maximum(abs(x) - t * l_l1 * pen, 0)
+    return prox_l1 / (1. + t * l_l2 * pen)
+
+
+def make_penalty_factors(X, D, levels):
+    levelSum = [0]
+    levelSum.extend(levels)
+    levelSum = np.cumsum(levelSum)
+    p = X.shape[1]
+    qL = len(levels)
+    q = np.sum(levels)
+    sds = np.reshape(np.std(X, axis=0), (p, 1))
+    ps = np.reshape(np.mean(D, axis=0), (q, 1))
+    B = np.ones((p, p)) - np.diag(np.repeat(1, p))
+    B = np.multiply(B, np.dot(sds, np.transpose(sds)))
+    Rho = np.ones((q, p))
+    Phi = np.ones((q, q))
+    alphap = np.zeros(p)
+    alphaq = np.zeros(q)
+    for r in range(0, qL):
+        Phi[int(levelSum[r]), :] = np.repeat(10, Phi.shape[1])
+        Phi[:, int(levelSum[r])] = np.repeat(10, Phi.shape[1])
+        ps_t = ps[int(levelSum[r]):int(levelSum[r]+levels[r])]
+        ps[int(levelSum[r]):int(levelSum[r]+levels[r])
+           ] = np.sqrt(np.sum(ps_t*(1-ps_t)))
+        Rho[int(levelSum[r]), :] = np.repeat(10, Rho.shape[1])
+    Rho = np.multiply(Rho, np.dot(ps, np.transpose(sds)))
+    Phi = np.multiply(Phi, np.dot(ps, np.transpose(ps)))
+    return(B, Rho, Phi, alphap, alphaq, p, q)
+
+
+def Fit_MGM(X, D, levels, lambda_seq, iterations, eps=1e-6):
+    p = X.shape[1]
+    q = D.shape[1]
+    start = make_starting_parameters(X, D, levels)
+    start = B_Rho_Phi_alphap_alphaq(
+        start[0], start[1], start[2], start[3], start[4])
+    penalty = make_penalty_factors(X, D, levels)
+    penalty = B_Rho_Phi_alphap_alphaq(
+        penalty[0], penalty[1], penalty[2], penalty[3], penalty[4])
+    x_start = np.zeros(penalty.shape[0])
+
+    def grad_f(x): return grad_f_temp(x + x_start, X, D, levels, p, q)
+
+    def fun(x): return neglogli_plain(x + x_start, X, D, levels, p, q)
+    x_list = [None]*lambda_seq.shape[0]
+    xtemp = start
+    for i in range(0, lambda_seq.shape[0]):
+        l_l1 = lambda_seq[i]
+        print("lambda =", l_l1)
+
+        def prox_g(x, l): return prox_enet(
+            x, l_l1, 0, t=l, pen=penalty, p0=p, tol0=eps)
+        x_fista = apg.solve(grad_f, prox_g, xtemp, eps=eps,
+                            max_iters=iterations, gen_plots=False,
+                            debug=False)
+        x_list[i] = Inv_B_Rho_Phi_alphap_alphaq(x_fista, p, q)
+        xtemp = x_fista
+    loss_list = []
+    k = 0
+    for j in range(0, len(x_list)):
+        k = k+1
+        loss_vec = neglogli(
+            x_list[j][0], x_list[j][1], x_list[j][2], x_list[j][3],
+            x_list[j][4], X, D, levels)
+        loss_list = np.append(loss_list, loss_vec)
+    return([x_list, loss_list])
```

### Comparing `adadmire-1.0.1/README.md` & `adadmire-1.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,138 @@
-# adadmire
-
-<!-- ATTENTION: this file will be displayed not only on Github, but also on PyPI, so NO relative relative to files in the repo must be used -->
-
-Functions for detecting anomalies in molecular data sets using Mixed Graphical Models.
-
-## Installation
-
-Enter the following commands in a shell like *bash*, *zsh* or *powershell*:
-
-```bash
-pip install -U adadmire
-```
-
-## Usage
-
-The usage example in this section require you to download the data files from folder [data](https://github.com/spang-lab/adadmire/tree/main/data) first. For a description of the contents of this folder, see section [Data](#data).
-
-### Example 1
-
-```python
-from adadmire import loo_cv_cor, get_threshold_continuous, get_threshold_discrete
-import numpy as np
-
-# download data/Feist_et_al
-# and load data
-X = np.load('data/Feist_et_al/scaled_data_raw.npy') # continuous data
-D = np.load('data/Feist_et_al/pheno.npy') # discrete data
-levels = np.load('data/Feist_et_al/levels.npy') # levels of discrete variables
-# define lambda sequence
-lam_zero = np.sqrt(np.log(X.shape[1] + D.shape[1]/2)/X.shape[0])
-lam_seq = np.array([-1.75,-2.0,-2.25])
-lam = [pow(2, x) for x in lam_seq]
-lam = np.array(lam)
-lam = lam_zero * lam
-# perform cross validation
-prob_hat, B_m, lam_opt,  x_hat, d_hat = loo_cv_cor(X,D,levels,lam)
-# determine continuous threshold
-X_cor, threshold_cont, n_ano_cont,  position_cont = get_threshold_continuous(X, x_hat, B_m)
-# returns: X corrected for detected anomalies, threshold, number of detected anomalies (n_ano_cont) and position
-print(n_ano_cont) # 46 detected continuous anomalies
-n_ano_disc, threshold_cont, position_disc = get_threshold_discrete(D, levels, d_hat)
-# returns:  number of detected anomalies (n_ano_disc), threshold and position
-print(n_ano_disc)
-# 0 detected discrete anomalies
-```
-
-### Example 2
-
-```python
-from adadmire import loo_cv_cor, get_threshold_continuous, place_anomalies_continuous
-import numpy as np
-X = np.load('data/Higuera_et_al/scaled_data_raw.npy') # continuous data
-D = np.load('data/Higuera_et_al/pheno.npy') # discrete data
-levels = np.load('data/Higuera_et_al/levels.npy') # levels of discrete variables
-
-# use originial data set and create simulations by introducing artificial anomalies with various strengths
-X_ano, pos = place_anomalies_continuous( X, n_ano = 1360, epsilon = np.array([0.6, 0.8, 1.0, 1.2, 1.4]))
-# n_ano: how many anomalies should be introduced?
-# epsilon defines "strength" of introduced anomalies
-
-# now detect anomalies using ADMIRE
-lam_zero = np.sqrt(np.log(X.shape[1] + D.shape[1]/2)/X.shape[0])
-lam_seq = np.array([-1.75,-2.0,-2.25])
-lam = [pow(2, x) for x in lam_seq]
-lam = np.array(lam)
-lam = lam_zero * lam
-prob_hat, B_m, lam_opt,  x_hat, d_hat = loo_cv_cor(X_ano[0],D,levels,lam) # perform cv and estimation 
-X_cor, threshold_cont, n_ano_cont,  position_cont = get_threshold_continuous(X_ano, x_hat, B_m) # determine threshold
-```
-
-### Data
-
-In the directory **data** you can find two sub directories:
-* **Feist_et_al**: contains data set as discribed in [Feist et al, 2018](#feist-et-al-2018) and [Buck et al, 2023](#buck-et-al-2023).
-    * **data_raw.xlsx**: raw, unscaled data, contains measurements of 100 samples and 49 metabolites
-    *  **scaled_data_raw.npy**: numpy file containing scaled version of **data_raw.xlsx**
-    *  **pheno_with_simulations.xlsx**: pheno data corresponding to **data_raw.xlsx**, also contains cell stimulations
-    *  **pheno.npy**: numpy file corresponding to **pheno_with_simulations.xlsx** (only contains variables batch and myc)
-    *  **levels.npy**: numpy file containing the levels of the discrete variables in **pheno.npy**
-* **Higuera_et_al**: contains down sampled data set from [Higuera et al, 2015](#higuera-et-al-2015) as described in [Buck et al, 2023](#buck-et-al-2023).
-    * **data_raw.xlsx**: raw, unscaled data, contains measurements of 400 samples and 68 proteins (down sampled from [Higuera et al, 2015](#higuera-et-al-2015))
-    *  **scaled_data_raw.npy**: numpy file containing scaled version of **data_raw.xlsx**
-    *  **pheno_.xlsx**: pheno data corresponding to **data_raw.xlsx**
-    *  **pheno.npy**: numpy file corresponding to **pheno.xlsx**
-    *  **levels.npy**: numpy file containing the levels of the discrete variables in **pheno.npy**
-
-## Contribute
-
-In case you have **questions**, **feature requests** or find any **bugs** in adadmire, please create a corresponding issue at [gitlab.spang-lab.de/bul38390/admire/issues](https://github.com/spang-lab/adadmire/issues).
-
-In case you want to **write code** for this package, see [Contribute](https://github.com/spang-lab/adadmire/blob/main/doc/contribute.md) for details.
-
-## References
-
-##### Feist et al, 2018
-
-Feist, Maren, et al. "Cooperative stat/nf-kb signaling regulates lymphoma metabolic reprogramming and aberrant got2 expression." Nature Communications, 2018
-
-##### Higuera et al, 2015
-
-Higuera, Clara et al, "Self-organizing feature maps identify proteins critical to learning in a mouse model of down syndrome." PLOS ONE, 2015
-
-##### Buck et al, 2023
-
-Buck, Lena et al. "Anomaly detection in mixed high dimensional molecular data"
+# adadmire
+
+<!-- ATTENTION: this file will be displayed not only on Github, but also on PyPI, so NO relative relative to files in the repo must be used -->
+
+Functions for detecting anomalies in molecular data sets using Mixed Graphical Models.
+
+## Installation
+
+Enter the following commands in a shell like *bash*, *zsh* or *powershell*:
+
+```bash
+pip install -U adadmire
+```
+
+## Usage
+
+The usage example in this section require you to download the data files from folder [data](https://github.com/spang-lab/adadmire/tree/main/data) first. For a description of the contents of this folder, see section [Data](#data).
+
+### Example 1
+
+```python
+from adadmire import loo_cv_cor, get_threshold_continuous, get_threshold_discrete
+import numpy as np
+
+# download data/Feist_et_al
+# and load data
+X = np.load('data/Feist_et_al/scaled_data_raw.npy') # continuous data
+D = np.load('data/Feist_et_al/pheno.npy') # discrete data
+levels = np.load('data/Feist_et_al/levels.npy') # levels of discrete variables
+# define lambda sequence
+lam_zero = np.sqrt(np.log(X.shape[1] + D.shape[1]/2)/X.shape[0])
+lam_seq = np.array([-1.75,-2.0,-2.25])
+lam = [pow(2, x) for x in lam_seq]
+lam = np.array(lam)
+lam = lam_zero * lam
+# perform cross validation
+prob_hat, B_m, lam_opt,  x_hat, d_hat = loo_cv_cor(X,D,levels,lam)
+# determine continuous threshold
+X_cor, threshold_cont, n_ano_cont,  position_cont = get_threshold_continuous(X, x_hat, B_m)
+# returns: X corrected for detected anomalies, threshold, number of detected anomalies (n_ano_cont) and position
+print(n_ano_cont) # 46 detected continuous anomalies
+n_ano_disc, threshold_cont, position_disc = get_threshold_discrete(D, levels, d_hat)
+# returns:  number of detected anomalies (n_ano_disc), threshold and position
+print(n_ano_disc)
+# 0 detected discrete anomalies
+```
+
+### Example 2
+
+```python
+from adadmire import loo_cv_cor, get_threshold_continuous, place_anomalies_continuous
+import numpy as np
+X = np.load('data/Higuera_et_al/scaled_data_raw.npy') # continuous data
+D = np.load('data/Higuera_et_al/pheno.npy') # discrete data
+levels = np.load('data/Higuera_et_al/levels.npy') # levels of discrete variables
+
+# use originial data set and create simulations by introducing artificial anomalies with various strengths
+X_ano, pos = place_anomalies_continuous( X, n_ano = 1360, epsilon = np.array([0.6, 0.8, 1.0, 1.2, 1.4]))
+# n_ano: how many anomalies should be introduced?
+# epsilon defines "strength" of introduced anomalies
+
+# now detect anomalies using ADMIRE
+lam_zero = np.sqrt(np.log(X.shape[1] + D.shape[1]/2)/X.shape[0])
+lam_seq = np.array([-1.75,-2.0,-2.25])
+lam = [pow(2, x) for x in lam_seq]
+lam = np.array(lam)
+lam = lam_zero * lam
+prob_hat, B_m, lam_opt,  x_hat, d_hat = loo_cv_cor(X_ano[0],D,levels,lam) # perform cv and estimation 
+X_cor, threshold_cont, n_ano_cont,  position_cont = get_threshold_continuous(X_ano, x_hat, B_m) # determine threshold
+```
+
+### Example 3
+
+```python
+from adadmire import impute
+import numpy as np
+
+# load data containing missing values in continuous
+X = np.load('data/Higuera_et_al/data_na_scaled.npy')
+# as well as in discrete features
+D = np.load('data/Higuera_et_al/pheno_na.npy')
+
+print(np.sum(np.isnan(X))) # 1360
+print(np.sum(np.isnan(D))) # 120
+
+levels = np.load('data/Higuera_et_al/levels.npy') # levels of discrete variables
+
+# define Lambda sequence
+lam_zero = np.sqrt(np.log(X.shape[1] + D.shape[1]/2)/X.shape[0])
+lam_seq = np.array([-1.75,-2.0,-2.25])
+lam = [pow(2, x) for x in lam_seq]
+lam = np.array(lam)
+lam = lam_zero * lam
+
+# now impute with ADMIRE
+X_imp, D_imp,lam_o = impute(X,D,levels,lam)
+
+print(np.sum(np.isnan(X_imp))) # 0
+print(np.sum(np.isnan(D_imp))) # 0
+```
+
+### Data
+
+In the directory **data** you can find two sub directories:
+* **Feist_et_al**: contains data set as discribed in [Feist et al, 2018](#feist-et-al-2018) and [Buck et al, 2023](#buck-et-al-2023).
+    * **data_raw.xlsx**: raw, unscaled data, contains measurements of 100 samples and 49 metabolites
+    *  **scaled_data_raw.npy**: numpy file containing scaled version of **data_raw.xlsx**
+    *  **pheno_with_simulations.xlsx**: pheno data corresponding to **data_raw.xlsx**, also contains cell stimulations
+    *  **pheno.npy**: numpy file corresponding to **pheno_with_simulations.xlsx** (only contains variables batch and myc)
+    *  **levels.npy**: numpy file containing the levels of the discrete variables in **pheno.npy**
+* **Higuera_et_al**: contains down sampled data set from [Higuera et al, 2015](#higuera-et-al-2015) as described in [Buck et al, 2023](#buck-et-al-2023).
+    * **data_raw.xlsx**: raw, unscaled data, contains measurements of 400 samples and 68 proteins (down sampled from [Higuera et al, 2015](#higuera-et-al-2015))
+    *  **scaled_data_raw.npy**: numpy file containing scaled version of **data_raw.xlsx**
+    *  **pheno_.xlsx**: pheno data corresponding to **data_raw.xlsx**
+    *  **pheno.npy**: numpy file corresponding to **pheno.xlsx**
+    *  **levels.npy**: numpy file containing the levels of the discrete variables in **pheno.npy**
+    *  **data_na_scaled.npy**: numpy file containing scaled version of **data_raw.xlsx** where 5% of the values are missing
+    *  **pheno_na.npy**: numpy file corresponding to **pheno.xlsx** with 5% of missing values included
+
+## Contribute
+
+In case you have **questions**, **feature requests** or find any **bugs** in adadmire, please create a corresponding issue at [gitlab.spang-lab.de/bul38390/admire/issues](https://github.com/spang-lab/adadmire/issues).
+
+In case you want to **write code** for this package, see [Contribute](https://github.com/spang-lab/adadmire/blob/main/doc/contribute.md) for details.
+
+## References
+
+##### Feist et al, 2018
+
+Feist, Maren, et al. "Cooperative stat/nf-kb signaling regulates lymphoma metabolic reprogramming and aberrant got2 expression." Nature Communications, 2018
+
+##### Higuera et al, 2015
+
+Higuera, Clara et al, "Self-organizing feature maps identify proteins critical to learning in a mouse model of down syndrome." PLOS ONE, 2015
+
+##### Buck et al, 2023
+
+Buck, Lena et al. "Anomaly detection in mixed high dimensional molecular data"
```

### Comparing `adadmire-1.0.1/pyproject.toml` & `adadmire-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "adadmire"
-version = "1.0.01"
-authors = [
-  { name="Lena Buck", email="lena.buck@ukr.de" },
-  { name="Tobias Schmidt", email="tobias2.schmidt@ukr.de" },
-]
-description = "Functions for detecting anomalies in tabular datasets using Mixed Graphical Models."
-dependencies = []
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/spang-lab/adadmire"
-"Bug Tracker" = "https://github.com/spang-lab/adadmire/issues"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "adadmire"
+version = "1.0.2"
+authors = [
+  { name="Lena Buck", email="lena.buck@ukr.de" },
+  { name="Tobias Schmidt", email="tobias2.schmidt@ukr.de" },
+]
+description = "Functions for detecting anomalies in tabular datasets using Mixed Graphical Models."
+dependencies = []
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/spang-lab/adadmire"
+"Bug Tracker" = "https://github.com/spang-lab/adadmire/issues"
```

### Comparing `adadmire-1.0.1/PKG-INFO` & `adadmire-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adadmire
-Version: 1.0.1
+Version: 1.0.2
 Summary: Functions for detecting anomalies in tabular datasets using Mixed Graphical Models.
 Project-URL: Homepage, https://github.com/spang-lab/adadmire
 Project-URL: Bug Tracker, https://github.com/spang-lab/adadmire/issues
 Author-email: Lena Buck <lena.buck@ukr.de>, Tobias Schmidt <tobias2.schmidt@ukr.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,14 +79,44 @@
 lam = [pow(2, x) for x in lam_seq]
 lam = np.array(lam)
 lam = lam_zero * lam
 prob_hat, B_m, lam_opt,  x_hat, d_hat = loo_cv_cor(X_ano[0],D,levels,lam) # perform cv and estimation 
 X_cor, threshold_cont, n_ano_cont,  position_cont = get_threshold_continuous(X_ano, x_hat, B_m) # determine threshold
 ```
 
+### Example 3
+
+```python
+from adadmire import impute
+import numpy as np
+
+# load data containing missing values in continuous
+X = np.load('data/Higuera_et_al/data_na_scaled.npy')
+# as well as in discrete features
+D = np.load('data/Higuera_et_al/pheno_na.npy')
+
+print(np.sum(np.isnan(X))) # 1360
+print(np.sum(np.isnan(D))) # 120
+
+levels = np.load('data/Higuera_et_al/levels.npy') # levels of discrete variables
+
+# define Lambda sequence
+lam_zero = np.sqrt(np.log(X.shape[1] + D.shape[1]/2)/X.shape[0])
+lam_seq = np.array([-1.75,-2.0,-2.25])
+lam = [pow(2, x) for x in lam_seq]
+lam = np.array(lam)
+lam = lam_zero * lam
+
+# now impute with ADMIRE
+X_imp, D_imp,lam_o = impute(X,D,levels,lam)
+
+print(np.sum(np.isnan(X_imp))) # 0
+print(np.sum(np.isnan(D_imp))) # 0
+```
+
 ### Data
 
 In the directory **data** you can find two sub directories:
 * **Feist_et_al**: contains data set as discribed in [Feist et al, 2018](#feist-et-al-2018) and [Buck et al, 2023](#buck-et-al-2023).
     * **data_raw.xlsx**: raw, unscaled data, contains measurements of 100 samples and 49 metabolites
     *  **scaled_data_raw.npy**: numpy file containing scaled version of **data_raw.xlsx**
     *  **pheno_with_simulations.xlsx**: pheno data corresponding to **data_raw.xlsx**, also contains cell stimulations
@@ -94,14 +124,16 @@
     *  **levels.npy**: numpy file containing the levels of the discrete variables in **pheno.npy**
 * **Higuera_et_al**: contains down sampled data set from [Higuera et al, 2015](#higuera-et-al-2015) as described in [Buck et al, 2023](#buck-et-al-2023).
     * **data_raw.xlsx**: raw, unscaled data, contains measurements of 400 samples and 68 proteins (down sampled from [Higuera et al, 2015](#higuera-et-al-2015))
     *  **scaled_data_raw.npy**: numpy file containing scaled version of **data_raw.xlsx**
     *  **pheno_.xlsx**: pheno data corresponding to **data_raw.xlsx**
     *  **pheno.npy**: numpy file corresponding to **pheno.xlsx**
     *  **levels.npy**: numpy file containing the levels of the discrete variables in **pheno.npy**
+    *  **data_na_scaled.npy**: numpy file containing scaled version of **data_raw.xlsx** where 5% of the values are missing
+    *  **pheno_na.npy**: numpy file corresponding to **pheno.xlsx** with 5% of missing values included
 
 ## Contribute
 
 In case you have **questions**, **feature requests** or find any **bugs** in adadmire, please create a corresponding issue at [gitlab.spang-lab.de/bul38390/admire/issues](https://github.com/spang-lab/adadmire/issues).
 
 In case you want to **write code** for this package, see [Contribute](https://github.com/spang-lab/adadmire/blob/main/doc/contribute.md) for details.
```

