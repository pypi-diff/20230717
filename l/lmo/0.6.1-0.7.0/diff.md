# Comparing `tmp/lmo-0.6.1.tar.gz` & `tmp/lmo-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.6.1.tar", max compression
+gzip compressed data, was "lmo-0.7.0.tar", max compression
```

## Comparing `lmo-0.6.1.tar` & `lmo-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
--rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.6.1/LICENSE
--rw-r--r--   0        0        0      792 2023-05-30 00:24:12.512261 lmo-0.6.1/README.md
--rw-r--r--   0        0        0      737 2023-06-04 10:26:56.859497 lmo-0.6.1/lmo/__init__.py
--rw-r--r--   0        0        0    24016 2023-07-03 13:37:20.582165 lmo-0.6.1/lmo/_lm.py
--rw-r--r--   0        0        0    12018 2023-07-03 01:24:30.178022 lmo-0.6.1/lmo/_lm_co.py
--rw-r--r--   0        0        0     2534 2023-07-03 01:16:46.763168 lmo-0.6.1/lmo/_lmm.py
--rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.6.1/lmo/_meta.py
--rw-r--r--   0        0        0     4802 2023-06-04 14:08:29.950996 lmo-0.6.1/lmo/_pwm.py
--rw-r--r--   0        0        0     1615 2023-06-03 20:03:40.058997 lmo-0.6.1/lmo/_utils.py
--rw-r--r--   0        0        0     2240 2023-06-05 14:45:24.686312 lmo-0.6.1/lmo/diagnostic.py
--rw-r--r--   0        0        0     4467 2023-05-30 20:47:52.462490 lmo-0.6.1/lmo/linalg.py
--rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.6.1/lmo/py.typed
--rw-r--r--   0        0        0      521 2023-06-26 00:03:03.516628 lmo-0.6.1/lmo/quad.py
--rw-r--r--   0        0        0     5394 2023-07-03 01:31:40.472197 lmo-0.6.1/lmo/stats.py
--rw-r--r--   0        0        0     1609 2023-05-29 19:12:59.718239 lmo-0.6.1/lmo/typing.py
--rw-r--r--   0        0        0     2147 2023-07-03 13:37:20.566165 lmo-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 lmo-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3865 2023-07-16 04:39:16.565156 lmo-0.7.0/README.md
+-rw-r--r--   0        0        0      752 2023-07-16 21:07:04.201216 lmo-0.7.0/lmo/__init__.py
+-rw-r--r--   0        0        0    21555 2023-07-17 20:38:35.304271 lmo-0.7.0/lmo/_lm.py
+-rw-r--r--   0        0        0    11915 2023-07-16 20:56:43.798563 lmo-0.7.0/lmo/_lm_co.py
+-rw-r--r--   0        0        0      160 2023-07-16 20:51:40.539410 lmo-0.7.0/lmo/_meta.py
+-rw-r--r--   0        0        0     5093 2023-07-16 20:51:26.919089 lmo-0.7.0/lmo/_pwm.py
+-rw-r--r--   0        0        0     4841 2023-07-16 20:46:14.547721 lmo-0.7.0/lmo/_utils.py
+-rw-r--r--   0        0        0     2278 2023-07-16 20:43:58.184505 lmo-0.7.0/lmo/diagnostic.py
+-rw-r--r--   0        0        0    10940 2023-07-16 20:42:19.250171 lmo-0.7.0/lmo/linalg.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.7.0/lmo/py.typed
+-rw-r--r--   0        0        0    10513 2023-07-16 20:22:06.045490 lmo-0.7.0/lmo/theoretical.py
+-rw-r--r--   0        0        0     1682 2023-07-16 19:21:00.902603 lmo-0.7.0/lmo/typing.py
+-rw-r--r--   0        0        0     3825 2023-07-17 21:24:40.836795 lmo-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5156 1970-01-01 00:00:00.000000 lmo-0.7.0/PKG-INFO
```

### Comparing `lmo-0.6.1/LICENSE` & `lmo-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmo-0.6.1/lmo/__init__.py` & `lmo-0.7.0/lmo/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+  # noqa: D104
 __all__ = (
     '__version__',
 
     'l_weights',
     'l_moment',
     'l_moment_cov',
     'l_ratio',
@@ -18,32 +19,32 @@
     'l_coscale',
     'l_corr',
     'l_coskew',
     'l_cokurtosis',
 )
 
 from typing import Final as _Final
-from ._meta import get_version as _get_version
 
 from ._lm import (
-    l_weights,
+    l_kurtosis,
+    l_loc,
     l_moment,
     l_moment_cov,
     l_ratio,
     l_ratio_se,
-    l_loc,
     l_scale,
-    l_variation,
     l_skew,
-    l_kurtosis,
+    l_variation,
+    l_weights,
 )
 from ._lm_co import (
+    l_cokurtosis,
+    l_coloc,
     l_comoment,
     l_coratio,
-    l_coloc,
-    l_coscale,
     l_corr,
+    l_coscale,
     l_coskew,
-    l_cokurtosis,
 )
+from ._meta import get_version as _get_version
 
 __version__: _Final[str] = _get_version()
```

### Comparing `lmo-0.6.1/lmo/_lm.py` & `lmo-0.7.0/lmo/_lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Unbiased sample estimators of the generalized trimmed L-moments.
-"""
+"""Unbiased sample estimators of the generalized trimmed L-moments."""
 
 __all__ = (
     'l_weights',
     'l_moment',
     'l_moment_cov',
     'l_ratio',
     'l_ratio_se',
@@ -17,158 +15,101 @@
 
 from typing import Any, Final, TypeVar, cast
 
 import numpy as np
 import numpy.typing as npt
 
 from ._pwm import b_moment_cov, b_weights
-from ._utils import clean_order, ensure_axis_at
-from .linalg import hosking_jacobi, sandwich, sh_legendre
-from .stats import ordered
+from ._utils import clean_order, ensure_axis_at, ordered
+from .linalg import sandwich, sh_legendre, trim_matrix
 from .typing import AnyInt, IntVector, SortKind
 
 T = TypeVar('T', bound=np.floating[Any])
 
 
 # Low-level weight methods
 
 _L_WEIGHTS_CACHE: Final[
     dict[
         tuple[int, int, int],  # (n, t_1, t_2)
-        npt.NDArray[np.floating[Any]]
+        npt.NDArray[np.floating[Any]],
     ]
 ] = {}
 
 def _l0_weights(
     r: int,
     n: int,
     /,
     dtype: np.dtype[T] | type[T] = np.float_,
-    *,
-    enforce_symmetry: bool = True,
 ) -> npt.NDArray[T]:
-    """
-    Efficiently calculates the projection matrix $P = [p_{k, i}]_{r \\times n}$
+    r"""
+    Efficiently calculates the projection matrix $P = [p_{k, i}]_{r \times n}$
     for the order statistics $x_{i:n}$.
-    This way, the $1, 2, ..., r$-th order sample L-moments of some sample vector
-    $x$, can be estimated with `np.sort(x) @ l_weights(len(x), r)`.
+    This way, the $1, 2, ..., r$-th order sample L-moments of some sample
+    vector $x$, can be estimated with `np.sort(x) @ l_weights(len(x), r)`.
 
     Parameters:
-        r: The amount of orders to evaluate, i.e. $k = 1, \\dots, r$.
+        r: The amount of orders to evaluate, i.e. $k = 1, \dots, r$.
         n: Sample count.
         dtype: Desired output floating data type.
 
-    Other parameters:
-        enforce_symmetry:
-            If set to False, disables symmetry-based numerical noise correction.
-
     Returns:
         P_r: 2-D array of shape `(r, n)`.
 
     References:
         - [J.R.M. Hosking (2007) - Some theory and practical uses of trimmed
             L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
-
     """
-    P_r = np.empty((r, n), dtype)
+    p_r = np.empty((r, n), dtype)
 
-    if r == 0:
-        return P_r
-
-    np.matmul(sh_legendre(r), b_weights(r, n, dtype), out=P_r)
+    if r > 0:
+        np.matmul(sh_legendre(r), b_weights(r, n, dtype), out=p_r)
 
-    if enforce_symmetry:
-        # enforce rotational symmetry of even orders `r = 2, 4, ...`, naturally
-        # centering them around 0
-        for k in range(2, r + 1, 2):
-            p_k: npt.NDArray[T] = P_r[k - 1]
-
-            med = 0.0
-            pk_neg, pk_pos = p_k < med, p_k > med
-            # n_neg, n_pos = pk_neg.sum(), pk_pos.sum()
-            n_neg, n_pos = np.count_nonzero(pk_neg), np.count_nonzero(pk_pos)
-
-            # attempt to correct 1-off asymmetry
-            if abs(n_neg - n_pos) == 1:
-                if n % 2:
-                    # balance the #negative and #positive for odd `n` by
-                    # ignoring the center
-                    mid = (n - 1) // 2
-                    pk_neg[mid] = pk_pos[mid] = False
-                    # n_neg, n_pos = pk_neg.sum(), pk_pos.sum()
-                    n_neg = np.count_nonzero(pk_neg)
-                    n_pos = np.count_nonzero(pk_pos)
-                else:
-                    # if one side is half of n, set the other to it's negation
-                    mid = n // 2
-                    if n_neg == mid:
-                        pk_pos = ~pk_neg
-                        n_pos = n_neg
-                    elif n_pos == mid:
-                        pk_neg = ~pk_pos
-                        n_neg = n_pos
-
-            # attempt to correct any large asymmetry offsets
-            # and don't worry; median is O(n)
-            if abs(n_neg - n_pos) > 1 and (med := np.median(p_k)):
-                pk_neg, pk_pos = p_k < med, p_k > med
-                n_neg = np.count_nonzero(pk_neg)
-                n_pos = np.count_nonzero(pk_pos)
-
-            if n_neg == n_pos:
-                # it's pretty rare that this isn't the case
-                p_k[pk_neg] = -p_k[pk_pos][::-1]
-
-        # enforce horizontal (axis 1) symmetry for the odd orders (except k=1)
-        # and shift to zero mean
-        P_r[2::2, :n // 2] = P_r[2::2, :(n - 1) // 2: -1]
-        P_r[2::2] -= P_r[2::2].mean(1, keepdims=True)
-
-    return P_r
+    return p_r
 
 
 def l_weights(
     r: int,
     n: int,
     /,
     trim: tuple[int, int] = (0, 0),
     dtype: np.dtype[T] | type[T] = np.float_,
     *,
-    cache: bool = False
+    cache: bool = False,
 ) -> npt.NDArray[T]:
-    """
+    r"""
     Projection matrix of the first $r$ (T)L-moments for $n$ samples.
 
     The matrix is a linear combination of the Power Weighted Moment
     (PWM) weight matrix (the sample estimator of $beta_{r_1}$), and the
     shifted Legendre polynomials.
 
     If `trim != (0, 1)`, a linearized (and corrected) adaptation of the
     recurrence relations from *Hosking (2007)* are applied, as well.
 
     $$
-    (2k + t_1 + t_2 - 1) \\lambda^{(t_1, t_2)}_k
-        = (k + t_1 + t_2) \\lambda^{(t_1 - 1, t_2)}_k
-        + \\frac{1}{k} (k + 1) (k + t_2) \\lambda^{(t_1 - 1, t_2)}_{k+1}
+    (2k + t_1 + t_2 - 1) \lambda^{(t_1, t_2)}_k
+        = (k + t_1 + t_2) \lambda^{(t_1 - 1, t_2)}_k
+        + \frac{1}{k} (k + 1) (k + t_2) \lambda^{(t_1 - 1, t_2)}_{k+1}
     $$
 
     for $t_1 > 0$, and
 
     $$
-    (2k + t_1 + t_2 - 1) \\lambda^{(t_1, t_2)}_k
-        = (k + t_1 + t_2) \\lambda^{(t_1, t_2 - 1)}_k
-        - \\frac{1}{k} (k + 1) (k + t_1) \\lambda^{(t_1, t_2 - 1)}_{k+1}
+    (2k + t_1 + t_2 - 1) \lambda^{(t_1, t_2)}_k
+        = (k + t_1 + t_2) \lambda^{(t_1, t_2 - 1)}_k
+        - \frac{1}{k} (k + 1) (k + t_1) \lambda^{(t_1, t_2 - 1)}_{k+1}
     $$
 
     for $t_2 > 0$.
 
     TLDR:
         This matrix (linearly) transforms $x_{i:n}$ (i.e. the sorted
         observation vector(s) of size $n$), into (an unbiased estimate of) the
-        *generalized trimmed L-moments*, with orders $\\le r$.
+        *generalized trimmed L-moments*, with orders $\le r$.
 
     Returns:
         P_r: 2-D array of shape `(r, n)`.
 
     Examples:
         >>> import lmo
         >>> lmo.l_weights(3, 4)
@@ -177,61 +118,60 @@
                [ 0.25      , -0.25      , -0.25      ,  0.25      ]])
         >>> _ @ [-1, 0, 1 / 2, 3 / 2]
         array([0.25      , 0.66666667, 0.        ])
 
     References:
         - [J.R.M. Hosking (2007) - Some theory and practical uses of trimmed
             L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
-
     """
     cache_key = n, *trim
     if (
         cache_key in _L_WEIGHTS_CACHE
-        and (P_r := _L_WEIGHTS_CACHE[cache_key]).shape[0] <= r
+        and (p_r := _L_WEIGHTS_CACHE[cache_key]).shape[0] <= r
     ):
-        if P_r.dtype is not np.dtype(dtype):
-            P_r = P_r.view(dtype)
-        if P_r.shape[0] < r:
-            P_r = P_r[:r]
+        if p_r.dtype is not np.dtype(dtype):
+            p_r = p_r.view(dtype)
+        if p_r.shape[0] < r:
+            p_r = p_r[:r]
 
         # ignore if r is larger that what's cached
-        if P_r.shape[0] == r:
-            assert P_r.shape == (r, n)
-            return cast(npt.NDArray[T], P_r)
+        if p_r.shape[0] == r:
+            assert p_r.shape == (r, n)
+            return cast(npt.NDArray[T], p_r)
 
 
     if sum(trim) == 0:
         return _l0_weights(r, n, dtype)
 
-    P_r = np.empty((r, n), dtype)
+    p_r = np.empty((r, n), dtype)
 
     if r == 0:
-        return P_r
+        return p_r
 
     # the k-th TL-(t_1, t_2) weights are a linear combination of L-weights
     # with orders k, ..., k + t_1 + t_2
 
     np.matmul(
-        hosking_jacobi(r, trim),
+        trim_matrix(r, trim),
         _l0_weights(r + sum(trim), n),
-        out=P_r
+        out=p_r,
     )
 
     # remove numerical noise from the trimmings, and correct for potential
     # shifts in means
     t1, t2 = trim
-    P_r[:, :t1] = P_r[:, n - t2:] = 0
-    P_r[1:, t1:n - t2] -= P_r[1:, t1:n - t2].mean(1, keepdims=True)
+    p_r[:, :t1] = p_r[:, n - t2:] = 0
+    p_r[1:, t1:n - t2] -= p_r[1:, t1:n - t2].mean(1, keepdims=True)
 
     if cache:
         # memoize, and mark as readonly to avoid corruping the cache
-        P_r.setflags(write=False)
-        _L_WEIGHTS_CACHE[cache_key] = P_r
+        p_r.setflags(write=False)
+        _L_WEIGHTS_CACHE[cache_key] = p_r
 
-    return P_r
+    return p_r
 
 
 # Summary statistics
 
 def l_moment(
     a: npt.ArrayLike,
     r: AnyInt | IntVector,
@@ -241,18 +181,18 @@
     dtype: np.dtype[T] | type[T] = np.float_,
     *,
     fweights: IntVector | None = None,
     aweights: npt.ArrayLike | None = None,
     sort: SortKind | None = 'stable',
     cache: bool = False,
 ) -> T | npt.NDArray[T]:
-    """
-    Estimates the generalized trimmed L-moment $\\lambda^{(t_1, t_2)}_r$ from
+    r"""
+    Estimates the generalized trimmed L-moment $\lambda^{(t_1, t_2)}_r$ from
     the samples along the specified axis. By default, this will be the regular
-    L-moment, $\\lambda_r = \\lambda^{(0, 0)}_r$.
+    L-moment, $\lambda_r = \lambda^{(0, 0)}_r$.
 
     Parameters:
         a:
             Array containing numbers whose L-moments is desired.
             If `a` is not an array, a conversion is attempted.
 
         r:
@@ -334,37 +274,29 @@
 
     References:
         - [J.R.M. Hosking (1990)](https://jstor.org/stable/2345653)
         - [E. Elamir & A. Seheult (2003) - Trimmed L-moments](
             https://doi.org/10.1016/S0167-9473(02)00250-5)
         - [J.R.M. Hosking (2007) - Some theory and practical uses of trimmed
             L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
-
     """
-    # weight-adjusted $x_{i:n}$
     x_k = ordered(
         a,
         axis=axis,
         dtype=dtype,
         fweights=fweights,
         aweights=aweights,
         sort=sort,
     )
     x_k = ensure_axis_at(x_k, axis, -1)
-
-    r_max: int = clean_order(cast(
-        int,
-        np.max(np.asarray(r))  # pyright: ignore [reportUnknownMemberType]
-    ))
     n = x_k.shape[-1]
 
-    # projection matrix
-    P_r = l_weights(r_max, n, trim, dtype=dtype, cache=cache)
+    r_max = clean_order(np.max(np.asarray(r)))
 
-    l_r = np.inner(P_r, x_k)
+    l_r = np.inner(l_weights(r_max, n, trim, dtype=dtype, cache=cache), x_k)
 
     # we like 0-based indexing; so if P_r starts at r=1, prepend all 1's
     # for r=0 (any zeroth moment is defined to be 1)
     l_r = np.r_[np.ones((1, *l_r.shape[1:]), dtype=l_r.dtype), l_r]
 
     assert np.all(l_r[0] == 1)
     assert len(l_r) == r_max + 1, (l_r.shape, r_max)
@@ -420,47 +352,49 @@
             https://doi.org/10.1016/S0167-9473(02)00250-5)
         - [E. Elamir & A. Seheult (2004) - Exact variance structure of sample
             L-moments](https://doi.org/10.1016/S0378-3758(03)00213-1)
 
     """
     ks = int(r_max + sum(trim))
     if ks < r_max:
-        raise ValueError('trimmings must be positive')
+        msg = 'trimmings must be positive'
+        raise ValueError(msg)
 
-    # PWM covariance matrix
-    S_b = b_moment_cov(a, ks, axis=axis, dtype=dtype, **kwargs)
 
     # projection matrix: PWMs -> generalized trimmed L-moments
-    P_l: npt.NDArray[np.floating[Any]]
-    P_l = hosking_jacobi(int(r_max), trim=trim, dtype=dtype) @ sh_legendre(ks)
+    p_l: npt.NDArray[np.floating[Any]]
+    p_l = trim_matrix(int(r_max), trim=trim, dtype=dtype) @ sh_legendre(ks)
     # clean some numerical noise
-    P_l = np.round(P_l, 12) + 0.  # pyright: ignore [reportUnknownMemberType]
+    p_l = np.round(p_l, 12) + 0.
+
+    # PWM covariance matrix
+    s_b = b_moment_cov(a, ks, axis=axis, dtype=dtype, **kwargs)
 
     # tasty, eh?
-    return sandwich(P_l, S_b, dtype=dtype)
+    return sandwich(p_l, s_b, dtype=dtype)
 
 
 def l_ratio(
     a: npt.ArrayLike,
     r: AnyInt | IntVector,
     s: AnyInt | IntVector,
     /,
     trim: tuple[int, int] = (0, 0),
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> T | npt.NDArray[T]:
-    """
+    r"""
     Estimates the generalized L-moment ratio:
 
     $$
-    \\tau^{(t_1, t_2)}_{rs} = \\frac{
-        \\lambda^{(t_1, t_2)}_r
+    \tau^{(t_1, t_2)}_{rs} = \frac{
+        \lambda^{(t_1, t_2)}_r
     }{
-        \\lambda^{(t_1, t_2)}_s
+        \lambda^{(t_1, t_2)}_s
     }
     $$
 
     Equivalent to `lmo.l_moment(a, r, *, **) / lmo.l_moment(a, s, *, **)`.
 
     Notes:
         The L-moment with `r=0` is `1`, so the `l_ratio(a, r, 0, *, **)` is
@@ -475,35 +409,34 @@
         >>> lmo.l_ratio(x, [1, 2, 3, 4], [0, 0, 2, 2])
         array([1.53196368, 0.77549561, 0.4463163 , 0.29752178])
         >>> lmo.l_ratio(x, [1, 2, 3, 4], [0, 0, 2, 2], trim=(0, 1))
         array([0.75646807, 0.32203446, 0.23887609, 0.07917904])
 
     See Also:
         - [`lmo.l_moment`][lmo.l_moment]
-
-    """
+    """  # noqa: D415
     _r, _s = np.asarray(r), np.asarray(s)
     rs = np.stack(np.broadcast_arrays(_r, _s))
 
     l_rs = cast(
         npt.NDArray[T],
-        l_moment(a, rs, trim, axis=axis, dtype=dtype, **kwargs)
+        l_moment(a, rs, trim, axis=axis, dtype=dtype, **kwargs),
     )
 
     r_eq_s = _r == _s
     if r_eq_s.ndim < l_rs.ndim - 1:
         r_eq_s = r_eq_s.reshape(
-            r_eq_s.shape + (1,) * (l_rs.ndim - r_eq_s.ndim - 1)
+            r_eq_s.shape + (1,) * (l_rs.ndim - r_eq_s.ndim - 1),
         )
 
     with np.errstate(divide='ignore'):
         return np.where(
             r_eq_s,
             np.ones_like(l_rs[0]),
-            np.divide(l_rs[0], l_rs[1], where=~r_eq_s)
+            np.divide(l_rs[0], l_rs[1], where=~r_eq_s),
         )[()]
 
 
 
 def l_ratio_se(
     a: npt.ArrayLike,
     r: AnyInt | IntVector,
@@ -542,34 +475,31 @@
             https://doi.org/10.1016/S0167-9473(02)00250-5)
         - [E. Elamir & A. Seheult (2004) - Exact variance structure of sample
             L-moments](https://doi.org/10.1016/S0378-3758(03)00213-1)
 
     """
     _r, _s = np.broadcast_arrays(np.asarray(r), np.asarray(s))
     _rs = np.stack((_r, _s))
-    r_max: AnyInt = np.amax(  # pyright: ignore [reportUnknownMemberType]
-        np.r_[_r, _s].ravel()
-    )
+    r_max: AnyInt = np.amax(np.r_[_r, _s].ravel())
 
     # L-moments
     l_rs = cast(npt.NDArray[T], l_moment(a, _rs, trim, axis, dtype, **kwargs))
     l_r, l_s = l_rs[0], l_rs[1]
 
     # L-moment auto-covariance matrix
-    S_l = l_moment_cov(a, r_max, trim, axis, dtype, **kwargs)
+    k_l = l_moment_cov(a, r_max, trim, axis, dtype, **kwargs)
     # prepend the "zeroth" moment, with has 0 (co)variance
-    S_l = np.pad(S_l, (1, 0), constant_values=0)
+    k_l = np.pad(k_l, (1, 0), constant_values=0)
 
-    s_rr = S_l[_r, _r]  # Var[l_r]
-    s_ss = S_l[_s, _s]  # Var[l_r]
-    s_rs = S_l[_r, _s]  # Cov[l_r, l_s]
+    s_rr = k_l[_r, _r]  # Var[l_r]
+    s_ss = k_l[_s, _s]  # Var[l_r]
+    s_rs = k_l[_r, _s]  # Cov[l_r, l_s]
 
     # the classic approximation to propagation of uncertainty for an RV ratio
     with np.errstate(divide='ignore', invalid='ignore'):
-        # TODO: np.piecewiese ?
         _s_tt = (l_r / l_s)**2 * (
             s_rr / l_r**2 +
             s_ss / l_s**2 -
             2 * s_rs / (l_r * l_s)
         )
         # Var[l_r / l_r] = Var[1] = 0
         _s_tt = np.where(_s == 0, s_rr, _s_tt)
@@ -583,17 +513,17 @@
     a: npt.ArrayLike,
     /,
     trim: tuple[int, int] = (0, 0),
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> T | npt.NDArray[T]:
-    """
+    r"""
     *L-location* (or *L-loc*): unbiased estimator of the first L-moment,
-    $\\lambda^{(t_1, t_2)}_1$.
+    $\lambda^{(t_1, t_2)}_1$.
 
     Alias for [`lmo.l_moment(a, 1, *, **)`][lmo.l_moment].
 
     Examples:
         >>> import lmo, numpy as np
         >>> x = np.random.default_rng(12345).standard_cauchy(99)
         >>> x.mean()
@@ -606,30 +536,29 @@
     Notes:
         If `trim = (0, 0)` (default), the L-location is equivalent to the
         [arithmetic mean](https://wikipedia.org/wiki/Arithmetic_mean).
 
     See Also:
         - [`lmo.l_moment`][lmo.l_moment]
         - [`numpy.average`][numpy.average]
-
     """
     return l_moment(a, 1, trim, axis, dtype, **kwargs)
 
 
 def l_scale(
     a: npt.ArrayLike,
     /,
     trim: tuple[int, int] = (0, 0),
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> T | npt.NDArray[T]:
-    """
+    r"""
     *L-scale*: unbiased estimator of the second L-moment,
-    $\\lambda^{(t_1, t_2)}_2$
+    $\lambda^{(t_1, t_2)}_2$.
 
     Alias for [`lmo.l_moment(a, 2, *, **)`][lmo.l_moment].
 
     Examples:
         >>> import lmo, numpy as np
         >>> x = np.random.default_rng(12345).standard_cauchy(99)
         >>> x.std()
@@ -643,35 +572,34 @@
         If `trim = (0, 0)` (default), the L-scale is equivalent to half the
         [Gini mean difference (GMD)](
         https://wikipedia.org/wiki/Gini_mean_difference).
 
     See Also:
         - [`lmo.l_moment`][lmo.l_moment]
         - [`numpy.std`][numpy.std]
-
     """
     return l_moment(a, 2, trim, axis, dtype, **kwargs)
 
 
 def l_variation(
     a: npt.ArrayLike,
     /,
     trim: tuple[int, int] = (0, 0),
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> T | npt.NDArray[T]:
-    """
+    r"""
     The *coefficient of L-variation* (or *L-CV*) unbiased sample estimator:
 
     $$
-    \\tau^{(t_1, t_2)} = \\frac{
-        \\lambda^{(t_1, t_2)}_2
+    \tau^{(t_1, t_2)} = \frac{
+        \lambda^{(t_1, t_2)}_2
     }{
-        \\lambda^{(t_1, t_2)}_1
+        \lambda^{(t_1, t_2)}_1
     }
     $$
 
     Alias for [`lmo.l_ratio(a, 2, 1, *, **)`][lmo.l_ratio].
 
     Examples:
         >>> import lmo, numpy as np
@@ -689,37 +617,36 @@
         and lies within the interval $(0, 1)$.
 
     See Also:
         - [Gini coefficient - Wikipedia](
             https://wikipedia.org/wiki/Gini_coefficient)
         - [`lmo.l_ratio`][lmo.l_ratio]
         - [`scipy.stats.variation.l_ratio`][scipy.stats.variation]
-
-    """
+    """  # noqa: D415
     return l_ratio(a, 2, 1, trim, axis, dtype, **kwargs)
 
 
 def l_skew(
     a: npt.ArrayLike,
     /,
     trim: tuple[int, int] = (0, 0),
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> T | npt.NDArray[T]:
-    """
+    r"""
     Unbiased sample estimator of the *coefficient of L-skewness*, or *L-skew*
     for short:
 
     $$
-    \\tau^{(t_1, t_2)}_3
-        = \\frac{
-            \\lambda^{(t_1, t_2)}_3
+    \tau^{(t_1, t_2)}_3
+        = \frac{
+            \lambda^{(t_1, t_2)}_3
         }{
-            \\lambda^{(t_1, t_2)}_2
+            \lambda^{(t_1, t_2)}_2
         }
     $$
 
     Alias for [`lmo.l_ratio(a, 3, 2, *, **)`][lmo.l_ratio].
 
     Examples:
         >>> import lmo, numpy as np
@@ -728,53 +655,51 @@
         0.38524343...
         >>> lmo.l_skew(x, trim=(0, 1))
         0.27116139...
 
     See Also:
         - [`lmo.l_ratio`][lmo.l_ratio]
         - [`scipy.stats.skew`][scipy.stats.skew]
-
-    """
+    """  # noqa: D415
     return l_ratio(a, 3, 2, trim, axis, dtype, **kwargs)
 
 
 def l_kurtosis(
     a: npt.ArrayLike,
     /,
     trim: tuple[int, int] = (0, 0),
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> T | npt.NDArray[T]:
-    """
+    r"""
     L-kurtosis coefficient; the 4th sample L-moment ratio.
 
     $$
-    \\tau^{(t_1, t_2)}_4
-        = \\frac{
-            \\lambda^{(t_1, t_2)}_4
+    \tau^{(t_1, t_2)}_4
+        = \frac{
+            \lambda^{(t_1, t_2)}_4
         }{
-            \\lambda^{(t_1, t_2)}_2
+            \lambda^{(t_1, t_2)}_2
         }
     $$
 
     Alias for [`lmo.l_ratio(a, 4, 2, *, **)`][lmo.l_ratio].
 
     Examples:
         >>> import lmo, numpy as np
         >>> x = np.random.default_rng(12345).standard_t(2, 99)
         >>> lmo.l_kurtosis(x)
         0.28912787...
         >>> lmo.l_kurtosis(x, trim=(1, 1))
         0.19928182...
 
     Notes:
-        The L-kurtosis $\\tau_4$ lies within the interval
-        $[-\\frac{1}{4}, 1)$, and by the L-skewness $\\tau_3$ as
-        $5 \\tau_3^2 - 1 \\le 4 \\tau_4$.
+        The L-kurtosis $\tau_4$ lies within the interval
+        $[-\frac{1}{4}, 1)$, and by the L-skewness $\\tau_3$ as
+        $5 \tau_3^2 - 1 \le 4 \tau_4$.
 
     See Also:
         - [`lmo.l_ratio`][lmo.l_ratio]
         - [`scipy.stats.kurtosis`][scipy.stats.kurtosis]
-
     """
     return l_ratio(a, 4, 2, trim, axis, dtype, **kwargs)
```

### Comparing `lmo-0.6.1/lmo/_lm_co.py` & `lmo-0.7.0/lmo/_lm_co.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 )
 
 from typing import Any, TypeVar, cast
 
 import numpy as np
 from numpy import typing as npt
 
-from ._utils import clean_order
 from ._lm import l_weights
-from .stats import ordered
+from ._utils import clean_order, ordered
 from .typing import AnyInt, IntVector, SortKind
 
 T = TypeVar('T', bound=np.floating[Any])
 
 
 def l_comoment(
     a: npt.ArrayLike,
@@ -28,32 +27,33 @@
     trim: tuple[int, int] = (0, 0),
     rowvar: bool = True,
     dtype: np.dtype[T] | type[T] = np.float_,
     *,
     sort: SortKind | None = 'stable',
     cache: bool = False,
 ) -> npt.NDArray[T]:
-    """
-    Multivariate extension of [`lmo.l_moment`][lmo.l_moment]. Estimates the
-    L-comoment matrix:
+    r"""
+    Multivariate extension of [`lmo.l_moment`][lmo.l_moment].
+
+    Estimates the L-comoment matrix:
 
     $$
-    \\Lambda_{r}^{(t_1, t_2)} =
-        \\left[
-            \\lambda_{r [ij]}^{(t_1, t_2)}
-        \\right]_{m \\times m}
+    \Lambda_{r}^{(t_1, t_2)} =
+        \left[
+            \lambda_{r [ij]}^{(t_1, t_2)}
+        \right]_{m \times m}
     $$
 
     Whereas the L-moments are calculated using the order statistics of the
     observations, i.e. by sorting, the L-comoment sorts $x_i$ using the
     order of $x_j$. This means that in general,
-    $\\lambda_{r [ij]}^{(t_1, t_2)} \\neq \\lambda_{r [ji]}^{(t_1, t_2)}$, i.e.
-    $\\Lambda_{r}^{(t_1, t_2)}$ is not symmetric.
+    $\lambda_{r [ij]}^{(t_1, t_2)} \neq \lambda_{r [ji]}^{(t_1, t_2)}$, i.e.
+    $\Lambda_{r}^{(t_1, t_2)}$ is not symmetric.
 
-    The $r$-th L-comoment $\\lambda_{r [ij]}^{(t_1, t_2)}$ reduces to the
+    The $r$-th L-comoment $\lambda_{r [ij]}^{(t_1, t_2)}$ reduces to the
     L-moment if $i=j$, and can therefore be seen as a generalization of the
     (univariate) L-moments. Similar to how the diagonal of a covariance matrix
     contains the variances, the diagonal of the L-comoment matrix contains the
     L-moments.
 
     Based on the proposed definition by Serfling & Xiao (2007) for L-comoments.
     Extended to allow for generalized trimming.
@@ -125,104 +125,100 @@
         The diagonal contains the univariate L-moments:
 
         >>> lmo.l_moment(x, 2, axis=-1)
         array([1.2766793 , 1.05990727])
 
     References:
         * [R. Serfling & P. Xiao (2007) - A Contribution to Multivariate
-            L-Moments: L-Comoment Matrices](https://doi.org/10.1016/j.jmva.2007.01.008)
-
+          L-Moments: L-Comoment Matrices](https://doi.org/10.1016/j.jmva.2007.01.008)
     """
     def _clean_array(arr: npt.ArrayLike) -> npt.NDArray[T]:
         out = np.asanyarray(arr, dtype=dtype)
         return out if rowvar else out.T
 
     x = np.atleast_2d(_clean_array(a))
     if x.ndim != 2:
-        raise ValueError(f'sample array must be 2-D, got {x.ndim}')
+        msg = f'sample array must be 2-D, got {x.ndim}'
+        raise ValueError(msg)
 
     _r = np.asarray(r)
-    r_max: int = clean_order(cast(
-        int,
-        np.max(_r)  # pyright: ignore [reportUnknownMemberType]
-    ))
+    r_max = clean_order(cast(int, np.max(_r)))
     m, n = x.shape
 
     if not m:
-        return np.empty(np.shape(_r) + (0, 0), dtype=dtype)
+        return np.empty((*np.shape(_r), 0, 0), dtype=dtype)
 
     # projection matrix of shape (r, n)
-    P_r = l_weights(r_max, n, trim, dtype=dtype, cache=cache)
+    p_r = l_weights(r_max, n, trim, dtype=dtype, cache=cache)
 
     # L-comoment matrices for r = 0, ..., r_max
-    L_ij = np.empty((r_max + 1, m, m), dtype=dtype)
+    l_ij = np.empty((r_max + 1, m, m), dtype=dtype)
 
     # the zeroth L-comoment is the delta function, so the L-comoment
     # matrix is the identity matrix
-    L_ij[0] = np.eye(m, dtype=dtype)
+    l_ij[0] = np.eye(m, dtype=dtype)
 
     for j in range(m):
         # concomitants of x[i] w.r.t. x[j] for all i
         x_k_ij = ordered(x, x[j], axis=-1, dtype=dtype, sort=sort)
 
-        L_ij[1:, :, j] = np.inner(P_r, x_k_ij)
+        l_ij[1:, :, j] = np.inner(p_r, x_k_ij)
 
-    return L_ij.take(_r, 0)  # pyright: ignore [reportUnknownMemberType]
+    return l_ij.take(_r, 0)  # pyright: ignore [reportUnknownMemberType]
 
 
 def l_coratio(
     a: npt.ArrayLike,
     r: AnyInt | IntVector,
     s: AnyInt | IntVector,
     /,
     trim: tuple[int, int] = (0, 0),
     rowvar: bool = True,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> npt.NDArray[T]:
-    """
-    Estimate the generalized matrix of L-comoment ratio's:
+    r"""
+    Estimate the generalized matrix of L-comoment ratio's.
 
     $$
-    \\tilde \\Lambda_{rs}^{(t_1, t_2)} =
-        \\left[
-            \\left. \\lambda_{r [ij]}^{(t_1, t_2)} \\right/
-            \\lambda_{s [jj]}^{(t_1, t_2)}
-        \\right]_{m \\times m}
+    \tilde \Lambda_{rs}^{(t_1, t_2)} =
+        \left[
+            \left. \lambda_{r [ij]}^{(t_1, t_2)} \right/
+            \lambda_{s [jj]}^{(t_1, t_2)}
+        \right]_{m \times m}
     $$
 
     See Also:
         - [`lmo.l_comoment`][lmo.l_comoment]
         - [`lmo.l_ratio`][lmo.l_ratio]
-
     """
     rs = np.stack(np.broadcast_arrays(np.asarray(r), np.asarray(s)))
-    L_r, L_s = l_comoment(a, rs, trim, rowvar=rowvar, dtype=dtype, **kwargs)
+    l_r, l_s = l_comoment(a, rs, trim, rowvar=rowvar, dtype=dtype, **kwargs)
 
-    l_s = np.diagonal(L_s, axis1=-2, axis2=-1)
+    l_s = np.diagonal(l_s, axis1=-2, axis2=-1)
 
-    return L_r / np.expand_dims(l_s, -1)
+    return l_r / np.expand_dims(l_s, -1)
 
 
 def l_coloc(
     a: npt.ArrayLike,
     /,
     trim: tuple[int, int] = (0, 0),
     rowvar: bool = True,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> npt.NDArray[T]:
-    """
-    L-colocation matrix of 1st L-comoment estimates, $\\Lambda^{(t_1, t_2)}_1$.
+    r"""
+    L-colocation matrix of 1st L-comoment estimates, $\Lambda^{(t_1, t_2)}_1$.
 
     Alias for [`lmo.l_comoment(a, 1, *, **)`][lmo.l_comoment].
 
     Notes:
         If `trim = (0, 0)` (default), the L-colocation for $[ij]$ is the
-        L-location $\\lambda_1$ of $x_i$, independent of $x_j$.
+        L-location $\lambda_1$ of $x_i$, independent of $x_j$.
 
     Examples:
         Without trimming, the L-colocation only provides marginal information:
 
         >>> import lmo, numpy as np
         >>> rng = np.random.default_rng(12345)
         >>> x = rng.multivariate_normal([0, 0], [[6, -3], [-3, 3.5]], 99).T
@@ -244,29 +240,28 @@
         been only been briefly *mentioned* once or twice in the literature.
 
 
     See Also:
         - [`lmo.l_comoment`][lmo.l_comoment]
         - [`lmo.l_loc`][lmo.l_loc]
         - [`numpy.mean`][numpy.mean]
-
     """
     return l_comoment(a, 1, trim, rowvar=rowvar, dtype=dtype, **kwargs)
 
 
 def l_coscale(
     a: npt.ArrayLike,
     /,
     trim: tuple[int, int] = (0, 0),
     rowvar: bool = True,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> npt.NDArray[T]:
-    """
-    L-coscale matrix of 2nd L-comoment estimates, $\\Lambda^{(t_1, t_2)}_2$.
+    r"""
+    L-coscale matrix of 2nd L-comoment estimates, $\Lambda^{(t_1, t_2)}_2$.
 
     Alias for [`lmo.l_comoment(a, 2, *, **)`][lmo.l_comoment].
 
     Analogous to the (auto-) variance-covariance matrix, the L-coscale matrix
     is positive semi-definite, and its main diagonal contains the L-scale's.
     conversely, the L-coscale matrix is inherently assymmetric, thus yielding
     more information.
@@ -281,29 +276,28 @@
         array([[ 0.66698774, -0.41025416],
                [-0.37918065,  0.54440895]])
 
     See Also:
         - [`lmo.l_comoment`][lmo.l_comoment]
         - [`lmo.l_scale`][lmo.l_scale]
         - [`numpy.cov`][numpy.cov]
-
     """
     return l_comoment(a, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
 
 
 def l_corr(
     a: npt.ArrayLike,
     /,
     trim: tuple[int, int] = (0, 0),
     rowvar: bool = True,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> npt.NDArray[T]:
-    """
-    Sample L-correlation coefficient matrix $\\tilde\\Lambda^{(t_1, t_2)}_2$;
+    r"""
+    Sample L-correlation coefficient matrix $\tilde\Lambda^{(t_1, t_2)}_2$;
     the ratio of the L-coscale matrix over the L-scale **column**-vectors.
 
     Alias for [`lmo.l_coratio(a, 2, 2, *, **)`][lmo.l_coratio].
 
     The diagonal consists of all 1's.
 
     Where the pearson correlation coefficient measures linearity, the
@@ -325,57 +319,52 @@
 
         and the (Pearson) correlation coefficient matrix:
 
         >>> np.corrcoef(x)
         array([[ 1.        , -0.66383285],
                [-0.66383285,  1.        ]])
 
-
-
     See Also:
         - [`lmo.l_coratio`][lmo.l_coratio]
         - [`numpy.corrcoef`][numpy.corrcoef]
-
     """
     return l_coratio(a, 2, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
 
 
 def l_coskew(
     a: npt.ArrayLike,
     /,
     trim: tuple[int, int] = (0, 0),
     rowvar: bool = True,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> npt.NDArray[T]:
-    """
-    Sample L-coskewness coefficient matrix $\\tilde\\Lambda^{(t_1, t_2)}_3$.
+    r"""
+    Sample L-coskewness coefficient matrix $\tilde\Lambda^{(t_1, t_2)}_3$.
 
     Alias for [`lmo.l_coratio(a, 3, 2, *, **)`][lmo.l_coratio].
 
     See Also:
         - [`lmo.l_coratio`][lmo.l_coratio]
         - [`lmo.l_skew`][lmo.l_skew]
-
     """
     return l_coratio(a, 3, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
 
 
 def l_cokurtosis(
     a: npt.ArrayLike,
     /,
     trim: tuple[int, int] = (0, 0),
     rowvar: bool = True,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> npt.NDArray[T]:
-    """
-    Sample L-cokurtosis coefficient matrix $\\tilde\\Lambda^{(t_1, t_2)}_4$.
+    r"""
+    Sample L-cokurtosis coefficient matrix $\tilde\Lambda^{(t_1, t_2)}_4$.
 
     Alias for [`lmo.l_coratio(a, 4, 2, *, **)`][lmo.l_coratio].
 
     See Also:
         - [`lmo.l_coratio`][lmo.l_coratio]
         - [`lmo.l_kurtosis`][lmo.l_kurtosis]
-
     """
     return l_coratio(a, 4, 2, trim, rowvar=rowvar, dtype=dtype, **kwargs)
```

### Comparing `lmo-0.6.1/lmo/_pwm.py` & `lmo-0.7.0/lmo/_pwm.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 __all__ = 'b_weights', 'b_moment_cov'
 
 from typing import Any, TypeVar, cast
 
 import numpy as np
 import numpy.typing as npt
 
-from .stats import ordered
+from ._utils import ordered
 
 T = TypeVar('T', bound=np.floating[Any])
 
 
 def b_weights(
     r: int,
     n: int,
     /,
     dtype: np.dtype[T] | type[T] = np.float_,
 ) -> npt.NDArray[T]:
-    """
-    Probability Weighted moment (PWM) projection matrix $B$  of the
-    unbiased estimator for $\\beta_{k} = M_{1,k,0}$ for $k = 0, \\dots, r - 1$.
+    r"""
+    Probability Weighted moment (PWM) projection matrix $B$ of the
+    unbiased estimator for $\beta_k = M_{1,k,0}$ for $k = 0, \dots, r - 1$.
 
     The PWM's are estimated by linear projection of the sample of order
     statistics, i.e. $b = B x_{i:n}$
 
     Parameters:
-        r: The amount of orders to evaluate, i.e. $k = 0, \\dots, r - 1$.
+        r: The amount of orders to evaluate, i.e. $k = 0, \dots, r - 1$.
         n: Sample count.
         dtype: Desired output floating data type.
 
     Returns:
         P_b: Upper-triangular projection matrix of shape `(r, n)`.
 
     Examples:
@@ -41,19 +41,18 @@
         array([[0.2       , 0.2       , 0.2       , 0.2       , 0.2       ],
                [0.        , 0.05      , 0.1       , 0.15      , 0.2       ],
                [0.        , 0.        , 0.03333333, 0.1       , 0.2       ],
                [0.        , 0.        , 0.        , 0.05      , 0.2       ]])
 
     """
     if not (0 <= r <= n):
-        raise ValueError(f'expected 0 <= r <= n, got {r=} and {n=}')
+        msg = f'expected 0 <= r <= n, got {r=} and {n=}'
+        raise ValueError(msg)
 
-    # pyright throws a tantrum with numpy.arange for some reason...
-    # i1 = np.arange(1, n + 1)
-    i1 = np.linspace(1, n, n)
+    i1 = np.arange(1, n + 1)
 
     w_r = np.zeros((r, n), dtype)
     if w_r.size == 0:
         return w_r
 
     w_r[0] = 1.
 
@@ -62,100 +61,107 @@
 
     # the + 0. eliminates negative zeros
     return cast(npt.NDArray[T], w_r / n + 0.)
 
 
 def b_moment_cov(
     a: npt.ArrayLike,
-    ks: int,
+    r: int,
     /,
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     **kwargs: Any,
 ) -> npt.NDArray[T]:
-    """
-    Distribution-free variance-covariance matrix of the $\\beta$ PWM point
-    estimates with orders `k = 0, ..., ks`.
+    r"""
+    Distribution-free variance-covariance matrix of the probability weighted
+    moment (PWM) point estimates $\beta_k = M_{1,k,0}$, with orders
+    $k = 0, \dots, r - 1$.
+
+    Parameters:
+        a: Array-like with observations.
+        r: The amount of orders to evaluate, i.e. $k = 0, \dots, r - 1$.
+        axis: The axis along which to calculate the covariance matrices.
+        dtype: Desired output floating data type.
+        **kwargs: Additional keywords to pass to `lmo.stats.ordered`.
 
     Returns:
-        S_b: Variance-covariance matrix/tensor of shape `(ks, ks, ...)`
+        S_b: Variance-covariance matrix/tensor of shape `(r, ...)`
 
     See Also:
         - https://wikipedia.org/wiki/Covariance_matrix
 
     References:
         - [E. Elmamir & A. Seheult (2004) - Exact variance structure of sample
             L-moments](https://doi.org/10.1016/S0378-3758(03)00213-1)
-
     """
     x = ordered(a, axis=axis, dtype=dtype, **kwargs)
 
     # ensure the samples are "in front" (along axis=0)
     if axis and x.ndim > 1:
         x = np.moveaxis(x, axis, 0)
 
     n = len(x)
-    P_k = b_weights(ks, n, dtype=dtype)
+    p_k = b_weights(r, n, dtype=dtype)
 
     # beta pwm estimates
-    b = P_k @ x if x.ndim == 1 else np.inner(P_k, x.T)
-    assert b.shape == (ks, *x.shape[1:])
+    b = p_k @ x if x.ndim == 1 else np.inner(p_k, x.T)
+    assert b.shape == (r, *x.shape[1:])
 
     # the covariance matrix
-    S_b = np.empty((ks, *b.shape), dtype=dtype)
+    s_b = np.empty((r, *b.shape), dtype=dtype)
 
     # dynamic programming approach for falling factorial ratios:
     # w_ki[k, i] = i^(k) / (n-1)^(k))
-    ffact = np.ones((ks, n), dtype=dtype)
-    for k in range(1, ks):
+    ffact = np.ones((r, n), dtype=dtype)
+    for k in range(1, r):
         ffact[k] = ffact[k - 1] * np.linspace((1 - k) / (n - k), 1, n)
 
     # ensure that at most ffact[..., -k_max] will give 0
-    ffact = np.c_[ffact, np.zeros((ks, ks))]
+    ffact = np.c_[ffact, np.zeros((r, r))]
 
     spec = 'i..., i...'
 
     # for k == l (variances on the diagonal):
     # sum(
     #     2 * i^(k) * (j-k-1)^(k) * x[i] * x[j]
     #     for j in range(i + 1, n)
     # ) / n^(k+l+2)
-    for k in range(ks):
+    for k in range(r):
         j_k = np.arange(-k, n - k - 1)  # pyright: ignore
         v_ki = np.empty(x.shape, dtype=dtype)
         for i in range(n):
             # sum(
             #     2 * i^(k) * (j-k-1)^(k) * x[i] * x[j]
             #     for j in range(i + 1, n)
             # )
             v_ki[i] = ffact[k, j_k[i:]] * 2 * ffact[k, i] @ x[i + 1:]
 
         # (n-k-1)^(k+1)
         denom = n * (n - 2 * k - 1) * ffact[k, n - k - 1]
         m_bb = np.einsum(spec, v_ki, x) / denom  # pyright: ignore
-        S_b[k, k] = b[k]**2 - m_bb
+        s_b[k, k] = b[k]**2 - m_bb
 
     # for k != l (actually k > l since symmetric)
     # sum(
     #     ( i^(k) * (j-k-1)^(l) + i^(l) * (j-l-1)^(k) )
     #     * x[i] * x[j]
     #     for j in range(i + 1, n)
     # ) / n^(k+l+2)
-    for k, m in zip(*np.tril_indices(ks, -1)):
+    for k, m in zip(*np.tril_indices(r, -1), strict=True):
         j_k: npt.NDArray[np.int_] = np.arange(-k, n - k - 1)  # pyright: ignore
         j_l: npt.NDArray[np.int_] = np.arange(-m, n - m - 1)  # pyright: ignore
 
         v_ki = np.empty(x.shape, dtype=dtype)
         for i in range(n):
             v_ki[i] = (
                 ffact[k, i] * ffact[m, j_k[i:]] +
                 ffact[m, i] * ffact[k, j_l[i:]]
             ) @ x[i + 1:]
 
-        # (n-k-1)^(l+1)
+        # `(n-k-1)^(l+1)`
         denom = n * (n - k - m - 1) * ffact[m, n - k - 1]
         m_bb = np.einsum(spec, v_ki, x) / denom  # pyright: ignore
 
         # because s_bb.T == s_bb
-        S_b[k, m] = S_b[m, k] = b[k] * b[m] - m_bb
+        s_b[k, m] = s_b[m, k] = b[k] * b[m] - m_bb
 
-    return S_b
+    return s_b
```

### Comparing `lmo-0.6.1/lmo/diagnostic.py` & `lmo-0.7.0/lmo/diagnostic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-__all__ = 'normaltest',
+"""Statistical test and tools."""
+
+__all__ = ('normaltest',)
 
 from typing import NamedTuple, cast
 
 import numpy as np
 import numpy.typing as npt
 
 from ._lm import l_ratio
@@ -14,24 +16,24 @@
 
 
 def normaltest(
     a: npt.ArrayLike,
     /,
     axis: int | None = None,
 ) -> NormaltestResult:
-    """
+    r"""
     Test the null hypothesis that a sample comes from a normal distribution.
     Based on the Harri & Coble (2011) test, and includes Hosking's correction.
 
     Args:
         a: The array-like data.
         axis: Axis along which to compute the test.
 
     Returns:
-        statistic: The $\\tau^2_{3, 4}$ test statistic.
+        statistic: The $\tau^2_{3, 4}$ test statistic.
         pvalue: A 2-sided chi squared probability for the hypothesis test.
 
     Examples:
         Compare the testing power with
         [`scipy.stats.normaltest`][scipy.stats.normaltest] given 10.000 samples
         from a contaminated normal distribution.
 
@@ -45,15 +47,14 @@
         0.04806618...
         >>> normaltest_scipy(x)[1]
         0.08435627...
 
     References:
         [A. Harri & K.H. Coble (2011) - Normality testing: Two new tests
         using L-moments](https://doi.org/10.1080/02664763.2010.498508)
-
     """
     x = np.asanyarray(a)
 
     # sample size
     n = x.size if axis is None else x.shape[axis]
 
     # L-skew and L-kurtosis
@@ -61,20 +62,20 @@
 
     # theoretical L-skew and L-kurtosis of the normal distribution (for all
     # loc/mu and scale/sigma)
     tau3, tau4 = 0.0, 30/np.pi * np.arctan(np.sqrt(2)) - 9
 
     z3 = (t3 - tau3) / np.sqrt(
         0.1866 / n
-        + (np.sqrt(0.8000) / n)**2
+        + (np.sqrt(0.8000) / n)**2,
     )
     z4 = (t4 - tau4) / np.sqrt(
         0.0883 / n
         + (np.sqrt(0.6800) / n)**2
-        + (np.cbrt(4.9000) / n)**3
+        + (np.cbrt(4.9000) / n)**3,
     )
 
     k2 = z3**2 + z4**2
 
     # chi2(k=2) survival function (sf)
     p_value = np.exp(-k2 / 2)
```

### Comparing `lmo-0.6.1/lmo/stats.py` & `lmo-0.7.0/lmo/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,70 @@
-__all__ = 'ordered', 'ostat_from_ppf', 'l_moment_from_ppf'
+__all__ = 'clean_order', 'ensure_axis_at', 'as_float_array', 'ordered'
 
-import functools
-import math
-from typing import Any, Callable, TypeVar
+from typing import Any, SupportsIndex, TypeVar
 
 import numpy as np
 import numpy.typing as npt
-from scipy import special as scipy_special
-from scipy import integrate as scipy_integrate
 
-from ._utils import as_float_array
-from .typing import AnyInt, IntVector, SortKind
+from .typing import IndexOrder, IntVector, SortKind
 
-T = TypeVar('T', bound=np.floating[Any])
+T = TypeVar('T', bound=np.generic)
+
+
+def clean_order(
+    order: SupportsIndex,
+    /,
+    name: str = 'r',
+    strict: bool = False,
+) -> int:
+    if (r := order.__index__()) < (r0 := int(strict)):
+        msg = f'expected {name} >= {r0}, got {r}'
+        raise TypeError(msg)
+
+    return r
+
+
+def ensure_axis_at(
+    a: npt.NDArray[T],
+    /,
+    source: int | None,
+    destination: int,
+    order: IndexOrder = 'C',
+) -> npt.NDArray[T]:
+    if a.ndim <= 1 or source == destination:
+        return a
+    if source is None:
+        return a.ravel(order)
+
+    source = source + a.ndim if source < 0 else source
+    destination = destination + a.ndim if destination < 0 else destination
+
+    return a if source == destination else np.moveaxis(a, source, destination)
+
+
+def as_float_array(
+    a: npt.ArrayLike,
+    /,
+    dtype: npt.DTypeLike = None,
+    order: IndexOrder | None = None,
+    *,
+    check_finite: bool = False,
+    flat: bool = False,
+) -> npt.NDArray[np.floating[Any]]:
+    """
+    Convert to array if needed, and only cast to float64 dtype if not a
+    floating type already. Similar as in e.g. `numpy.mean`.
+    """
+    asarray = np.asarray_chkfinite if check_finite else np.asarray
+
+    x = asarray(a, dtype=dtype, order=order)
+    out = x if isinstance(x.dtype.type, np.floating) else x.astype(np.float_)
+
+    # the `_[()]` ensures that 0-d arrays become scalars
+    return (out.ravel() if flat and out.ndim != 1 else out)[()]
 
 
 def _apply_aweights(
     x: npt.NDArray[np.floating[Any]],
     v: npt.NDArray[np.floating[Any]],
     axis: int,
 ) -> npt.NDArray[np.float_]:
@@ -34,15 +82,16 @@
 
     x_jk: npt.NDArray[np.floating[Any]]
     w_jk: npt.NDArray[np.floating[Any]]
     v_jk: npt.NDArray[np.float_]
     for j in np.ndindex(out.shape[:-1]):
         x_jk, w_jk = x[j], vv[j]
         if w_jk[-1] <= 0:
-            raise ValueError('weight sum must be positive')
+            msg = 'weight sum must be positive'
+            raise ValueError(msg)
 
         # linearly interpolate to effectively "stretch" samples with large
         # weight, and "compress" those with small weights
         v_jk = np.linspace(w_jk[0], w_jk[-1], len(w_jk), dtype=np.float_)
         out[j] = np.interp(v_jk, w_jk, x_jk)  # pyright: ignore
 
     # unswap the axes if previously swapped
@@ -65,129 +114,46 @@
     If `y` is provided, the order of `y` is used instead.
     """
     if fweights is not None:
         # avoid uneccesary repeats by normalizing by the GCD
         r = np.asarray(fweights)
         # noinspection PyUnresolvedReferences
         if (gcd := np.gcd.reduce(r)) <= 0:
-            raise ValueError(
-                'fweights must be non-negative and have a positive sum'
-            )
+            msg = 'fweights must be non-negative and have a positive sum'
+            raise ValueError(msg)
+
         r = r // gcd if gcd > 1 else r
     else:
         r = None
 
     def _clean_array(a: npt.ArrayLike) -> npt.NDArray[np.floating[Any]]:
         out = as_float_array(a, dtype=dtype, flat=axis is None)
         return out if r is None else np.repeat(out, r, axis=axis)
 
     _x = _clean_array(x)
 
     if aweights is None and y is None:
         return np.sort(_x, axis=axis, kind=sort)
-    elif y is not None:
+    if y is not None:
         _y = _clean_array(y)
         i_k = np.argsort(_y, axis=axis if _y.ndim > 1 else -1, kind=sort)
     else:
         i_k = np.argsort(_x, axis=axis, kind=sort)
 
     def _sort_like(a: npt.NDArray[T]) -> npt.NDArray[T]:
         return (
             np.take(  # pyright: ignore [reportUnknownMemberType]
                 a,
                 i_k,
-                axis=None if a.ndim == i_k.ndim else axis
+                axis=None if a.ndim == i_k.ndim else axis,
             )
             if min(a.ndim, i_k.ndim) <= 1
             else np.take_along_axis(a, i_k, axis)
         )
 
     x_k = _sort_like(_x)
 
     if aweights is None:
         return x_k
 
     w_k = _sort_like(_clean_array(aweights))
     return _apply_aweights(x_k, w_k, axis=axis or 0)
-
-
-
-R = TypeVar('R', bound=float | npt.NDArray[np.float_])
-
-
-def ostat_from_ppf(
-    ppf: Callable[[float], R],
-    /,
-    *,
-    p_min: float = 0.0,
-    p_max: float = 1.0,
-    cache: bool = True,
-
-    **quad_options: Any,
-) -> Callable[[int, int], R]:
-    # TODO: docstring, example, tests
-
-    ppf_cached = functools.cache(ppf) if cache else ppf
-
-    def u_ppf(
-        p: float,
-        i: int,
-        n: int,
-        /,
-    ) -> R:
-        return (
-            ppf_cached(p)
-            * p**(i - 1)
-            * (1 - p)**(n - i)
-            * math.comb(n - 1, i - 1)
-            * n
-        )
-
-    def u_mean(i: int, n: int, /) -> R:
-        if not (0 < i <= n):
-            raise ValueError(f'expected 0 < i <= n, got {i = } and {n = }')
-
-        val = scipy_integrate.quad(
-            u_ppf,
-            p_min,
-            p_max,
-            args=(i, n),
-            **quad_options
-        )[0]
-        return np.round(val, 15)
-
-    return u_mean
-
-
-def l_moment_from_ppf(
-    ppf: Callable[[float], R],
-    r: AnyInt | IntVector,
-    /,
-    trim: tuple[int, int] = (0, 0),
-    **options: Any,
-) -> float | npt.NDArray[np.float_]:
-    # TODO: docstring, example, tests
-    t1, t2 = trim
-    u = ostat_from_ppf(ppf, **options)
-
-    def l_moment(_r: int) -> float | npt.NDArray[np.float_]:
-        if _r < 0:
-            raise ValueError(f'r must be >=0, got {_r}')
-        if _r == 0:
-            return 1.0
-
-        return np.array([
-            (-1) ** _k
-            * scipy_special.comb(_r - 1, _k, exact=True, legacy=False)
-            * u(t1 + _r - _k, t1 + t2 + _r)
-            for _k in range(_r)
-        ]).mean()
-
-    rs = np.asarray(r)
-    if rs.ndim == 0:
-        return l_moment(rs[()])
-
-    l_r = np.empty(rs.shape)
-    for ix in np.ndindex(*rs.shape):
-        l_r[ix] = l_moment(rs[ix])
-
-    return np.round(l_r, 12)
```

### Comparing `lmo-0.6.1/lmo/typing.py` & `lmo-0.7.0/lmo/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Numpy-related type aliasses for internal use."""
+
 __all__ = (
     'AnyNDArray',
 
     'AnyBool',
     'AnyInt',
     'AnyFloat',
 
@@ -13,28 +15,27 @@
     'FloatMatrix',
     'FloatTensor',
 
     'SortKind',
     'IndexOrder',
 )
 
+from collections.abc import Sequence
 from typing import (
     Any,
     Literal,
     Protocol,
-    Sequence,
     TypeAlias,
     TypeVar,
     runtime_checkable,
 )
 
 import numpy as np
 import numpy.typing as npt
 
-
 T = TypeVar('T', bound=np.generic)
 T_co = TypeVar('T_co', covariant=True, bound=np.generic)
 
 @runtime_checkable
 class _SupportsArray(Protocol[T_co]):
     def __array__(self) -> npt.NDArray[T_co]: ...
 
@@ -55,12 +56,10 @@
 IntMatrix: TypeAlias = AnyNDArray[_NumpyInteger] | Sequence[IntVector]
 IntTensor: TypeAlias = AnyNDArray[_NumpyInteger] | Sequence['IntTensor']
 
 FloatVector: TypeAlias = AnyNDArray[_NumpyFloating] | Sequence[AnyFloat]
 FloatMatrix: TypeAlias = AnyNDArray[_NumpyFloating] | Sequence[FloatVector]
 FloatTensor: TypeAlias = AnyNDArray[_NumpyFloating] | Sequence['FloatTensor']
 
-
-
 # for numpy.sort
 SortKind: TypeAlias = Literal['quicksort', 'heapsort', 'stable']
 IndexOrder: TypeAlias = Literal['C', 'F', 'A', 'K']
```

