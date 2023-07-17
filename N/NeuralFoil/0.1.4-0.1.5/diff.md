# Comparing `tmp/NeuralFoil-0.1.4.tar.gz` & `tmp/NeuralFoil-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralFoil-0.1.4.tar", last modified: Wed Jul 12 01:31:53 2023, max compression
+gzip compressed data, was "NeuralFoil-0.1.5.tar", last modified: Mon Jul 17 16:36:43 2023, max compression
```

## Comparing `NeuralFoil-0.1.4.tar` & `NeuralFoil-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:31:53.902888 NeuralFoil-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:31:53.894888 NeuralFoil-0.1.4/NeuralFoil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-07-12 01:31:53.000000 NeuralFoil-0.1.4/NeuralFoil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-12 01:31:53.000000 NeuralFoil-0.1.4/NeuralFoil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:31:53.000000 NeuralFoil-0.1.4/NeuralFoil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-12 01:31:53.000000 NeuralFoil-0.1.4/NeuralFoil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 01:31:53.000000 NeuralFoil-0.1.4/NeuralFoil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-07-12 01:31:53.902888 NeuralFoil-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21867 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:31:53.894888 NeuralFoil-0.1.4/neuralfoil/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/CL_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/neuralfoil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:31:53.898888 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/
--rw-r--r--   0 runner    (1001) docker     (123)   139485 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-large.npz
--rw-r--r--   0 runner    (1001) docker     (123)    39576 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-medium.npz
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-small.npz
--rw-r--r--   0 runner    (1001) docker     (123)   532014 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xsmall.npz
--rw-r--r--   0 runner    (1001) docker     (123)   779729 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz
--rw-r--r--   0 runner    (1001) docker     (123)  3052473 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:31:53.902888 NeuralFoil-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:36:43.018868 NeuralFoil-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:36:43.014868 NeuralFoil-0.1.5/NeuralFoil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-07-17 16:36:42.000000 NeuralFoil-0.1.5/NeuralFoil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-17 16:36:42.000000 NeuralFoil-0.1.5/NeuralFoil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:36:42.000000 NeuralFoil-0.1.5/NeuralFoil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-17 16:36:42.000000 NeuralFoil-0.1.5/NeuralFoil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 16:36:42.000000 NeuralFoil-0.1.5/NeuralFoil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-07-17 16:36:43.018868 NeuralFoil-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:36:43.014868 NeuralFoil-0.1.5/neuralfoil/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/CL_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/neuralfoil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:36:43.018868 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/
+-rw-r--r--   0 runner    (1001) docker     (123)   139485 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-large.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    39576 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-medium.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-small.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   532014 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   779729 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)  3052473 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:36:43.018868 NeuralFoil-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-17 16:36:29.000000 NeuralFoil-0.1.5/setup.py
```

### Comparing `NeuralFoil-0.1.4/LICENSE.txt` & `NeuralFoil-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.4/NeuralFoil.egg-info/PKG-INFO` & `NeuralFoil-0.1.5/NeuralFoil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.4
+Version: 0.1.5
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
@@ -33,14 +33,18 @@
 
 -----
 
 NeuralFoil is a small Python/NumPy tool for rapid aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/). It is also a small subset of the larger [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here as a standalone. Under the hood, NeuralFoil consists of physics-informed neural networks trained on [tens of millions of XFoil runs](#geometry-parameterization-and-training-data). NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient code-base](./neuralfoil).
 
 NeuralFoil is ~10x faster than XFoil for a single analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in accuracy compared to XFoil](#performance). It also has [many nice features](#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/NumPy) that make it much easier to use.
 
+```
+pip install neuralfoil
+```
+
 ## Overview
 
 NeuralFoil comes with 8 different neural network models, with increasing levels of complexity:
 
 <div align="center">
 	<table>
 	 <tr>
@@ -59,15 +63,15 @@
 This spectrum offers a tradeoff between accuracy and computational cost.
 
 In addition to its neural network models, NeuralFoil also has a bonus "Linear $C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function of angle of attack $\alpha$. This model is well-suited for linear lifting-line or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used to solve the resulting system of equations "in one shot" as a linear solve, rather than a less-numerically-robust iterative nonlinear solve.
 
 Using NeuralFoil is dead-simple, and also offers several possible "entry points" for inputs. Here's an example showing this:
 
 ```python
-import neuralfoil as nf
+import neuralfoil as nf  # `pip install neuralfoil`
 import numpy as np
 
 aero = nf.get_aero_from_dat_file(  # You can use a .dat file as an entry point
     dat_file_path="/path/to/my_airfoil_file.dat",
     alpha=5,  # Angle of attack [deg]
     Re=5e6,  # Reynolds number [-]
     model_size="xlarge",  # Optionally, specify your model size.
@@ -75,32 +79,32 @@
 
 aero = nf.get_aero_from_coordinates(  # You can use xy airfoil coordinates as an entry point
     coordinates=n_by_2_numpy_ndarray_of_airfoil_coordinates,
     alpha=np.linspace(-25, 25, 1000),  # Vectorize your evaluations across `alpha` and `Re`
     Re=5e6,
 )
 
-aero = nf.get_aero_from_airfoil(  # You can AeroSandbox airfoils as an entry point
+aero = nf.get_aero_from_airfoil(  # You can use AeroSandbox airfoils as an entry point
     airfoil=asb.Airfoil("naca4412"),  # `import aerosandbox as asb`, any UIUC or NACA airfoil name works
     alpha=5, Re=5e6,
 )
 
-# `aero` is a dict with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
+# `aero` is a dictionary with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
 ```
 
 ## Performance
 
 Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
 
 <a name="clcd-polar"></a>
 <p align="center">
 	<img src="./benchmarking/neuralfoil_point_validation.svg" width="1000" />
 </p>
 
-NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the UIUC-database training set will have even more accurate results. 
+NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the training set will have even more accurate results. 
 
 NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is obviously incorrect, which would otherwise make optimization difficult. 
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
@@ -113,21 +117,17 @@
 > 
 > ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
 
 Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
-Notably, most of the computational overhead of calling NeuralFoil is actually in the airfoil preprocessing step, where the airfoil is converted from a set of coordinates to a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-and-training-data)) - not in the aerodynamics analysis itself. This pre-processing takes around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://github.com/peterdsharpe/AeroSandbox/blob/c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/airfoil_families.py#L265), but in theory a pure-NumPy implementation is possible that would be much faster by exploiting linearity (sub-millisecond). If you're interested in working on this, open an issue and let me know! In the meantime, you can eliminate this overhead by using [`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to one of NeuralFoil's other functions.
-
 ## Installation
 
-[Install from PyPI](https://pypi.org/project/NeuralFoil/) with:
-
-`pip install neuralfoil`
+[Install from PyPI](https://pypi.org/project/NeuralFoil/) with `pip install neuralfoil`.
 
 <a name="dependencies-question"></a>
 To run models, NeuralFoil currently requires minimal dependencies:
 
 * Python 3.7+
 * [NumPy](https://numpy.org/)
 * [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) 4.0.10+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.4 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.5 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
@@ -27,51 +27,53 @@
 networks trained on [tens of millions of XFoil runs](#geometry-
 parameterization-and-training-data). NeuralFoil aims to be lightweight, with
 [minimal dependencies](#dependencies-question) and a [tight, efficient code-
 base](./neuralfoil). NeuralFoil is ~10x faster than XFoil for a single
 analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in
 accuracy compared to XFoil](#performance). It also has [many nice features]
 (#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/
-NumPy) that make it much easier to use. ## Overview NeuralFoil comes with 8
-different neural network models, with increasing levels of complexity:
+NumPy) that make it much easier to use. ``` pip install neuralfoil ``` ##
+Overview NeuralFoil comes with 8 different neural network models, with
+increasing levels of complexity:
    "xxsmall" "xsmall" "small" "medium" "large" "xlarge" "xxlarge" "xxxlarge"
 This spectrum offers a tradeoff between accuracy and computational cost. In
 addition to its neural network models, NeuralFoil also has a bonus "Linear
 $C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function
 of angle of attack $\alpha$. This model is well-suited for linear lifting-line
 or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used
 to solve the resulting system of equations "in one shot" as a linear solve,
 rather than a less-numerically-robust iterative nonlinear solve. Using
 NeuralFoil is dead-simple, and also offers several possible "entry points" for
-inputs. Here's an example showing this: ```python import neuralfoil as nf
-import numpy as np aero = nf.get_aero_from_dat_file( # You can use a .dat file
-as an entry point dat_file_path="/path/to/my_airfoil_file.dat", alpha=5, #
-Angle of attack [deg] Re=5e6, # Reynolds number [-] model_size="xlarge", #
-Optionally, specify your model size. ) aero = nf.get_aero_from_coordinates( #
-You can use xy airfoil coordinates as an entry point
-coordinates=n_by_2_numpy_ndarray_of_airfoil_coordinates, alpha=np.linspace(-25,
-25, 1000), # Vectorize your evaluations across `alpha` and `Re` Re=5e6, ) aero
-= nf.get_aero_from_airfoil( # You can AeroSandbox airfoils as an entry point
-airfoil=asb.Airfoil("naca4412"), # `import aerosandbox as asb`, any UIUC or
-NACA airfoil name works alpha=5, Re=5e6, ) # `aero` is a dict with keys: ["CL",
-"CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"] ``` ## Performance Qualitatively,
-NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$
-values. In the figure below, we compare the performance of NeuralFoil to XFoil
-on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was
-developed "from scratch" for a [real-world aircraft development program](https:
-//www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-
-research-aircraft-301633713.html) and is completely separate from [the airfoils
-used during NeuralFoil's training](#geometry-parameterization-and-training-
-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance:
+inputs. Here's an example showing this: ```python import neuralfoil as nf #
+`pip install neuralfoil` import numpy as np aero = nf.get_aero_from_dat_file( #
+You can use a .dat file as an entry point dat_file_path="/path/to/
+my_airfoil_file.dat", alpha=5, # Angle of attack [deg] Re=5e6, # Reynolds
+number [-] model_size="xlarge", # Optionally, specify your model size. ) aero =
+nf.get_aero_from_coordinates( # You can use xy airfoil coordinates as an entry
+point coordinates=n_by_2_numpy_ndarray_of_airfoil_coordinates,
+alpha=np.linspace(-25, 25, 1000), # Vectorize your evaluations across `alpha`
+and `Re` Re=5e6, ) aero = nf.get_aero_from_airfoil( # You can use AeroSandbox
+airfoils as an entry point airfoil=asb.Airfoil("naca4412"), # `import
+aerosandbox as asb`, any UIUC or NACA airfoil name works alpha=5, Re=5e6, ) #
+`aero` is a dictionary with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr",
+"Bot_Xtr"] ``` ## Performance Qualitatively, NeuralFoil tracks XFoil very
+closely across a wide range of $\alpha$ and $Re$ values. In the figure below,
+we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar
+prediction. Notably, the airfoil analyzed here was developed "from scratch" for
+a [real-world aircraft development program](https://www.prnewswire.com/news-
+releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html)
+and is completely separate from [the airfoils used during NeuralFoil's
+training](#geometry-parameterization-and-training-data), so NeuralFoil isn't
+cheating by "memorizing" this airfoil's performance:
                [./benchmarking/neuralfoil_point_validation.svg]
 NeuralFoil is typically accurate to within a few percent of XFoil's
 predictions. Note that this figure is on a truly out-of-sample airfoil, so
-airfoils that are closer to the UIUC-database training set will have even more
-accurate results. NeuralFoil also [has the benefit of smoothing out XFoil's
-"jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at
+airfoils that are closer to the training set will have even more accurate
+results. NeuralFoil also [has the benefit of smoothing out XFoil's "jagged"
+predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at
 $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is
 obviously incorrect, which would otherwise make optimization difficult. In the
 table below, we quantify the performance of the NeuralFoil ("NF") models with
 respect to XFoil more precisely. At a basic level, we care about two things: -
 **Accuracy**: how close are the predictions to XFoil's? - **Computational
 Cost**: how long does it take to run? This table details both of these
 considerations. The first few columns show the error with respect to XFoil on
@@ -127,29 +129,16 @@
 Larger models will be more complicated ("less parsimonious," as the math kids
 would say), which means that they may have more "wiggles" in their
 outputsâthis might be undesirable for gradient-based optimization. On the
 other hand, larger models will be able to capture a wider range of airfoils
 (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-
 optimization), so larger models could have a benefit in that sense. If you try
 a specific application and have better/worse results with a specific model, let
-me know by opening a GitHub issue! Notably, most of the computational overhead
-of calling NeuralFoil is actually in the airfoil preprocessing step, where the
-airfoil is converted from a set of coordinates to a CST (Kulfan)
-parameterization ([more info here](#geometry-parameterization-and-training-
-data)) - not in the aerodynamics analysis itself. This pre-processing takes
-around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://
-github.com/peterdsharpe/AeroSandbox/blob/
-c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/
-airfoil_families.py#L265), but in theory a pure-NumPy implementation is
-possible that would be much faster by exploiting linearity (sub-millisecond).
-If you're interested in working on this, open an issue and let me know! In the
-meantime, you can eliminate this overhead by using
-[`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to
-one of NeuralFoil's other functions. ## Installation [Install from PyPI](https:
-//pypi.org/project/NeuralFoil/) with: `pip install neuralfoil`  To run models,
+me know by opening a GitHub issue! ## Installation [Install from PyPI](https://
+pypi.org/project/NeuralFoil/) with `pip install neuralfoil`.  To run models,
 NeuralFoil currently requires minimal dependencies: * Python 3.7+ * [NumPy]
 (https://numpy.org/) * [AeroSandbox](https://github.com/peterdsharpe/
 AeroSandbox) 4.0.10+ Currently, NeuralFoil only uses AeroSandbox for airfoil
 geometry parameterization (i.e., converting from a set of points to a CST
 parameterization, which is solved as an optimization problem)âthe actual math
 is implemented in pure NumPy. Recent progress on this CST parameterization-
 fitting problem has allowed it to be recast as a least-squares problem, which
```

### Comparing `NeuralFoil-0.1.4/NeuralFoil.egg-info/SOURCES.txt` & `NeuralFoil-0.1.5/NeuralFoil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.4/PKG-INFO` & `NeuralFoil-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.4
+Version: 0.1.5
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
@@ -33,14 +33,18 @@
 
 -----
 
 NeuralFoil is a small Python/NumPy tool for rapid aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/). It is also a small subset of the larger [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here as a standalone. Under the hood, NeuralFoil consists of physics-informed neural networks trained on [tens of millions of XFoil runs](#geometry-parameterization-and-training-data). NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient code-base](./neuralfoil).
 
 NeuralFoil is ~10x faster than XFoil for a single analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in accuracy compared to XFoil](#performance). It also has [many nice features](#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/NumPy) that make it much easier to use.
 
+```
+pip install neuralfoil
+```
+
 ## Overview
 
 NeuralFoil comes with 8 different neural network models, with increasing levels of complexity:
 
 <div align="center">
 	<table>
 	 <tr>
@@ -59,15 +63,15 @@
 This spectrum offers a tradeoff between accuracy and computational cost.
 
 In addition to its neural network models, NeuralFoil also has a bonus "Linear $C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function of angle of attack $\alpha$. This model is well-suited for linear lifting-line or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used to solve the resulting system of equations "in one shot" as a linear solve, rather than a less-numerically-robust iterative nonlinear solve.
 
 Using NeuralFoil is dead-simple, and also offers several possible "entry points" for inputs. Here's an example showing this:
 
 ```python
-import neuralfoil as nf
+import neuralfoil as nf  # `pip install neuralfoil`
 import numpy as np
 
 aero = nf.get_aero_from_dat_file(  # You can use a .dat file as an entry point
     dat_file_path="/path/to/my_airfoil_file.dat",
     alpha=5,  # Angle of attack [deg]
     Re=5e6,  # Reynolds number [-]
     model_size="xlarge",  # Optionally, specify your model size.
@@ -75,32 +79,32 @@
 
 aero = nf.get_aero_from_coordinates(  # You can use xy airfoil coordinates as an entry point
     coordinates=n_by_2_numpy_ndarray_of_airfoil_coordinates,
     alpha=np.linspace(-25, 25, 1000),  # Vectorize your evaluations across `alpha` and `Re`
     Re=5e6,
 )
 
-aero = nf.get_aero_from_airfoil(  # You can AeroSandbox airfoils as an entry point
+aero = nf.get_aero_from_airfoil(  # You can use AeroSandbox airfoils as an entry point
     airfoil=asb.Airfoil("naca4412"),  # `import aerosandbox as asb`, any UIUC or NACA airfoil name works
     alpha=5, Re=5e6,
 )
 
-# `aero` is a dict with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
+# `aero` is a dictionary with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
 ```
 
 ## Performance
 
 Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
 
 <a name="clcd-polar"></a>
 <p align="center">
 	<img src="./benchmarking/neuralfoil_point_validation.svg" width="1000" />
 </p>
 
-NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the UIUC-database training set will have even more accurate results. 
+NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the training set will have even more accurate results. 
 
 NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is obviously incorrect, which would otherwise make optimization difficult. 
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
@@ -113,21 +117,17 @@
 > 
 > ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
 
 Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
-Notably, most of the computational overhead of calling NeuralFoil is actually in the airfoil preprocessing step, where the airfoil is converted from a set of coordinates to a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-and-training-data)) - not in the aerodynamics analysis itself. This pre-processing takes around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://github.com/peterdsharpe/AeroSandbox/blob/c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/airfoil_families.py#L265), but in theory a pure-NumPy implementation is possible that would be much faster by exploiting linearity (sub-millisecond). If you're interested in working on this, open an issue and let me know! In the meantime, you can eliminate this overhead by using [`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to one of NeuralFoil's other functions.
-
 ## Installation
 
-[Install from PyPI](https://pypi.org/project/NeuralFoil/) with:
-
-`pip install neuralfoil`
+[Install from PyPI](https://pypi.org/project/NeuralFoil/) with `pip install neuralfoil`.
 
 <a name="dependencies-question"></a>
 To run models, NeuralFoil currently requires minimal dependencies:
 
 * Python 3.7+
 * [NumPy](https://numpy.org/)
 * [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) 4.0.10+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.4 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.5 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
@@ -27,51 +27,53 @@
 networks trained on [tens of millions of XFoil runs](#geometry-
 parameterization-and-training-data). NeuralFoil aims to be lightweight, with
 [minimal dependencies](#dependencies-question) and a [tight, efficient code-
 base](./neuralfoil). NeuralFoil is ~10x faster than XFoil for a single
 analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in
 accuracy compared to XFoil](#performance). It also has [many nice features]
 (#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/
-NumPy) that make it much easier to use. ## Overview NeuralFoil comes with 8
-different neural network models, with increasing levels of complexity:
+NumPy) that make it much easier to use. ``` pip install neuralfoil ``` ##
+Overview NeuralFoil comes with 8 different neural network models, with
+increasing levels of complexity:
    "xxsmall" "xsmall" "small" "medium" "large" "xlarge" "xxlarge" "xxxlarge"
 This spectrum offers a tradeoff between accuracy and computational cost. In
 addition to its neural network models, NeuralFoil also has a bonus "Linear
 $C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function
 of angle of attack $\alpha$. This model is well-suited for linear lifting-line
 or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used
 to solve the resulting system of equations "in one shot" as a linear solve,
 rather than a less-numerically-robust iterative nonlinear solve. Using
 NeuralFoil is dead-simple, and also offers several possible "entry points" for
-inputs. Here's an example showing this: ```python import neuralfoil as nf
-import numpy as np aero = nf.get_aero_from_dat_file( # You can use a .dat file
-as an entry point dat_file_path="/path/to/my_airfoil_file.dat", alpha=5, #
-Angle of attack [deg] Re=5e6, # Reynolds number [-] model_size="xlarge", #
-Optionally, specify your model size. ) aero = nf.get_aero_from_coordinates( #
-You can use xy airfoil coordinates as an entry point
-coordinates=n_by_2_numpy_ndarray_of_airfoil_coordinates, alpha=np.linspace(-25,
-25, 1000), # Vectorize your evaluations across `alpha` and `Re` Re=5e6, ) aero
-= nf.get_aero_from_airfoil( # You can AeroSandbox airfoils as an entry point
-airfoil=asb.Airfoil("naca4412"), # `import aerosandbox as asb`, any UIUC or
-NACA airfoil name works alpha=5, Re=5e6, ) # `aero` is a dict with keys: ["CL",
-"CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"] ``` ## Performance Qualitatively,
-NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$
-values. In the figure below, we compare the performance of NeuralFoil to XFoil
-on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was
-developed "from scratch" for a [real-world aircraft development program](https:
-//www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-
-research-aircraft-301633713.html) and is completely separate from [the airfoils
-used during NeuralFoil's training](#geometry-parameterization-and-training-
-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance:
+inputs. Here's an example showing this: ```python import neuralfoil as nf #
+`pip install neuralfoil` import numpy as np aero = nf.get_aero_from_dat_file( #
+You can use a .dat file as an entry point dat_file_path="/path/to/
+my_airfoil_file.dat", alpha=5, # Angle of attack [deg] Re=5e6, # Reynolds
+number [-] model_size="xlarge", # Optionally, specify your model size. ) aero =
+nf.get_aero_from_coordinates( # You can use xy airfoil coordinates as an entry
+point coordinates=n_by_2_numpy_ndarray_of_airfoil_coordinates,
+alpha=np.linspace(-25, 25, 1000), # Vectorize your evaluations across `alpha`
+and `Re` Re=5e6, ) aero = nf.get_aero_from_airfoil( # You can use AeroSandbox
+airfoils as an entry point airfoil=asb.Airfoil("naca4412"), # `import
+aerosandbox as asb`, any UIUC or NACA airfoil name works alpha=5, Re=5e6, ) #
+`aero` is a dictionary with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr",
+"Bot_Xtr"] ``` ## Performance Qualitatively, NeuralFoil tracks XFoil very
+closely across a wide range of $\alpha$ and $Re$ values. In the figure below,
+we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar
+prediction. Notably, the airfoil analyzed here was developed "from scratch" for
+a [real-world aircraft development program](https://www.prnewswire.com/news-
+releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html)
+and is completely separate from [the airfoils used during NeuralFoil's
+training](#geometry-parameterization-and-training-data), so NeuralFoil isn't
+cheating by "memorizing" this airfoil's performance:
                [./benchmarking/neuralfoil_point_validation.svg]
 NeuralFoil is typically accurate to within a few percent of XFoil's
 predictions. Note that this figure is on a truly out-of-sample airfoil, so
-airfoils that are closer to the UIUC-database training set will have even more
-accurate results. NeuralFoil also [has the benefit of smoothing out XFoil's
-"jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at
+airfoils that are closer to the training set will have even more accurate
+results. NeuralFoil also [has the benefit of smoothing out XFoil's "jagged"
+predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at
 $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is
 obviously incorrect, which would otherwise make optimization difficult. In the
 table below, we quantify the performance of the NeuralFoil ("NF") models with
 respect to XFoil more precisely. At a basic level, we care about two things: -
 **Accuracy**: how close are the predictions to XFoil's? - **Computational
 Cost**: how long does it take to run? This table details both of these
 considerations. The first few columns show the error with respect to XFoil on
@@ -127,29 +129,16 @@
 Larger models will be more complicated ("less parsimonious," as the math kids
 would say), which means that they may have more "wiggles" in their
 outputsâthis might be undesirable for gradient-based optimization. On the
 other hand, larger models will be able to capture a wider range of airfoils
 (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-
 optimization), so larger models could have a benefit in that sense. If you try
 a specific application and have better/worse results with a specific model, let
-me know by opening a GitHub issue! Notably, most of the computational overhead
-of calling NeuralFoil is actually in the airfoil preprocessing step, where the
-airfoil is converted from a set of coordinates to a CST (Kulfan)
-parameterization ([more info here](#geometry-parameterization-and-training-
-data)) - not in the aerodynamics analysis itself. This pre-processing takes
-around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://
-github.com/peterdsharpe/AeroSandbox/blob/
-c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/
-airfoil_families.py#L265), but in theory a pure-NumPy implementation is
-possible that would be much faster by exploiting linearity (sub-millisecond).
-If you're interested in working on this, open an issue and let me know! In the
-meantime, you can eliminate this overhead by using
-[`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to
-one of NeuralFoil's other functions. ## Installation [Install from PyPI](https:
-//pypi.org/project/NeuralFoil/) with: `pip install neuralfoil`  To run models,
+me know by opening a GitHub issue! ## Installation [Install from PyPI](https://
+pypi.org/project/NeuralFoil/) with `pip install neuralfoil`.  To run models,
 NeuralFoil currently requires minimal dependencies: * Python 3.7+ * [NumPy]
 (https://numpy.org/) * [AeroSandbox](https://github.com/peterdsharpe/
 AeroSandbox) 4.0.10+ Currently, NeuralFoil only uses AeroSandbox for airfoil
 geometry parameterization (i.e., converting from a set of points to a CST
 parameterization, which is solved as an optimization problem)âthe actual math
 is implemented in pure NumPy. Recent progress on this CST parameterization-
 fitting problem has allowed it to be recast as a least-squares problem, which
```

### Comparing `NeuralFoil-0.1.4/README.md` & `NeuralFoil-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 -----
 
 NeuralFoil is a small Python/NumPy tool for rapid aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/). It is also a small subset of the larger [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) package, but it is offered here as a standalone. Under the hood, NeuralFoil consists of physics-informed neural networks trained on [tens of millions of XFoil runs](#geometry-parameterization-and-training-data). NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient code-base](./neuralfoil).
 
 NeuralFoil is ~10x faster than XFoil for a single analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in accuracy compared to XFoil](#performance). It also has [many nice features](#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/NumPy) that make it much easier to use.
 
+```
+pip install neuralfoil
+```
+
 ## Overview
 
 NeuralFoil comes with 8 different neural network models, with increasing levels of complexity:
 
 <div align="center">
 	<table>
 	 <tr>
@@ -37,15 +41,15 @@
 This spectrum offers a tradeoff between accuracy and computational cost.
 
 In addition to its neural network models, NeuralFoil also has a bonus "Linear $C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function of angle of attack $\alpha$. This model is well-suited for linear lifting-line or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used to solve the resulting system of equations "in one shot" as a linear solve, rather than a less-numerically-robust iterative nonlinear solve.
 
 Using NeuralFoil is dead-simple, and also offers several possible "entry points" for inputs. Here's an example showing this:
 
 ```python
-import neuralfoil as nf
+import neuralfoil as nf  # `pip install neuralfoil`
 import numpy as np
 
 aero = nf.get_aero_from_dat_file(  # You can use a .dat file as an entry point
     dat_file_path="/path/to/my_airfoil_file.dat",
     alpha=5,  # Angle of attack [deg]
     Re=5e6,  # Reynolds number [-]
     model_size="xlarge",  # Optionally, specify your model size.
@@ -53,32 +57,32 @@
 
 aero = nf.get_aero_from_coordinates(  # You can use xy airfoil coordinates as an entry point
     coordinates=n_by_2_numpy_ndarray_of_airfoil_coordinates,
     alpha=np.linspace(-25, 25, 1000),  # Vectorize your evaluations across `alpha` and `Re`
     Re=5e6,
 )
 
-aero = nf.get_aero_from_airfoil(  # You can AeroSandbox airfoils as an entry point
+aero = nf.get_aero_from_airfoil(  # You can use AeroSandbox airfoils as an entry point
     airfoil=asb.Airfoil("naca4412"),  # `import aerosandbox as asb`, any UIUC or NACA airfoil name works
     alpha=5, Re=5e6,
 )
 
-# `aero` is a dict with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
+# `aero` is a dictionary with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
 ```
 
 ## Performance
 
 Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
 
 <a name="clcd-polar"></a>
 <p align="center">
 	<img src="./benchmarking/neuralfoil_point_validation.svg" width="1000" />
 </p>
 
-NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the UIUC-database training set will have even more accurate results. 
+NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the training set will have even more accurate results. 
 
 NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is obviously incorrect, which would otherwise make optimization difficult. 
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
@@ -91,21 +95,17 @@
 > 
 > ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
 
 Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
-Notably, most of the computational overhead of calling NeuralFoil is actually in the airfoil preprocessing step, where the airfoil is converted from a set of coordinates to a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-and-training-data)) - not in the aerodynamics analysis itself. This pre-processing takes around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://github.com/peterdsharpe/AeroSandbox/blob/c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/airfoil_families.py#L265), but in theory a pure-NumPy implementation is possible that would be much faster by exploiting linearity (sub-millisecond). If you're interested in working on this, open an issue and let me know! In the meantime, you can eliminate this overhead by using [`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to one of NeuralFoil's other functions.
-
 ## Installation
 
-[Install from PyPI](https://pypi.org/project/NeuralFoil/) with:
-
-`pip install neuralfoil`
+[Install from PyPI](https://pypi.org/project/NeuralFoil/) with `pip install neuralfoil`.
 
 <a name="dependencies-question"></a>
 To run models, NeuralFoil currently requires minimal dependencies:
 
 * Python 3.7+
 * [NumPy](https://numpy.org/)
 * [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) 4.0.10+
@@ -200,8 +200,8 @@
 @misc{neuralfoil,
   author = {Peter Sharpe},
   title = {{NeuralFoil}: An airfoil aerodynamics analysis tool using physics-informed machine learning},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/peterdsharpe/NeuralFoil}},
-```
+```
```

#### html2text {}

```diff
@@ -13,51 +13,53 @@
 networks trained on [tens of millions of XFoil runs](#geometry-
 parameterization-and-training-data). NeuralFoil aims to be lightweight, with
 [minimal dependencies](#dependencies-question) and a [tight, efficient code-
 base](./neuralfoil). NeuralFoil is ~10x faster than XFoil for a single
 analysis, and ~1000x faster for multipoint analysis, all with [minimal loss in
 accuracy compared to XFoil](#performance). It also has [many nice features]
 (#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python/
-NumPy) that make it much easier to use. ## Overview NeuralFoil comes with 8
-different neural network models, with increasing levels of complexity:
+NumPy) that make it much easier to use. ``` pip install neuralfoil ``` ##
+Overview NeuralFoil comes with 8 different neural network models, with
+increasing levels of complexity:
    "xxsmall" "xsmall" "small" "medium" "large" "xlarge" "xxlarge" "xxxlarge"
 This spectrum offers a tradeoff between accuracy and computational cost. In
 addition to its neural network models, NeuralFoil also has a bonus "Linear
 $C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function
 of angle of attack $\alpha$. This model is well-suited for linear lifting-line
 or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used
 to solve the resulting system of equations "in one shot" as a linear solve,
 rather than a less-numerically-robust iterative nonlinear solve. Using
 NeuralFoil is dead-simple, and also offers several possible "entry points" for
-inputs. Here's an example showing this: ```python import neuralfoil as nf
-import numpy as np aero = nf.get_aero_from_dat_file( # You can use a .dat file
-as an entry point dat_file_path="/path/to/my_airfoil_file.dat", alpha=5, #
-Angle of attack [deg] Re=5e6, # Reynolds number [-] model_size="xlarge", #
-Optionally, specify your model size. ) aero = nf.get_aero_from_coordinates( #
-You can use xy airfoil coordinates as an entry point
-coordinates=n_by_2_numpy_ndarray_of_airfoil_coordinates, alpha=np.linspace(-25,
-25, 1000), # Vectorize your evaluations across `alpha` and `Re` Re=5e6, ) aero
-= nf.get_aero_from_airfoil( # You can AeroSandbox airfoils as an entry point
-airfoil=asb.Airfoil("naca4412"), # `import aerosandbox as asb`, any UIUC or
-NACA airfoil name works alpha=5, Re=5e6, ) # `aero` is a dict with keys: ["CL",
-"CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"] ``` ## Performance Qualitatively,
-NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$
-values. In the figure below, we compare the performance of NeuralFoil to XFoil
-on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was
-developed "from scratch" for a [real-world aircraft development program](https:
-//www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-
-research-aircraft-301633713.html) and is completely separate from [the airfoils
-used during NeuralFoil's training](#geometry-parameterization-and-training-
-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance:
+inputs. Here's an example showing this: ```python import neuralfoil as nf #
+`pip install neuralfoil` import numpy as np aero = nf.get_aero_from_dat_file( #
+You can use a .dat file as an entry point dat_file_path="/path/to/
+my_airfoil_file.dat", alpha=5, # Angle of attack [deg] Re=5e6, # Reynolds
+number [-] model_size="xlarge", # Optionally, specify your model size. ) aero =
+nf.get_aero_from_coordinates( # You can use xy airfoil coordinates as an entry
+point coordinates=n_by_2_numpy_ndarray_of_airfoil_coordinates,
+alpha=np.linspace(-25, 25, 1000), # Vectorize your evaluations across `alpha`
+and `Re` Re=5e6, ) aero = nf.get_aero_from_airfoil( # You can use AeroSandbox
+airfoils as an entry point airfoil=asb.Airfoil("naca4412"), # `import
+aerosandbox as asb`, any UIUC or NACA airfoil name works alpha=5, Re=5e6, ) #
+`aero` is a dictionary with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr",
+"Bot_Xtr"] ``` ## Performance Qualitatively, NeuralFoil tracks XFoil very
+closely across a wide range of $\alpha$ and $Re$ values. In the figure below,
+we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar
+prediction. Notably, the airfoil analyzed here was developed "from scratch" for
+a [real-world aircraft development program](https://www.prnewswire.com/news-
+releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html)
+and is completely separate from [the airfoils used during NeuralFoil's
+training](#geometry-parameterization-and-training-data), so NeuralFoil isn't
+cheating by "memorizing" this airfoil's performance:
                [./benchmarking/neuralfoil_point_validation.svg]
 NeuralFoil is typically accurate to within a few percent of XFoil's
 predictions. Note that this figure is on a truly out-of-sample airfoil, so
-airfoils that are closer to the UIUC-database training set will have even more
-accurate results. NeuralFoil also [has the benefit of smoothing out XFoil's
-"jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at
+airfoils that are closer to the training set will have even more accurate
+results. NeuralFoil also [has the benefit of smoothing out XFoil's "jagged"
+predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at
 $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is
 obviously incorrect, which would otherwise make optimization difficult. In the
 table below, we quantify the performance of the NeuralFoil ("NF") models with
 respect to XFoil more precisely. At a basic level, we care about two things: -
 **Accuracy**: how close are the predictions to XFoil's? - **Computational
 Cost**: how long does it take to run? This table details both of these
 considerations. The first few columns show the error with respect to XFoil on
@@ -113,29 +115,16 @@
 Larger models will be more complicated ("less parsimonious," as the math kids
 would say), which means that they may have more "wiggles" in their
 outputsâthis might be undesirable for gradient-based optimization. On the
 other hand, larger models will be able to capture a wider range of airfoils
 (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-
 optimization), so larger models could have a benefit in that sense. If you try
 a specific application and have better/worse results with a specific model, let
-me know by opening a GitHub issue! Notably, most of the computational overhead
-of calling NeuralFoil is actually in the airfoil preprocessing step, where the
-airfoil is converted from a set of coordinates to a CST (Kulfan)
-parameterization ([more info here](#geometry-parameterization-and-training-
-data)) - not in the aerodynamics analysis itself. This pre-processing takes
-around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://
-github.com/peterdsharpe/AeroSandbox/blob/
-c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/
-airfoil_families.py#L265), but in theory a pure-NumPy implementation is
-possible that would be much faster by exploiting linearity (sub-millisecond).
-If you're interested in working on this, open an issue and let me know! In the
-meantime, you can eliminate this overhead by using
-[`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to
-one of NeuralFoil's other functions. ## Installation [Install from PyPI](https:
-//pypi.org/project/NeuralFoil/) with: `pip install neuralfoil`  To run models,
+me know by opening a GitHub issue! ## Installation [Install from PyPI](https://
+pypi.org/project/NeuralFoil/) with `pip install neuralfoil`.  To run models,
 NeuralFoil currently requires minimal dependencies: * Python 3.7+ * [NumPy]
 (https://numpy.org/) * [AeroSandbox](https://github.com/peterdsharpe/
 AeroSandbox) 4.0.10+ Currently, NeuralFoil only uses AeroSandbox for airfoil
 geometry parameterization (i.e., converting from a set of points to a CST
 parameterization, which is solved as an optimization problem)âthe actual math
 is implemented in pure NumPy. Recent progress on this CST parameterization-
 fitting problem has allowed it to be recast as a least-squares problem, which
```

### Comparing `NeuralFoil-0.1.4/neuralfoil/CL_linear_regression.py` & `NeuralFoil-0.1.5/neuralfoil/CL_linear_regression.py`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.4/neuralfoil/neuralfoil.py` & `NeuralFoil-0.1.5/neuralfoil/neuralfoil.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
         Re: Union[float, np.ndarray],
         model_size="large"
 ) -> Dict[str, Union[float, np.ndarray]]:
 
     ### Load the neural network parameters
     filename = npz_file_directory / f"nn-{model_size}.npz"
     if not filename.exists():
-        raise FileNotFoundError(f"Could not find the neural network file {filename}, which contains the weights and biases.")
+        raise FileNotFoundError(
+            f"Could not find the neural network file {filename}, which contains the weights and biases.")
 
     data: Dict[str, np.ndarray] = np.load(filename)
 
     ### Prepare the inputs for the neural network
     input_rows: List[Union[float, np.ndarray]] = [
         4 * np.sind(2 * alpha),
         20 * (1 - np.cosd(alpha) ** 2),
@@ -99,54 +100,58 @@
         input_rows_flipped[i] = np.ones(N_cases) * row
 
     x_flipped = np.stack(input_rows_flipped, axis=0)
 
     y_flipped = net(x_flipped)
 
     ### The resulting outputs will also be flipped, so we need to flip them back to their normal orientation
-    y_flipped = np.stack([
-        -y_flipped[0, :],  # "CL"
-        y_flipped[1, :],  # "ln_CD + 4"
-        -y_flipped[2, :],  # "CM * 20"
-        y_flipped[3, :],  # "u_max_over_u - 1"
-        y_flipped[5, :],  # "Top_Xtr" (flipped with bot)
-        y_flipped[4, :],  # "Bot_Xtr" (flipped with top)
-    ])
+    y_flipped = y_flipped * np.array([
+        -1,  # "CL"
+        1,  # "ln_CD + 4"
+        -1,  # "CM * 20"
+        1,  # "u_max_over_u - 1"
+        1,  # "Top_Xtr" (flipped with bot)
+        1,  # "Bot_Xtr" (flipped with top)
+    ]).reshape((-1, 1))
 
     ### Then, average the two outputs to get the "symmetric" result
     y = (y + y_flipped) / 2
 
     # Unpack the neural network outputs
-    return {
+    results = {
         "CL"     : y[0, :],
         "CD"     : np.exp(y[1, :] - 4),
         "CM"     : y[2, :] / 20,
         "Cpmin"  : 1 - y[3, :] ** 2,
         "Top_Xtr": y[4, :],
         "Bot_Xtr": y[5, :],
     }
+    return {key: np.reshape(value, -1) for key, value in results.items()}
 
 
 def get_aero_from_airfoil(
         airfoil: asb.Airfoil,
         alpha: Union[float, np.ndarray],
         Re: Union[float, np.ndarray],
         model_size="large",
 ) -> Dict[str, Union[float, np.ndarray]]:
+
+    airfoil_normalization = airfoil.normalize(return_dict=True)
+
     from aerosandbox.geometry.airfoil.airfoil_families import get_kulfan_parameters
 
     kulfan_parameters = get_kulfan_parameters(
-        airfoil.coordinates,
+        airfoil_normalization["airfoil"].coordinates,
         n_weights_per_side=8
     )
 
     return get_aero_from_kulfan_parameters(
         kulfan_parameters=kulfan_parameters,
-        alpha=alpha,
-        Re=Re,
+        alpha=alpha + airfoil_normalization["rotation_angle"],
+        Re=Re / airfoil_normalization["scale_factor"],
         model_size=model_size
     )
 
 
 def get_aero_from_coordinates(
         coordinates: np.ndarray,
         alpha: Union[float, np.ndarray],
@@ -179,15 +184,16 @@
         Re=Re,
         model_size=model_size
     )
 
 
 if __name__ == '__main__':
 
-    airfoil = asb.Airfoil("dae11").repanel().normalize()
+    # airfoil = asb.Airfoil("dae11").repanel().normalize()
+    airfoil = asb.Airfoil("naca0012").add_control_surface(10, hinge_point_x=0.5)
 
     alpha = np.linspace(-15, 15, 100)
     Re = 1e6
 
     aeros = {}
 
     for model_size in ["xxsmall", "xsmall", "small", "medium", "large", "xlarge", "xxlarge", "xxxlarge"]:
@@ -240,10 +246,11 @@
     ax[1, 0].set_ylabel("$C_M$")
 
     ax[1, 1].set_xlabel("$C_D$")
     ax[1, 1].set_ylabel("$C_L$")
     ax[1, 1].set_xlim(left=0)
 
     from aerosandbox.tools.string_formatting import eng_string
+
     plt.suptitle(f"\"{airfoil.name}\" Airfoil at $Re_c = \\mathrm{{{eng_string(Re)}}}$")
 
     p.show_plot()
```

### Comparing `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-large.npz` & `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-large.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-medium.npz` & `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-medium.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-small.npz` & `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-small.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xlarge.npz` & `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xsmall.npz` & `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xsmall.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz` & `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz` & `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz` & `NeuralFoil-0.1.5/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.4/setup.py` & `NeuralFoil-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         'Programming Language :: Python :: 3',
     ],
     keywords='python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network',
     packages=["neuralfoil"],  # find_packages(exclude=['docs', 'media', 'examples', 'studies'])
     python_requires='>=3.7',
     install_requires=[
         'numpy >= 1',
-        'aerosandbox >= 4.0.10'
+        'aerosandbox >= 4.0.11'
     ],
     extras_require={
         "training": [
             'torch',
             'ray',
             'polars',
             'tqdm'
```

