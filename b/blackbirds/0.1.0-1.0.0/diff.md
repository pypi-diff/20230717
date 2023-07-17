# Comparing `tmp/blackbirds-0.1.0.tar.gz` & `tmp/blackbirds-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackbirds-0.1.0.tar", last modified: Mon Jul  3 10:58:13 2023, max compression
+gzip compressed data, was "blackbirds-1.0.0.tar", last modified: Mon Jul 17 13:30:53 2023, max compression
```

## Comparing `blackbirds-0.1.0.tar` & `blackbirds-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-07-03 10:58:13.549454 blackbirds-0.1.0/
--rw-r--r--   0 arnull     (504) staff       (20)     1077 2023-05-11 09:09:43.000000 blackbirds-0.1.0/LICENSE
--rw-r--r--   0 arnull     (504) staff       (20)       25 2023-06-15 14:47:56.000000 blackbirds-0.1.0/MANIFEST.in
--rw-r--r--   0 arnull     (504) staff       (20)      782 2023-07-03 10:58:13.549304 blackbirds-0.1.0/PKG-INFO
--rw-r--r--   0 arnull     (504) staff       (20)      440 2023-06-15 14:47:04.000000 blackbirds-0.1.0/README.md
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-07-03 10:58:13.546593 blackbirds-0.1.0/blackbirds/
--rw-r--r--   0 arnull     (504) staff       (20)       22 2023-05-16 15:58:40.000000 blackbirds-0.1.0/blackbirds/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)    10635 2023-07-03 10:29:19.000000 blackbirds-0.1.0/blackbirds/calibrator.py
--rw-r--r--   0 arnull     (504) staff       (20)    14699 2023-07-03 10:29:21.000000 blackbirds-0.1.0/blackbirds/forecast.py
--rw-r--r--   0 arnull     (504) staff       (20)     2622 2023-05-11 13:14:22.000000 blackbirds-0.1.0/blackbirds/jacfwd.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-07-03 10:58:13.548288 blackbirds-0.1.0/blackbirds/models/
--rw-r--r--   0 arnull     (504) staff       (20)       25 2023-05-20 14:25:23.000000 blackbirds-0.1.0/blackbirds/models/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)     1391 2023-07-03 10:29:22.000000 blackbirds-0.1.0/blackbirds/models/autoregressive.py
--rw-r--r--   0 arnull     (504) staff       (20)     1924 2023-07-03 10:29:23.000000 blackbirds-0.1.0/blackbirds/models/brock_hommes.py
--rw-r--r--   0 arnull     (504) staff       (20)     2493 2023-07-03 10:29:27.000000 blackbirds-0.1.0/blackbirds/models/june.py
--rw-r--r--   0 arnull     (504) staff       (20)     1854 2023-06-16 15:55:21.000000 blackbirds-0.1.0/blackbirds/models/model.py
--rw-r--r--   0 arnull     (504) staff       (20)     2806 2023-07-03 10:29:29.000000 blackbirds-0.1.0/blackbirds/models/rama_cont.py
--rw-r--r--   0 arnull     (504) staff       (20)     1500 2023-07-03 10:43:02.000000 blackbirds-0.1.0/blackbirds/models/random_walk.py
--rw-r--r--   0 arnull     (504) staff       (20)     5172 2023-07-03 10:29:31.000000 blackbirds-0.1.0/blackbirds/models/sir.py
--rw-r--r--   0 arnull     (504) staff       (20)        0 2023-05-18 09:18:10.000000 blackbirds-0.1.0/blackbirds/models/stochastic_volatility.py
--rw-r--r--   0 arnull     (504) staff       (20)      195 2023-05-16 15:58:40.000000 blackbirds-0.1.0/blackbirds/mpi_setup.py
--rw-r--r--   0 arnull     (504) staff       (20)      965 2023-06-15 14:30:53.000000 blackbirds-0.1.0/blackbirds/posterior_estimators.py
--rw-r--r--   0 arnull     (504) staff       (20)     1582 2023-07-03 10:29:33.000000 blackbirds-0.1.0/blackbirds/regularisation.py
--rw-r--r--   0 arnull     (504) staff       (20)      561 2023-05-16 15:58:40.000000 blackbirds-0.1.0/blackbirds/utils.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-07-03 10:58:13.547178 blackbirds-0.1.0/blackbirds.egg-info/
--rw-r--r--   0 arnull     (504) staff       (20)      782 2023-07-03 10:58:13.000000 blackbirds-0.1.0/blackbirds.egg-info/PKG-INFO
--rw-r--r--   0 arnull     (504) staff       (20)      877 2023-07-03 10:58:13.000000 blackbirds-0.1.0/blackbirds.egg-info/SOURCES.txt
--rw-r--r--   0 arnull     (504) staff       (20)        1 2023-07-03 10:58:13.000000 blackbirds-0.1.0/blackbirds.egg-info/dependency_links.txt
--rw-r--r--   0 arnull     (504) staff       (20)      108 2023-07-03 10:58:13.000000 blackbirds-0.1.0/blackbirds.egg-info/requires.txt
--rw-r--r--   0 arnull     (504) staff       (20)       11 2023-07-03 10:58:13.000000 blackbirds-0.1.0/blackbirds.egg-info/top_level.txt
--rw-r--r--   0 arnull     (504) staff       (20)      108 2023-07-03 09:10:56.000000 blackbirds-0.1.0/requirements.txt
--rw-r--r--   0 arnull     (504) staff       (20)       38 2023-07-03 10:58:13.549497 blackbirds-0.1.0/setup.cfg
--rw-r--r--   0 arnull     (504) staff       (20)      921 2023-07-03 10:29:48.000000 blackbirds-0.1.0/setup.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-07-03 10:58:13.549111 blackbirds-0.1.0/test/
--rw-r--r--   0 arnull     (504) staff       (20)     3717 2023-07-03 10:55:37.000000 blackbirds-0.1.0/test/test_calibrator.py
--rw-r--r--   0 arnull     (504) staff       (20)       38 2023-05-16 15:58:55.000000 blackbirds-0.1.0/test/test_example.py
--rw-r--r--   0 arnull     (504) staff       (20)     5428 2023-07-03 10:29:54.000000 blackbirds-0.1.0/test/test_forecast.py
--rw-r--r--   0 arnull     (504) staff       (20)      549 2023-07-03 10:29:54.000000 blackbirds-0.1.0/test/test_jacfwd.py
--rw-r--r--   0 arnull     (504) staff       (20)      837 2023-07-03 10:29:55.000000 blackbirds-0.1.0/test/test_posterior_estimators.py
--rw-r--r--   0 arnull     (504) staff       (20)      890 2023-07-03 10:29:55.000000 blackbirds-0.1.0/test/test_regularisation.py
--rw-r--r--   0 arnull     (504) staff       (20)      510 2023-07-03 10:29:56.000000 blackbirds-0.1.0/test/test_utils.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-07-17 13:30:53.719943 blackbirds-1.0.0/
+-rw-r--r--   0 arnull     (504) staff       (20)     1077 2023-05-11 09:09:43.000000 blackbirds-1.0.0/LICENSE
+-rw-r--r--   0 arnull     (504) staff       (20)       25 2023-06-15 14:47:56.000000 blackbirds-1.0.0/MANIFEST.in
+-rw-r--r--   0 arnull     (504) staff       (20)     3352 2023-07-17 13:30:53.719808 blackbirds-1.0.0/PKG-INFO
+-rw-r--r--   0 arnull     (504) staff       (20)     3009 2023-07-14 13:04:09.000000 blackbirds-1.0.0/README.md
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-07-17 13:30:53.717015 blackbirds-1.0.0/blackbirds/
+-rw-r--r--   0 arnull     (504) staff       (20)       22 2023-07-03 12:49:29.000000 blackbirds-1.0.0/blackbirds/__init__.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-07-17 13:30:53.718055 blackbirds-1.0.0/blackbirds/infer/
+-rw-r--r--   0 arnull     (504) staff       (20)       69 2023-07-13 15:27:12.000000 blackbirds-1.0.0/blackbirds/infer/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)    10237 2023-07-13 15:27:15.000000 blackbirds-1.0.0/blackbirds/infer/mcmc.py
+-rw-r--r--   0 arnull     (504) staff       (20)     2644 2023-07-13 15:27:12.000000 blackbirds-1.0.0/blackbirds/infer/smd.py
+-rw-r--r--   0 arnull     (504) staff       (20)    22524 2023-07-13 15:27:15.000000 blackbirds-1.0.0/blackbirds/infer/vi.py
+-rw-r--r--   0 arnull     (504) staff       (20)     2622 2023-07-03 12:49:29.000000 blackbirds-1.0.0/blackbirds/jacfwd.py
+-rw-r--r--   0 arnull     (504) staff       (20)     4108 2023-07-14 12:23:40.000000 blackbirds-1.0.0/blackbirds/losses.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-07-17 13:30:53.719093 blackbirds-1.0.0/blackbirds/models/
+-rw-r--r--   0 arnull     (504) staff       (20)       25 2023-07-03 12:49:29.000000 blackbirds-1.0.0/blackbirds/models/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1928 2023-07-03 12:49:29.000000 blackbirds-1.0.0/blackbirds/models/brock_hommes.py
+-rw-r--r--   0 arnull     (504) staff       (20)     2493 2023-07-03 12:49:29.000000 blackbirds-1.0.0/blackbirds/models/june.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1854 2023-07-03 12:49:29.000000 blackbirds-1.0.0/blackbirds/models/model.py
+-rw-r--r--   0 arnull     (504) staff       (20)      576 2023-07-13 15:27:15.000000 blackbirds-1.0.0/blackbirds/models/normal.py
+-rw-r--r--   0 arnull     (504) staff       (20)     2885 2023-07-03 12:49:29.000000 blackbirds-1.0.0/blackbirds/models/rama_cont.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1511 2023-07-13 15:27:12.000000 blackbirds-1.0.0/blackbirds/models/random_walk.py
+-rw-r--r--   0 arnull     (504) staff       (20)     5183 2023-07-13 15:27:12.000000 blackbirds-1.0.0/blackbirds/models/sir.py
+-rw-r--r--   0 arnull     (504) staff       (20)        0 2023-07-03 12:49:29.000000 blackbirds-1.0.0/blackbirds/models/stochastic_volatility.py
+-rw-r--r--   0 arnull     (504) staff       (20)      195 2023-07-03 12:49:29.000000 blackbirds-1.0.0/blackbirds/mpi_setup.py
+-rw-r--r--   0 arnull     (504) staff       (20)      965 2023-07-03 12:49:29.000000 blackbirds-1.0.0/blackbirds/posterior_estimators.py
+-rw-r--r--   0 arnull     (504) staff       (20)     3354 2023-07-13 15:27:12.000000 blackbirds-1.0.0/blackbirds/simulate.py
+-rw-r--r--   0 arnull     (504) staff       (20)      561 2023-07-03 12:49:29.000000 blackbirds-1.0.0/blackbirds/utils.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-07-17 13:30:53.717604 blackbirds-1.0.0/blackbirds.egg-info/
+-rw-r--r--   0 arnull     (504) staff       (20)     3352 2023-07-17 13:30:53.000000 blackbirds-1.0.0/blackbirds.egg-info/PKG-INFO
+-rw-r--r--   0 arnull     (504) staff       (20)      884 2023-07-17 13:30:53.000000 blackbirds-1.0.0/blackbirds.egg-info/SOURCES.txt
+-rw-r--r--   0 arnull     (504) staff       (20)        1 2023-07-17 13:30:53.000000 blackbirds-1.0.0/blackbirds.egg-info/dependency_links.txt
+-rw-r--r--   0 arnull     (504) staff       (20)      125 2023-07-17 13:30:53.000000 blackbirds-1.0.0/blackbirds.egg-info/requires.txt
+-rw-r--r--   0 arnull     (504) staff       (20)       11 2023-07-17 13:30:53.000000 blackbirds-1.0.0/blackbirds.egg-info/top_level.txt
+-rw-r--r--   0 arnull     (504) staff       (20)      125 2023-07-03 11:52:04.000000 blackbirds-1.0.0/requirements.txt
+-rw-r--r--   0 arnull     (504) staff       (20)       38 2023-07-17 13:30:53.719977 blackbirds-1.0.0/setup.cfg
+-rw-r--r--   0 arnull     (504) staff       (20)      922 2023-07-17 13:30:50.000000 blackbirds-1.0.0/setup.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-07-17 13:30:53.719636 blackbirds-1.0.0/test/
+-rw-r--r--   0 arnull     (504) staff       (20)      549 2023-07-03 12:49:29.000000 blackbirds-1.0.0/test/test_jacfwd.py
+-rw-r--r--   0 arnull     (504) staff       (20)     2347 2023-07-14 12:23:40.000000 blackbirds-1.0.0/test/test_losses.py
+-rw-r--r--   0 arnull     (504) staff       (20)      837 2023-07-03 12:49:29.000000 blackbirds-1.0.0/test/test_posterior_estimators.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1642 2023-07-13 15:27:12.000000 blackbirds-1.0.0/test/test_simulate.py
+-rw-r--r--   0 arnull     (504) staff       (20)      510 2023-07-03 12:49:29.000000 blackbirds-1.0.0/test/test_utils.py
```

### Comparing `blackbirds-0.1.0/LICENSE` & `blackbirds-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blackbirds-0.1.0/blackbirds/calibrator.py` & `blackbirds-1.0.0/blackbirds/infer/mcmc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,231 +1,278 @@
+from abc import ABC, abstractmethod
+import logging
 import numpy as np
-from copy import deepcopy
 import torch
-from torch.utils.tensorboard import SummaryWriter
-from tqdm import tqdm
-import logging
-from collections import defaultdict
-from typing import Callable, List
+from tqdm import trange
+from typing import Callable
 
-from blackbirds.mpi_setup import mpi_rank
-from blackbirds.models.model import Model
-from blackbirds.regularisation import compute_regularisation_loss
-from blackbirds.forecast import compute_and_differentiate_forecast_loss
+logger = logging.getLogger("mcmc")
 
-logger = logging.getLogger("calibrator")
+class MCMCKernel(ABC):
 
-
-class Calibrator:
     """
-    Class that handles the training of the posterior_estimator given the model, data, and prior.
+    Abstract base class for MCMC kernels. These kernels specify how to sample the next step in
+    a generic MCMC chain.
 
-    **Arguments:**
+    **Arguments**
 
-    - `model`: The simulator model.
-    - `prior`: The prior distribution.
-    - `posterior_estimator`: The variational distribution that approximates the generalised posterior.
-    - `data`: The observed data to calibrate against. It must be given as a list of tensors that matches the output of the model.
-    - `w`: The weight of the regularisation loss in the total loss.
-    - `initialize_flow_to_prior`: Whether to fit the posterior estimator to the prior before training the forecast term.
-    - `initialization_lr`: The learning rate to use for the initialization.
+    - `prior`: The prior distribution. Must be differentiable in its argument.
+    - `w`: The weight hyperparameter in generalised posterior.
     - `gradient_clipping_norm`: The norm to which the gradients are clipped.
-    - `forecast_loss`: The loss function to use for the forecast loss.
-    - `optimizer`: The optimizer to use for training.
-    - `n_samples_per_epoch`: The number of samples to draw from the variational distribution per epoch.
-    - `n_samples_regularisation`: The number of samples used to evaluate the regularisation loss.
+    - `loss`: The loss function used in the exponent of the generalised likelihood term. Maps from data and chain state to loss.
     - `diff_mode`: The differentiation mode to use. Can be either 'reverse' or 'forward'.
-    - `gradient_estimation_method`: The method to use for estimating the gradients of the forecast loss. Can be either 'pathwise' or 'score'.
-    - `jacobian_chunk_size` : The number of rows computed at a time for the model Jacobian. Set to None to compute the full Jacobian at once.
+    - `jacobian_chunk_size`: The number of rows computed at a time for the model Jacobian. Set to None to compute the full Jacobian at once.
     - `gradient_horizon`: The number of timesteps to use for the gradient horizon. Set 0 to use the full trajectory.
     - `device`: The device to use for training.
-    - `progress_bar`: Whether to display a progress bar during training.
-    - `progress_info` : Whether to display loss data during training.
-    - `log_tensorboard`: Whether to log tensorboard data.
-    - `tensorboard_log_dir`: The directory to log tensorboard data to.
     """
 
     def __init__(
         self,
-        model: Model,
         prior: torch.distributions.Distribution,
-        posterior_estimator: torch.nn.Module,
-        data: List[torch.Tensor],
-        w: float = 0.0,
-        initialize_flow_to_prior: bool = False,
-        initialization_lr: float = 1e-3,
+        loss: Callable,
+        w: float = 1.0,
         gradient_clipping_norm: float = np.inf,
-        forecast_loss: Callable | None = None,
-        optimizer: torch.optim.Optimizer | None = None,
-        n_samples_per_epoch: int = 10,
-        n_samples_regularisation: int = 10_000,
         diff_mode: str = "reverse",
-        gradient_estimation_method: str = "pathwise",
         jacobian_chunk_size: int | None = None,
-        gradient_horizon: int = 0,
+        gradient_horizon: int = np.inf,
         device: str = "cpu",
-        progress_bar: bool = True,
-        progress_info: bool = True,
-        log_tensorboard: bool = False,
-        tensorboard_log_dir: str | None = None,
+        discretisation_method: str = "e-m",
     ):
-        self.model = model
         self.prior = prior
-        self.posterior_estimator = posterior_estimator
-        self.data = data
         self.w = w
-        self.initialize_flow_to_prior = initialize_flow_to_prior
-        self.initialization_lr = initialization_lr
         self.gradient_clipping_norm = gradient_clipping_norm
-        if forecast_loss is None:
-            forecast_loss = torch.nn.MSELoss()
-        self.forecast_loss = forecast_loss
-        if optimizer is None:
-            optimizer = torch.optim.Adam(posterior_estimator.parameters(), lr=1e-3)
-        self.optimizer = optimizer
-        self.n_samples_per_epoch = n_samples_per_epoch
-        self.n_samples_regularisation = n_samples_regularisation
-        self.progress_bar = progress_bar
-        self.progress_info = progress_info
+        self.loss = loss
         self.diff_mode = diff_mode
-        self.gradient_estimation_method = gradient_estimation_method
         self.jacobian_chunk_size = jacobian_chunk_size
         self.gradient_horizon = gradient_horizon
         self.device = device
-        self.tensorboard_log_dir = tensorboard_log_dir
-        self.log_tensorboard = log_tensorboard
+        self._dim = self._verify_dim()
 
-    def step(self):
+    def _verify_dim(self):
         """
-        Performs one training step.
+        Checks the parameter dimension.
         """
-        if mpi_rank == 0:
-            self.optimizer.zero_grad()
-        # compute and differentiate forecast loss
-        forecast_loss = compute_and_differentiate_forecast_loss(
-            loss_fn=self.forecast_loss,
-            model=self.model,
-            posterior_estimator=self.posterior_estimator,
-            n_samples=self.n_samples_per_epoch,
-            observed_outputs=self.data,
-            diff_mode=self.diff_mode,
-            gradient_estimation_method=self.gradient_estimation_method,
-            jacobian_chunk_size=self.jacobian_chunk_size,
-            gradient_horizon=self.gradient_horizon,
-            device=self.device,
+        return self.prior.sample((1,)).shape[-1]
+
+    @abstractmethod
+    def step(
+        self,
+        current_state: torch.Tensor,
+        data: torch.Tensor,
+        *args,
+        **kwargs
+    ):
+        pass
+        
+
+class MALA(MCMCKernel):
+    """
+    Class that generates a step in the chain of a Metropolis-Adjusted Langevin Algorithm run.
+
+    **Arguments**
+
+    - `prior`: The prior distribution. Must be differentiable in its argument.
+    - `w`: The weight hyperparameter in generalised posterior.
+    - `gradient_clipping_norm`: The norm to which the gradients are clipped.
+    - `loss`: The loss function used in the exponent of the generalised likelihood term. Maps from data and chain state to loss.
+    - `diff_mode`: The differentiation mode to use. Can be either 'reverse' or 'forward'.
+    - `jacobian_chunk_size`: The number of rows computed at a time for the model Jacobian. Set to None to compute the full Jacobian at once.
+    - `gradient_horizon`: The number of timesteps to use for the gradient horizon. Set 0 to use the full trajectory.
+    - `device`: The device to use for training.
+    - `discretisation_method`: How to discretise the overdamped Langevin diffusion. Default 'e-m' for Euler-Maruyama
+    """
+
+    def __init__(
+        self,
+        *args,
+        discretisation_method: str = "e-m",
+        **kwargs
+    ):
+        super().__init__(*args, **kwargs)
+        self.discretisation_method = discretisation_method
+        self._previous_log_density = None
+        self._previous_grad_theta_of_log_density = None
+        self._proposal = None
+
+    def _compute_log_density_and_grad(self, state, data):
+        _state = state.clone().detach()
+        _state.requires_grad = True
+        ell = self.loss(_state, data)
+        log_prior_pdf = self.prior.log_prob(_state)
+        log_density = -ell + log_prior_pdf * self.w
+        log_density.backward()
+        torch.nn.utils.clip_grad_norm_([_state], self.gradient_clipping_norm)
+        return log_density.detach(), _state.grad
+
+    def initialise_chain(self, state, data):
+        log_density, grad_theta_of_log_density = self._compute_log_density_and_grad(
+            state, data
         )
-        # compute and differentiate regularisation loss
-        if mpi_rank == 0:
-            if self.w != 0.0:
-                regularisation_loss = self.w * compute_regularisation_loss(
-                    posterior_estimator=self.posterior_estimator,
-                    prior=self.prior,
-                    n_samples=self.n_samples_regularisation,
+        self._previous_log_density = log_density
+        self._previous_grad_theta_of_log_density = grad_theta_of_log_density
+        self._proposal = None
+
+    def step(
+        self,
+        current_state,
+        data,
+        scale: float = 1.0,
+        covariance: torch.Tensor | None = None,
+    ):
+        """
+        Returns a (torch.Tensor, bool) pair corresponding to (the current state of the chain, whether
+        the current state resulted from an accept or reject decision in the Metropolis step).
+        """
+
+        if covariance is None:
+            covariance = torch.eye(self._dim)
+        sC = scale * covariance
+        if self._previous_log_density is None:
+            # This would happen if the user hasn't initialised the chain themselves
+            self.initialise_chain(current_state, data)
+        if self.discretisation_method == "e-m":
+            if self._proposal is None:
+                # This would happen if the user hasn't initialised the chain themselves
+                gradient_term = torch.matmul(
+                    sC, self._previous_grad_theta_of_log_density
                 )
-                # differentiate regularisation
-                regularisation_loss.backward()
-            else:
-                regularisation_loss = torch.zeros(1, device=forecast_loss.device)
-            # clip gradients
-            torch.nn.utils.clip_grad_norm_(
-                self.posterior_estimator.parameters(), self.gradient_clipping_norm
-            )
-            self.optimizer.step()
-            loss = forecast_loss + regularisation_loss
-            return loss, forecast_loss, regularisation_loss
-        return None, None, None
-
-    def initialize_flow(self, max_epochs_without_improvement=50, atol=1e-2):
-        """
-        Initialization step where the flow is fitted to just the prior.
-        """
-        epoch = 0
-        if mpi_rank == 0:
-            optimizer = torch.optim.Adam(
-                self.posterior_estimator.parameters(), lr=self.initialization_lr
-            )
-            best_loss = torch.tensor(np.inf)
-            while True:
-                optimizer.zero_grad()
-                loss = compute_regularisation_loss(
-                    posterior_estimator=self.posterior_estimator,
-                    prior=self.prior,
-                    n_samples=self.n_samples_regularisation,
+                mean = current_state + gradient_term
+                logger.debug("Total mean =", mean)
+                logger.debug("Gradient_term =", gradient_term)
+                proposal = torch.distributions.multivariate_normal.MultivariateNormal(
+                    mean, covariance_matrix=2 * sC
                 )
-                if self.log_tensorboard:
-                    self.writer.add_scalar("Loss/init_loss", loss, epoch)
-                loss.backward()
-                optimizer.step()
-                if loss < best_loss:
-                    best_loss = loss.item()
-                    num_epochs_without_improvement = 0
-                else:
-                    num_epochs_without_improvement += 1
-                if (
-                    num_epochs_without_improvement >= max_epochs_without_improvement
-                    or (loss.abs().item() < atol)
-                ):
-                    break
-                epoch += 1
-
-    def run(self, n_epochs, max_epochs_without_improvement=20):
-        """
-        Runs the calibrator for {n_epochs} epochs. Stops if the loss does not improve for {max_epochs_without_improvement} epochs.
-
-        Arguments:
-            n_epochs (int | np.inf): The number of epochs to run the calibrator for.
-            max_epochs_without_improvement (int): The number of epochs without improvement after which the calibrator stops.
-        """
-        if mpi_rank == 0 and self.log_tensorboard:
-            self.writer = SummaryWriter(log_dir=self.tensorboard_log_dir)
-        if self.initialize_flow_to_prior:
-            self.initialize_flow()
-            torch.save(self.posterior_estimator.state_dict(), "model_fit_to_prior.pt")
-        self.best_loss = torch.tensor(np.inf)
-        self.best_model_state_dict = None
-        num_epochs_without_improvement = 0
-        iterator = range(n_epochs)
-        if self.progress_bar and mpi_rank == 0:
-            iterator = tqdm(iterator)
-        self.losses_hist = defaultdict(list)
-        for epoch in iterator:
-            loss, forecast_loss, regularisation_loss = self.step()
-            if mpi_rank == 0:
-                self.losses_hist["total"].append(loss.item())
-                self.losses_hist["forecast"].append(forecast_loss.item())
-                self.losses_hist["regularisation"].append(regularisation_loss.item())
-                if self.log_tensorboard:
-                    self.writer.add_scalar("Loss/total", loss, epoch)
-                    self.writer.add_scalar("Loss/forecast", forecast_loss, epoch)
-                    self.writer.add_scalar(
-                        "Loss/regularisation", regularisation_loss, epoch
-                    )
-                torch.save(self.best_model_state_dict, "last_model.pt")
-                if loss < self.best_loss:
-                    self.best_loss = loss
-                    self.best_model_state_dict = deepcopy(
-                        self.posterior_estimator.state_dict()
+                self._proposal = proposal
+            new_state = self._proposal.sample()
+        else:
+            raise NotImplementedError("Discretisation method not yet implemented")
+
+        (
+            new_log_density,
+            grad_theta_of_new_log_density,
+        ) = self._compute_log_density_and_grad(new_state, data)
+
+        # Metropolis accept/reject step
+        log_alpha = torch.log(torch.rand((1,))[0])
+        # Compute reverse proposal logpdf
+        if self.discretisation_method == "e-m":
+            try:
+                rev_proposal = (
+                    torch.distributions.multivariate_normal.MultivariateNormal(
+                        new_state + torch.matmul(sC, grad_theta_of_new_log_density),
+                        covariance_matrix=2 * sC,
                     )
-                    torch.save(self.best_model_state_dict, "best_model.pt")
-                    num_epochs_without_improvement = 0
-                else:
-                    num_epochs_without_improvement += 1
-                if self.progress_bar and self.progress_info:
+                )
+            except ValueError as e:
+                logger.debug(new_state, grad_theta_of_new_log_density)
+                raise e
+        else:
+            raise NotImplementedError("Discretisation method not yet implemented")
+        log_accept_prob = (
+            new_log_density
+            + rev_proposal.log_prob(current_state)
+            - self._previous_log_density
+            - self._proposal.log_prob(new_state)
+        )
+        logger.debug("Current, new:", current_state, new_state)
+        logger.debug(
+            "Lalpha",
+            log_accept_prob.item(),
+            " = ",
+            new_log_density.item(),
+            "+",
+            rev_proposal.log_prob(current_state).item(),
+            "-",
+            self._previous_log_density.item(),
+            "-",
+            self._proposal.log_prob(new_state).item(),
+        )
+        logger.debug("")
+        accept = log_alpha < log_accept_prob
+        if accept:
+            self._previous_log_density = new_log_density
+            self._previous_grad_theta_of_log_density = grad_theta_of_new_log_density
+            self._proposal = rev_proposal
+            return new_state, True
+        return current_state, False
+
+
+class MCMC:
+    """
+    Class that runs an MCMC chain.
+
+    **Arguments**
+
+    - `kernel`: An object with a .step() method that is used to generate the next sample in the chain.
+    - `num_samples`: An integer specifying the number of samples to generate in the MCMC chain.
+    - `progress_bar`: Whether to display a progress bar during training.
+    - `progress_info`: Whether to display loss data during training.
+    """
+
+    def __init__(
+        self,
+        kernel: MCMCKernel,
+        num_samples: int = 100_000,
+        progress_bar: bool = True,
+        progress_info: bool = True,
+    ):
+        self.kernel = kernel
+        self.num_samples = num_samples
+        self.progress_bar = progress_bar
+        self.progress_info = progress_info
+        # I suppose just in case something stops the program and you want to save the samples?
+        self._samples = []
+
+    def reset(self):
+        self._samples = []
+
+    def run(
+        self,
+        initial_state: torch.Tensor, 
+        data: torch.Tensor, 
+        *args, 
+        seed: int = 0,
+        T: int = 1, 
+        **kwargs
+    ):
+
+        """
+        Runs the MCMC chain.
+
+        **Arguments**
+
+        - `initial_state`: Starting location of the MCMC chain.
+        - `data`: A torch.Tensor containing the data against which the simulator is compared.
+        - `seed`: An integer specifying the initial random state of the RNG.
+        - `T`: An integer specifying the number of steps between updates of the progress info (if shown).
+
+        Additional arguments and keyword arguments can be passed, which will be passed to the kernel 
+        .step() method.
+        """
+
+        assert isinstance(initial_state, torch.Tensor), "Initial state of the MCMC chain must be a torch.Tensor"
+        assert isinstance(data, torch.Tensor), "The data must be passed as a torch.Tensor"
+
+        if seed is not None:
+            torch.manual_seed(seed)
+        self.reset()
+
+        if self.progress_bar:
+            iterator = trange(self.num_samples)
+        else:
+            iterator = range(self.num_samples)
+
+        self._samples.append(initial_state)
+        state = initial_state
+        if self.progress_info:
+            total_accepted = 0
+        for t in iterator:
+            state, accept_step = self.kernel.step(state, data, *args, **kwargs)
+            self._samples.append(state)
+            if self.progress_info:
+                if accept_step:
+                    total_accepted += 1
+                if t % T == 0:
                     iterator.set_postfix(
-                        {
-                            "Forecast": forecast_loss.item(),
-                            "Reg.": regularisation_loss.item(),
-                            "total": loss.item(),
-                            "best loss": self.best_loss.item(),
-                            "epochs since improv.": num_epochs_without_improvement,
-                        }
-                    )
-                if num_epochs_without_improvement >= max_epochs_without_improvement:
-                    logger.info(
-                        "Stopping early because the loss did not improve for {} epochs.".format(
-                            max_epochs_without_improvement
-                        )
+                        {"Acceptance rate": float(total_accepted) / (t + 1.0)}
                     )
-                    break
-        if mpi_rank == 0 and self.log_tensorboard:
-            self.writer.flush()
-            self.writer.close()
+        return self._samples
```

### Comparing `blackbirds-0.1.0/blackbirds/forecast.py` & `blackbirds-1.0.0/blackbirds/infer/vi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,65 @@
-import torch
 import numpy as np
-import warnings
-from typing import Callable
+import torch
+import logging
+from tqdm import tqdm
+from copy import deepcopy
 from itertools import chain
+from typing import Callable, List
+from collections import defaultdict
+from torch.utils.tensorboard import SummaryWriter
 
-from blackbirds.mpi_setup import mpi_size, mpi_rank, mpi_comm
+from blackbirds.mpi_setup import mpi_rank
 from blackbirds.jacfwd import jacfwd
+from blackbirds.mpi_setup import mpi_size, mpi_rank, mpi_comm
 
+logger = logging.getLogger("vi")
 
-def simulate_and_observe_model(
-    model: torch.nn.Module,
-    params: torch.Tensor,
-    gradient_horizon: int | None = None,
-):
-    """Runs the simulator for the given parameters and calls the model's observe method.
-    To avoid gradient instabilities, the `gradient_horizon` argument limits the number of past time-steps
-    that are taken into account for the gradient's calculation. That is, if `gradient_horizon` is 10, then
-    only the last 10 time-steps are used to calculate the gradient.
-
-    **Arguments:**
-
-    - `model`: A torch.nn.Module implemnting the `initialize`, `forward` and `observe` methods.
-    - `params`: The parameters taken by the model's `forward` method.
-    - `n_timesteps`: Number of timesteps to simulate.
-    - `gradient_horizon`: Gradient window, if None then all time-steps are used to calculate the gradient.
-    """
-    if gradient_horizon is None:
-        gradient_horizon = model.n_timesteps
-    # Initialize the model
-    time_series = model.initialize(params)
-    observed_outputs = model.observe(time_series)
-    for t in range(model.n_timesteps):
-        time_series = model.trim_time_series(
-            time_series
-        )  # gets past time-steps needed to compute the next one.
-        # only consider the past gradient_horizon time-steps to calculate the gradient
-        if t > gradient_horizon:
-            time_series = model.detach_gradient_horizon(time_series, gradient_horizon)
-        x = model(params, time_series)
-        observed_outputs = [
-            torch.cat((observed_output, output))
-            for observed_output, output in zip(observed_outputs, model.observe(x))
-        ]
-        time_series = torch.cat((time_series, x))
-    return observed_outputs
 
+def compute_regularisation_loss(
+    posterior_estimator: torch.nn.Module,
+    prior: torch.distributions.Distribution,
+    n_samples: int,
+):
+    r"""Estimates the KL divergence between the posterior and the prior using n_samples through Monte Carlo using
 
-def compute_loss(
-    loss_fn: Callable,
-    observed_outputs: list[torch.Tensor],
-    simulated_outputs: list[torch.Tensor],
-) -> torch.Tensor:
-    """Compute the loss between observed and simulated outputs.
+    $$
+    \mathbb{E}_{q(z|x)}[\log q(z|x) - \log p(z)] \approx \frac{1}{N} \sum_{i=1}^N \left(\log q(z_i|x) - \log p(z_i)\right)
+    $$
 
-    **Arguments:**
+    **Arguments**:
 
-    - loss_fn : loss function
-    - observed_outputs : list of data tensors to calibrate to
-    - simulated_outputs: list of simulated outputs
+    - `posterior_estimator`: The posterior distribution.
+    - `prior`: The prior distribution.
+    - `n_samples`: The number of samples to use for the Monte Carlo estimate.
 
     !!! example
         ```python
-        loss_fn = torch.nn.MSELoss()
-        observed_outputs = [torch.tensor([1, 2, 3]), torch.tensor([4, 5, 6])]
-        simulated_outputs = [torch.tensor([1, 2, 3]), torch.tensor([4, 5, 6])]
-        compute_loss(loss_fn, observed_outputs, simulated_outputs) # tensor(0.)
+            import torch
+            from blackbirds.regularisation import compute_regularisation
+            # define two normal distributions
+            dist1 = torch.distributions.Normal(0, 1)
+            dist2 = torch.distributions.Normal(0, 1)
+            compute_regularisation(dist1, dist2, 1000)
+            # tensor(0.)
+            dist1 = torch.distributions.Normal(0, 1)
+            dist2 = torch.distributions.Normal(1, 1)
+            compute_regularisation(dist1, dist2, 1000)
+            # tensor(0.5)
         ```
     """
-    try:
-        assert len(observed_outputs) == len(simulated_outputs)
-    except AssertionError:
-        raise ValueError("Number of observed and simulated outputs must be the same.")
-    loss = 0
-    is_nan = True
-    for observed_output, simulated_output in zip(observed_outputs, simulated_outputs):
-        try:
-            assert observed_output.shape == simulated_output.shape
-        except AssertionError:
-            raise ValueError("Observed and simulated outputs must have the same shape")
-        if torch.isnan(simulated_output).any():
-            warnings.warn("Simulation produced nan -- ignoring")
-            continue
-        loss += loss_fn(simulated_output, observed_output)
-        is_nan = False
-    if is_nan:
-        return torch.tensor(torch.nan), torch.tensor(torch.nan)
-    return loss, loss  # need to return it twice for jac calculation
+    # sample from the posterior
+    z, log_prob_posterior = posterior_estimator.sample(n_samples)
+    # compute the log probability of the samples under the prior
+    # log_prob_posterior = posterior_estimator.log_prob(z)
+    log_prob_prior = prior.log_prob(z)
+    # compute the Monte Carlo estimate of the KL divergence
+    kl_divergence = (log_prob_posterior - log_prob_prior).mean()
+    # kl_divergence = torch.clamp(kl_divergence, min=0.0, max=1)
+    return kl_divergence
 
 
 def _sample_and_scatter_parameters(
     posterior_estimator: Callable,
     n_samples: int,
 ) -> (torch.Tensor, np.ndarray):
     """Sample parameters and scatter them across devices.
@@ -113,36 +83,33 @@
         logprobs_list = None
     # scatter the parameters to all ranks
     if mpi_comm is not None:
         params_list_comm = mpi_comm.bcast(params_list_comm, root=0)
     return params_list, params_list_comm, logprobs_list
 
 
-def _differentiate_forecast_loss_pathwise(forecast_parameters, forecast_jacobians):
+def _differentiate_loss_pathwise(parameters, jacobians):
     """
-    Differentiates forecast loss and regularisation loss through the flows and the simulator.
+    Differentiates loss and regularisation loss through the flows and the simulator.
 
     Arguments:
-        forecast_parameters (List[torch.Tensor]): The parameters of the simulator that are differentiated through.
-        forecast_jacobians (List[torch.Tensor]): The jacobians of the simulator that are differentiated through.
+        parameters (List[torch.Tensor]): The parameters of the simulator that are differentiated through.
+        jacobians (List[torch.Tensor]): The jacobians of the simulator that are differentiated through.
     """
     # then we differentiate the parameters through the flow also tkaing into account the jacobians of the simulator
-    device = forecast_parameters.device
+    device = parameters.device
     to_diff = torch.zeros(1, device=device)
-    for i in range(len(forecast_jacobians)):
-        to_diff += torch.dot(
-            forecast_jacobians[i].to(device), forecast_parameters[i, :]
-        )
-    to_diff = to_diff / len(forecast_jacobians)
+    for i in range(len(jacobians)):
+        to_diff += torch.dot(jacobians[i].to(device), parameters[i, :])
+    to_diff = to_diff / len(jacobians)
     to_diff.backward()
 
 
-def compute_forecast_loss_and_jacobian_pathwise(
+def compute_loss_and_jacobian_pathwise(
     loss_fn: Callable,
-    model: torch.nn.Module,
     posterior_estimator: Callable,
     n_samples: int,
     observed_outputs: list[torch.Tensor],
     diff_mode: str = "reverse",
     jacobian_chunk_size: int | None = None,
     gradient_horizon: int = 0,
     device: str = "cpu",
@@ -161,15 +128,14 @@
 
     The jacobian is computed using the forward or reverse mode differentiation and the computation is parallelized
     across the available devices.
 
     **Arguments:**
 
     - `loss_fn`: loss function
-    - `model`: PyTorch model
     - `posterior_estimator`: Object that implements the `sample` method computing a parameter and its log_prob
     - `n_samples`: number of samples
     - `observed_outputs`: observed outputs
     - `diff_mode`: differentiation mode can be "reverse" or "forward"
     - `jacobian_chunk_size`: chunk size for the Jacobian computation (set None to get maximum chunk size)
     - `gradient_horizon`: horizon for the gradient computation
     - `device`: device to use for the computation
@@ -181,21 +147,20 @@
     # select forward or reverse jacobian calculator
     if diff_mode == "reverse":
         jacobian_diff_mode = torch.func.jacrev
     else:
         jacobian_diff_mode = lambda **kwargs: jacfwd(randomness="same", **kwargs)
 
     # define loss to differentiate
-    def loss_f(params):
-        simulated_outputs = simulate_and_observe_model(model, params, gradient_horizon)
-        loss = compute_loss(loss_fn, observed_outputs, simulated_outputs)
-        return loss
+    def loss_aux(params):
+        loss_v = loss_fn(params, observed_outputs)
+        return loss_v, loss_v  # need double return for jacobian calculation.
 
     jacobian_calculator = jacobian_diff_mode(
-        func=loss_f,
+        func=loss_aux,
         argnums=0,
         has_aux=True,
         chunk_size=jacobian_chunk_size,
     )
     # make each rank compute the loss for its parameters
     loss = 0
     jacobians_per_rank = []
@@ -227,17 +192,16 @@
         parameters = params_list[indices]
         loss = loss / len(parameters)
         return parameters, loss, jacobians
     else:
         return [], 0.0, []
 
 
-def compute_and_differentiate_forecast_loss_score(
+def compute_and_differentiate_loss_score(
     loss_fn: Callable,
-    model: torch.nn.Module,
     posterior_estimator: torch.nn.Module,
     n_samples: int,
     observed_outputs: list[torch.Tensor],
     device: str = "cpu",
 ):
     r"""Computes the loss and the jacobian of the loss for each sample using a differentiable simulator. That is, we compute
 
@@ -253,33 +217,29 @@
 
     The jacobian is computed using the forward or reverse mode differentiation and the computation is parallelized
     across the available devices.
 
     **Arguments:**
 
     - `loss_fn`: loss function
-    - `model`: PyTorch model
     - `posterior_estimator`: posterior estimator, must implement a sample and a log_prob method
     - `n_samples`: number of samples
     - `observed_outputs`: observed outputs
     - `device`: device to use for the computation
     """
     # sample parameters and scatter them across devices
     _, params_list_comm, logprobs_list = _sample_and_scatter_parameters(
         posterior_estimator, n_samples
     )
     # make each rank compute the loss for its parameters
     loss_per_parameter = []
     indices_per_rank = []  # need to keep track of which parameter has which loss
     for i in range(mpi_rank, len(params_list_comm), mpi_size):
         params = torch.tensor(params_list_comm[i], device=device)
-        simulated_outputs = simulate_and_observe_model(
-            model, params, gradient_horizon=0
-        )
-        loss_i, _ = compute_loss(loss_fn, observed_outputs, simulated_outputs)
+        loss_i = loss_fn(params, observed_outputs)
         loss_per_parameter.append(loss_i.detach().cpu().numpy())
         indices_per_rank.append(i)
     # gather the losses from all ranks
     if mpi_size > 1:
         loss_per_parameter = mpi_comm.gather(loss_per_parameter, root=0)
         indices_per_rank = mpi_comm.gather(indices_per_rank, root=0)
     else:
@@ -308,68 +268,278 @@
         total_loss = total_loss / n_samples_non_nan
         # differentiate through the posterior estimator
         to_backprop.backward()
         return total_loss
     return None
 
 
-def compute_and_differentiate_forecast_loss(
+def compute_and_differentiate_loss(
     loss_fn: Callable,
-    model: torch.nn.Module,
     posterior_estimator: torch.nn.Module,
     n_samples: int,
     observed_outputs: list[torch.Tensor],
     diff_mode: str = "reverse",
     gradient_estimation_method: str = "pathwise",
     jacobian_chunk_size: int | None = None,
     gradient_horizon: int = 0,
     device: str = "cpu",
 ):
-    r"""Computes and differentiates the forecast loss according to the chosen gradient estimation method
+    r"""Computes and differentiates the loss according to the chosen gradient estimation method
     and automatic differentiation mechanism.
     **Arguments:**
 
     - `loss_fn`: loss function
-    - `model`: PyTorch model
     - `posterior_estimator`: posterior estimator, must implement a sample and a log_prob method
     - `n_samples`: number of samples
     - `observed_outputs`: observed outputs
     - `diff_mode`: differentiation mode can be "reverse" or "forward"
     - `gradient_estimation_method`: gradient estimation method can be "pathwise" or "score"
     - `jacobian_chunk_size`: chunk size for the Jacobian computation (set None to get maximum chunk size)
     - `gradient_horizon`: horizon for the gradient computation
     - `device`: device to use for the computation
     """
     if gradient_estimation_method == "pathwise":
         (
-            forecast_parameters,
-            forecast_loss,
-            forecast_jacobians,
-        ) = compute_forecast_loss_and_jacobian_pathwise(
+            parameters,
+            loss,
+            jacobians,
+        ) = compute_loss_and_jacobian_pathwise(
             loss_fn=loss_fn,
-            model=model,
             posterior_estimator=posterior_estimator,
             observed_outputs=observed_outputs,
             n_samples=n_samples,
             diff_mode=diff_mode,
             device=device,
             jacobian_chunk_size=jacobian_chunk_size,
             gradient_horizon=gradient_horizon,
         )
         if mpi_rank == 0:
-            _differentiate_forecast_loss_pathwise(
-                forecast_parameters, forecast_jacobians
-            )
+            _differentiate_loss_pathwise(parameters, jacobians)
     elif gradient_estimation_method == "score":
-        forecast_loss = compute_and_differentiate_forecast_loss_score(
+        loss = compute_and_differentiate_loss_score(
             loss_fn=loss_fn,
-            model=model,
             posterior_estimator=posterior_estimator,
             observed_outputs=observed_outputs,
             n_samples=n_samples,
             device=device,
         )
     else:
         raise ValueError(
             f"Unknown gradient estimation method {gradient_estimation_method}."
         )
-    return forecast_loss
+    return loss
+
+
+class VI:
+    """
+    Class to handle (Generalized) Variational Inferece.
+
+    **Arguments:**
+
+    - `loss` : A callable that returns a (differentiable) loss. Needs to take (parameters, data) as input and return a scalar tensor.
+    - `prior`: The prior distribution.
+    - `posterior_estimator`: The variational distribution that approximates the (generalised) posterior.
+    - `w`: The weight of the regularisation loss in the total loss.
+    - `initialize_estimator_to_prior`: Whether to fit the posterior estimator to the prior before training.
+    - `initialization_lr`: The learning rate to use for the initialization.
+    - `gradient_clipping_norm`: The norm to which the gradients are clipped.
+    - `optimizer`: The optimizer to use for training.
+    - `n_samples_per_epoch`: The number of samples to draw from the variational distribution per epoch.
+    - `n_samples_regularisation`: The number of samples used to evaluate the regularisation loss.
+    - `diff_mode`: The differentiation mode to use. Can be either 'reverse' or 'forward'.
+    - `gradient_estimation_method`: The method to use for estimating the gradients of the loss. Can be either 'pathwise' or 'score'.
+    - `jacobian_chunk_size` : The number of rows computed at a time for the model Jacobian. Set to None to compute the full Jacobian at once.
+    - `gradient_horizon`: The number of timesteps to use for the gradient horizon. Set 0 to use the full trajectory.
+    - `device`: The device to use for training.
+    - `progress_bar`: Whether to display a progress bar during training.
+    - `progress_info` : Whether to display loss data during training.
+    - `log_tensorboard`: Whether to log tensorboard data.
+    - `tensorboard_log_dir`: The directory to log tensorboard data to.
+    """
+
+    def __init__(
+        self,
+        loss: Callable,
+        prior: torch.distributions.Distribution,
+        posterior_estimator: torch.nn.Module,
+        w: float = 1.0,
+        initialize_estimator_to_prior: bool = False,
+        initialization_lr: float = 1e-3,
+        gradient_clipping_norm: float = np.inf,
+        optimizer: torch.optim.Optimizer | None = None,
+        n_samples_per_epoch: int = 10,
+        n_samples_regularisation: int = 10_000,
+        diff_mode: str = "reverse",
+        gradient_estimation_method: str = "pathwise",
+        jacobian_chunk_size: int | None = None,
+        gradient_horizon: int | float = np.inf,
+        device: str = "cpu",
+        progress_bar: bool = True,
+        progress_info: bool = True,
+        log_tensorboard: bool = False,
+        tensorboard_log_dir: str | None = None,
+    ):
+        self.loss = loss
+        self.prior = prior
+        self.posterior_estimator = posterior_estimator
+        self.w = w
+        self.initialize_estimator_to_prior = initialize_estimator_to_prior
+        self.initialization_lr = initialization_lr
+        self.gradient_clipping_norm = gradient_clipping_norm
+        if optimizer is None:
+            optimizer = torch.optim.Adam(posterior_estimator.parameters(), lr=1e-3)
+        self.optimizer = optimizer
+        self.n_samples_per_epoch = n_samples_per_epoch
+        self.n_samples_regularisation = n_samples_regularisation
+        self.progress_bar = progress_bar
+        self.progress_info = progress_info
+        self.diff_mode = diff_mode
+        self.gradient_estimation_method = gradient_estimation_method
+        self.jacobian_chunk_size = jacobian_chunk_size
+        self.gradient_horizon = gradient_horizon
+        self.device = device
+        self.tensorboard_log_dir = tensorboard_log_dir
+        self.log_tensorboard = log_tensorboard
+
+    def step(self, data):
+        """
+        Performs one training step.
+        """
+        if mpi_rank == 0:
+            self.optimizer.zero_grad()
+        # compute and differentiate loss
+        loss = compute_and_differentiate_loss(
+            loss_fn=self.loss,
+            posterior_estimator=self.posterior_estimator,
+            n_samples=self.n_samples_per_epoch,
+            observed_outputs=data,
+            diff_mode=self.diff_mode,
+            gradient_estimation_method=self.gradient_estimation_method,
+            jacobian_chunk_size=self.jacobian_chunk_size,
+            gradient_horizon=self.gradient_horizon,
+            device=self.device,
+        )
+        # compute and differentiate regularisation loss
+        if mpi_rank == 0:
+            if self.w != 0.0:
+                regularisation_loss = self.w * compute_regularisation_loss(
+                    posterior_estimator=self.posterior_estimator,
+                    prior=self.prior,
+                    n_samples=self.n_samples_regularisation,
+                )
+                # differentiate regularisation
+                regularisation_loss.backward()
+            else:
+                regularisation_loss = torch.zeros(1, device=loss.device)
+            # clip gradients
+            torch.nn.utils.clip_grad_norm_(
+                self.posterior_estimator.parameters(), self.gradient_clipping_norm
+            )
+            self.optimizer.step()
+            total_loss = loss + regularisation_loss
+            return total_loss, loss, regularisation_loss
+        return None, None, None
+
+    def initialize_estimator(self, max_epochs_without_improvement=50, atol=1e-2):
+        """
+        Initialization step where the estimator is fitted to just the prior.
+        """
+        epoch = 0
+        if mpi_rank == 0:
+            optimizer = torch.optim.Adam(
+                self.posterior_estimator.parameters(), lr=self.initialization_lr
+            )
+            best_loss = torch.tensor(np.inf)
+            while True:
+                optimizer.zero_grad()
+                loss = compute_regularisation_loss(
+                    posterior_estimator=self.posterior_estimator,
+                    prior=self.prior,
+                    n_samples=self.n_samples_regularisation,
+                )
+                if self.log_tensorboard:
+                    self.writer.add_scalar("Loss/init_loss", loss, epoch)
+                loss.backward()
+                optimizer.step()
+                if loss < best_loss:
+                    best_loss = loss.item()
+                    num_epochs_without_improvement = 0
+                else:
+                    num_epochs_without_improvement += 1
+                if (
+                    num_epochs_without_improvement >= max_epochs_without_improvement
+                    or (loss.abs().item() < atol)
+                ):
+                    break
+                epoch += 1
+
+    def run(
+        self,
+        data: List[torch.Tensor],
+        n_epochs: int,
+        max_epochs_without_improvement: int = 20,
+    ):
+        """
+        Runs the calibrator for {n_epochs} epochs. Stops if the loss does not improve for {max_epochs_without_improvement} epochs.
+
+        **Arguments:**
+
+        - `data`: The observed data to calibrate against. It must be given as a list of tensors that matches the output of the model.
+        - `n_epochs`: The number of epochs to run the calibrator for.
+        - `max_epochs_without_improvement`: The number of epochs without improvement after which the calibrator stops.
+        """
+        if mpi_rank == 0 and self.log_tensorboard:
+            self.writer = SummaryWriter(log_dir=self.tensorboard_log_dir)
+        if self.initialize_estimator_to_prior:
+            self.initialize_estimator()
+            torch.save(
+                self.posterior_estimator.state_dict(), "estimator_fit_to_prior.pt"
+            )
+        self.best_loss = torch.tensor(np.inf)
+        self.best_estimator_state_dict = None
+        num_epochs_without_improvement = 0
+        iterator = range(n_epochs)
+        if self.progress_bar and mpi_rank == 0:
+            iterator = tqdm(iterator)
+        self.losses_hist = defaultdict(list)
+        for epoch in iterator:
+            total_loss, loss, regularisation_loss = self.step(data)
+            if mpi_rank == 0:
+                self.losses_hist["total"].append(total_loss.item())
+                self.losses_hist["loss"].append(loss.item())
+                self.losses_hist["regularisation"].append(regularisation_loss.item())
+                if self.log_tensorboard:
+                    self.writer.add_scalar("Loss/total", total_loss, epoch)
+                    self.writer.add_scalar("Loss/loss", loss, epoch)
+                    self.writer.add_scalar(
+                        "Loss/regularisation", regularisation_loss, epoch
+                    )
+                torch.save(self.best_estimator_state_dict, "last_estimator.pt")
+                if loss < self.best_loss:
+                    self.best_loss = loss
+                    self.best_estimator_state_dict = deepcopy(
+                        self.posterior_estimator.state_dict()
+                    )
+                    torch.save(self.best_estimator_state_dict, "best_estimator.pt")
+                    num_epochs_without_improvement = 0
+                else:
+                    num_epochs_without_improvement += 1
+                if self.progress_bar and self.progress_info:
+                    iterator.set_postfix(
+                        {
+                            "loss": loss.item(),
+                            "reg.": regularisation_loss.item(),
+                            "total": total_loss.item(),
+                            "best loss": self.best_loss.item(),
+                            "epochs since improv.": num_epochs_without_improvement,
+                        }
+                    )
+                if num_epochs_without_improvement >= max_epochs_without_improvement:
+                    logger.info(
+                        "Stopping early because the loss did not improve for {} epochs.".format(
+                            max_epochs_without_improvement
+                        )
+                    )
+                    break
+        if mpi_rank == 0 and self.log_tensorboard:
+            self.writer.flush()
+            self.writer.close()
```

### Comparing `blackbirds-0.1.0/blackbirds/jacfwd.py` & `blackbirds-1.0.0/blackbirds/jacfwd.py`

 * *Files identical despite different names*

### Comparing `blackbirds-0.1.0/blackbirds/models/autoregressive.py` & `blackbirds-1.0.0/blackbirds/models/random_walk.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 import torch
 
 from blackbirds.models.model import Model
 
 
-class Autoregressive(Model):
-    def __init__(self, n_timesteps: int, sigma_eps: float = 1.0):
-        r"""
-        Implements an autoregressive model of order `p`.
+class RandomWalk(Model):
+    def __init__(self, n_timesteps, tau_softmax=0.1):
+        r"""Implements a differentiable random walk.
 
         $$
-        X_t = \sum_{i=1}^p \phi_i X_{t-i} + \epsilon_t
+            X_t = \sum_{i=1}^t (2\eta - 1),
         $$
 
-        **Arguments:**
+        where
+
+        $$
+        \eta \sim \text{Bernoulli}(p).
+        $$
+
+        **Arguments**:
 
-        - `n_timesteps`: The number of timesteps to predict into the future.
-        - `sigma_eps`: The standard deviation of the gaussian noise.
+        - `n_timesteps` (int): Number of timesteps to simulate.
+        - `tau_softmax` (float): Temperature parameter for the Gumbel-Softmax
         """
+        super().__init__()
         self.n_timesteps = n_timesteps
-        self.sigma_eps = torch.tensor(sigma_eps)
+        self.tau_softmax = tau_softmax
 
     def initialize(self, params):
-        """
-        Initializes the model with the given parameters.
+        return torch.zeros(1).reshape(1, 1)
 
-        The fist time-step is just some random gaussian noise.
-        """
-        # return random noise
-        return torch.normal(0.0, self.sigma_eps).reshape(1, 1)
+    def trim_time_series(self, x):
+        return x[-1:]
 
     def step(self, params, x):
-        """
-        Implements a single step of the autoregressive model.
+        """Simulates a random walk step using the Gumbel-Softmax trick.
 
         **Arguments:**
 
-        - `params`: The parameters of the model.
-        - `x`: The current state of the model.
+        - `params`: a tensor of shape (1,) containing the logit probability of moving forward at each timestep.
+        - `x`: a tensor of shape (n,) containing the time-series of positions.
+
+        !!! danger
+            probability is given in logit, so the input is transformed using the sigmoid function.
         """
-        n_past_timesteps = min(x.shape[0], params.shape[0])
-        return torch.sum(
-            params[:n_past_timesteps] * x[-n_past_timesteps:]
-        ) + torch.normal(0.0, self.sigma_eps).reshape(1, 1)
+        p = torch.sigmoid(params)
+        logits = torch.vstack((p, 1 - p)).log()
+        step = torch.nn.functional.gumbel_softmax(
+            logits, dim=0, tau=self.tau_softmax, hard=True
+        )
+        return (x[-1] + step[0] - step[1]).reshape(1, 1)
 
     def observe(self, x):
         return [x]
-
-    def trim_time_series(self, x):
-        return x
```

### Comparing `blackbirds-0.1.0/blackbirds/models/brock_hommes.py` & `blackbirds-1.0.0/blackbirds/models/brock_hommes.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         **Arguments:**
 
         - `params`: A list of parameters. Parameters follow the order: log_beta, g1, g2, g3, g4, b1, b2, b3, b4, log_sigma, log_r
         - `x`: The current state of the model.
 
         !!! danger
-        beta, sigma, and r are given in log.
+            beta, sigma, and r are given in log.
         """
         beta = torch.exp(params[0])
         g = params[1:5]
         b = params[5:9]
         sigma = torch.exp(params[-2])
         r = torch.exp(params[-1])
         R = 1.0 + r
```

### Comparing `blackbirds-0.1.0/blackbirds/models/june.py` & `blackbirds-1.0.0/blackbirds/models/june.py`

 * *Files identical despite different names*

### Comparing `blackbirds-0.1.0/blackbirds/models/model.py` & `blackbirds-1.0.0/blackbirds/models/model.py`

 * *Files identical despite different names*

### Comparing `blackbirds-0.1.0/blackbirds/models/rama_cont.py` & `blackbirds-1.0.0/blackbirds/models/rama_cont.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import torch
 
 from blackbirds.models.model import Model
 
 
 class RamaCont(Model):
     def __init__(self, n_agents, n_timesteps, s, sigmoid_k):
-        """
+        r"""
         Implementation of the Rama Cont model from Rama Cont (2005).
 
-        **Arguments**
+        **Arguments:**
 
         - `n_agents`: Number of agents
         - `n_timesteps`: Number of timesteps
         - `s`: Probability of updating the threshold $\nu_i$.
         - `sigmoid_k`: Steepness of the sigmoid function.
         """
         super().__init__()
@@ -61,14 +61,17 @@
             self.sigmoid_k * (-nu_t - epsilon_t)
         )
 
     def compute_order_hard(self, epsilon_t, nu_t):
         return (epsilon_t > nu_t).float() - (epsilon_t < -nu_t).float()
 
     def compute_order(self, epsilon_t, nu_t):
+        """
+        We do a trick similar to the gumbel-softmax.
+        """
         soft = self.compute_order_soft(epsilon_t, nu_t)
         return self.compute_order_hard(epsilon_t, nu_t) + soft - soft.detach()
 
     def compute_returns(self, order, eta):
         return 1.0 / (self.n_agents * eta) * order.sum()
 
     def compute_new_nu_t(self, nu_t, s, returns):
```

### Comparing `blackbirds-0.1.0/blackbirds/models/sir.py` & `blackbirds-1.0.0/blackbirds/models/sir.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         - `graph`: a networkx graph
         - `n_timesteps`: the number of timesteps to run the model for
         - `device` : device to use (eg. "cpu" or "cuda:0")
         """
         super().__init__()
         self.n_timesteps = n_timesteps
         # convert graph from networkx to pytorch geometric
-        self.graph = torch_geometric.utils.convert.from_networkx(graph)
+        self.graph = torch_geometric.utils.convert.from_networkx(graph).to(device)
         self.mp = SIRMessagePassing(aggr="add", node_dim=-1)
 
     def sample_bernoulli_gs(self, probs: torch.Tensor, tau: float = 0.1):
         """
         Samples from a Bernoulli distribution in a diferentiable way using Gumble-Softmax
 
         **Arguments:**
```

### Comparing `blackbirds-0.1.0/blackbirds/posterior_estimators.py` & `blackbirds-1.0.0/blackbirds/posterior_estimators.py`

 * *Files identical despite different names*

### Comparing `blackbirds-0.1.0/blackbirds/utils.py` & `blackbirds-1.0.0/blackbirds/utils.py`

 * *Files identical despite different names*

### Comparing `blackbirds-0.1.0/setup.py` & `blackbirds-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
 
 setup(
     name="blackbirds",
-    version="0.1.0",
-    description="Bayesian inference for differentiable simulators.",
+    version="1.0.0",
+    description="Black-Box Inference foR Differentiable Simulators.",
     url="https://github.com/arnauqb/blackbirds",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Ayush Chopra and Joel Dyer and Arnau Quera-Bofarull",
     author_email="arnauq@protonmail.com",
     license="MIT License",
     install_requires=requirements,
```

### Comparing `blackbirds-0.1.0/test/test_jacfwd.py` & `blackbirds-1.0.0/test/test_jacfwd.py`

 * *Files identical despite different names*

### Comparing `blackbirds-0.1.0/test/test_posterior_estimators.py` & `blackbirds-1.0.0/test/test_posterior_estimators.py`

 * *Files identical despite different names*

