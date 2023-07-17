# Comparing `tmp/pycmtensor-1.3.2.tar.gz` & `tmp/pycmtensor-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycmtensor-1.3.2.tar", max compression
+gzip compressed data, was "pycmtensor-1.4.0.tar", max compression
```

## Comparing `pycmtensor-1.3.2.tar` & `pycmtensor-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1070 2023-06-23 09:45:45.165672 pycmtensor-1.3.2/LICENSE
--rw-r--r--   0        0        0    10842 2023-06-23 09:45:45.165672 pycmtensor-1.3.2/README.md
--rw-r--r--   0        0        0      362 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/__init__.py
--rw-r--r--   0        0        0     6050 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/config.py
--rw-r--r--   0        0        0    11593 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/data.py
--rw-r--r--   0        0        0    13948 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/expressions.py
--rw-r--r--   0        0        0    11511 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/functions.py
--rw-r--r--   0        0        0     1366 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/logger.py
--rw-r--r--   0        0        0     3208 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/models/MNL.py
--rw-r--r--   0        0        0      189 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/models/ResLogit.py
--rw-r--r--   0        0        0       21 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/models/__init__.py
--rw-r--r--   0        0        0     6890 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/models/layers.py
--rw-r--r--   0        0        0    18014 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/optimizers.py
--rw-r--r--   0        0        0    11944 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/pycmtensor.py
--rw-r--r--   0        0        0     4959 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/results.py
--rw-r--r--   0        0        0     7126 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/scheduler.py
--rw-r--r--   0        0        0     3798 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/statistics.py
--rw-r--r--   0        0        0      420 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/utils.py
--rw-r--r--   0        0        0     2943 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pyproject.toml
--rw-r--r--   0        0        0    12987 1970-01-01 00:00:00.000000 pycmtensor-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-17 07:06:42.126320 pycmtensor-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2255 2023-07-17 07:06:42.126320 pycmtensor-1.4.0/README.md
+-rw-r--r--   0        0        0     2623 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/__init__.py
+-rw-r--r--   0        0        0     2424 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/config.py
+-rw-r--r--   0        0        0     6313 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/dataset.py
+-rw-r--r--   0        0        0    15712 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/expressions.py
+-rw-r--r--   0        0        0    11310 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/functions.py
+-rw-r--r--   0        0        0     1366 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/logger.py
+-rw-r--r--   0        0        0     5000 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/models/MNL.py
+-rw-r--r--   0        0        0      189 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/models/ResLogit.py
+-rw-r--r--   0        0        0       80 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/models/__init__.py
+-rw-r--r--   0        0        0    10110 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/models/basic.py
+-rw-r--r--   0        0        0     6890 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/models/layers.py
+-rw-r--r--   0        0        0    20737 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/optimizers.py
+-rw-r--r--   0        0        0    16177 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/pycmtensor.py
+-rw-r--r--   0        0        0     5168 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/results.py
+-rw-r--r--   0        0        0     7126 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/scheduler.py
+-rw-r--r--   0        0        0     3800 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/statistics.py
+-rw-r--r--   0        0        0      268 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pycmtensor/utils.py
+-rw-r--r--   0        0        0     2166 2023-07-17 07:06:42.202322 pycmtensor-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 pycmtensor-1.4.0/PKG-INFO
```

### Comparing `pycmtensor-1.3.2/LICENSE` & `pycmtensor-1.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022, Melvin Wong
+Copyright (c) 2023, Melvin Wong
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pycmtensor-1.3.2/pycmtensor/expressions.py` & `pycmtensor-1.4.0/pycmtensor/expressions.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 __all__ = ["FLOATX", "Param", "Beta", "Sigma", "Bias", "Weight"]
 FLOATX = aesara.config.floatX
 
 
 class ExpressionParser:
     """Base class for the ExpressionParser object"""
 
-    def __init__(self):
-        pass
+    def __init__(self, expression=None):
+        if expression is not None:
+            self.expression = str(pprint(expression))
 
     def parse(self, expression):
         """Returns a list of str words found in expression
 
         Args:
             expression (TensorVariable): the symbolic Tensor object to parse
         """
@@ -36,27 +37,42 @@
             ",",
             "[",
             "]",
             "{",
             "}",
             "=",
             "-1",
-            "Shape",
             "AdvancedSubtensor",
             "Reshape",
+            "Abs",
             "join",
             "sum",
             "dtype",
             "ARange",
             ":",
             "int64",
             "axis",
             "Softmax",
             "None",
             "log",
+            "Assert",
+            "i0",
+            "i1",
+            "i2",
+            "i3",
+            "AND",
+            "OR",
+            "EQ",
+            "not",
+            "Shape",
+            "Switch",
+            "BroadcastTo",
+            "Composite",
+            "Could",
+            "ScalarFromTensor",
         ]:
             stdout = str.replace(stdout, s, " ")
         symbols = [s for s in str.split(stdout, " ") if len(s) > 1]
         symbols = list(set(symbols))
         return symbols
 
 
@@ -65,91 +81,91 @@
 
     def __init__(self):
         pass
 
     def __add__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return self() + other
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return self() + other()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __radd__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return other + self()
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return other() + self()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __sub__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return self() - other
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return self() - other()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __rsub__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return other - self()
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return other() - self()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __mul__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             if self().ndim > 1:
                 return aet.dot(other, self().T)
             else:
                 return self() * other
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return self() * other()
         else:
             raise NotImplementedError(
-                f"{other} must be a TensorVariable or TensorShared Variable object"
+                f"__mul__ {other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __rmul__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             if self().ndim > 1:
                 return aet.dot(other, self().T)
             else:
                 return self() * other
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return self() * other()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __div__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return self() / other
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return self() / other()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __rdiv__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return other / self()
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return other() / self()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __neg__(self):
@@ -161,91 +177,98 @@
             raise NotImplementedError(
                 f"{self} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __pow__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.pow(self(), other)
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return aet.pow(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __rpow__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.pow(other, self())
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return aet.pow(other(), self())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __lt__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.lt(self(), other)
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return aet.lt(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __le__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.le(self(), other)
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return aet.le(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __gt__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.gt(self(), other)
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return aet.gt(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __ge__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.ge(self(), other)
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return aet.ge(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __eq__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.eq(self(), other)
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return aet.eq(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __ne__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.neq(self(), other)
-        elif isinstance(other, Beta):
+        elif isinstance(other, (Beta, RandomDraws)):
             return aet.neq(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
+    # def is_dataarray(self, other):
+    #     if isinstance(other, xr.DataArray):
+    #         if hasattr(other, "x"):
+    #             return other.x
+    #         return other.y
+    #     return other
+
 
 class Param(Expressions):
     def __init__(self, name: str, value=None):
         """Constructor for model param object"""
         self._name = name
         if value is not None:
             if not isinstance(value, np.ndarray):
@@ -275,15 +298,15 @@
 
     def get_value(self):
         """Returns the numpy representation of the parameter value"""
         return self.shared_var.get_value()
 
     def reset_value(self):
         """Resets the value of the shared variable to the initial value"""
-        self.shared_var = aesara.shared(self.init_value, name=self.name, borrow=False)
+        self.shared_var.set_value(self.init_value)
 
 
 class Beta(Param):
     def __init__(self, name, value=0.0, lb=None, ub=None, status=0):
         """Class object for Beta parameters
 
         Args:
@@ -302,28 +325,59 @@
         self.shared_var = aesara.shared(self.init_value, name=name, borrow=True)
 
     @property
     def status(self):
         return self._status
 
     def __repr__(self):
-        return f"Beta({self.name}, {self.shape})"
+        return f"Beta({self.name}, {self.get_value()})"
 
 
 class Sigma(Beta):
     def __init__(self, name, value=1.0, ub=None, status=0, dist="NORMAL"):
         super().__init__(name, value, 0, ub, status)
         self._dist = dist
         self.srng = RandomStream(seed=42069)
 
     @property
     def dist(self):
         return self._dist
 
 
+class RandomDraws(Expressions):
+    """Constructor for model random draws"""
+
+    def __init__(self, name: str, draw_type: str, n_draws: int):
+        self._name = name
+        self.n_draws = n_draws
+        srng = RandomStream(seed=234)
+        draw_type = draw_type.lower()
+        if draw_type == "normal":
+            rv_n = srng.normal(0, 1, size=(n_draws, 1))
+        elif draw_type == "lognormal":
+            rv_n = srng.lognormal(0, 1, size=(n_draws, 1))
+        else:
+            rv_n = getattr(srng, draw_type.lower())(size=(n_draws, 1))
+        self.shared_var = rv_n
+
+    @property
+    def name(self):
+        return self._name
+
+    def __call__(self):
+        return self.shared_var
+
+    def __repr__(self):
+        return f"RandomDraws({self.name}, size=({self.n_draws}, 1))"
+
+    def get_value(self):
+        """Returns the numpy representation of the parameter value"""
+        return self.shared_var.get_value()
+
+
 class Bias(Param):
     def __init__(self, name: str, size: tuple, init_value=None):
         Param.__init__(self, name)
         if not ((len(size) == 1) and isinstance(size, (list, tuple))):
             raise ValueError(f"Invalid size argument or type")
         if init_value is None:
             init_value = np.zeros(size, dtype=FLOATX)
```

### Comparing `pycmtensor-1.3.2/pycmtensor/functions.py` & `pycmtensor-1.4.0/pycmtensor/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 # functions.py
 """PyCMTensor functions module"""
 from ctypes import util
 from typing import Union
 
+import aesara
 import aesara.tensor as aet
 import aesara.tensor.nlinalg as nlinalg
 import numpy as np
 from aesara.tensor.sharedvar import TensorSharedVariable
 from aesara.tensor.var import TensorVariable
 
-from pycmtensor.expressions import Beta, Param
-
-from .logger import error, log
+from pycmtensor.expressions import Beta, Expressions, Param
+from pycmtensor.logger import error, log
 
 __all__ = [
     "exp_mov_average",
     "logit",
     "loglikelihood",
     "rmse",
     "mae",
     "kl_divergence",
     "kl_multivar_norm",
     "errors",
-    "hessians",
-    "bhhh",
-    "gnorm",
+    "second_order_derivative",
+    "first_order_derivative",
 ]
 
 
 def exp_mov_average(
     batch_avg: TensorVariable, moving_avg: TensorVariable, alpha: float = 0.1
 ):
     """Calculates the exponential moving average (EMA) of a new minibatch
 
     Args:
-        batch_avg (TensorVariable): the new batch value of the mean
-        moving_avg (TensorVariable): the moving value of the accumulated mean
-        alpha (float): the moving average factor of the batch mean
+        batch_avg: the new batch value of the mean
+        moving_avg: the moving value of the accumulated mean
+        alpha: the moving average factor of the batch mean
 
     Returns:
-        TensorVariable: the new moving average
+        (TensorVariable): the new moving average
 
     Note:
         The moving average will decay by the difference between the existing value
-        and the new value multiplied by the moving average factor. A higher ``alpha``
+        and the new value multiplied by the moving average factor. A higher `alpha`
         value results in faster changing moving average.
 
         Formula:
 
-        .. math::
-
-            x_{EMA} = \\alpha * x_t + x_{EMA} * (1-\\alpha)
+        $$x_{EMA} = \\alpha * x_t + x_{EMA} * (1-\\alpha)$$
     """
 
     while moving_avg.ndim < batch_avg.ndim:
         moving_avg = aet.expand_dims(moving_avg, -1)
 
     ema = batch_avg * alpha + moving_avg * (1 - alpha)
     return ema
@@ -63,89 +60,112 @@
 def logit(
     utility: Union[list, tuple, TensorVariable],
     avail: Union[list, tuple, TensorVariable] = None,
 ):
     """Computes the Logit function, with availability conditions.
 
     Args:
-        utility (list, tuple, TensorVariable): list of :math:`M` utility equations
-        avail (list, tuple, TensorVariable): list of :math:`M` availability conditions,
-            if no availability conditions are provided, defaults to 1 for all
+        utility: list of M utility equations
+        avail: list of M availability conditions,
+            if no availability conditions are provided, defaults to `1` for all
             availabilities.
 
     Returns:
-        TensorVariable: A NxM matrix of probabilities.
+        (TensorVariable): A NxM matrix of probabilities.
 
     Note:
-        The 0-th dimension is the numbering of alternatives.
+        The 0-th dimension is the numbering of alternatives, the N-th dimension is the size of the input (# rows).
     """
 
     if isinstance(utility, (list, tuple)):
         if (avail != None) and (len(utility) != len(avail)):
             msg = f"{utility} must have the same length as {avail}"
             raise ValueError(msg)
         _utility = utility
         for n, u in enumerate(_utility):
-            if not isinstance(u, (TensorVariable, TensorSharedVariable)):
-                utility[n] = u()
-            if utility[n].ndim == 0:
-                utility[n] = aet.expand_dims(utility[n], -1)
+            # convert u to vector representation if u is a scalar
+            if not isinstance(u, TensorVariable):
+                utility[n] = aet.as_tensor_variable(u())
+
+        # get maximum ndim from set of utlity equations
+        max_ndim = max([u.ndim for u in utility])
+        _utility = utility
+
+        # pad tensors to the left to have the same number of dimensions
+        utility = [aet.atleast_Nd(u, n=max_ndim) for u in _utility]
+
+        # broadcast tensors across each other before stacking
+        utility = aet.broadcast_arrays(*utility)
+
+        # stack list of tensors to into a max_ndim+1 tensor
         U = aet.stack(utility)
+
+    # use the utility inputs as is if given as a TensorVariable
     elif isinstance(utility, TensorVariable):
         U = utility
     else:
         raise NotImplementedError(
             f"utility {utility} has to be a list, tuple or TensorVariable instance"
         )
 
+    # calculate the probabilities
     prob = aet.special.softmax(U, axis=0)
+
+    # update probabilities by availability conditions
     if avail != None:
+        # stack availabilities and convert to tensor
         AV = aet.stack(avail)
+
         while AV.ndim < prob.ndim:
-            AV = aet.expand_dims(AV, 1)
+            # insert new axes after choice axis (choice axis = 0)
+            AV = aet.shape_padaxis(AV, axis=1)
+
         prob = prob * AV
+
+        # normalize probabilities to sum to 1
         prob = prob / aet.sum(prob, axis=0, keepdims=1)
+
     return prob
 
 
 def log_likelihood(prob: TensorVariable, y: TensorVariable):
     """Symbolic representation of the log likelihood cost function.
 
     Args:
-        prob (TensorVariable): matrix describing the choice probabilites
-        y (TensorVariable): ``TensorVariable`` referencing the choice column
+        prob: a `TensorVariable` matrix describing the choice probabilites
+        y: a `TensorVariable` referencing the choice variable
 
     Returns:
-        TensorVariable: a symbolic representation of the log likelihood with ndim=0.
+        (TensorVariable): a symbolic representation of the log likelihood with `ndim=0`.
 
     Note:
-        The 0-th dimension is the numbering of alternatives.
+        The 0-th dimension is the numbering of alternatives, the N-th dimension is the size of the input (# rows).
     """
-    return aet.sum(aet.log(prob)[y, ..., aet.arange(y.shape[0])])
+    # calculate the log probabilitiy of axis 0
+    logprob = aet.log(prob)[y, ..., aet.arange(y.shape[0])]
+
+    # take the average over all other non choice, non-n axes
+    while logprob.ndim > 1:
+        logprob = aet.mean(logprob, axis=1)
+
+    return aet.sum(logprob)
 
 
 def rmse(y_hat: TensorVariable, y: TensorVariable):
     """Computes the root mean squared error (RMSE) between pairs of observations
 
     Args:
-        y_hat (TensorVariable): model estimated values
-        y (TensorVariable): ground truth values
+        y_hat: model estimated values
+        y: ground truth values
 
     Returns:
-        TensorVariable: symbolic scalar representation of the rmse
+        (TensorVariable): symbolic scalar representation of the rmse
 
     Note:
-        Tensor is flattened to an N-vector if the input args are :math:`N\\times 1`
-        matrices.
-
-        Formula:
-
-        .. math::
-
-            RMSE = \\sqrt{\\frac{1}{N}\\sum_{i=1}^N(\\hat{y}_i-y_i)^2}
+        Tensor is flattened to a `dim=1` vector if the input tensor is `dim=2`.
 
     """
     if y_hat.ndim != y.ndim:
         msg = f"y_hat should have the same dimensions as y. y_hat.ndim: {y_hat.ndim}, q.ndim: {y.ndim}"
         raise ValueError(msg)
     if y_hat.ndim < 1:
         y_hat = aet.flatten(y_hat)
@@ -154,90 +174,86 @@
     return aet.sqrt(aet.mean(aet.sqr(y_hat - y)))
 
 
 def mae(y_hat: TensorVariable, y: TensorVariable):
     """Computes the mean absolute error (MAE) between pairs of observations
 
     Args:
-        y_hat (TensorVariable): model estimated values
-        y (TensorVariable): ground truth values
+        y_hat: model estimated values
+        y : ground truth values
 
     Returns:
-        TensorVariable: symbolic scalar representation of the mae
+        (TensorVariable): symbolic scalar representation of the mean absolute error
 
     Note:
-        Tensor is flattened to an N-vector if the input args are :math:`N\\times 1` matrices.
-
-        Formula:
-
-        .. math::
-
-            MAE = \\frac{\sum_{i=1}^N|\\hat{y}_i-y_i|}{N}
+        Tensor is flattened to a `dim=1` vector if the input tensor is `dim=2`.
     """
     if y_hat.ndim != y.ndim:
         msg = f"y_hat should have the same dimensions as y. y_hat.ndim: {y_hat.ndim}, q.ndim: {y.ndim}"
         raise ValueError(msg)
     if y_hat.ndim < 1:
         y_hat = aet.flatten(y_hat)
         y = aet.flatten(y)
 
     return aet.mean(aet.abs(y_hat - y))
 
 
 def kl_divergence(p: TensorVariable, q: TensorVariable):
-    """Computes the KL divergence loss between discrete distributions ``p`` and ``q``.
+    """Computes the KL divergence loss between discrete distributions `p` and `q`.
 
     Args:
-        p (TensorVariable): model output probabilities
-        q (TensorVariable): ground truth probabilities
+        p: model output probabilities
+        q: ground truth probabilities
 
     Returns:
-        TensorVariable: a symbolic representation of the KL loss with
+        (TensorVariable): a symbolic representation of the KL loss 
 
     Note:
         Formula:
 
-        .. math::
-
-            L = \\begin{cases}
-                \\sum_{i=1}^N (p_i * log(p_i/q_i)) & p>0\\\\
-                0 & p<=0
-            \\end{cases}
+        $$
+        L = \\begin{cases}
+            \\sum_{i=1}^N (p_i * log(p_i/q_i)) & p>0\\\\
+            0 & p<=0
+        \\end{cases}
+        $$
+        
     """
     if p.ndim != q.ndim:
         msg = f"p should have the same shape as q. p.ndim: {p.ndim}, q.ndim: {q.ndim}"
         raise ValueError(msg)
 
     return aet.sum(aet.switch(aet.neq(p, 0), p * aet.log(p / q), 0))
 
 
 def kl_multivar_norm(m0, v0, m1, v1, epsilon=1e-6):
     """Computes the KL divergence loss between two multivariate normal distributions.
 
     Args:
-        m0: mean vector of the first Normal m.v. distribution :math:`N_0`
-        v0: (co-)variance matrix of the first Normal m.v. distribution :math:`N_0`
-        m1: mean vector of the second Normal m.v. distribution :math:`N_1`
-        v1: (co-)variance of the second Normal m.v. distribution :math:`N_1`
+        m0 (TensorVariable): mean vector of the first Normal m.v. distribution $N_0$
+        v0 (TensorVariable): (co-)variance matrix of the first Normal m.v. distribution
+            $N_0$
+        m1 (TensorVariable): mean vector of the second Normal m.v. distribution $N_1$
+        v1 (TensorVariable): (co-)variance of the second Normal m.v. distribution $N_1$
         epsilon (float): small value to prevent divide-by-zero error
 
     Note:
         k = dimension of the distribution.
 
         Formula:
 
-        .. math::
-
+        $$
             D_{KL}(N_0||N_1) = 0.5 * \\Big(\\ln\\big(\\frac{|v_1|}{|v_0|}\\big) + trace(v_1^{-1} v_0) + (m_1-m_0)^T v_1^{-1} (m_1-m_0) - k\\Big)
+        $$
 
         In variational inference, the kl divergence is the relative entropy between a
-        diagonal multivariate Normal and a standard Normal distribution, N(0, 1),
-        therefore, for VI, ``m1=aet.constant(0)``, ``v1=aet.constant(1)``
+        diagonal multivariate Normal and a standard Normal distribution, $N(0, 1)$,
+        therefore, for VI, `m1=1`, `v1=1`
 
-        For two univariate distributions, dimensions of m0,m1,v0,v1 = 0
+        For two univariate distributions, dimensions of `m0,m1,v0,v1 = 0`
     """
     if not (
         (m0.ndim >= m1.ndim)
         and (v0.ndim >= v1.ndim)
         and (m0.ndim <= 1)
         and (v0.ndim <= 2)
     ):
@@ -269,95 +285,69 @@
     return kld
 
 
 def errors(prob: TensorVariable, y: TensorVariable):
     """Symbolic representation of the discrete prediction as a percentage error.
 
     Args:
-        prob (TensorVariable): matrix describing the choice probabilites
-        y (TensorVariable): the ``TensorVariable`` referencing the choice column
+        prob: matrix describing the choice probabilites
+        y: the `TensorVariable` referencing the choice column
 
     Returns:
-        TensorVariable: the mean prediction error over the input ``y``
+        (TensorVariable): the mean prediction error over `y`
     """
     pred = aet.argmax(prob, axis=0)
 
     if y.dtype.startswith("int"):
         return aet.mean(aet.neq(pred, y))
     else:
         raise NotImplementedError(f"y should be int32 or int64", ("y.dtype:", y.dtype))
 
 
-def hessians(ll: TensorVariable, params: list[Beta]):
-    """Symbolic representation of the Hessian matrix given the log likelihood.
+def second_order_derivative(cost: TensorVariable, params: list[Beta]):
+    """Symbolic representation of the 2nd order Hessian matrix given cost.
 
     Args:
-        ll (TensorVariable): the loglikelihood to compute the gradients over
-        params (list): list of params to compute the gradients over
+        cost: the cost function to compute the gradients over
+        params: list of params to compute the gradients over
 
     Returns:
-        TensorVariable: the Hessian matrix
+        (TensorVariable): the Hessian matrix of the cost function wrt to the params
 
     Note:
-        Parameters with status=1 are ignored.
+        Parameters with `status=1` are ignored.
     """
     if not isinstance(params, list):
         raise TypeError(f"params is not list instance. type(params)={type(params)}")
     params = [p() for p in params if (p.status != 1)]
-    grads = aet.grad(ll, params, disconnected_inputs="ignore")
+    grads = aet.grad(cost, params, disconnected_inputs="ignore")
     mat = aet.as_tensor_variable(np.zeros((len(grads), len(grads))))
     for i in range(len(grads)):
         mat = aet.set_subtensor(
             x=mat[i, :],
             y=aet.grad(grads[i], params, disconnected_inputs="ignore"),
         )
     return mat
 
 
-def bhhh(ll: TensorVariable, params: list[Beta]):
-    """Symbolic representation of the Berndt-Hall-Hall-Hausman (BHHH) algorithm given
-    the log likelihood.
-
-    Args:
-        ll (TensorVariable): the loglikelihood to compute the gradients over
-        params (list): list of params to compute the gradients over
-
-    Returns:
-        TensorVariable: the outer product of the gradient with ndim=2
-
-    Note:
-        Parameters with status=1 are ignored.
-    """
-    if not isinstance(params, (dict, list)):
-        raise TypeError(
-            f"params is not list or dict instance. type(params)={type(params)}"
-        )
-    if isinstance(params, dict):
-        params = list(params.values())
-    params = [p() for p in params if (p.status != 1)]
-    grads = aet.grad(ll, params, disconnected_inputs="ignore")
-    mat = aet.outer(aet.as_tensor_variable(grads), aet.as_tensor_variable(grads).T)
-    return mat
-
-
-def gnorm(cost: TensorVariable, params: list[Beta]):
-    """Symbolic representation of the gradient norm given the cost.
+def first_order_derivative(cost: TensorVariable, params: list[Beta]):
+    """Symbolic representation of the 1st order gradient vector given the cost.
 
     Args:
-        cost (TensorVariable): the cost to compute the gradients over
-        params (list): list of params to compute the gradients over
+        cost: the cost function to compute the gradients over
+        params: list of params to compute the gradients over
 
     Returns:
-        TensorVariable: the gradient norm value
+        (TensorVariable): the gradient vector of the cost function wrt to the params
 
     Note:
-        Parameters with status=1 are ignored.
+        Parameters with `status=1` are ignored.
     """
     if not isinstance(params, (dict, list)):
         raise TypeError(
             f"params is not list or dict instance. type(params)={type(params)}"
         )
     if isinstance(params, dict):
         params = list(params.values())
     params = [p() for p in params if (p.status != 1)]
     grads = aet.grad(cost, params, disconnected_inputs="ignore")
-    return nlinalg.norm(grads, ord=None)
+    return aet.as_tensor_variable(grads)
```

### Comparing `pycmtensor-1.3.2/pycmtensor/logger.py` & `pycmtensor-1.4.0/pycmtensor/logger.py`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.3.2/pycmtensor/models/layers.py` & `pycmtensor-1.4.0/pycmtensor/models/layers.py`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.3.2/pycmtensor/optimizers.py` & `pycmtensor-1.4.0/pycmtensor/optimizers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # optimizers.py
 """PyCMTensor optimizers module"""
 import aesara
 import aesara.tensor as aet
+import aesara.tensor.nlinalg as nlinalg
+import numpy as np
 from aesara import shared
+from aesara.ifelse import ifelse
 from aesara.tensor.sharedvar import TensorSharedVariable
+from numpy import nan_to_num as nan2num
 
-from .data import FLOATX
+from pycmtensor.expressions import Beta
+
+FLOATX = aesara.config.floatX
 
 __all__ = [
+    "BFGS",
     "Adam",
     "Nadam",
     "Adamax",
     "Adadelta",
     "RMSProp",
     "Momentum",
     "NAG",
-    "Adagrad",
+    "AdaGrad",
     "SGD",
 ]
 
 
 class Optimizer:
     def __init__(self, name, epsilon=1e-8, **kwargs):
         """Base optimizer class
@@ -495,7 +502,83 @@
 
         updates = []
         for param, grad in zip(params, grads):
             p_t = param - lr * grad
             updates.append((param, p_t))
 
         return updates
+
+
+class BFGS(Optimizer):
+    def __init__(self, params: list, config=None, **kwargs):
+        """An optimizer that implements the stochastic gradient algorithm
+
+        Args:
+            params (list): a list of ``TensorSharedVariable``
+        """
+        super().__init__(name="BFGS")
+        if config is not None:
+            if hasattr(config, "BFGS_warmup"):
+                self.warmup = config.BFGS_warmup
+            else:
+                raise KeyError
+
+        self._t = aesara.shared(1.0)
+        self._y = [
+            shared(aet.zeros_like(p()).eval())
+            for p in params
+            if ((p.status != 1) and (isinstance(p, Beta)))
+        ]
+        self._s = [
+            shared(p().eval())
+            for p in params
+            if ((p.status != 1) and (isinstance(p, Beta)))
+        ]
+        self._accu = [
+            shared(aet.zeros_like(p()).eval())
+            for p in params
+            if ((p.status != 1) and (isinstance(p, Beta)))
+        ]
+        self._H0 = aesara.shared(aet.eye(len(self._y), dtype=FLOATX).eval())
+
+        self.I = aesara.shared(aet.eye(len(self._y), dtype=FLOATX).eval())
+
+    def update(self, cost, params: list, lr: float = 0.001):
+        T = self.warmup
+        params = [p() for p in params if p.status != 1]
+        grads = aet.grad(cost, params, disconnected_inputs="ignore")
+
+        updates = []
+        for n, (param, grad, s, y) in enumerate(zip(params, grads, self._s, self._y)):
+            B = ifelse(
+                aet.lt(self._t, 2 * T),
+                then_branch=grad,
+                else_branch=aet.sum(self._H0[n, :] * grad),
+            )
+            # a_t = a + aet.sqr(grad)
+            # p_t = param - lr / aet.sqrt(a_t + self.epsilon) * B
+            # updates.append((a, a_t))
+            p_t = param - lr * B
+            updates.append((param, p_t))
+
+            s_new = param - s
+            updates.append((s, s_new))
+
+            y_new = grad - y
+            updates.append((y, y_new))
+
+        s_t = aet.atleast_2d(self._s, left=False)
+        y_t = aet.atleast_2d(self._y, left=False)
+        rho_t = 1 / (s_t.T @ y_t)
+        li = self.I - rho_t * (s_t @ y_t.T)
+        ri = self.I - rho_t * (y_t @ s_t.T)
+        h_res = rho_t * (s_t @ s_t.T)
+        H_new = ifelse(
+            aet.ge(self._t, T) * aet.eq(self._t % T, 0),
+            then_branch=li @ self._H0 @ ri + h_res,
+            else_branch=self._H0,
+        )
+        updates.append((self._H0, H_new))
+
+        updates.append((self._t, self._t + 1))
+
+        return updates
```

### Comparing `pycmtensor-1.3.2/pycmtensor/pycmtensor.py` & `pycmtensor-1.4.0/pycmtensor/models/basic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,334 +1,272 @@
-# pycmtensor.py
-"""PyCMTensor main module"""
 from collections import OrderedDict
 from time import perf_counter
 from typing import Union
 
-import aesara.tensor as aet
-import dill as pickle
 import numpy as np
-from aesara import function
-from aesara.tensor.var import TensorVariable
 
-from pycmtensor import config, rng
-
-from .expressions import Beta, ExpressionParser, Weight
-from .functions import bhhh, errors, gnorm, hessians
-from .logger import debug, info, warning
-from .optimizers import Adam, Optimizer
-from .results import Results
-from .utils import time_format
-
-
-class PyCMTensorModel:
-    def __init__(self, db, **kwargs):
-        """Base model class object"""
-        self.name = "PyCMTensorModel"
+from pycmtensor import config
+from pycmtensor.expressions import Beta, ExpressionParser, Param
+from pycmtensor.logger import debug, info, warning
+from pycmtensor.results import Results
+from pycmtensor.utils import time_format
+
+
+class BaseModel(object):
+    def __init__(self, **kwargs):
+        """Basic model class object
+
+        Attributes:
+            name (str): name of the model
+            config (Config): pycmtensor config object
+            rng (Generator): random number generator
+            params (list): list of model parameters (betas & weights)
+            betas (list): list of model scalar betas
+            weights (list): list of model weight matrices
+            updates (list): list of (param, update) tuples
+            inputs (list): list of TensorVariables
+            outputs (TensorVariable): symbolic reference to the output TensorVariable
+            learning_rate (TensorVariable): symbolic reference to the learning rate
+            results (Results): stores the results of the model estimation
+        """
+        self.name = "BaseModel"
         self.config = config
-        self.params = []  # keep track of all the params
+        self.rng = np.random.default_rng(config.seed)
+        self.params = []  # keep track of all the Params
         self.betas = []  # keep track of the Betas
         self.weights = []  # keep track of the Weights
         self.updates = []  # keep track of the updates
-        self.inputs = db.all
-        self.learning_rate = aet.scalar("learning_rate")
-        self.optimizer = Adam
         self.results = Results()
 
         for key, value in kwargs.items():
-            if key == "optimizer" or key == "opt":
-                if not isinstance(value, Optimizer):
-                    raise TypeError(f"invalid optimizer {value}")
-                self.optimizer = value
+            self.config.add(key, value)
 
         debug(f"Building model...")
 
-    def add_params(self, params: Union[dict, list]):
-        """Method to load locally defined variables
-
-        Args:
-            params (Union[dict, list]): a dict or list of ``TensorSharedVariable``
-        """
-        if not isinstance(params, (dict, list)):
-            raise TypeError(f"params must be of Type dict or list")
-
-        # create a dict of str(param): param, if params is given as a list
-        if isinstance(params, list):
-            params = {str(p): p for p in params}
-
-        # iterate through the dict of params:
-        if not hasattr(self, "cost"):
-            raise ValueError(f"No valid cost function defined.")
-
-        symbols = ExpressionParser().parse(getattr(self, "cost"))
-        seen = set()
-        for _, p in params.items():
-            if not isinstance(p, (Beta, Weight)):
-                continue
-
-            if p.name in seen:
-                continue
-                # raise NameError(f"Duplicate param names defined: {p.name}.")
-
-            if (p.name not in symbols) and (p.status == 0):
-                warning(f"Unused Beta {p.name} removed from computational graph")
-                continue
-
-            self.params.append(p)
-            seen.add(p.name)
-
-            if isinstance(p, (Beta)):
-                self.betas.append(p)
-            else:
-                self.weights.append(p)
-
-    def add_regularizers(self, l_reg: TensorVariable):
-        """Adds regularizer to model cost function
-
-        Args:
-            l_reg (TensorVariable): symbolic variable defining the regularizer term
-        """
-        if not hasattr(self, "cost"):
-            raise ValueError("No valid cost function defined.")
-
-        self.cost += l_reg
-
     @property
-    def n_params(self):
-        """Get the total number of parameters"""
-        return self.n_betas + sum(self.n_weights)
+    def n_params(self) -> int:
+        """Return the total number of estimated parameters"""
+        return self.n_betas + self.n_weights
 
     @property
-    def n_betas(self):
-        """Get the count of Beta parameters"""
+    def n_betas(self) -> int:
+        """Return the number of estimated Betas"""
         return len(self.betas)
 
     @property
-    def n_weights(self):
-        """Get the total number of elements of each weight matrix"""
-        return [w.size for w in self.get_weights()]
-
-    def get_betas(self) -> dict:
-        """Returns the Beta (key, value) pairs as a dict"""
-        return {beta.name: beta.get_value() for beta in self.betas}
+    def n_weights(self) -> int:
+        """Return the total number of estimated Weight parameters"""
+        return sum([w.size for w in self.get_weights()])
 
-    def get_weights(self) -> list[np.ndarray]:
-        """Returns the Weights as a list of matrices"""
+    def get_weights(self) -> list:
+        """Returns a list of Weight values"""
         return [w.get_value() for w in self.weights]
 
+    def get_betas(self) -> list:
+        """Returns a list of Beta values"""
+        return [beta.get_value() for beta in self.betas]
+
     def reset_values(self):
-        """Resets param values to their initial values"""
+        """Resets Model parameters to their initial value"""
         for p in self.params:
             p.reset_value()
 
-    def model_loglikelihood(self):
-        """Loads the function to ``self.loglikelihood()`` to output the loglikelihood
-        value of the model given inputs"""
-        self.loglikelihood = function(
-            name="loglikelihood",
-            inputs=self.inputs,
-            outputs=self.ll,
-        )
-
-    def model_choice_probabilities(self):
-        """Loads the function to ``self.choice_probabilities()`` to output discrete
-        choice probabilities. Axes of outputs are swapped"""
-        self.choice_probabilities = function(
-            name="choice probabilities",
-            inputs=self.inputs,
-            outputs=self.p_y_given_x.swapaxes(0, 1),
-        )
-
-    def model_choice_predictions(self):
-        """Loads the function to ``self.choice_predictions()`` to output discrete
-        choice predictions"""
-        self.choice_predictions = function(
-            name="choice predictions",
-            inputs=self.inputs,
-            outputs=self.pred,
-        )
-
-    def model_prediction_error(self):
-        """Loads the function to ``self.prediction_error()`` to output the model error
-        wrt inputs"""
-        self.prediction_error = function(
-            name="prediction error",
-            inputs=self.inputs,
-            outputs=errors(self.p_y_given_x, self.y),
-        )
 
-    def model_H(self):
-        """Loads the function to ``self.H()`` to calculate the Hessian matrix or the
-        2nd-order partial derivatives of the model.
-        """
-        self.H = function(
-            name="Hessian matrix",
-            inputs=self.inputs,
-            outputs=hessians(self.ll, self.betas),
-        )
-
-    def model_BHHH(self):
-        """Loads the function to ``self.BHHH()`` to calculate the Berndt-Hall-Hall-
-        Hausman (BHHH) approximation.
-        """
-        self.BHHH = function(
-            name="BHHH matrix",
-            inputs=self.inputs,
-            outputs=bhhh(self.ll, self.betas),
-        )
-
-    def model_gnorm(self):
-        """Loads the function to ``self.gradient_norm()`` to calculate the gradient
-        norm of the model cost function.
-        """
-        self.gradient_norm = function(
-            name="Gradient norm",
-            inputs=self.inputs,
-            outputs=gnorm(self.cost, self.betas),
-        )
+def extract_params(cost, variables: Union[dict, list]):
+    """Extracts Param objects from variables
 
-    def predict(self, db, return_choices: bool = True):
-        """Returns the predicted choice or choice probabilites
-
-        Args:
-            db (pycmtensor.Data): database for prediction
-            return_choices (bool): if `True` then returns discrete choices instead of
-                probabilities
-
-        Returns:
-            numpy.ndarray: the output vector
-        """
-        if not return_choices:
-            return self.choice_probabilities(*db.valid_data)
-        else:
-            return self.choice_predictions(*db.valid_data)
-
-    def train(self, db, **kwargs):
-        """Function to train the model
-
-        Args:
-            db (pycmtensor.Data): database used to train the model
-            **kwargs: keyword arguments for adjusting training configuration.
-                Possible values are `max_steps:int`, `patience:int`,
-                `lr_scheduler:scheduler.Scheduler`, `batch_size:int`. For more
-                information and other possible options, see
-                :py:data:`hyperparameters <pycmtensor.config.Config.hyperparameters>`
-        """
-        self.config.set_hyperparameter(**kwargs)
-
-        # [train-start]
-        lr_scheduler = self.config["lr_scheduler"]
-        batch_size = self.config["batch_size"]
-        max_steps = self.config["max_steps"]
-        patience = self.config["patience"]
-        patience_increase = self.config["patience_increase"]
-        validation_threshold = self.config["validation_threshold"]
-
-        db.n_train_batches = db.n_train_samples // batch_size
-        validation_frequency = db.n_train_batches
-        max_iterations = max_steps * db.n_train_batches
-
-        # initalize results array
-        self.results.performance_graph = OrderedDict()
-
-        # compute the inital results of the model
-        self.results.init_loglikelihood = self.loglikelihood(*db.train_data)
-        self.results.best_loglikelihood = self.results.init_loglikelihood
-        self.results.best_valid_error = self.prediction_error(*db.valid_data)
-
-        # loop parameters
-        done_looping = False
-        step = 0
-        iteration = 0
-        shift = 0
-
-        # set learning rate
-        learning_rate = lr_scheduler(step)
-
-        # main loop
-        start_time = perf_counter()
-        info(f"Start (n={db.n_train_samples})")
-
-        while (step < max_steps) and (not done_looping):
-            # loop over batch
-            learning_rate = lr_scheduler(step)
-            for index in range(db.n_train_batches):
-                if patience <= iteration:
-                    done_looping = True
-                    debug(f"Early stopping... (step={step})")
-                    break
-
-                # increment iteration
-                iteration += 1
-
-                # set index and shift slices
-                if self.config["batch_shuffle"]:
-                    index = rng.integers(0, db.n_train_batches)
-                    shift = rng.integers(0, batch_size)
-
-                # get data slice from dataset
-                batch_data = db.get_train_data(self.inputs, index, batch_size, shift)
-
-                # model update step
-                self.update_wrt_cost(*batch_data, learning_rate)
-
-                # model validate step
-                if iteration % validation_frequency != 0:
-                    continue
-
-                train_ll = self.loglikelihood(*db.train_data)
-                valid_error = self.prediction_error(*db.valid_data)
-                self.results.performance_graph[step] = (
-                    np.round(train_ll, 2),
-                    np.round(valid_error, 4),
+    Args:
+        cost (TensorVariable): the cost function to look for Param objects
+        variables: dictionary or list of local variables from the current program
+    """
+    params = []
+    symbols = ExpressionParser().parse(cost)
+    seen = set()
+
+    if isinstance(variables, dict):
+        variables = [v for _, v in variables.items()]
+
+    for variable in variables:
+        if (not isinstance(variable, Param)) or (variable.name in seen):
+            continue
+
+        if variable.name not in symbols:
+            # raise a warning if variable is not in any utility function
+            warning(f"{variable.name} not in any utility functions")
+            continue
+
+        params.append(variable)
+        seen.add(variable.name)
+
+    return params
+
+
+def drop_unused_variables(cost, params: Param, variables: dict) -> list:
+    symbols = ExpressionParser().parse(cost)
+    param_names = [p.name for p in params]
+    symbols = [s for s in symbols if s not in param_names]
+    return [var for var in list(variables) if var not in symbols]
+
+
+def train(model, ds, **kwargs):
+    for key, value in kwargs.items():
+        model.config.add(key, value)
+
+    batch_size = model.config.batch_size
+    if (batch_size == 0) or (batch_size == None):
+        model.config.batch_size = ds.n_train
+        batch_size = model.config.batch_size
+
+    n_train = ds.n_train
+    n_valid = ds.n_valid
+    n_train_batches = n_train // batch_size
+    model.config.BFGS_warmup = model.config.BFGS_warmup * n_train_batches
+
+    patience = max(model.config.patience, n_train_batches)
+    patience_inc = model.config.patience_increase
+    validation_threshold = model.config.validation_threshold
+    convergence_threshold = model.config.convergence_threshold
+    validation_freq = n_train_batches
+    max_steps = model.config.max_steps
+    max_iterations = max_steps * n_train_batches
+
+    done_looping = False
+    converged = False
+    step = 0
+    iteration = 0
+    shift = 0
+    gnorm_tol = np.inf
+
+    optimizer = model.config.optimizer(model.params, config=model.config)
+    updates = optimizer.update(model.cost, model.params, model.learning_rate)
+    model.build_cost_updates_fn(updates)
+
+    lr_scheduler = model.config.lr_scheduler(
+        lr=model.config.base_learning_rate,
+        factor=model.config.lr_stepLR_factor,
+        drop_every=model.config.lr_stepLR_drop_every,
+        power=model.config.lr_PolynomialLR_power,
+        cycle_steps=model.config.lr_CLR_cycle_steps,
+        gamma=model.config.lr_ExpRangeCLR_gamma,
+    )
+
+    performance_graph = OrderedDict()
+
+    x_and_y = model.x + [model.y]
+    train_data = ds.train_dataset(x_and_y)
+    valid_data = ds.valid_dataset(x_and_y)
+    log_likelihood = model.log_likelihood_fn(*train_data)
+    error = model.prediction_error_fn(*valid_data)
+
+    model.results.null_loglikelihood = log_likelihood
+    model.results.best_loglikelihood = log_likelihood
+    model.results.best_valid_error = error
+    model.results.params = model.params
+    model.results.n_train = n_train
+    model.results.n_valid = n_valid
+    model.results.n_params = model.n_params
+    model.results.seed = model.config.seed
+
+    start_time = perf_counter()
+    info(
+        f"Start (n={n_train}, Step={step}, LL={model.results.null_loglikelihood:.2f}, Error={model.results.best_valid_error*100:.2f}%)"
+    )
+
+    params_prev = [p.get_value() for p in model.params if isinstance(p, Beta)]
+
+    batch_data = []
+    for batch in range(n_train_batches):
+        batch_data.append(ds.train_dataset(x_and_y, batch, batch_size, shift))
+
+    while (step < max_steps) and (not done_looping):
+        learning_rate = lr_scheduler(step)  # get learning rate at this step
+
+        for i in range(n_train_batches):
+            model.cost_updates_fn(*batch_data[i], learning_rate)  # update model
+
+            if iteration % validation_freq == 0:
+                log_likelihood = model.log_likelihood_fn(*train_data)
+                performance_graph[step] = {"log likelihood": log_likelihood}
+
+                params = [p.get_value() for p in model.params if isinstance(p, Beta)]
+                diff = [p_prev - p for p_prev, p in zip(params_prev, params)]
+                gnorm = np.sqrt(np.sum(np.square(diff)))
+
+                params_prev = params
+
+                if gnorm < (gnorm_tol / 5.0):
+                    gnorm_tol = gnorm
+                    info(
+                        f"Train (Step={step}, LL={log_likelihood:.2f}, Error={error*100:.2f}%, gnorm={gnorm:.5e}, {iteration}/{patience})"
+                    )
+
+                if log_likelihood > model.results.best_loglikelihood:
+                    # validate if loglikelihood improves
+                    error = model.prediction_error_fn(*valid_data)
+
+                    this_ll = log_likelihood
+                    best_ll = model.results.best_loglikelihood
+                    if this_ll > best_ll / validation_threshold:
+                        # increase patience if model is not converged
+                        patience = int(
+                            min(max(patience, iteration * patience_inc), max_iterations)
+                        )
+
+                    model.results.best_step = step
+                    model.results.best_iteration = iteration
+                    model.results.best_loglikelihood = log_likelihood
+                    model.results.best_valid_error = error
+                    model.results.params = model.params
+                    model.results.gnorm = gnorm
+
+                if gnorm < convergence_threshold:
+                    converged = True
+                else:
+                    patience = int(
+                        min(max(patience, iteration * patience_inc), max_iterations)
+                    )
+
+            iteration += 1
+
+            # reached convergence
+            if (iteration > patience) or converged:
+                iteration -= 1
+                info(
+                    f"Train (Step={step}, LL={log_likelihood:.2f}, Error={error*100:.2f}%, gnorm={gnorm:.5e}, {iteration}/{patience})"
                 )
 
-                if valid_error >= self.results.best_valid_error:
-                    continue
-                msg = f"Best validation error = {valid_error*100:.3f}%, (s={step}, i={iteration}, p={patience}, ll={train_ll:.2f})"
-                debug(msg)
-
-                self.results.best_step = step
-                self.results.best_iteration = iteration
-                self.results.best_loglikelihood = train_ll
-                self.results.best_valid_error = valid_error
-
-                self.results.betas = self.betas
-                self.results.weights = self.weights
-
-                # increase patience if past validation threshold
-                if train_ll > (self.results.best_loglikelihood / validation_threshold):
-                    continue
-
-                patience = min(
-                    max(patience, iteration * patience_increase), max_iterations
-                )
+                done_looping = True  # break loop if convergence reached
+                break
 
-            # increment step
-            step += 1
+        step += 1  # increment step
 
-        train_time = round(perf_counter() - start_time, 3)
-        self.results.train_time = time_format(train_time)
-        self.results.iterations_per_sec = round(iteration / train_time, 2)
-        msg = f"End (t={self.results.train_time}, VE={self.results.best_valid_error*100:.2f}%, LL={self.results.best_loglikelihood:.2f}, Step={self.results.best_step})"
-        info(msg)
-
-        self.betas = self.results.betas
-        self.weights = self.results.weights
-        self.results.n_train_samples = db.n_train_samples
-        self.results.n_valid_samples = db.n_valid_samples
-        self.results.n_params = self.n_params
-        self.results.seed = self.config["seed"]
-        self.results.lr_history_graph = self.config["lr_scheduler"].history
-
-        # statistical analysis step
-        self.results.gnorm = self.gradient_norm(*db.train_data)
-        self.results.hessian_matrix = self.H(*db.train_data)
-        self.results.bhhh_matrix = self.BHHH(*db.train_data)
-
-    def export_to_pickle(self, f):
-        """to be removed in 1.4.0"""
-        model = self
-        pickle.dump(model, f)
+    train_time = round(perf_counter() - start_time, 3)
+    model.results.train_time = time_format(train_time)
+    model.results.iterations_per_sec = round(iteration / train_time, 2)
+    if converged:
+        info(f"Model converged (t={train_time})")
+    else:
+        info(
+            f"Maximum number of iterations reached: {iteration}/{patience} (t={train_time})"
+        )
 
-    def __str__(self):
-        return f"{self.name}"
+    model.results.lr_history_graph = lr_scheduler.history
+    model.results.performance_graph = performance_graph
+    model.params = model.results.params
+
+    betas = [param for param in model.params if isinstance(param, Beta)]
+    n_betas = len([b for b in betas if (b.status != 1)])
+    gradient_vector = np.zeros((n_train, n_betas))
+    hessian = np.zeros((n_train, n_betas, n_betas))
+    for n in range(n_train):
+        data = [[d[n]] for d in train_data]
+        gradient_vector[n, :] = model.gradient_vector_fn(*data)
+        hessian[n, :, :] = model.hessian_fn(*data)
+
+    bhhh = gradient_vector[:, :, None] * gradient_vector[:, None, :]
+
+    model.results.bhhh_matrix = bhhh
+    model.results.hessian_matrix = hessian
+
+    info(
+        f"Best results obtained at Step {model.results.best_step}: LL={model.results.best_loglikelihood:.2f}, Error={model.results.best_valid_error*100:.2f}%, gnorm={model.results.gnorm:.5e}"
+    )
```

### Comparing `pycmtensor-1.3.2/pycmtensor/results.py` & `pycmtensor-1.4.0/pycmtensor/results.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # results.py
 """PyCMTensor results module"""
 import numpy as np
 import pandas as pd
 from numpy import nan_to_num as nan2num
 
-from .statistics import *
+from pycmtensor.expressions import Beta
+from pycmtensor.statistics import *
 
 __all__ = ["Results"]
 
 
 class Results:
     """Class object to hold model results"""
 
     def __init__(self):
         self.build_time = None
         self.train_time = None
         self.iterations_per_sec = None
         self.n_params = None
-        self.n_train_samples = None
-        self.n_valid_samples = None
+        self.n_train = None
+        self.n_valid = None
         self.seed = None
 
         self.null_loglikelihood = -np.inf
-        self.init_loglikelihood = -np.inf
         self.best_loglikelihood = -np.inf
         self.best_valid_error = 1.0
         self.best_step = 0
 
         self.gnorm = None
         self.hessian_matrix = None
         self.bhhh_matrix = None
+        self.params = None
         self.betas = None
         self.weights = None
 
         self.performance_graph = None
         self.lr_history_graph = None
 
     def rho_square(self):
@@ -53,56 +54,57 @@
         """Returns the Akaike Information Criterion"""
         k = self.n_params
         return 2.0 * (k - self.best_loglikelihood)
 
     def BIC(self):
         """Returns the Bayesian Information Criterion"""
         k = self.n_params
-        n = self.n_train_samples
+        n = self.n_train
         return -2.0 * self.best_loglikelihood + k * np.log(n)
 
     def benchmark(self):
         """Returns a pandas DataFrame of a summary of the model benchmark"""
         stats = pd.DataFrame(columns=["value"])
         stats.loc["Seed"] = self.seed
         stats.loc["Model build time"] = self.build_time
         stats.loc["Model train time"] = self.train_time
-        stats.loc["iterations per sec"] = f"{self.iterations_per_sec}/s"
+        stats.loc["iterations per sec"] = f"{self.iterations_per_sec} iter/s"
         return stats
 
     def model_statistics(self):
         """Returns a pandas DataFrame of a summary of the model training"""
         stats = pd.DataFrame(columns=["value"]).astype("object")
-        stats.loc["Number of training samples used"] = int(self.n_train_samples)
-        stats.loc["Number of validation samples used"] = int(self.n_valid_samples)
-        stats.loc["Init. log likelihood"] = self.init_loglikelihood
+        stats.loc["Number of training samples used"] = int(self.n_train)
+        stats.loc["Number of validation samples used"] = int(self.n_valid)
+        stats.loc["Null. log likelihood"] = self.null_loglikelihood
         stats.loc["Final log likelihood"] = self.best_loglikelihood
         stats.loc["Accuracy"] = f"{100*(1-self.best_valid_error):.2f}%"
         stats.loc["Likelihood ratio test"] = self.loglikelihood_ratio_test()
         stats.loc["Rho square"] = self.rho_square()
         stats.loc["Rho square bar"] = self.rho_square_bar()
         stats.loc["Akaike Information Criterion"] = self.AIC()
         stats.loc["Bayesian Information Criterion"] = self.BIC()
-        stats.loc["Final gradient norm"] = self.gnorm
+        stats.loc["Final gradient norm"] = f"{self.gnorm:.5e}"
         return stats
 
     def beta_statistics(self):
         """Returns a pandas DataFrame of the model beta statistics"""
-        betas = self.betas
-        h = self.hessian_matrix
-        bhhh = self.bhhh_matrix
+        n = len(self.hessian_matrix)
+        betas = [p for p in self.params if isinstance(p, Beta)]
+        h = self.hessian_matrix.sum(axis=0)
+        bh = self.bhhh_matrix.sum(axis=0)
 
         stats = pd.DataFrame(
             index=[b.name for b in betas if (b.status != 1)], columns=["value"]
         )
         stats["std err"] = stderror(h, betas)
         stats["t-test"] = t_test(stats["std err"], betas)
         stats["p-value"] = p_value(stats["std err"], betas)
 
-        stats["rob. std err"] = rob_stderror(h, bhhh, betas)
+        stats["rob. std err"] = rob_stderror(h, bh, betas)
         stats["rob. t-test"] = t_test(stats["rob. std err"], betas)
         stats["rob. p-value"] = p_value(stats["rob. std err"], betas)
         stats.drop("value", axis=1, inplace=True)
 
         df = pd.DataFrame(
             data=[b().eval() for b in betas],
             index=[b.name for b in betas],
@@ -110,31 +112,31 @@
         )
         stats = pd.concat([df, stats], axis=1).sort_index().fillna("-").astype("O")
 
         return stats
 
     def model_correlation_matrix(self):
         """Returns a pandas DataFrame of the model correlation matrix"""
-        betas = self.betas
-        h = self.hessian_matrix
+        betas = [p for p in self.params if isinstance(p, Beta)]
+        h = self.hessian_matrix.sum(axis=0)
 
         mat = pd.DataFrame(
             columns=[b.name for b in betas if (b.status != 1)],
             index=[b.name for b in betas if (b.status != 1)],
             data=correlation_matrix(h),
         )
 
         return mat
 
     def model_robust_correlation_matrix(self):
         """Returns a pandas DataFrame of the model (robust) correlation matrix"""
-        betas = self.betas
-        h = self.hessian_matrix
-        bhhh = self.bhhh_matrix
+        betas = [p for p in self.params if isinstance(p, Beta)]
+        h = self.hessian_matrix.sum(axis=0)
+        bh = self.bhhh_matrix.sum(axis=0)
 
         mat = pd.DataFrame(
             columns=[b.name for b in betas if (b.status != 1)],
             index=[b.name for b in betas if (b.status != 1)],
-            data=rob_correlation_matrix(h, bhhh),
+            data=rob_correlation_matrix(h, bh),
         )
 
         return mat
```

### Comparing `pycmtensor-1.3.2/pycmtensor/scheduler.py` & `pycmtensor-1.4.0/pycmtensor/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 
 __all__ = [
     "Scheduler",
     "ConstantLR",
     "StepLR",
     "PolynomialLR",
     "CyclicLR",
-    "Triangular2CLR",
+    "TriangularCLR",
     "ExpRangeCLR",
 ]
 
 
 class Scheduler:
     """Base class for Scheduler object"""
 
-    def __init__(self):
+    def __init__(self, lr):
         """Constructor for Scheduler class object"""
         self.name = "Scheduler"
+        self._base_lr = lr
+        self._history = OrderedDict()
 
     def __str__(self):
         return f"{self.name}"
 
     def __repr__(self):
         msg = f"{self.name}("
         attrs = [d for d in dir(self) if not d.startswith("_")]
@@ -32,53 +34,52 @@
             if a == "name":
                 continue
             if isinstance(getattr(self, a), (int, str, float)):
                 msg += f"{a}={getattr(self, a)}, "
 
         return msg[:-2] + ")"
 
+    @property
+    def lr(self):
+        """Returns the learning rate value"""
+        return self._base_lr
+
+    @property
+    def history(self):
+        """Returns the histroy of the learning rate"""
+        return self._history
+
+    def _record(self, step, lr):
+        """Saves the history of the learning rate and returns the current rate"""
+        self._history[step] = lr
+        return lr
+
 
 class ConstantLR(Scheduler):
     """Base class for constant learning rate scheduler"""
 
-    def __init__(self, lr=0.01):
+    def __init__(self, lr=0.01, **kwargs):
         """Constructor for ConstantLR class object
 
         Args:
             lr (float, optional): learning rate value
         """
+        super().__init__(lr)
         self.name = "ConstantLR"
-        self._base_lr = lr
-        self._history = OrderedDict()
-
-    @property
-    def lr(self):
-        """Returns the learning rate value"""
-        return self._base_lr
-
-    @property
-    def history(self):
-        """Returns the histroy of the learning rate"""
-        return self._history
 
     def __call__(self, step):
         """Computes the learning rate for this step"""
         self._record(step, self.lr)
         return self.lr
 
-    def _record(self, step, lr):
-        """Saves the history of the learning rate and returns the current rate"""
-        self._history[step] = lr
-        return lr
-
 
 class StepLR(ConstantLR):
     """Base class for step learning rate scheduler"""
 
-    def __init__(self, lr=0.01, factor=0.25, drop_every=10):
+    def __init__(self, lr=0.01, factor=0.25, drop_every=10, **kwargs):
         """Constructor for StepLR class object
 
         Args:
             lr (float): initial learning rate value
             factor (float, optional): percentage reduction to the learning rate
             drop_every (int, optional): step down the learning rate after every n steps
         """
@@ -109,15 +110,15 @@
         lr = float(self.lr * decay)
         return self._record(step, lr)
 
 
 class PolynomialLR(ConstantLR):
     """Base class for polynomial decay learning rate scheduler"""
 
-    def __init__(self, max_steps, lr=0.01, power=1.0):
+    def __init__(self, max_steps, lr=0.01, power=1.0, **kwargs):
         """Constructor for PolynomialLR class object
 
         Args:
             lr (float): initial learning rate value
             max_steps (int): the max number of training steps to take
             power (float, optional): the exponential factor to decay
         """
@@ -145,15 +146,15 @@
         lr = float(self.lr * decay)
         return self._record(step, lr)
 
 
 class CyclicLR(ConstantLR):
     """Base class for cyclical learning rate scheduler"""
 
-    def __init__(self, lr=0.01, max_lr=0.1, cycle_steps=16, scale_fn=None):
+    def __init__(self, lr=0.01, max_lr=0.1, cycle_steps=16, scale_fn=None, **kwargs):
         """Constructor for ConstantLR class object
 
         Args:
             lr (float, optional): the base learning rate value
             max_lr (float, optional): the maximum learning rate value
             cycle_steps (int, optional): the number of steps to complete a cycle
             scale_fn (func, optional): custom scaling policy defined by a single arg
@@ -183,24 +184,21 @@
         x = np.abs(step / (self.cycle_steps / 2) - 2 * cycle + 1)
         height = (self.max_lr - self.lr) * self.scale_fn(cycle)
         lr = self.lr + height * np.maximum(0, 1 - x)
         return self._record(step, lr)
 
     def scale_fn(self, k):
         """Custom scaling policy"""
-        if self._scale_fn is None:
-            return 1.0
-        else:
-            return self._scale_fn(k)
+        return 1.0
 
 
-class Triangular2CLR(CyclicLR):
-    """Class object for the Triangular2 Cyclic LR scheduler"""
+class TriangularCLR(CyclicLR):
+    """Class object for the Triangular Cyclic LR scheduler"""
 
-    def __init__(self, lr=0.01, max_lr=0.1, cycle_steps=16):
+    def __init__(self, lr=0.01, max_lr=0.1, cycle_steps=16, **kwargs):
         """Constructor for Triangular2CLR class object
 
         Args:
             lr (float, optional): the base learning rate value
             max_lr (float, optional): the maximum learning rate value
             cycle_steps (int, optional): the number of steps to complete a cycle
         """
@@ -211,15 +209,15 @@
         """Calculates the cycle amplitude scale"""
         return float(1.0 / (2.0 ** (k - 1.0)))
 
 
 class ExpRangeCLR(CyclicLR):
     """Class object for the exponential range Cyclic LR scheduler"""
 
-    def __init__(self, lr=0.01, max_lr=0.1, cycle_steps=16, gamma=0.5):
+    def __init__(self, lr=0.01, max_lr=0.1, cycle_steps=16, gamma=0.5, **kwargs):
         """Constructor for Triangular2CLR class object
 
         Args:
             lr (float, optional): the base learning rate value
             max_lr (float, optional): the maximum learning rate value
             cycle_steps (int, optional): the number of steps to complete a cycle
         """
```

### Comparing `pycmtensor-1.3.2/pycmtensor/statistics.py` & `pycmtensor-1.4.0/pycmtensor/statistics.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,24 +15,24 @@
     "stderror",
     "t_test",
     "elasticities",
 ]
 
 
 def variance_covariance(h):
-    """Returns the var-covar matrix given the Hessian (``h``)"""
-    return -nlinalg.pinv(nan2num(h)).eval()
+    """Returns the variance covariance matrix given the Hessian (``h``)"""
+    return nlinalg.pinv(nan2num(-h)).eval()
 
 
-def rob_variance_covariance(h, bhhh):
+def rob_variance_covariance(h, bh):
     """Returns the rob. var-covar matrix given the Hessian (``h``) and the BHHH
-    matrix (``bhhh``)
+    matrix (``bh``)
     """
-    var_covar = variance_covariance(h)
-    return var_covar.dot(bhhh.dot(var_covar))
+    cr = variance_covariance(h)
+    return cr.dot(bh.dot(cr))
 
 
 def t_test(stderr, params):
     """Returns the t stats of ``params`` given the standard error (``stderr``)"""
     params = [p() for p in params if (p.status != 1)]
     return [p.eval() / s for p, s in zip(params, stderr)]
 
@@ -40,34 +40,38 @@
 def p_value(stderr, params):
     """Returns the p-value of ``params`` given the standard error (``stderr``)"""
     tTest = t_test(stderr, params)
     return [2.0 * (1.0 - stats.norm.cdf(abs(t))) for t in tTest]
 
 
 def stderror(h, params):
-    """Returns the standard error of ``params`` given the Hessian (``h``)"""
+    """Returns the standard error of ``params`` given the Hessian (``h``)
+
+    The std err is calculated as the square root of the variance covariance
+    matrix.
+
+    """
     params = [p() for p in params if (p.status != 1)]
     varCovar = variance_covariance(h)
     stdErr = []
     for i in range(len(params)):
         if varCovar[i, i] < 0:
             stdErr.append(np.finfo(float).max)
         else:
             stdErr.append(np.sqrt(varCovar[i, i] + 1e-8))  # for numerical stability
 
     return stdErr
 
 
-def rob_stderror(h, bhhh, params):
+def rob_stderror(h, bh, params):
     """Returns the rob. standard error of ``params`` given the Hessian (``h``) and the
-    BHHH matrix (``bhhh``)
+    BHHH matrix (``bh``)
     """
     params = [p() for p in params if (p.status != 1)]
-    varCovar = variance_covariance(h)
-    robVarCovar = varCovar.dot(bhhh.dot(varCovar))
+    robVarCovar = rob_variance_covariance(h, bh)
     robstderr = []
     for i in range(len(params)):
         if robVarCovar[i, i] < 0:
             robstderr.append(np.finfo(float).max)
         else:
             robstderr.append(np.sqrt(robVarCovar[i, i] + 1e-8))
 
@@ -84,17 +88,17 @@
         mat = diag_inv.dot(var_covar.dot(diag_inv))
     else:
         mat = np.full_like(var_covar, np.finfo(float).max)
 
     return mat
 
 
-def rob_correlation_matrix(h, bhhh):
+def rob_correlation_matrix(h, bh):
     """Returns the correlation matrix given the Hessian and the BHHH matrix"""
-    rob_var_covar = rob_variance_covariance(h, bhhh)
+    rob_var_covar = rob_variance_covariance(h, bh)
     rd = np.diag(rob_var_covar)
     if (rd > 0).all():
         diag = np.diag(np.sqrt(rd))
         diag_inv = nlinalg.inv(diag).eval()
         mat = diag_inv.dot(rob_var_covar.dot(diag_inv))
     else:
         mat = np.full_like(rob_var_covar, np.finfo(float).max)
@@ -119,9 +123,9 @@
         outputs=aet.grad(
             aet.sum(model.p_y_given_x[y]), db[x], disconnected_inputs="ignore"
         )
         * db[x]
         / model.p_y_given_x[y],
         on_unused_input="ignore",
     )
-    data = db.pandas.inputs(model.inputs, split_type="train")
+    data = db.train(model.inputs)
     return fn_elasticity(*data)
```

### Comparing `pycmtensor-1.3.2/pyproject.toml` & `pycmtensor-1.4.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pycmtensor"
-version = "1.3.2"
+version = "1.4.0"
 description = "Python Tensor based package for discrete choice modelling."
 authors = ["Melvin Wong <m.j.w.wong@tue.nl>"]
-license = "MIT License"
+license = "MIT"
 readme = "README.md"
 
 homepage = ""
 repository = "https://github.com/mwong009/pycmtensor"
 documentation = ""
 
 keywords = []
@@ -22,53 +22,45 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.dependencies]
-# Core
-python = "~3.11"
-aesara = "~2.9"
-numpy = "^1.21.2"
-scipy = "^1.7.1"
+python = "^3.9, <3.12"
 pandas = "^1.4.1"
-pydot = "^1.4.2"
-dill = "^0.3.4"
+scipy = "^1.7.1"
 watermark = "^2.3.1"
 
-# Formatters
-black = { version = "^23.3.0", optional = true } 
-isort = { version = "^5.9.1", optional = true } 
-
-#Linters
-pydocstyle = { version = "^6.1.1", optional = true } 
-rstcheck = { version = "^6.1.2", optional = true } 
-
-# Documentation
-Sphinx = { version = "^5.3.0", optional = true } 
-sphinx-book-theme = { version = "^1.0.1", optional = true } 
-sphinx-design = {version = "^0.4.1", optional = true}
-sphinx-autoapi = { version = "^2.1.1", optional = true } 
-myst-nb = {version = "^0.17.2", optional = true}
-
-# Tooling
-pre-commit = { version = "^3.3.3", optional = true } 
-commitizen = { version = "^3.3.0", optional = true } 
 
-[tool.poetry.dev-dependencies]
-# Testing
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1.0"
 
-[tool.poetry.extras]
-lint = ["black", "isort", "pydocstyle", "rstcheck"]
-commit = ["commitizen", "pre-commit"]
-docs = ["Sphinx", "sphinx-book-theme", "sphinx-autoapi", "myst-nb", "sphinx-design"]
-dev = ["black", "isort", "pydocstyle", "rstcheck", "Sphinx", "sphinx-book-theme", "sphinx-design", "sphinx-autoapi", "myst-nb", "commitizen", "pre-commit"]
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+isort = "^5.9.1"
+pre-commit = "^3.3.3"
+commitizen = "^3.3.0"
+ipykernel = "^6.24.0"
+
+[tool.poetry.group.doc]
+optional = true
+
+[tool.poetry.group.doc.dependencies]
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.18"
+pymdown-extensions = "^10.0.1"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
@@ -77,39 +69,25 @@
 [tool.black]
 line-length = 88
 target-version = ["py311"]
 quiet = false
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.3.2"
+version = "1.4.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version",
     "pycmtensor/__init__.py",
-    "docs/conf.py",
-    "docs/index.md",
-    "README.md"
 ]
 
 [tool.pytest]
 markers = []
-# command: 
-# poetry run pytest .
+## poetry run pytest .
 
 [tool.pytest.ini_options]
-addopts = [
-    "--cov=pycmtensor",
-    "--cov-report=xml",
-    # "--ignore-glob=*performance.py",
-]
-
-filterwarnings = [
-    "error",
-    "ignore::UserWarning",
-    "ignore::DeprecationWarning",
-]
+addopts = ["--cov=pycmtensor", "--cov-report=xml"]
+filterwarnings = ["error", "ignore::UserWarning", "ignore::DeprecationWarning"]
 
 [tool.coverage.run]
 omit = [".*", "*/site-packages/*", "tests/*", "docs/*", "samples/*"]
-# command:
 # poetry run coverage run -m pytest && poetry run coverage report
```

