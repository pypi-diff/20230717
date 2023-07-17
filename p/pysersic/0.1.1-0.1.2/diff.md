# Comparing `tmp/pysersic-0.1.1.tar.gz` & `tmp/pysersic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysersic-0.1.1.tar", last modified: Mon Jun  5 18:12:04 2023, max compression
+gzip compressed data, was "pysersic-0.1.2.tar", last modified: Mon Jul 17 05:06:10 2023, max compression
```

## Comparing `pysersic-0.1.1.tar` & `pysersic-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2023-06-05 18:12:04.092319 pysersic-0.1.1/
--rw-r--r--   0 ipasha     (501) staff       (20)     1065 2023-01-18 18:39:41.000000 pysersic-0.1.1/LICENSE
--rw-r--r--   0 ipasha     (501) staff       (20)      277 2023-06-05 18:12:04.092447 pysersic-0.1.1/PKG-INFO
--rw-r--r--   0 ipasha     (501) staff       (20)     3173 2023-06-05 18:06:05.000000 pysersic-0.1.1/README.md
-drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2023-06-05 18:12:04.089944 pysersic-0.1.1/pysersic/
--rw-r--r--   0 ipasha     (501) staff       (20)      260 2023-06-05 17:14:25.000000 pysersic-0.1.1/pysersic/__init__.py
--rw-r--r--   0 ipasha     (501) staff       (20)     6804 2023-06-05 17:14:25.000000 pysersic-0.1.1/pysersic/galfit.py
--rw-r--r--   0 ipasha     (501) staff       (20)    10866 2023-06-05 17:14:25.000000 pysersic-0.1.1/pysersic/loss.py
--rw-r--r--   0 ipasha     (501) staff       (20)    29883 2023-06-05 17:14:25.000000 pysersic-0.1.1/pysersic/priors.py
--rw-r--r--   0 ipasha     (501) staff       (20)    23260 2023-06-05 17:16:21.000000 pysersic-0.1.1/pysersic/pysersic.py
--rw-r--r--   0 ipasha     (501) staff       (20)    41946 2023-05-15 16:03:09.000000 pysersic-0.1.1/pysersic/rendering.py
--rw-r--r--   0 ipasha     (501) staff       (20)    20176 2023-06-05 17:14:25.000000 pysersic-0.1.1/pysersic/results.py
-drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2023-06-05 18:12:04.091987 pysersic-0.1.1/pysersic.egg-info/
--rw-r--r--   0 ipasha     (501) staff       (20)      277 2023-06-05 18:12:03.000000 pysersic-0.1.1/pysersic.egg-info/PKG-INFO
--rw-r--r--   0 ipasha     (501) staff       (20)      334 2023-06-05 18:12:04.000000 pysersic-0.1.1/pysersic.egg-info/SOURCES.txt
--rw-r--r--   0 ipasha     (501) staff       (20)        1 2023-06-05 18:12:03.000000 pysersic-0.1.1/pysersic.egg-info/dependency_links.txt
--rw-r--r--   0 ipasha     (501) staff       (20)       89 2023-06-05 18:12:03.000000 pysersic-0.1.1/pysersic.egg-info/requires.txt
--rw-r--r--   0 ipasha     (501) staff       (20)        9 2023-06-05 18:12:03.000000 pysersic-0.1.1/pysersic.egg-info/top_level.txt
--rw-r--r--   0 ipasha     (501) staff       (20)       79 2023-06-05 18:12:04.093031 pysersic-0.1.1/setup.cfg
--rw-r--r--   0 ipasha     (501) staff       (20)      586 2023-06-05 18:11:50.000000 pysersic-0.1.1/setup.py
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2023-07-17 05:06:10.825367 pysersic-0.1.2/
+-rw-r--r--   0 ipasha     (501) staff       (20)     1065 2023-01-18 18:39:41.000000 pysersic-0.1.2/LICENSE
+-rw-r--r--   0 ipasha     (501) staff       (20)      277 2023-07-17 05:06:10.825508 pysersic-0.1.2/PKG-INFO
+-rw-r--r--   0 ipasha     (501) staff       (20)     3717 2023-06-30 17:38:35.000000 pysersic-0.1.2/README.md
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2023-07-17 05:06:10.819848 pysersic-0.1.2/pysersic/
+-rw-r--r--   0 ipasha     (501) staff       (20)      289 2023-06-30 20:31:35.000000 pysersic-0.1.2/pysersic/__init__.py
+-rw-r--r--   0 ipasha     (501) staff       (20)      204 2023-06-30 20:09:06.000000 pysersic-0.1.2/pysersic/exceptions.py
+-rw-r--r--   0 ipasha     (501) staff       (20)     6804 2023-06-06 01:01:14.000000 pysersic-0.1.2/pysersic/galfit.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    10866 2023-06-06 01:01:14.000000 pysersic-0.1.2/pysersic/loss.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    29883 2023-06-06 01:01:14.000000 pysersic-0.1.2/pysersic/priors.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    25249 2023-06-30 20:46:02.000000 pysersic-0.1.2/pysersic/pysersic.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    42318 2023-06-30 17:58:46.000000 pysersic-0.1.2/pysersic/rendering.py
+-rw-r--r--   0 ipasha     (501) staff       (20)    20176 2023-06-06 01:01:14.000000 pysersic-0.1.2/pysersic/results.py
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2023-07-17 05:06:10.822282 pysersic-0.1.2/pysersic.egg-info/
+-rw-r--r--   0 ipasha     (501) staff       (20)      277 2023-07-17 05:06:10.000000 pysersic-0.1.2/pysersic.egg-info/PKG-INFO
+-rw-r--r--   0 ipasha     (501) staff       (20)      443 2023-07-17 05:06:10.000000 pysersic-0.1.2/pysersic.egg-info/SOURCES.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)        1 2023-07-17 05:06:10.000000 pysersic-0.1.2/pysersic.egg-info/dependency_links.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)       89 2023-07-17 05:06:10.000000 pysersic-0.1.2/pysersic.egg-info/requires.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)        9 2023-07-17 05:06:10.000000 pysersic-0.1.2/pysersic.egg-info/top_level.txt
+-rw-r--r--   0 ipasha     (501) staff       (20)       79 2023-07-17 05:06:10.826076 pysersic-0.1.2/setup.cfg
+-rw-r--r--   0 ipasha     (501) staff       (20)      586 2023-07-17 05:04:59.000000 pysersic-0.1.2/setup.py
+drwxr-xr-x   0 ipasha     (501) staff       (20)        0 2023-07-17 05:06:10.824824 pysersic-0.1.2/tests/
+-rw-r--r--   0 ipasha     (501) staff       (20)     6001 2023-06-06 01:01:14.000000 pysersic-0.1.2/tests/test_fitters.py
+-rw-r--r--   0 ipasha     (501) staff       (20)      676 2023-06-06 01:01:14.000000 pysersic-0.1.2/tests/test_loss.py
+-rw-r--r--   0 ipasha     (501) staff       (20)     3444 2023-06-06 01:01:14.000000 pysersic-0.1.2/tests/test_priors.py
+-rw-r--r--   0 ipasha     (501) staff       (20)     3652 2023-06-06 01:01:14.000000 pysersic-0.1.2/tests/test_renderers.py
```

### Comparing `pysersic-0.1.1/LICENSE` & `pysersic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.1/README.md` & `pysersic-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 ![pysersic logo featuring a spiral s-galaxy as the S](misc/pysersic.png)
- 
-![License](https://img.shields.io/badge/license-MIT-blue)
+[![status](https://joss.theoj.org/papers/4214c6e588774490458e34630e8052c1/status.svg)](https://joss.theoj.org/papers/4214c6e588774490458e34630e8052c1)
+[![PyPi version](https://img.shields.io/pypi/v/pysersic?color=blue)](https://pypi.org/project/pysersic)
+[![GitHub release](https://img.shields.io/github/v/release/pysersic/pysersic)](https://github.com/pysersic/pysersic/releases/)
 [![Documentation Status](https://readthedocs.org/projects/pysersic/badge/?version=latest)](https://pysersic.readthedocs.io/en/latest/?badge=latest)
 ![tests](https://github.com/pysersic/pysersic/actions/workflows/pytest.yml/badge.svg)
+![License](https://img.shields.io/badge/license-MIT-blue)
 
 pysersic is a code for fitting sersic profiles to galaxy images using Bayesian Inference. It is written in python using [jax](https://github.com/google/jax) with inference performed using [numpyro](https://github.com/pyro-ppl/numpyro)
 
 ## Installation
 
 First you should install jax. The easiest way to do this is to use ``` pip install 'jax[cpu]' ```, however if you are on windows or planning on running it on a GPU, the installation can be a little more complicated, please see the guide [here](https://github.com/google/jax#installation). The other package dependencies for ```pysersic``` are:
 - arviz
@@ -18,15 +20,20 @@
 - numpy
 - numpyro
 - pandas
 - photutils
 - scipy
 - tqdm
 
-Next you can install pysersic! We will be uploading it to pypi very soon, but for now you should install it locally by cloning the github repo.
+Next you can install pysersic! To install the latest stable release, you can simply pip install via 
+
+```
+pip install pysersic
+```
+If you would like the bleeding edge, development build (or would like to modify, add to, or otherwise access ```pysersic``` source files), you can also install from the github:
 
 ```
 git clone https://github.com/pysersic/pysersic.git
 cd pysersic
 pip install -e .
 ```
```

### Comparing `pysersic-0.1.1/pysersic/galfit.py` & `pysersic-0.1.2/pysersic/galfit.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.1/pysersic/loss.py` & `pysersic-0.1.2/pysersic/loss.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.1/pysersic/priors.py` & `pysersic-0.1.2/pysersic/priors.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.1/pysersic/pysersic.py` & `pysersic-0.1.2/pysersic/pysersic.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 import pandas
 import tqdm
 from jax.random import PRNGKey
 from numpyro import deterministic, infer, optim
 from numpyro.handlers import condition, trace
 from numpyro.infer import SVI, Trace_ELBO
 from numpyro.infer.svi import SVIRunResult
-
+from pysersic.exceptions import *
 from pysersic.priors import PySersicMultiPrior, PySersicSourcePrior
 from pysersic.rendering import BaseRenderer, HybridRenderer
 from pysersic.results import PySersicResults
 
 from .loss import gaussian_loss
 
 ArrayLike = Union[np.array, jax.numpy.array]
 
+
 class BaseFitter(ABC):
     """
     Base class for Pysersic Fitters
     """
     def __init__(self,
         data: ArrayLike,
         rms: ArrayLike,
@@ -54,27 +55,21 @@
         renderer_kwargs : Optional[dict], optional
             Any additional arguments to pass to the renderer, by default {}
         """
 
         
         self.loss_func = loss_func
 
-        if data.shape != rms.shape:
-            raise AssertionError('rms map ndims must match input data')
-            
+        
         self.data = jnp.array(data) 
         self.rms = jnp.array(rms)
         self.psf = jnp.array(psf)
-
-        if mask is None:
-            self.mask = jnp.ones_like(self.data).astype(jnp.bool_)
-        else:
-            self.mask = jnp.logical_not(jnp.array(mask)).astype(jnp.bool_)
-
-        self.renderer = renderer(data.shape, jnp.array(psf), **renderer_kwargs)
+        self.mask = parse_mask(mask,self.data)
+        data_isgood = check_input_data(self.data,rms=self.rms,psf=self.psf,mask=jnp.logical_not(self.mask))
+        self.renderer = renderer(data.shape, psf, **renderer_kwargs)
     
         self.prior_dict = {}
 
     
     def set_loss_func(self, loss_func: Callable) -> None:
         """Set loss function to be used for inference
 
@@ -531,7 +526,57 @@
                 t.set_postfix_str(f'Round = {r:d},step_size = {lr_cur:.1e} loss: {best_loss:.3e}',refresh=False)
                 losses.append(loss)
         
         all_losses.append(losses)
 
     return SVIRunResult(svi_class.get_params(best_state), svi_state,losses)
     
+
+def parse_mask(mask:ArrayLike=None,data:ArrayLike=None):
+    if mask is None:
+        return jnp.ones_like(data).astype(jnp.bool_)
+    else:
+        return jnp.logical_not(jnp.array(mask)).astype(jnp.bool_)
+
+def check_input_data(data:ArrayLike,rms:ArrayLike,psf:ArrayLike,mask:ArrayLike=None):
+    """Check input data for certain conditions and raise warnings or exceptions if needed
+
+    Parameters
+    ----------
+    data : ArrayLike
+        input image (galaxy/cutout)
+    rms : ArrayLike
+       rms/error map of the data. 
+    psf : ArrayLike
+        pixelized PSF
+    mask :ArrayLike, optional
+       mask with True/1 indicating a pixel should be masked, by default None
+
+    Raises
+    ------
+    RMSWarning
+        If the rms map is highly discrepant from the rms of the data
+    PSFNormalizationWarning
+        if the pst normalization is not ~1
+    KernelError
+        if the provided PSF is larger than the input image (exception)
+    MaskWarning
+        If more than 50% of the image is masked. 
+    """
+    rms = jnp.array(rms)
+    data = jnp.array(data)
+    psf = jnp.array(psf)
+    if data.shape != rms.shape:
+        raise ShapeMatchError('RMS map ndims must match input data ndims.')
+    if jnp.mean(rms) > 5*jnp.std(data):
+        raise RMSWarning('Input RMS map appears to be highly offset (>5x) in magnitude from the rms of the pixels in the input image.')
+    if not jnp.isclose(jnp.sum(psf),1.0,0.1):
+        raise PSFNormalizationWarning('PSF does not appear to be appropriately normalized; Sum(psf) is more than 0.1 away from 1.')
+    if jnp.all(data.shape<psf.shape):
+        raise KernelError('PSF pixel image size must be smaller than science image.')
+    if mask is not None:
+        mask = parse_mask(mask,data)
+        if jnp.sum(mask)/jnp.prod(jnp.array(mask.shape))<0.5:
+            raise MaskWarning('More than 50 percent of input image is masked. Is this correct? (Pysersic treats True/1 as masked; you may need to flip your boolean array.) ')
+        if mask.shape !=data.shape:
+            raise ShapeMatchError('Mask ndims must match input data ndims.')
+    return True
```

### Comparing `pysersic-0.1.1/pysersic/rendering.py` & `pysersic-0.1.2/pysersic/rendering.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from jax import jit
 from scipy.special import comb
 from functools import partial
+from pysersic.exceptions import * 
 
 base_profile_types = ['sersic','doublesersic','pointsource','exp','dev']
 base_profile_params =dict( 
     zip(base_profile_types,
     [ ['xc','yc','flux','r_eff','n','ellip','theta'],
     ['xc','yc','flux','f_1', 'r_eff_1','n_1','ellip_1', 'r_eff_2','n_2','ellip_2','theta'],
     ['xc','yc','flux'],
     ['xc','yc','flux','r_eff','ellip','theta'],
     ['xc','yc','flux','r_eff','ellip','theta'],]
     )
 )
 
 
+
 class BaseRenderer(object):
     def __init__(self, 
             im_shape: Iterable, 
             pixel_PSF: jax.numpy.array
             )-> None:
         """Base class for different Renderers
 
@@ -32,16 +34,19 @@
         im_shape : Iterable
             Tuple or list containing the shape of the desired output
         pixel_PSF : jax.numpy.array
             Pixelized version of the PSF
         """
         self.im_shape = im_shape
         self.pixel_PSF = pixel_PSF
+        if not jnp.isclose(jnp.sum(self.pixel_PSF),1.0,0.1):
+            raise PSFNormalizationWarning('PSF does not appear to be appropriately normalized; Sum(psf) is more than 0.1 away from 1.')
         self.psf_shape = jnp.shape(self.pixel_PSF)
-
+        if jnp.all(self.im_shape<self.psf_shape):
+            raise KernelError('PSF pixel image size must be smaller than science image.')
         self.x = jnp.arange(self.im_shape[0])
         self.y = jnp.arange(self.im_shape[1])
         self.X,self.Y = jnp.meshgrid(self.x,self.y)
         self.x_mid = self.im_shape[0]/2. - 0.5
         self.y_mid = self.im_shape[1]/2. - 0.5
 
         # Set up pre-FFTed PSF
```

### Comparing `pysersic-0.1.1/pysersic/results.py` & `pysersic-0.1.2/pysersic/results.py`

 * *Files identical despite different names*

### Comparing `pysersic-0.1.1/setup.py` & `pysersic-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 setuptools.setup(
     name="pysersic",
-    version="0.1.1",
+    version="0.1.2",
     author="Imad Pasha & Tim Miller",
     author_email="imad.pasha@yale.edu",
     description="A Tool for fitting sersic profiles in python",
-    download_url="https://github.com/pysersic/pysersic/archive/refs/tags/v0.1.1.tar.gz",
+    download_url="https://github.com/pysersic/pysersic/archive/refs/tags/v0.1.2.tar.gz",
     packages=["pysersic",],
     install_requires=['numpy',
         'scipy',
         'matplotlib',
         'pandas',
         'astropy',
         'corner',
```

