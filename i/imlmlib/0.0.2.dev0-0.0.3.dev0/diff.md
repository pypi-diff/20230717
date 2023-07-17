# Comparing `tmp/imlmlib-0.0.2.dev0.tar.gz` & `tmp/imlmlib-0.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imlmlib-0.0.2.dev0.tar", max compression
+gzip compressed data, was "imlmlib-0.0.3.dev0.tar", max compression
```

## Comparing `imlmlib-0.0.2.dev0.tar` & `imlmlib-0.0.3.dev0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-03-09 16:42:28.654825 imlmlib-0.0.2.dev0/LICENSE
--rw-r--r--   0        0        0     1329 2023-03-09 08:42:45.345552 imlmlib-0.0.2.dev0/imlmlib/ACTR_2005.py
--rw-r--r--   0        0        0       28 2023-04-06 16:03:27.202899 imlmlib-0.0.2.dev0/imlmlib/__init__.py
--rw-r--r--   0        0        0    12655 2023-04-06 14:17:58.826258 imlmlib-0.0.2.dev0/imlmlib/exponential_forgetting.py
--rw-r--r--   0        0        0     8852 2023-04-06 14:07:43.550669 imlmlib-0.0.2.dev0/imlmlib/mem_utils.py
--rw-r--r--   0        0        0     8573 2023-04-06 15:26:08.825945 imlmlib-0.0.2.dev0/imlmlib/mle_utils.py
--rw-r--r--   0        0        0      551 2023-04-06 16:03:27.202899 imlmlib-0.0.2.dev0/pyproject.toml
--rw-r--r--   0        0        0      741 2023-04-06 16:03:57.381568 imlmlib-0.0.2.dev0/setup.py
--rw-r--r--   0        0        0      646 2023-04-06 16:03:57.381757 imlmlib-0.0.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-09 16:42:28.654825 imlmlib-0.0.3.dev0/LICENSE
+-rw-r--r--   0        0        0     1329 2023-03-09 08:42:45.345552 imlmlib-0.0.3.dev0/imlmlib/ACTR_2005.py
+-rw-r--r--   0        0        0       28 2023-07-17 09:10:03.661287 imlmlib-0.0.3.dev0/imlmlib/__init__.py
+-rw-r--r--   0        0        0     1923 2023-07-12 09:51:38.886470 imlmlib-0.0.3.dev0/imlmlib/abc.py
+-rw-r--r--   0        0        0    22012 2023-07-17 09:09:09.621749 imlmlib-0.0.3.dev0/imlmlib/exponential_forgetting.py
+-rw-r--r--   0        0        0    10872 2023-07-11 08:55:35.929085 imlmlib-0.0.3.dev0/imlmlib/mem_utils.py
+-rw-r--r--   0        0        0     7073 2023-07-13 14:12:27.299119 imlmlib-0.0.3.dev0/imlmlib/mle_utils.py
+-rw-r--r--   0        0        0      629 2023-07-17 09:10:03.661287 imlmlib-0.0.3.dev0/pyproject.toml
+-rw-r--r--   0        0        0      850 2023-07-17 09:29:23.515954 imlmlib-0.0.3.dev0/setup.py
+-rw-r--r--   0        0        0      811 2023-07-17 09:29:23.516133 imlmlib-0.0.3.dev0/PKG-INFO
```

### Comparing `imlmlib-0.0.2.dev0/LICENSE` & `imlmlib-0.0.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `imlmlib-0.0.2.dev0/imlmlib/ACTR_2005.py` & `imlmlib-0.0.3.dev0/imlmlib/ACTR_2005.py`

 * *Files identical despite different names*

### Comparing `imlmlib-0.0.2.dev0/imlmlib/mem_utils.py` & `imlmlib-0.0.3.dev0/imlmlib/mem_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     :return: (queries, memory_model), where queries = [(good recall?, recall_probability)]
     :rtype: list(tuple(boolean, float))
     """
     queries = []
     if reset:
         memory_model.reset()
     for item, time in schedule:
-        queries.append(memory_model.query_item(item, time))
+        query = memory_model.query_item(item, time)
+        queries.append(query)
         memory_model.update(item, time)
     return queries, memory_model
 
 
 def experiment(population_model, schedule, replications=1):
     """experiment run a memory experiment with a population model, a fixed schedule, and a set amount of replications per participant
 
@@ -64,21 +65,33 @@
     :type schedule: inherits from an imlmlib Schedule
     :param replications: number of replications for each participant, defaults to 1
     :type replications: int, optional
     :return: the simulated data
     :rtype: numpy.array((replication, 2, len(schedule), population size))
     """
     data = numpy.zeros((replications, 2, len(schedule), population_model.pop_size))
-    for i in range(replications):
-        for n, memory_model in enumerate(population_model):
+
+    n = 0
+    for memory_model in population_model:
+        for i in range(replications):
             trial_data = numpy.array(trial(memory_model, schedule)[0])
             data[i, :, :, n] = trial_data.T
+        n += 1
     return data
 
 
+def serialize_experiment(data):
+    _shape = data.shape
+    data = data.reshape(_shape[0], _shape[1], -1, order="F")  # careful for the order
+    k_vector = []
+    for i in range(_shape[3]):
+        k_vector += [k for k in range(-1, _shape[2] - 1)]
+    return data, k_vector
+
+
 class Schedule:
     """Iterate over (items, times) pairs.
 
     A schedule is an association between presented items and the times at which these where presented. One can iterate over a schedule to get a pair (item, time).
     """
 
     def __init__(self, items, times):
@@ -103,24 +116,72 @@
 
     def __iter__(self):
         self.counter = 0
         return self
 
     def __next__(self):
         if self.counter < self.max:
-            ret_value = (self.items[self.counter], self.times[self.counter])
+            ret_value = self[self.counter]
             self.counter += 1
             return ret_value
         else:
             raise StopIteration
 
     def __repr__(self):
         return f"items: {self.items}\ntimes: {self.times}"
 
 
+class BlockBasedSchedule(Schedule):
+    def __init__(self, nitems, intertrial_time, interblock_time, repet_trials=2, seed = None, sigma_t = None):
+
+        self.seed = seed
+        self.rng = numpy.random.default_rng(self.seed)
+        self.sigma_t = sigma_t
+
+        self.nitems = nitems
+        self.intertrial_time = intertrial_time
+        self.interblock_time = interblock_time
+        self.repet_trials = repet_trials if repet_trials is not None else 1
+
+        self.items, self.times, self.blocks = self.regen_schedule()
+        self.max = numpy.array(self.times).squeeze().shape[0]
+        
+
+    def regen_schedule(
+        self, intertrial_time=None, interblock_time=None, repet_trials=None
+    ):
+        self.intertrial_time = (
+            self.intertrial_time if intertrial_time is None else intertrial_time
+        )
+        self.interblock_time = (
+            self.interblock_time if interblock_time is None else interblock_time
+        )
+        self.repet_trials = self.repet_trials if repet_trials is None else repet_trials
+
+        items = []
+        times = []
+        blocks = []
+        t = 0
+        for nb, ibt in enumerate((self.interblock_time + [0])):
+            for r in range(self.repet_trials):
+                if self.sigma_t is not None:
+                    _rdm = self.rng.lognormal(sigma = self.sigma_t, size = (self.nitems,))
+                else:
+                    _rdm = numpy.zeros((self.nitems,))
+                for i,r in zip(range(self.nitems), _rdm):
+                    items.append(i)
+                    times.append(t)
+                    
+                    t += self.intertrial_time + r
+                    blocks.append(nb)
+            t += ibt
+
+        return items, times, blocks
+    
+
 class Player:
     def __init__(self, schedule, memory_model):
         self._schedule = schedule
         self.memory_model = memory_model
         self.step_counter = 0
 
     def reset(self):
```

### Comparing `imlmlib-0.0.2.dev0/imlmlib/mle_utils.py` & `imlmlib-0.0.3.dev0/imlmlib/mle_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy
+import scipy
 import scipy.optimize as opti
 import functools
+import matplotlib.pyplot as plt
 from matplotlib.patches import Ellipse
-import matplotlib.transforms as transforms
 from tqdm import tqdm
 from itertools import chain
 
 from imlmlib.mem_utils import experiment
 from imlmlib.exponential_forgetting import (
     ef_get_per_participant_likelihood_transform,
     ef_ddq1_dalpha_dalpha_sample,
@@ -14,190 +15,117 @@
     ef_ddq1_dbeta_dbeta_sample,
     ef_ddq0_dalpha_dalpha_sample,
     ef_ddq0_dalpha_dbeta_sample,
     ef_ddq0_dbeta_dbeta_sample,
 )
 
 
-def grid_ll(likelihood, schedule, xp_data, discretize, verbose=False):
-    """grid_ll _summary_
+# class ConfidenceEllipsisNotDefinedError(Exception):
+#     """ConfidenceEllipsisNotDefinedError
 
-    import matplotlib.pyplot as plt
+#     Raised when the estimated covariance matrix is singular
+#     """
 
-    discretize = (40, 10)
-    res = grid_ll(ef_get_global_likelihood, schedule_one, data, discretize)
-    ll = numpy.clip(res[:, 2], max(res[:, 2]) * 2, max(res[:, 2])).reshape(*discretize)
-    maxll = res[numpy.argmax(ll), :2]
-    plt.imshow(ll)
-    plt.plot(maxll[1] * 10, 29, "rD")
-    plt.plot(0.5 * 10, (-2 + 5) * 10)
-    plt.show()
-    exit()
-    """
-    # invert sign and deal with argument shape
-    ll_lambda = lambda guess, args: -likelihood(guess, *args)
-
-    data = xp_data[0]
-
-    grid = numpy.dstack(
-        numpy.meshgrid(
-            numpy.linspace(-5, -1, discretize[0]),
-            numpy.linspace(0, 0.99, discretize[1]),
-        )
-    ).reshape(-1, 2)
-
-    ll = numpy.zeros((grid.shape[0], 3))
-    for i, theta in enumerate(grid):
-        ll[i, :2] = theta
-        ll[i, 2] = -ll_lambda(theta, [data, schedule])
+#     pass
 
-    return ll
 
 
 def estim_mle_one_trial(
-    times,
-    recalls,
-    transform,
-    k_vector,
-    likelihood_function,
-    optimizer_kwargs,
-    guess,
+    times, recalls, k_vector, likelihood_function, optimizer_kwargs, guess, **kwargs
 ):
+    # note: removed possibility to specify transform function
+    # note: check the k_vector
+
     # invert sign and deal with argument shape
     ll_lambda = lambda guess, args: -likelihood_function(guess, *args)
 
     res = opti.minimize(
-        ll_lambda, guess, args=[times, recalls, transform, k_vector], **optimizer_kwargs
+        ll_lambda, guess, args=[times, recalls, k_vector], **optimizer_kwargs
     )
 
     return res
 
 
-def confidence_ellipse(x, y, cov, ax, n_std=3.0, facecolor="none", **kwargs):
-    """straightforward adaptation from :
-    https://matplotlib.org/stable/gallery/statistics/confidence_ellipse.html
-
-    Create a plot of the covariance confidence ellipse of *x* and *y*.
-
-    Parameters
-    ----------
-    cov : array-like, shape (n, n)
-        Input data.
-
-    ax : matplotlib.axes.Axes
-        The axes object to draw the ellipse into.
+numpy.seterr(divide="raise")
 
-    n_std : float
-        The number of standard deviations to determine the ellipse's radiuses.
 
-    **kwargs
-        Forwarded to `~matplotlib.patches.Ellipse`
+def _confidence_ellipsis(x, cov, critical_value = 5.991, **kwargs):
+    # critical values can be looked up in a chisquared table with df = 2
 
-    Returns
-    -------
-    matplotlib.patches.Ellipse
-    """
-
-    pearson = cov[0, 1] / numpy.sqrt(cov[0, 0] * cov[1, 1])
-    # Using a special case to obtain the eigenvalues of this
-    # two-dimensional dataset.
-    ell_radius_x = numpy.sqrt(1 + pearson)
-    ell_radius_y = numpy.sqrt(1 - pearson)
-    ellipse = Ellipse(
-        (0, 0),
-        width=ell_radius_x * 2,
-        height=ell_radius_y * 2,
-        facecolor=facecolor,
-        **kwargs,
-    )
-
-    # Calculating the standard deviation of x from
-    # the squareroot of the variance and multiplying
-    # with the given number of standard deviations.
-    scale_x = numpy.sqrt(cov[0, 0]) * n_std
-
-    # calculating the standard deviation of y ...
-    scale_y = numpy.sqrt(cov[1, 1]) * n_std
-
-    transf = (
-        transforms.Affine2D().rotate_deg(45).scale(scale_x, scale_y).translate(x, y)
-    )
+    eigen_values, eigen_vectors = numpy.linalg.eig(cov)
+    indexes = eigen_values.argsort()[::-1]
+    eigen_values = eigen_values[indexes]
+    eigen_vectors = eigen_vectors[:,indexes]
+
+    ellipsis_orientation = numpy.arctan2(eigen_vectors[:,0][1], eigen_vectors[:,0][0])
+    
+    ellipsis_large_axis = 2*numpy.sqrt(critical_value*eigen_values[0])
+    ellipsis_small_axis = 2*numpy.sqrt(critical_value*eigen_values[1])
+    return Ellipse(x, ellipsis_large_axis, ellipsis_small_axis, ellipsis_orientation, **kwargs)
+
+
+def confidence_ellipse(inferred_parameters, estimated_covariance_matrix,  alpha_scale = 'log', confidence_levels = [.68, .95], plot = False, ax = None, colors = ['#B0E0E6', '#87CEEB'], CI95 = False, plot_kwargs = {'color': 'red', 'marker': 'D', 'label' : 'MLE'}):
+    """estimated_covariance_matrix = numpy.linalg.inv(J)"""
+    
+
+    x = inferred_parameters
+    if alpha_scale == 'log':
+        estimated_covariance_matrix, CI_log_alpha, CI_beta = delta_method_log_CI(*x, estimated_covariance_matrix)
+        x = (numpy.log10(x[0]), x[1])
+
+    if plot is False:
+        return CI_log_alpha, CI_beta
+    if ax is None:
+        fig, ax = plt.subplots(nrows = 1, ncols = 1)
+    critical_values = [scipy.stats.chi2.ppf(cl, 2) for cl in confidence_levels]
+    for critical_value, color, cl in zip(critical_values[::-1], colors[::-1], confidence_levels[::-1]):
+        ax.add_patch(_confidence_ellipsis(x, estimated_covariance_matrix, critical_value, fill = True, facecolor = color, edgecolor= 'b', label = f'Confidence level:{cl}'))
+
+    ax.plot(*x, **plot_kwargs)
+        
+
+    if CI95:
+        return ax, CI_log_alpha, CI_beta
+    else:
+        return ax
 
-    ellipse.set_transform(transf + ax.transData)
-    return ax.add_patch(ellipse)
 
 
 def identify_alpha_beta_from_recall_sequence(
     recall_sequence,
     deltas,
     guess=(1e-3, 0.5),
     optim_kwargs={"method": "L-BFGS-B", "bounds": [(1e-7, 5e-1), (0, 0.99)]},
     verbose=True,
     k_vector=None,
 ):
 
-    # for r, d, k in zip(recall_sequence, deltas, k_vector):
-    #     print(r, d, k)
-
     infer_results = estim_mle_one_trial(
         deltas,
         recall_sequence,
-        lambda a, b: (a, b),
         k_vector,
         ef_get_per_participant_likelihood_transform,
         optim_kwargs,
         guess,
     )
 
     if verbose:
         print(infer_results)
 
-    I, _, CI_alpha, CI_beta = get_confidence_single(
-        recall_sequence, deltas, *infer_results.x, verbose=verbose
-    )
-    return infer_results, I, CI_alpha, CI_beta
-
+    return infer_results
 
-def sample_mle(REPL, Nseq, population_model, schedule):
-    data = experiment(population_model, schedule, replications=REPL * Nseq)
-    results = numpy.zeros((8, REPL))
-    for r in tqdm(range(REPL)):
-        recall_sequence = data[r * Nseq : (r + 1) * Nseq, 0, :, 0]
-        recall = recall_sequence[:, 1:].ravel(order="C")
-        k_vector = list(
-            chain(*[list(range(recall_sequence.shape[1] - 1)) for u in range(Nseq)])
-        )
-        deltas = list(chain(*[numpy.diff(schedule.times) for u in range(Nseq)]))
-        optim_kwargs = {"method": "L-BFGS-B", "bounds": [(1e-5, 1e-1), (0, 0.99)]}
-        verbose = False
-        guess = (1e-3, 0.5)
-        (
-            inference_results,
-            I,
-            CI_alpha,
-            CI_beta,
-        ) = identify_alpha_beta_from_recall_sequence(
-            recall,
-            deltas,
-            optim_kwargs=optim_kwargs,
-            verbose=verbose,
-            guess=guess,
-            k_vector=k_vector,
-        )
-        results[:6, r] = *inference_results.x, *CI_alpha, *CI_beta
-        new_I, CI_alpha, CI_beta = delta_method_log_CI(*inference_results.x, I)
-        results[6:, r] = (*CI_alpha,)
-    return results, new_I
 
 
-def ef_get_sequence_observed_information_matrix(recall_sequence, deltas, alpha, beta):
+def ef_get_sequence_observed_information_matrix(
+    recall_sequence, deltas, alpha, beta, k_vector=None
+):
     """ef_get_sequence_observed_information_matrix _summary_
 
-    Returns the observed information matrix J divided by N the number of observations.
-    Asymptotically, J/N converges to the fischer information matrix, which we can use to create confidence intervals.
+    Returns the observed information matrix J.
+
 
     :param recall_sequence: _description_
     :type recall_sequence: _type_
     :param time_sequence: _description_
     :type time_sequence: _type_
     :param alpha: _description_
     :type alpha: _type_
@@ -206,69 +134,87 @@
     :raises ValueError: _description_
     :return: _description_
     :rtype: _type_
     """
     J_11 = 0
     J_12 = 0
     J_22 = 0
-    for n, (recall, delta) in enumerate(zip(recall_sequence, deltas)):
+    if k_vector is None:
+        k_vector = list(range(1, len(deltas)))
+
+    # print(recall_sequence, deltas, k_vector)
+    for recall, delta, k in zip(recall_sequence, deltas, k_vector):
+        # print(recall, delta, k)
         if recall == 1:
-            J_11 += ef_ddq1_dalpha_dalpha_sample(alpha, beta, n, delta)
-            J_12 += ef_ddq1_dalpha_dbeta_sample(alpha, beta, n, delta)
-            J_22 += ef_ddq1_dbeta_dbeta_sample(alpha, beta, n, delta)
+            J_11 += ef_ddq1_dalpha_dalpha_sample(alpha, beta, k, delta)
+            J_12 += ef_ddq1_dalpha_dbeta_sample(alpha, beta, k, delta)
+            J_22 += ef_ddq1_dbeta_dbeta_sample(alpha, beta, k, delta)
         elif recall == 0:
-            J_11 += ef_ddq0_dalpha_dalpha_sample(alpha, beta, n, delta)
-            J_12 += ef_ddq0_dalpha_dbeta_sample(alpha, beta, n, delta)
-            J_22 += ef_ddq0_dbeta_dbeta_sample(alpha, beta, n, delta)
+            J_11 += ef_ddq0_dalpha_dalpha_sample(alpha, beta, k, delta)
+            J_12 += ef_ddq0_dalpha_dbeta_sample(alpha, beta, k, delta)
+            J_22 += ef_ddq0_dbeta_dbeta_sample(alpha, beta, k, delta)
         else:
             raise ValueError(f"recall is not either 1 or 0, but is {recall}")
 
     J = -numpy.array([[J_11, J_12], [J_12, J_22]])
-    return numpy.linalg.inv(J), J, n
+    return J, len(deltas)
 
 
 def delta_method_log_CI(alpha, beta, var):
+    """var should be inverse of J observed information matrix
+    """
     grad = numpy.array([[1 / alpha / numpy.log(10), 0], [0, 1]])
-
     new_var = grad.T @ var @ grad
     CI_alpha_low, CI_alpha_high, CI_beta_low, CI_beta_high = _CI_asymptotical(
-        numpy.log10(alpha), beta, new_var
+        numpy.log10(alpha), beta, new_var[0,0], new_var[1,1]
     )
 
     return new_var, (CI_alpha_low, CI_alpha_high), (CI_beta_low, CI_beta_high)
 
 
-def _CI_asymptotical(alpha, beta, var):
+def _CI_asymptotical(alpha, beta, inv_J_00, inv_J_11, critical_value=1.96):
     with numpy.errstate(invalid="raise"):
         try:
-            CI_alpha_low = alpha - 1.96 * numpy.sqrt(var[0, 0])
-            CI_alpha_high = alpha + 1.96 * numpy.sqrt(var[0, 0])
+            CI_alpha_low = alpha - critical_value * numpy.sqrt(inv_J_00)
+            CI_alpha_high = alpha + critical_value * numpy.sqrt(inv_J_00)
         except FloatingPointError:
             CI_alpha_low = numpy.nan
             CI_alpha_high = numpy.nan
+
         try:
-            CI_beta_low = beta - 1.96 * numpy.sqrt(var[1, 1])
-            CI_beta_high = beta + 1.96 * numpy.sqrt(var[1, 1])
+            CI_beta_low = beta - critical_value * numpy.sqrt(inv_J_11)
+            CI_beta_high = beta + critical_value * numpy.sqrt(inv_J_11)
         except FloatingPointError:
             CI_beta_low = numpy.nan
             CI_beta_high = numpy.nan
-    return CI_alpha_low, CI_alpha_high, CI_beta_low, CI_beta_high
 
+    return CI_alpha_low, CI_alpha_high, CI_beta_low, CI_beta_high
 
-def get_confidence_single(recall_sequence, deltas, alpha, beta, verbose=True):
 
-    I, J, n = ef_get_sequence_observed_information_matrix(
-        recall_sequence, deltas, alpha, beta
+def observed_information_matrix(recall_sequence, deltas, alpha, beta, k_vector=None):
+    J, n = ef_get_sequence_observed_information_matrix(
+        recall_sequence, deltas, alpha, beta, k_vector=k_vector
     )
+    return J
 
+def get_confidence_single(
+    J, level=0.05, verbose=True
+):
+    
+
+    inv_J = numpy.linalg.inv(J)
+
+    if level != 0.05:
+        raise NotImplementedError
     CI_alpha_low, CI_alpha_high, CI_beta_low, CI_beta_high = _CI_asymptotical(
-        alpha, beta, I
+        alpha, beta, inv_J[0, 0], inv_J[1, 1], critical_value=1.96
     )
 
     if verbose:
         print(f"N observations: {n}")
-        print(f"Observed Information Matrix: {I}")
+        print(f"Observed Information Matrix: {inv_J}")
         print("Asymptotic confidence intervals (only valid for large N)")
         print(f"alpha: [{CI_alpha_low:.3e}, {CI_alpha_high:.3e}]")
         print(f"beta: [{CI_beta_low:.3e}, {CI_beta_high:.3e}]")
 
-    return I, J, (CI_alpha_low, CI_alpha_high), (CI_beta_low, CI_beta_high)
+    return J, (CI_alpha_low, CI_alpha_high), (CI_beta_low, CI_beta_high)
+
```

### Comparing `imlmlib-0.0.2.dev0/pyproject.toml` & `imlmlib-0.0.3.dev0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [tool.poetry]
 name = "imlmlib"
-version = "0.0.2-dev0"
+version = "0.0.3-dev0"
 description = "Utilities for parametric modeling of interaction modalities that leverage memory"
 authors = ["jgori <juliengori@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 numpy = "^1.24.2"
 scipy = "^1.10.1"
 matplotlib = "^3.7.1"
 tqdm = "^4.65.0"
+seaborn = "^0.12.2"
+statsmodels = "^0.14.0"
+arviz = "^0.15.1"
+pymc = "^5.6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.2"
 bumpversion = "^0.6.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools>=45", "wheel", "setuptools_scm>=6.2"]
```

### Comparing `imlmlib-0.0.2.dev0/setup.py` & `imlmlib-0.0.3.dev0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 packages = \
 ['imlmlib']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['matplotlib>=3.7.1,<4.0.0',
+['arviz>=0.15.1,<0.16.0',
+ 'matplotlib>=3.7.1,<4.0.0',
  'numpy>=1.24.2,<2.0.0',
+ 'pymc>=5.6.0,<6.0.0',
  'scipy>=1.10.1,<2.0.0',
+ 'seaborn>=0.12.2,<0.13.0',
+ 'statsmodels>=0.14.0,<0.15.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'imlmlib',
-    'version': '0.0.2.dev0',
+    'version': '0.0.3.dev0',
     'description': 'Utilities for parametric modeling of interaction modalities that leverage memory',
     'long_description': None,
     'author': 'jgori',
     'author_email': 'juliengori@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `imlmlib-0.0.2.dev0/PKG-INFO` & `imlmlib-0.0.3.dev0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: imlmlib
-Version: 0.0.2.dev0
+Version: 0.0.3.dev0
 Summary: Utilities for parametric modeling of interaction modalities that leverage memory
 License: MIT
 Author: jgori
 Author-email: juliengori@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: arviz (>=0.15.1,<0.16.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: pymc (>=5.6.0,<6.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
+Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
```

