# Comparing `tmp/openirt-0.1.7.tar.gz` & `tmp/openirt-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openirt-0.1.7.tar", last modified: Tue May 30 12:30:57 2023, max compression
+gzip compressed data, was "openirt-0.1.8.tar", last modified: Mon Jul 17 10:18:02 2023, max compression
```

## Comparing `openirt-0.1.7.tar` & `openirt-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:30:57.089722 openirt-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-30 12:30:36.000000 openirt-0.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 12:30:57.089722 openirt-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-30 12:30:36.000000 openirt-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:30:57.088722 openirt-0.1.7/openirt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6938 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/bayes3PL.py
--rw-rw-rw-   0 root         (0) root         (0)     2081 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3932 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/irt_instance.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/item_model.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/newclass.py
--rw-rw-rw-   0 root         (0) root         (0)     3387 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/norm_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2745 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/pl1.py
--rw-rw-rw-   0 root         (0) root         (0)     4615 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/pl2.py
--rw-rw-rw-   0 root         (0) root         (0)     5984 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/pl3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:30:57.089722 openirt-0.1.7/openirt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 12:30:57.000000 openirt-0.1.7/openirt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2023-05-30 12:30:57.000000 openirt-0.1.7/openirt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 12:30:57.000000 openirt-0.1.7/openirt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-30 12:30:57.000000 openirt-0.1.7/openirt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 12:30:57.089722 openirt-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-30 12:30:36.000000 openirt-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:30:57.089722 openirt-0.1.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-30 12:30:36.000000 openirt-0.1.7/tests/test_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.822258 openirt-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-17 10:17:41.000000 openirt-0.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      256 2023-07-17 10:18:02.822258 openirt-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-17 10:17:41.000000 openirt-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.819258 openirt-0.1.8/openirt/
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6938 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/bayes3PL.py
+-rw-rw-rw-   0 root         (0) root         (0)     2081 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3933 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/irt_instance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.821258 openirt-0.1.8/openirt/item_models/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6462 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3236 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/norm.py
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/pl1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4592 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/pl2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4379 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/pl3.py
+-rw-rw-rw-   0 root         (0) root         (0)    10759 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/mixed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.821258 openirt-0.1.8/openirt/mmle/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/mmle/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5523 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/mmle/generic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.820258 openirt-0.1.8/openirt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      256 2023-07-17 10:18:02.000000 openirt-0.1.8/openirt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2023-07-17 10:18:02.000000 openirt-0.1.8/openirt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 10:18:02.000000 openirt-0.1.8/openirt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 10:18:02.000000 openirt-0.1.8/openirt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 10:18:02.822258 openirt-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      672 2023-07-17 10:17:41.000000 openirt-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.822258 openirt-0.1.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2445 2023-07-17 10:17:41.000000 openirt-0.1.8/tests/test_p1.py
```

### Comparing `openirt-0.1.7/LICENSE` & `openirt-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openirt-0.1.7/openirt/bayes3PL.py` & `openirt-0.1.8/openirt/bayes3PL.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.7/openirt/cli.py` & `openirt-0.1.8/openirt/cli.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.7/openirt/irt_instance.py` & `openirt-0.1.8/openirt/irt_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import os
 import pandas as pd
 # from pl1 import PL1
 from pl2 import PL2
 # from pl3 import PL3
 from norm_model import NormModel
```

### Comparing `openirt-0.1.7/openirt/norm_model.py` & `openirt-0.1.8/openirt/item_models/norm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from item_model import ItemModel
+from model import Model
 import numpy as np
 from scipy.stats import norm
 from typing import Union
 
-class NormModel():
+class Norm(Model):
+    def __init__(self):
+        super().__init__(Norm.norm_p, 2, True)
     
-    def prob(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
+    @staticmethod
+    def norm_p(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
         """_summary_
         takes array of a abilities (n*1) and array of params (2*m) and returns prob (n*m)
 
         Args:
             ability (Union[list, np.ndarray, float]): _description_
             params (Union[list, np.ndarray]): _description_
 
@@ -17,75 +20,67 @@
             np.ndarray: _description_
         """
         ability = np.array(ability)
         params = np.array(params)
         z = np.matmul(ability[:, np.newaxis], [params[1]])
         z += np.tile(params[0], (len(ability), 1))
         return norm.cdf(z)
-
     
-    def norm_density(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
+    @staticmethod
+    def __norm_density(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
         ability = np.array(ability)
         params = np.array(params)
         z = np.matmul(ability[:, np.newaxis], [params[1]])
         z += np.tile(params[0], (len(ability), 1))
         return norm.pdf(z)
-        
-    def estimate_parameters(self, 
+    
+    @staticmethod
+    def convert_param_form(self, params):
+        return np.array([-params[0] / params[1], 1 / params[1]])
+    
+    def estimate_ability_max_lik(self, params: Union[list, np.ndarray], 
+                         results: Union[list, np.ndarray],
+                         end=0.00000001,
+                         eps=0.01) -> np.ndarray:
+        est = 0.5
+        prev_est = 0
+        while abs(est - prev_est) > end:
+            P = self.prob(est, params)[0]
+            W = (1 - P) * P
+            h = self.norm_density(est, params)[0]
+            prev_est = est
+            denom = np.sum(params[1]**2 * W)
+            if denom < eps or np.any(W < eps):
+                break
+            est = est + (np.sum(params[1] * W  * ((results - P)/ h)) / denom)
+        return est
+    
+    def estimate_item_params_max_lik(self, 
                             ability: Union[list, np.ndarray], 
                             result: Union[list, np.ndarray], 
                             sigm_orig=0,
                             lamb_orig=1, 
                             end=0.0000001,  
                             eps=0.1) -> np.ndarray:
         ability = np.array(ability)
         result = np.array(result)
         est = [sigm_orig, lamb_orig]
         prev_est = [0, 0]
         while abs(est[0] - prev_est[0]) > end or abs(est[1] - prev_est[1]) > end:
             P = self.prob(
                 ability, [[est[0]], [est[1]]]).transpose()[0]
             h = self.norm_density(ability, [[est[0]], [est[1]]]).transpose()[0]
-            # break
             W = h**2 / (P * (1 - P))
             L11 = -np.sum(W)
             L12 = -np.sum(ability * W)
             L22 = -np.sum(ability**2 * W)
             L = np.array([[L11, L12], [L12, L22]])
 
             if abs(np.linalg.det(L)) < eps:
                 break
             L_inv = np.linalg.inv(L)
 
             v = (result - P) / h
             obs_mat = np.array([np.sum(W * v), np.sum(W * v * ability)])
             prev_est = est
             est = est - np.matmul(L_inv, obs_mat)
-        return est
-    
-    def estimate_ability(self, params: Union[list, np.ndarray], 
-                         results: Union[list, np.ndarray],
-                         end=0.00000001,
-                         eps=0.01) -> np.ndarray:
-        est = 0.5
-        prev_est = 0
-        while abs(est - prev_est) > end:
-            P = self.prob(est, params)[0]
-            W = (1 - P) * P
-            h = self.norm_density(est, params)[0]
-            prev_est = est
-            denom = np.sum(params[1]**2 * W)
-            if denom < eps or np.any(W < eps):
-                break
-            est = est + (np.sum(params[1] * W  * ((results - P)/ h)) / denom)
-        return est
-    
-    def convert_param_form(self, params):
-        return np.array([-params[0] / params[1], 1 / params[1]])
-
-if __name__ == "__main__":
-    nm = NormModel()
-    results = np.array([0, 1, 1, 0, 1, 1, 1, 1, 1])
-    abilities = [-2, -1.5, -1, -0.5, 0, 0.5, 1, 1.5, 2]
-    
-    params = nm.estimate_parameters(abilities, results)
-    nm.plot_item_curve(np.array([params]).T)
+        return est
```

### Comparing `openirt-0.1.7/openirt/pl1.py` & `openirt-0.1.8/openirt/item_models/pl1.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,82 @@
-from pathlib import Path
-import sys
-if str(Path(__file__).parent) not in sys.path:
-    sys.path.append(str(Path(__file__).parent))
-from openirt.item_model import ItemModel
-from typing import Union
+from model import Model
 import numpy as np
 from pl2 import PL2
 
-class PL1(ItemModel):
-    def prob(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
+
+class PL1(Model):
+    """
+    1-parameter logistic model (Rasch model).
+    p(\\theta) = 1 / (1 + e^{-(\\zeta + \\theta)}
+    """
+    def __init__(self):
+        super().__init__(
+            PL1.pl1_p,
+            num_params=1,
+            multi=True,
+            prov_params=[0],
+            loc_param=0,
+            param_bounds=[(-7, 7)],
+            loc_param_asc=False,
+        )
+
+    @staticmethod
+    def pl1_p(
+        ability: np.ndarray, 
+        params: np.ndarray
+    ) -> np.ndarray:
         """
-        Calculate the probability of a correct response given the ability and item parameters.
+        Probability of a correct response given the ability and item 
+        parameters.
 
         Args:
-            ability: A list, numpy array, or float representing the ability of the individual.
-            params: A list or numpy array containing the item parameters.
+            ability : np.ndarray 
+                Array of abilities.
+            params : np.ndarray
+                Item parameters. Item parameters. Each column is a different
+                item, each row is a different parameter.
 
         Returns:
-            A numpy array representing the probabilities of correct responses.
+            np.ndarray: Array of probabilities. Each row is a different
+            individual, each column is a different item.
+        """
+        return PL2().pl2_p(ability, [params[0], np.ones(len(params[0]))])
+
+    def estimate_ability_max_lik(
+        self,
+        params: Union[list, np.ndarray],
+        results: Union[list, np.ndarray],
+        end=0.00000001,
+        eps=0.01,
+        eps2=0.000001,
+    ) -> np.ndarray:
         """
-        return PL2().prob(ability, [params[0], np.ones(len(params[0]))])
+        Estimate the ability of an individual given the item parameters and responses.
 
-    def estimate_parameters(self, ability: Union[list, np.ndarray], result: Union[list, np.ndarray],
-                            sigm_orig=0, end=0.0000001, eps=0.0001) -> np.ndarray:
+        Args:
+            params: A list or numpy array representing the item parameters.
+            results: A list or numpy array representing the item responses.
+            end: The convergence threshold.
+            eps: The threshold for detecting a near-singular matrix.
+
+        Returns:
+            A numpy array representing the estimated ability.
+        """
+        return PL2().estimate_ability_max_lik(
+            [params[0], np.ones(len(params[0]))], results, end, eps, eps2
+        )
+
+    def estimate_item_params_max_lik(
+        self,
+        ability: Union[list, np.ndarray],
+        result: Union[list, np.ndarray],
+        sigm_orig=0,
+        end=0.0000001,
+        eps=0.0001,
+    ) -> np.ndarray:
         """
         Estimate the parameters of the model given the abilities and item responses.
 
         Args:
             ability: A list or numpy array containing the abilities of individuals.
             result: A list or numpy array representing the item responses.
             sigm_orig: The initial value for the parameter sigm.
@@ -37,33 +87,17 @@
             A numpy array representing the estimated parameters.
         """
         ability = np.array(ability)
         result = np.array(result)
         est = sigm_orig
         prev_est = est + 2 * end
         while abs(est - prev_est) > end:
-            P = self.prob(ability, [[est]]).transpose()[0]
+            P = self.pl1_p(ability, [[est]]).transpose()[0]
             L1 = np.sum(result - P)
             L2 = -np.sum(P * (1 - P))
 
             if abs(L2) < eps:
                 break
 
             prev_est = est
             est = est - L1 / L2
         return np.array([est])
-
-    def estimate_ability(self, params: Union[list, np.ndarray], results: Union[list, np.ndarray],
-                         end=0.00000001, eps=0.01) -> np.ndarray:
-        """
-        Estimate the ability of an individual given the item parameters and responses.
-
-        Args:
-            params: A list or numpy array representing the item parameters.
-            results: A list or numpy array representing the item responses.
-            end: The convergence threshold.
-            eps: The threshold for detecting a near-singular matrix.
-
-        Returns:
-            A numpy array representing the estimated ability.
-        """
-        return PL2().estimate_ability([params[0], np.ones(len(params[0]))], results, end, eps)
```

### Comparing `openirt-0.1.7/openirt/pl2.py` & `openirt-0.1.8/openirt/item_models/pl2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,97 @@
-from pathlib import Path
-import sys
-if str(Path(__file__).parent) not in sys.path:
-    sys.path.append(str(Path(__file__).parent))
-from item_model import ItemModel
+from model import Model
 from typing import Union
 import numpy as np
-import matplotlib.pyplot as plt
 
-class PL2(ItemModel):
-    def prob(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
+
+class PL2(Model):
+    """
+    2-parameter logistic model.
+    p(\\theta) = 1 / (1 + e^{-(\\zeta + \\lambda\\theta)}
+    """
+    def __init__(self):
+        super().__init__(
+            PL2.pl2_p,
+            num_params=2,
+            multi=True,
+            prov_params=[0, 1],
+            loc_param=0,
+            param_bounds=((-10, 10), (0, 5)),
+            loc_param_asc=False,
+        )
+
+    @staticmethod
+    def pl2_p(
+        ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]
+    ) -> np.ndarray:
         """
-        Calculate the probability of a correct response given the ability and item parameters.
+        Probability of a correct response given the ability and item
+        parameters.
 
         Args:
-            ability: A list, numpy array, or float representing the ability of the individual.
-            params: A list or numpy array containing the item parameters.
+            ability (np.ndarray): Array of abilities.
+            params (np.ndarray): Item parameters. Item parameters. Each column
+            is a different item, each row is a different parameter.
 
         Returns:
-            A numpy array representing the probabilities of correct responses.
+            np.ndarray: Array of probabilities. Each row is a different
+            individual, each column is a different item.
         """
         items = np.array(params).shape[1]
         num_abilities = 1
         if np.array(ability).shape != ():
             num_abilities = np.array(ability).shape[0]
         ability = np.tile(np.array([ability]).transpose(), (1, items))
 
         params = np.tile(params, num_abilities).reshape((2, num_abilities, items))
         return 1 / (1 + np.exp(-params[0] - (params[1] * ability)))
 
-    def estimate_parameters(self, ability: Union[list, np.ndarray], result: Union[list, np.ndarray],
-                            sigm_orig=-1, lamb_orig=1, end=0.00001, eps=0.1) -> np.ndarray:
+    def estimate_ability_max_lik(
+        self,
+        params: Union[list, np.ndarray],
+        results: Union[list, np.ndarray],
+        end=0.00000001,
+        eps=0.01,
+        eps2=0.1,
+    ) -> np.ndarray:
+        """
+        Estimate the ability of an individual given the item parameters and responses.
+
+        Args:
+            params: A list or numpy array representing the item parameters.
+            results: A list or numpy array representing the item responses.
+            end: The convergence threshold.
+            eps: The threshold for detecting a near-singular matrix.
+
+        Returns:
+            A numpy array representing the estimated ability.
+        """
+        params = np.array(params)
+        results = np.array(results)
+        est = 0.5
+        prev_est = 0
+        while abs(est - prev_est) > end:
+            P = self.p(est, params)[0]
+            W = (1 - P) * P
+            denom = np.sum(params[1] ** 2 * W)
+            if abs(denom) < eps or np.any(np.abs(W) < eps2):
+                break
+            prev_est = est
+            est = est + (np.sum(params[1] * W * ((results - P) / W)) / denom)
+        return est
+
+    def estimate_item_params_max_lik(
+        self,
+        ability: Union[list, np.ndarray],
+        result: Union[list, np.ndarray],
+        sigm_orig=-1,
+        lamb_orig=1,
+        end=0.00001,
+        eps=0.1,
+    ) -> np.ndarray:
         """
         Estimate the parameters of the model given the abilities and item responses.
 
         Args:
             ability: A list or numpy array containing the abilities of individuals.
             result: A list or numpy array representing the item responses.
             sigm_orig: The initial value for the parameter sigm.
@@ -45,74 +103,33 @@
             A numpy array representing the estimated parameters.
         """
         ability = np.array(ability)
         result = np.array(result)
         est = [sigm_orig, lamb_orig]
         prev_est = [0, 0]
         while abs(est[0] - prev_est[0]) > end or abs(est[1] - prev_est[1]) > end:
-            P = self.prob(ability, [[est[0]], [est[1]]]).transpose()[0]
+            P = self.p(ability, [[est[0]], [est[1]]]).transpose()[0]
             W = P * (1 - P)
             L11 = -np.sum(W)
             L12 = -np.sum(ability * W)
             L22 = -np.sum(ability**2 * W)
             L = np.array([[L11, L12], [L12, L22]])
             if abs(np.linalg.det(L)) < eps:
                 break
             L_inv = np.linalg.inv(L)
 
             obs_mat = np.array([np.sum(result - P), np.sum((result - P) * ability)])
             prev_est = est
             est = est - np.matmul(L_inv, obs_mat)
         return est
 
-    def estimate_ability(self, params: Union[list, np.ndarray], results: Union[list, np.ndarray],
-                         end=0.00000001, eps=0.01) -> np.ndarray:
-        """
-        Estimate the ability of an individual given the item parameters and responses.
-
-        Args:
-            params: A list or numpy array representing the item parameters.
-            results: A list or numpy array representing the item responses.
-            end: The convergence threshold.
-            eps: The threshold for detecting a near-singular matrix.
-
-        Returns:
-            A numpy array representing the estimated ability.
-        """
-        params = np.array(params)
-        results = np.array(results)
-        est = 0.5
-        prev_est = 0
-        while abs(est - prev_est) > end:
-            P = self.prob(est, params)[0]
-            W = (1 - P) * P
-            denom = np.sum(params[1]**2 * W)
-            if abs(denom) < eps or np.any(np.abs(W) < eps):
-                break
-            prev_est = est
-            est = est + (np.sum(params[1] * W * ((results - P) / W)) / denom)
-        return est
-    
     def convert_param_form(self, params):
         """
         Convert item parameters from one form to another.
 
         Args:
             params: A list or numpy array representing the item parameters.
 
         Returns:
             A numpy array representing the converted item parameters.
         """
         return np.array([-params[0] / params[1], 1 / params[1]])
-
-    def plot_item_curve(self, p):
-        """
-        Plot item curves for given item parameters.
-
-        Args:
-            p: A numpy array representing the item parameters.
-        """
-        ability = np.linspace(-4, 4, 100)
-        for i in range(p.shape[1]):
-            plt.plot(ability, self.prob(ability, p[:,i].reshape(p.shape[0], 1)), label=f'Question{i+1}')
-        plt.legend()
-        plt.show()
```

### Comparing `openirt-0.1.7/openirt/pl3.py` & `openirt-0.1.8/openirt/item_models/pl3.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-from pathlib import Path
-import sys
-if str(Path(__file__).parent) not in sys.path:
-    sys.path.append(str(Path(__file__).parent))
-from item_model import ItemModel
+from model import Model
 from typing import Union
 import numpy as np
-import matplotlib.pyplot as plt
-from scipy.optimize import minimize
 
-
-class PL3(ItemModel):
-    def prob(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
+class PL3(Model):
+    def __init__(self):
+        super().__init__(PL3.pl3_p, 3, True)
+    
+    @staticmethod
+    def pl3_p(ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
         """
         Calculate the probability of a correct response given the ability and item parameters.
 
         Args:
             ability: A list, numpy array, or float representing the ability of the individual.
             params: A list or numpy array containing the item parameters.
 
@@ -26,17 +23,19 @@
         if np.array(ability).shape != ():
             num_abilities = np.array(ability).shape[0]
         ability = np.tile(np.array([ability]).transpose(), (1, items))
 
         params = np.tile(params, num_abilities).reshape((3, num_abilities, items))
         return params[2] + (1 - params[2]) / (1 + np.exp(-params[0] * (ability - params[1])))
 
-    def prob2PM(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
+    @staticmethod
+    def pl2_p(ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
         """
         Calculate the probability of a correct response using the 2-parameter logistic model.
+        This uses standard a,b,c form.
 
         Args:
             ability: A list, numpy array, or float representing the ability of the individual.
             params: A list or numpy array containing the item parameters.
 
         Returns:
             A numpy array representing the probabilities of correct responses using the 2-parameter logistic model.
@@ -46,39 +45,45 @@
         if np.array(ability).shape != ():
             num_abilities = np.array(ability).shape[0]
         ability = np.tile(np.array([ability]).transpose(), (1, items))
 
         params = np.tile(params, num_abilities).reshape((3, num_abilities, items))
         return 1 / (1 + np.exp(-params[0] * (ability - params[1])))
 
-    def estimate_parameters(self, ability: Union[list, np.ndarray], result: Union[list, np.ndarray],
-                            a_orig=1, b_orig=0.1, c_orig=0.1, end=0.0000001, eps=0.1) -> np.ndarray:
-        """
-        Estimate the parameters of the model given the abilities and item responses.
+    def estimate_ability_max_lik(self, params: Union[list, np.ndarray], results: Union[list, np.ndarray],
+                         end=0.00000001, eps=0.01) -> np.ndarray:
+        params = np.array(params)
+        results = np.array(results)
+        est = 0.5
+        prev_est = 0
+        while abs(est - prev_est) > end:
+            P = self.pl3_p(est, params)[0]
+            Q = 1 - P
+            P_2pm = self.pl2_p(est, params)[0]
+            W = P_2pm * (1 - P_2pm)
 
-        Args:
-            ability: A list or numpy array containing the abilities of individuals.
-            result: A list or numpy array representing the item responses.
-            a_orig: The initial value for parameter a.
-            b_orig: The initial value for parameter b.
-            c_orig: The initial value for parameter c.
-            end: The convergence threshold.
-            eps: The threshold for detecting a near-singular matrix.
+            denom = - np.sum(params[0] ** 2 * W * (P_2pm / P) ** 2)
 
-        Returns:
-            A numpy array representing the estimated parameters.
-        """
+            if abs(denom) < eps:
+                break
+            num = np.sum(params[0] * W * ((results - P) / (P * Q)) * (P_2pm / P))
+            prev_est = est
+            est = est + (num / denom)
+        return est
+
+    def estimate_item_params_max_lik(self, ability: Union[list, np.ndarray], result: Union[list, np.ndarray],
+                            a_orig=1, b_orig=0.1, c_orig=0.1, end=0.0000001, eps=0.1) -> np.ndarray:
         ability = np.array(ability)
         result = np.array(result)
         est = np.array([a_orig, b_orig, c_orig])
         prev_est = est + 2 * end
         while np.all(np.abs(prev_est - est) > end):
-            P = self.prob(ability, est.reshape((3, 1))).T[0]
+            P = self.pl3_p(ability, est.reshape((3, 1))).T[0]
             Q = 1 - P
-            P_2pm = self.prob2PM(ability, est.reshape((3, 1))).T[0]
+            P_2pm = self.pl2_p(ability, est.reshape((3, 1))).T[0]
 
             L11 = -np.sum((ability - est[1]) ** 2 * P * Q * (P_2pm / P) ** 2)
             L12 = np.sum(est[0] * (ability - est[1]) * P * Q * (P_2pm / P))
             L13 = -np.sum((ability - est[1]) * (Q / (1 - est[2])) * (P_2pm / P))
 
             L22 = -est[0] ** 2 * np.sum(P * Q * (P_2pm / P))
             L23 = np.sum(est[0] * (Q / (1 - est[2])) * (P_2pm / P))
@@ -95,53 +100,7 @@
             L2 = -est[0] * np.sum((result - P) * (P_2pm / P))
             L3 = np.sum((result - P) / (P - est[2]) * (P_2pm / P))
             obs_mat = np.array([L1, L2, L3])
             prev_est = est
             est = est - np.matmul(L_inv, obs_mat)
         return est
 
-    def estimate_ability(self, params: Union[list, np.ndarray], results: Union[list, np.ndarray],
-                         end=0.00000001, eps=0.01) -> np.ndarray:
-        """
-        Estimate the ability of an individual given the item parameters and responses.
-
-        Args:
-            params: A list or numpy array representing the item parameters.
-            results: A list or numpy array representing the item responses.
-            end: The convergence threshold.
-            eps: The threshold for detecting a near-singular matrix.
-
-        Returns:
-            A numpy array representing the estimated ability.
-        """
-        params = np.array(params)
-        results = np.array(results)
-        est = 0.5
-        prev_est = 0
-        while abs(est - prev_est) > end:
-            P = self.prob(est, params)[0]
-            Q = 1 - P
-            P_2pm = self.prob2PM(est, params)[0]
-            W = P_2pm * (1 - P_2pm)
-
-            denom = - np.sum(params[0] ** 2 * W * (P_2pm / P) ** 2)
-
-            if abs(denom) < eps:
-                break
-            num = np.sum(params[0] * W * ((results - P) / (P * Q)) * (P_2pm / P))
-            prev_est = est
-            est = est + (num / denom)
-        return est
-
-    def plot_item_curve(self, p):
-        """
-        Plot the item response curves for given item parameters.
-
-        Args:
-            p: A numpy array representing the item parameters.
-        """
-        ability = np.linspace(-4, 4, 100)
-        for i in range(p.shape[1]):
-            plt.plot(ability, self.prob(ability, p[:, i].reshape(p.shape[0], 1)), label=f'Question{i + 1}')
-        plt.legend()
-        plt.show()
-
```

