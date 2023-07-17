# Comparing `tmp/adbench-0.0.4.tar.gz` & `tmp/adbench-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\adbench-0.0.4.tar", last modified: Tue Jul 11 10:13:14 2023, max compression
+gzip compressed data, was "dist\adbench-0.1.0.tar", last modified: Mon Jul 17 15:38:09 2023, max compression
```

## Comparing `adbench-0.0.4.tar` & `adbench-0.1.0.tar`

### file list

```diff
@@ -1,151 +1,139 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/
--rw-rw-rw-   0        0        0      187 2023-07-08 02:17:37.000000 adbench-0.0.4/.gitattributes
--rw-rw-rw-   0        0        0       69 2023-07-08 02:17:37.000000 adbench-0.0.4/.gitignore
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/.idea/
--rw-rw-rw-   0        0        0      184 2023-07-08 02:17:37.000000 adbench-0.0.4/.idea/.gitignore
--rw-rw-rw-   0        0        0      334 2023-07-11 05:42:23.000000 adbench-0.0.4/.idea/ADBench.iml
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      179 2023-07-08 02:17:37.000000 adbench-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      198 2023-07-11 05:42:23.000000 adbench-0.0.4/.idea/misc.xml
--rw-rw-rw-   0        0        0      273 2023-07-08 02:17:37.000000 adbench-0.0.4/.idea/modules.xml
--rw-rw-rw-   0        0        0      185 2023-07-08 02:17:37.000000 adbench-0.0.4/.idea/vcs.xml
--rw-rw-rw-   0        0        0     1349 2023-07-08 02:17:37.000000 adbench-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       77 2023-07-08 02:17:37.000000 adbench-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      950 2023-07-11 10:13:14.000000 adbench-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    21380 2023-07-11 08:28:24.000000 adbench-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/adbench/
--rw-rw-rw-   0        0        0        0 2023-07-11 01:14:34.000000 adbench-0.0.4/adbench/__init__.py
--rw-rw-rw-   0        0        0    11421 2023-07-08 02:17:46.000000 adbench-0.0.4/adbench/myutils.py
--rw-rw-rw-   0        0        0    13264 2023-07-11 09:40:24.000000 adbench-0.0.4/adbench/run.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/adbench.egg-info/
--rw-rw-rw-   0        0        0      950 2023-07-11 10:13:01.000000 adbench-0.0.4/adbench.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3683 2023-07-11 10:13:14.000000 adbench-0.0.4/adbench.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 10:13:01.000000 adbench-0.0.4/adbench.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-11 10:13:01.000000 adbench-0.0.4/adbench.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-11 10:13:01.000000 adbench-0.0.4/adbench.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DAGMM/
--rw-rw-rw-   0        0        0        8 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/.gitignore
--rw-rw-rw-   0        0        0     3287 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/forward_step.py
--rw-rw-rw-   0        0        0     1895 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/main.py
--rw-rw-rw-   0        0        0     1775 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/model.py
--rw-rw-rw-   0        0        0     2003 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/preprocess.py
--rw-rw-rw-   0        0        0     4193 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/DAGMM/run.py
--rw-rw-rw-   0        0        0     5411 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/test.py
--rw-rw-rw-   0        0        0     1983 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/train.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DAGMM/utils/
--rw-rw-rw-   0        0        0      528 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DAGMM/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/
--rw-rw-rw-   0        0        0     1087 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/LICENSE
--rw-rw-rw-   0        0        0     6935 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/README.md
--rw-rw-rw-   0        0        0      138 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/ae_results.json
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/imgs/
--rw-rw-rw-   0        0        0   319030 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/imgs/fig1.png
--rw-rw-rw-   0        0        0   104296 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/log.txt
--rw-rw-rw-   0        0        0      298 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/requirements.txt
--rw-rw-rw-   0        0        0    16944 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/results.json
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/base/
--rw-rw-rw-   0        0        0      148 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/__init__.py
--rw-rw-rw-   0        0        0     1032 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/base_dataset.py
--rw-rw-rw-   0        0        0      823 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/base_net.py
--rw-rw-rw-   0        0        0     1166 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/base_trainer.py
--rw-rw-rw-   0        0        0     1682 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/odds_dataset.py
--rw-rw-rw-   0        0        0      846 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/base/torchvision_dataset.py
--rw-rw-rw-   0        0        0    13565 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baseline_SemiDGM.py
--rw-rw-rw-   0        0        0     9937 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baseline_isoforest.py
--rw-rw-rw-   0        0        0     9478 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baseline_kde.py
--rw-rw-rw-   0        0        0     9062 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baseline_ocsvm.py
--rw-rw-rw-   0        0        0     9157 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baseline_ssad.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/
--rw-rw-rw-   0        0        0     5610 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/SemiDGM.py
--rw-rw-rw-   0        0        0      202 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/__init__.py
--rw-rw-rw-   0        0        0     5879 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/isoforest.py
--rw-rw-rw-   0        0        0     6702 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/kde.py
--rw-rw-rw-   0        0        0     9033 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/ocsvm.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/shallow_ssad/
--rw-rw-rw-   0        0        0       37 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/shallow_ssad/__init__.py
--rw-rw-rw-   0        0        0     8022 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py
--rw-rw-rw-   0        0        0    10201 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/baselines/ssad.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/
--rw-rw-rw-   0        0        0      215 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/__init__.py
--rw-rw-rw-   0        0        0     3609 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/cifar10.py
--rw-rw-rw-   0        0        0     3663 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/fmnist.py
--rw-rw-rw-   0        0        0      325 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/main.py
--rw-rw-rw-   0        0        0     3598 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/mnist.py
--rw-rw-rw-   0        0        0     1468 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/odds.py
--rw-rw-rw-   0        0        0     3629 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/datasets/preprocessing.py
--rw-rw-rw-   0        0        0     7051 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/deepsad.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/
--rw-rw-rw-   0        0        0      706 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/__init__.py
--rw-rw-rw-   0        0        0     3085 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/cifar10_LeNet.py
--rw-rw-rw-   0        0        0     4405 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/dgm.py
--rw-rw-rw-   0        0        0     2584 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/fmnist_LeNet.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/inference/
--rw-rw-rw-   0        0        0     1256 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/inference/distributions.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/layers/
--rw-rw-rw-   0        0        0     1705 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/layers/standard.py
--rw-rw-rw-   0        0        0     1511 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/layers/stochastic.py
--rw-rw-rw-   0        0        0     1501 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/main.py
--rw-rw-rw-   0        0        0     2328 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/mlp.py
--rw-rw-rw-   0        0        0     2222 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/mnist_LeNet.py
--rw-rw-rw-   0        0        0     4826 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/networks/vae.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/
--rw-rw-rw-   0        0        0     7116 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/DeepSAD_trainer.py
--rw-rw-rw-   0        0        0     7554 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/SemiDGM_trainer.py
--rw-rw-rw-   0        0        0      230 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/__init__.py
--rw-rw-rw-   0        0        0     5379 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/ae_trainer.py
--rw-rw-rw-   0        0        0     5247 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/vae_trainer.py
--rw-rw-rw-   0        0        0     2816 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/optim/variational.py
--rw-rw-rw-   0        0        0     4957 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/DeepSAD/src/run.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/
--rw-rw-rw-   0        0        0      163 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/__init__.py
--rw-rw-rw-   0        0        0      682 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/config.py
--rw-rw-rw-   0        0        0     1468 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/misc.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/visualization/
--rw-rw-rw-   0        0        0      803 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/DevNet/
--rw-rw-rw-   0        0        0    10544 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/DevNet/run.py
--rw-rw-rw-   0        0        0     2367 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/DevNet/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/FEAWAD/
--rw-rw-rw-   0        0        0    18593 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/FEAWAD/run.py
--rw-rw-rw-   0        0        0     1533 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/FEAWAD/toolsdev.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/FTTransformer/
--rw-rw-rw-   0        0        0     6098 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/FTTransformer/run.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/GANomaly/
--rw-rw-rw-   0        0        0     3001 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/GANomaly/fit.py
--rw-rw-rw-   0        0        0     1260 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/GANomaly/model.py
--rw-rw-rw-   0        0        0     3005 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/GANomaly/run.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/PReNet/
--rw-rw-rw-   0        0        0     1219 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/PReNet/fit.py
--rw-rw-rw-   0        0        0      703 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/PReNet/model.py
--rw-rw-rw-   0        0        0     2936 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/PReNet/run.py
--rw-rw-rw-   0        0        0     2931 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/PReNet/utils.py
--rw-rw-rw-   0        0        0    13241 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/PyOD.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/baseline/REPEN/
--rw-rw-rw-   0        0        0    12601 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/REPEN/model.py
--rw-rw-rw-   0        0        0     1680 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/REPEN/run.py
--rw-rw-rw-   0        0        0     2011 2023-07-08 02:17:37.000000 adbench-0.0.4/baseline/REPEN/utils.py
--rw-rw-rw-   0        0        0     1491 2023-07-11 01:16:07.000000 adbench-0.0.4/baseline/Supervised.py
--rw-rw-rw-   0        0        0        0 2023-07-11 01:13:54.000000 adbench-0.0.4/baseline/__init__.py
--rw-rw-rw-   0        0        0   342901 2023-07-11 08:43:19.000000 adbench-0.0.4/demo.ipynb
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/figs/
--rw-rw-rw-   0        0        0   211827 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/ADBench.png
--rw-rw-rw-   0        0        0   211827 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/ADBenchV2.png
--rw-rw-rw-   0        0        0   654664 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/Algorithms.png
--rw-rw-rw-   0        0        0   318580 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/MNIST-C.png
--rw-rw-rw-   0        0        0   238201 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/MVTec-AD(ViT).png
--rw-rw-rw-   0        0        0   238487 2023-07-08 02:17:46.000000 adbench-0.0.4/figs/MVTec-AD.png
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/other_utils/
-drwxrwxrwx   0        0        0        0 2023-07-11 10:13:14.000000 adbench-0.0.4/other_utils/gmm/
--rw-rw-rw-   0        0        0     1090 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/LICENSE.md
--rw-rw-rw-   0        0        0      863 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/README.md
--rw-rw-rw-   0        0        0   131595 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/example.png
--rw-rw-rw-   0        0        0     2111 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/example.py
--rw-rw-rw-   0        0        0    19852 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/gmm.py
--rw-rw-rw-   0        0        0     6856 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/test.py
--rw-rw-rw-   0        0        0     1129 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/gmm/utils.py
--rw-rw-rw-   0        0        0    14138 2023-07-08 02:17:46.000000 adbench-0.0.4/other_utils/utils.py
--rw-rw-rw-   0        0        0      125 2023-07-11 10:11:50.000000 adbench-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 10:13:14.000000 adbench-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1392 2023-07-11 10:12:56.000000 adbench-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:09.000000 adbench-0.1.0/
+-rw-rw-rw-   0        0        0     1349 2023-07-08 02:17:37.000000 adbench-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       79 2023-07-17 08:18:24.000000 adbench-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      950 2023-07-17 15:38:09.000000 adbench-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    22048 2023-07-17 11:22:03.000000 adbench-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/
+-rw-rw-rw-   0        0        0       79 2023-07-17 11:51:08.000000 adbench-0.1.0/adbench/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DAGMM/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/DAGMM/__init__.py
+-rw-rw-rw-   0        0        0     3287 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DAGMM/forward_step.py
+-rw-rw-rw-   0        0        0     1941 2023-07-17 12:11:45.000000 adbench-0.1.0/adbench/baseline/DAGMM/main.py
+-rw-rw-rw-   0        0        0     1775 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DAGMM/model.py
+-rw-rw-rw-   0        0        0     2003 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DAGMM/preprocess.py
+-rw-rw-rw-   0        0        0     4209 2023-07-17 12:11:45.000000 adbench-0.1.0/adbench/baseline/DAGMM/run.py
+-rw-rw-rw-   0        0        0     5384 2023-07-12 01:46:26.000000 adbench-0.1.0/adbench/baseline/DAGMM/test.py
+-rw-rw-rw-   0        0        0     1915 2023-07-17 12:11:45.000000 adbench-0.1.0/adbench/baseline/DAGMM/train.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DAGMM/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/DAGMM/utils/__init__.py
+-rw-rw-rw-   0        0        0      528 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DAGMM/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DeepSAD/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/DeepSAD/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/base/
+-rw-rw-rw-   0        0        0      148 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/base/__init__.py
+-rw-rw-rw-   0        0        0     1032 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/base/base_dataset.py
+-rw-rw-rw-   0        0        0      823 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/base/base_net.py
+-rw-rw-rw-   0        0        0     1166 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/base/base_trainer.py
+-rw-rw-rw-   0        0        0     1682 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/base/odds_dataset.py
+-rw-rw-rw-   0        0        0      846 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/base/torchvision_dataset.py
+-rw-rw-rw-   0        0        0    13565 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baseline_SemiDGM.py
+-rw-rw-rw-   0        0        0     9937 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baseline_isoforest.py
+-rw-rw-rw-   0        0        0     9478 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baseline_kde.py
+-rw-rw-rw-   0        0        0     9062 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baseline_ocsvm.py
+-rw-rw-rw-   0        0        0     9157 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baseline_ssad.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/
+-rw-rw-rw-   0        0        0     5610 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/SemiDGM.py
+-rw-rw-rw-   0        0        0      202 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/__init__.py
+-rw-rw-rw-   0        0        0     5879 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/isoforest.py
+-rw-rw-rw-   0        0        0     6702 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/kde.py
+-rw-rw-rw-   0        0        0     9033 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/ocsvm.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/
+-rw-rw-rw-   0        0        0       37 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/__init__.py
+-rw-rw-rw-   0        0        0     8022 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py
+-rw-rw-rw-   0        0        0    10201 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/ssad.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/
+-rw-rw-rw-   0        0        0      215 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3609 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/cifar10.py
+-rw-rw-rw-   0        0        0     3663 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/fmnist.py
+-rw-rw-rw-   0        0        0      325 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/main.py
+-rw-rw-rw-   0        0        0     3606 2023-07-12 01:46:27.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/mnist.py
+-rw-rw-rw-   0        0        0     1389 2023-07-12 01:46:27.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/odds.py
+-rw-rw-rw-   0        0        0     3629 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/preprocessing.py
+-rw-rw-rw-   0        0        0     7054 2023-07-12 01:46:27.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/deepsad.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/
+-rw-rw-rw-   0        0        0      706 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/__init__.py
+-rw-rw-rw-   0        0        0     3085 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/cifar10_LeNet.py
+-rw-rw-rw-   0        0        0     4405 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/dgm.py
+-rw-rw-rw-   0        0        0     2584 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/fmnist_LeNet.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/inference/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/inference/__init__.py
+-rw-rw-rw-   0        0        0     1256 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/inference/distributions.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/layers/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/layers/__init__.py
+-rw-rw-rw-   0        0        0     1705 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/layers/standard.py
+-rw-rw-rw-   0        0        0     1511 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/layers/stochastic.py
+-rw-rw-rw-   0        0        0     1501 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/main.py
+-rw-rw-rw-   0        0        0     2327 2023-07-12 01:46:26.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/mlp.py
+-rw-rw-rw-   0        0        0     2222 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/mnist_LeNet.py
+-rw-rw-rw-   0        0        0     4826 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/vae.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/
+-rw-rw-rw-   0        0        0     7050 2023-07-12 01:46:27.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/DeepSAD_trainer.py
+-rw-rw-rw-   0        0        0     7565 2023-07-17 12:35:57.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/SemiDGM_trainer.py
+-rw-rw-rw-   0        0        0      228 2023-07-17 12:35:19.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/__init__.py
+-rw-rw-rw-   0        0        0     5381 2023-07-12 01:46:27.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/ae_trainer.py
+-rw-rw-rw-   0        0        0     5252 2023-07-12 01:46:27.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/vae_trainer.py
+-rw-rw-rw-   0        0        0     2832 2023-07-12 01:46:27.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/variational.py
+-rw-rw-rw-   0        0        0     4957 2023-07-11 01:16:07.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/run.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/utils/
+-rw-rw-rw-   0        0        0      163 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      682 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/utils/config.py
+-rw-rw-rw-   0        0        0     1468 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:09.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/utils/visualization/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/utils/visualization/__init__.py
+-rw-rw-rw-   0        0        0      803 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:09.000000 adbench-0.1.0/adbench/baseline/DevNet/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/DevNet/__init__.py
+-rw-rw-rw-   0        0        0    10603 2023-07-17 12:37:39.000000 adbench-0.1.0/adbench/baseline/DevNet/run.py
+-rw-rw-rw-   0        0        0     2367 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/DevNet/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:09.000000 adbench-0.1.0/adbench/baseline/FEAWAD/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/FEAWAD/__init__.py
+-rw-rw-rw-   0        0        0    18613 2023-07-12 00:41:49.000000 adbench-0.1.0/adbench/baseline/FEAWAD/run.py
+-rw-rw-rw-   0        0        0     1533 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/FEAWAD/toolsdev.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:09.000000 adbench-0.1.0/adbench/baseline/FTTransformer/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/FTTransformer/__init__.py
+-rw-rw-rw-   0        0        0     6098 2023-07-11 01:16:07.000000 adbench-0.1.0/adbench/baseline/FTTransformer/run.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:09.000000 adbench-0.1.0/adbench/baseline/GANomaly/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/GANomaly/__init__.py
+-rw-rw-rw-   0        0        0     2878 2023-07-12 01:46:27.000000 adbench-0.1.0/adbench/baseline/GANomaly/fit.py
+-rw-rw-rw-   0        0        0     1260 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/GANomaly/model.py
+-rw-rw-rw-   0        0        0     2998 2023-07-17 12:11:45.000000 adbench-0.1.0/adbench/baseline/GANomaly/run.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:09.000000 adbench-0.1.0/adbench/baseline/PReNet/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/PReNet/__init__.py
+-rw-rw-rw-   0        0        0     1227 2023-07-17 12:38:15.000000 adbench-0.1.0/adbench/baseline/PReNet/fit.py
+-rw-rw-rw-   0        0        0      703 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/PReNet/model.py
+-rw-rw-rw-   0        0        0     2952 2023-07-12 01:46:27.000000 adbench-0.1.0/adbench/baseline/PReNet/run.py
+-rw-rw-rw-   0        0        0     2931 2023-07-11 01:16:07.000000 adbench-0.1.0/adbench/baseline/PReNet/utils.py
+-rw-rw-rw-   0        0        0    13241 2023-07-11 01:16:07.000000 adbench-0.1.0/adbench/baseline/PyOD.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:09.000000 adbench-0.1.0/adbench/baseline/REPEN/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.0/adbench/baseline/REPEN/__init__.py
+-rw-rw-rw-   0        0        0    12481 2023-07-12 00:46:22.000000 adbench-0.1.0/adbench/baseline/REPEN/model.py
+-rw-rw-rw-   0        0        0     1928 2023-07-17 12:37:11.000000 adbench-0.1.0/adbench/baseline/REPEN/run.py
+-rw-rw-rw-   0        0        0     2011 2023-07-08 02:17:37.000000 adbench-0.1.0/adbench/baseline/REPEN/utils.py
+-rw-rw-rw-   0        0        0     1491 2023-07-11 01:16:07.000000 adbench-0.1.0/adbench/baseline/Supervised.py
+-rw-rw-rw-   0        0        0       79 2023-07-17 11:47:13.000000 adbench-0.1.0/adbench/baseline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:09.000000 adbench-0.1.0/adbench/datasets/
+-rw-rw-rw-   0        0        0       79 2023-07-17 11:51:08.000000 adbench-0.1.0/adbench/datasets/__init__.py
+-rw-rw-rw-   0        0        0    17216 2023-07-17 13:23:37.000000 adbench-0.1.0/adbench/datasets/data_generator.py
+-rw-rw-rw-   0        0        0    12211 2023-07-17 11:41:56.000000 adbench-0.1.0/adbench/myutils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:09.000000 adbench-0.1.0/adbench/other_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:49:49.000000 adbench-0.1.0/adbench/other_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:09.000000 adbench-0.1.0/adbench/other_utils/gmm/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:49:49.000000 adbench-0.1.0/adbench/other_utils/gmm/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-07-08 02:17:46.000000 adbench-0.1.0/adbench/other_utils/gmm/example.py
+-rw-rw-rw-   0        0        0    19823 2023-07-12 01:49:59.000000 adbench-0.1.0/adbench/other_utils/gmm/gmm.py
+-rw-rw-rw-   0        0        0     6856 2023-07-08 02:17:46.000000 adbench-0.1.0/adbench/other_utils/gmm/test.py
+-rw-rw-rw-   0        0        0     1129 2023-07-08 02:17:46.000000 adbench-0.1.0/adbench/other_utils/gmm/utils.py
+-rw-rw-rw-   0        0        0    14138 2023-07-08 02:17:46.000000 adbench-0.1.0/adbench/other_utils/utils.py
+-rw-rw-rw-   0        0        0    14299 2023-07-17 15:19:42.000000 adbench-0.1.0/adbench/run.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench.egg-info/
+-rw-rw-rw-   0        0        0      950 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4419 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-17 15:38:08.000000 adbench-0.1.0/adbench.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      125 2023-07-17 10:51:48.000000 adbench-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 15:38:09.000000 adbench-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1393 2023-07-17 15:31:13.000000 adbench-0.1.0/setup.py
```

### Comparing `adbench-0.0.4/LICENSE` & `adbench-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/PKG-INFO` & `adbench-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbench
-Version: 0.0.4
+Version: 0.1.0
 Summary: Python package of ADBench
 Home-page: https://github.com/Minqi824/ADBench
 Author: Minqi Jiang
 Author-email: <jiangmq95@163.com>
 Keywords: anomaly detection,outlier detection,tabular data,benchmark
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `adbench-0.0.4/README.md` & `adbench-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,30 +55,57 @@
 
 - **Have better understanding of anomaly detection algorithms**: please read our [paper](https://arxiv.org/abs/2206.09426) for details.
 - **Conduct future research on anomaly detection**: we list 4 important future research questions in the paper--see Section 4 to see some thoughts!
 - **Access rich algorithm implementation and datasets**: see details below for how to use them
 - **Benchmark your anomaly detection algorithms**: see [notebook](https://github.com/Minqi824/ADBench/blob/main/demo.ipynb) for instruction.
 
 
-### Dependency
-The experiment code is written in Python 3 and built on a number of Python packages:  
+[comment]: <> (### Dependency)
 
-- scikit-learn==0.20.3
-- pyod==1.0.0
-- torch==1.9.0
-- rtdl==0.0.13
-- keras
-- tensorflow
-- delu
-- lightgbm
-- xgboost
-- catboost 
-- copulas
-- combo
-- barbar
+[comment]: <> (The experiment code is written in Python 3 and built on a number of Python packages:  )
+
+[comment]: <> (- scikit-learn==0.20.3)
+
+[comment]: <> (- pyod==1.0.0)
+
+[comment]: <> (- torch==1.9.0)
+
+[comment]: <> (- rtdl==0.0.13)
+
+[comment]: <> (- keras)
+
+[comment]: <> (- tensorflow)
+
+[comment]: <> (- delu)
+
+[comment]: <> (- lightgbm)
+
+[comment]: <> (- xgboost)
+
+[comment]: <> (- catboost )
+
+[comment]: <> (- copulas)
+
+[comment]: <> (- combo)
+
+[comment]: <> (- barbar)
+
+We provide full guidence of ADBench in the [notebook](guidence.ipynb)
+### Installation
+```python
+pip install adbench
+pip install --upgrade adbench
+```
+
+_Prerequisite: Downloading datasets in ADBench from the remote repo_
+```python
+from adbench.myutils import Utils
+utils = Utils() # utility function
+utils.download_datasets() # download datasets from the remote github repo
+```
 
 ### Quickly implement ADBench for benchmarking AD algorithms.
 We present the following example for quickly implementing ADBench in _three different Angles_ illustrated
 in the paper. Currently, [57 datasets](#datasets) can be used for evaluating [30 algorithms](#algorithms) in ADBench,
 and we encourage to test your customized datasets/algorithms in our ADBench testbed.
 
 
@@ -95,15 +122,15 @@
 data = data_generator.generator(la=0.1)
 
 # or specify the X and y of your customized data
 # data_generator = DataGenerator(dataset=None)
 # data = data_generator.generator(X=X, y=y, la=0.1)
 
 # import AD algorithms (e.g., DevNet) and initialization
-from baseline.DevNet.run import DevNet
+from adbench.baseline import DevNet
 
 model = DevNet(seed=42)
 
 # fitting
 model.fit(X_train=data['X_train'], y_train=data['y_train'])
 
 # prediction
@@ -127,15 +154,15 @@
 ```python
 # For Angle III, different data noises and corruptions are added as the following
 data_generator = DataGenerator(dataset='6_cardio.npz')
 # the type of anomalies could be 'duplicated_anomalies', 'irrelevant_features' or 'label_contamination'.
 data = data_generator.generator(noise_type='duplicated_anomalies')
 ```
 
-- We also provide an example for quickly implementing ADBench, as shown in [notebook](demo.ipynb).
+- We also provide an example for quickly implementing ADBench, as shown in [notebook](guidence.ipynb).
 - For **complete results** of ADBench, please refer to our [paper](https://arxiv.org/abs/2206.09426).
 - For **reproduce** experiment results of ADBench, please run the [code](adbench/run.py).
 
 ### Datasets
 ADBench includes [57 datasets](https://github.com/Minqi824/ADBench/tree/main/datasets), as shown in the following Table. 
 
 - Among them, **47 widely-used real-world datasets** are gathered for model evaluation, which cover many application domains, 
@@ -239,18 +266,19 @@
 For each algorithm, we also introduce its specific implementation in the following Table.
 The only thing worth noting is that model name should be specified 
 (especially for those models deployed by their corresponding package, e.g., [PyOD](https://github.com/yzhao062/pyod)). 
 The following codes show the example to import AD models. 
 Please see the Table for complete AD models included in ADBench and their import methods.
 
 ```python
-from baseline.PyOD import PYOD
-model = PYOD(model_name='XGBOD') # initialization
-model.fit(X_train, y_train) # fit
-score = model.predict_score(X_test) # predict
+from adbench.baseline import PYOD
+
+model = PYOD(model_name='XGBOD')  # initialization
+model.fit(X_train, y_train)  # fit
+score = model.predict_score(X_test)  # predict
 ```
 
 |  Model  | Year | Type |  DL  |       Import       |  Source  |
 | :-----: | :--------: | :--: | :--: | :-----------------: | :------: |
 | [PCA](https://apps.dtic.mil/sti/pdfs/ADA465712.pdf) | Before 2017 | Unsup |  &cross;   | from baseline.PyOD import PYOD | [Link](https://pyod.readthedocs.io/en/latest/#) |
 | [OCSVM](https://proceedings.neurips.cc/paper/1999/file/8725fb777f25776ffa9076e44fcfd776-Paper.pdf) | Before 2017  | Unsup |  &cross;   | from baseline.PyOD import PYOD | [Link](https://pyod.readthedocs.io/en/latest/#) |
 | [LOF](https://dl.acm.org/doi/pdf/10.1145/342009.335388) | Before 2017  | Unsup |  &cross;   | from baseline.PyOD import PYOD | [Link](https://pyod.readthedocs.io/en/latest/#) |
```

#### html2text {}

```diff
@@ -44,47 +44,55 @@
 ADBench? We envision three primary usages of ADBench: - **Have better
 understanding of anomaly detection algorithms**: please read our [paper](https:
 //arxiv.org/abs/2206.09426) for details. - **Conduct future research on anomaly
 detection**: we list 4 important future research questions in the paper--see
 Section 4 to see some thoughts! - **Access rich algorithm implementation and
 datasets**: see details below for how to use them - **Benchmark your anomaly
 detection algorithms**: see [notebook](https://github.com/Minqi824/ADBench/
-blob/main/demo.ipynb) for instruction. ### Dependency The experiment code is
-written in Python 3 and built on a number of Python packages: - scikit-
-learn==0.20.3 - pyod==1.0.0 - torch==1.9.0 - rtdl==0.0.13 - keras - tensorflow
-- delu - lightgbm - xgboost - catboost - copulas - combo - barbar ### Quickly
-implement ADBench for benchmarking AD algorithms. We present the following
-example for quickly implementing ADBench in _three different Angles_
+blob/main/demo.ipynb) for instruction. [comment]: <> (### Dependency)
+[comment]: <> (The experiment code is written in Python 3 and built on a number
+of Python packages: ) [comment]: <> (- scikit-learn==0.20.3) [comment]: <> (-
+pyod==1.0.0) [comment]: <> (- torch==1.9.0) [comment]: <> (- rtdl==0.0.13)
+[comment]: <> (- keras) [comment]: <> (- tensorflow) [comment]: <> (- delu)
+[comment]: <> (- lightgbm) [comment]: <> (- xgboost) [comment]: <> (- catboost
+) [comment]: <> (- copulas) [comment]: <> (- combo) [comment]: <> (- barbar) We
+provide full guidence of ADBench in the [notebook](guidence.ipynb) ###
+Installation ```python pip install adbench pip install --upgrade adbench ```
+_Prerequisite: Downloading datasets in ADBench from the remote repo_ ```python
+from adbench.myutils import Utils utils = Utils() # utility function
+utils.download_datasets() # download datasets from the remote github repo ```
+### Quickly implement ADBench for benchmarking AD algorithms. We present the
+following example for quickly implementing ADBench in _three different Angles_
 illustrated in the paper. Currently, [57 datasets](#datasets) can be used for
 evaluating [30 algorithms](#algorithms) in ADBench, and we encourage to test
 your customized datasets/algorithms in our ADBench testbed. **_Angle I:
 Availability of Ground Truth Labels (Supervision)_** ```python from
 datasets.data_generator import DataGenerator from adbench.myutils import Utils
 # one can use our already included datasets data_generator = DataGenerator
 (dataset='6_cardio.npz') # specify the ratio of labeled anomalies to generate X
 and y # la could be any float number in [0.0, 1.0] data =
 data_generator.generator(la=0.1) # or specify the X and y of your customized
 data # data_generator = DataGenerator(dataset=None) # data =
 data_generator.generator(X=X, y=y, la=0.1) # import AD algorithms (e.g.,
-DevNet) and initialization from baseline.DevNet.run import DevNet model =
-DevNet(seed=42) # fitting model.fit(X_train=data['X_train'], y_train=data
-['y_train']) # prediction score = model.predict_score(data['X_test']) #
-evaluation utils = Utils() result = utils.metric(y_true=data['y_test'],
-y_score=score) ``` **_Angle II: Types of Anomalies_** ```python # For Angle II,
-different types of anomalies are generated as the following data_generator =
-DataGenerator(dataset='6_cardio.npz') # the type of anomalies could be 'local',
-'global', 'dependency' or 'cluster'. data = data_generator.generator
+DevNet) and initialization from adbench.baseline import DevNet model = DevNet
+(seed=42) # fitting model.fit(X_train=data['X_train'], y_train=data['y_train'])
+# prediction score = model.predict_score(data['X_test']) # evaluation utils =
+Utils() result = utils.metric(y_true=data['y_test'], y_score=score) ```
+**_Angle II: Types of Anomalies_** ```python # For Angle II, different types of
+anomalies are generated as the following data_generator = DataGenerator
+(dataset='6_cardio.npz') # the type of anomalies could be 'local', 'global',
+'dependency' or 'cluster'. data = data_generator.generator
 (realistic_synthetic_mode='local') ``` **_Angle III: Model Robustness with
 Noisy and Corrupted Data_** ```python # For Angle III, different data noises
 and corruptions are added as the following data_generator = DataGenerator
 (dataset='6_cardio.npz') # the type of anomalies could be
 'duplicated_anomalies', 'irrelevant_features' or 'label_contamination'. data =
 data_generator.generator(noise_type='duplicated_anomalies') ``` - We also
 provide an example for quickly implementing ADBench, as shown in [notebook]
-(demo.ipynb). - For **complete results** of ADBench, please refer to our
+(guidence.ipynb). - For **complete results** of ADBench, please refer to our
 [paper](https://arxiv.org/abs/2206.09426). - For **reproduce** experiment
 results of ADBench, please run the [code](adbench/run.py). ### Datasets ADBench
 includes [57 datasets](https://github.com/Minqi824/ADBench/tree/main/datasets),
 as shown in the following Table. - Among them, **47 widely-used real-world
 datasets** are gathered for model evaluation, which cover many application
 domains, including healthcare (e.g., disease diagnosis), audio and language
 processing (e.g., speech recognition), image processing (e.g., object
@@ -156,15 +164,15 @@
 unsupervised, 7 semi-supervised, and 9 supervised algorithms) in ADBench. !
 [Algorithms](figs/Algorithms.png) For each algorithm, we also introduce its
 specific implementation in the following Table. The only thing worth noting is
 that model name should be specified (especially for those models deployed by
 their corresponding package, e.g., [PyOD](https://github.com/yzhao062/pyod)).
 The following codes show the example to import AD models. Please see the Table
 for complete AD models included in ADBench and their import methods. ```python
-from baseline.PyOD import PYOD model = PYOD(model_name='XGBOD') #
+from adbench.baseline import PYOD model = PYOD(model_name='XGBOD') #
 initialization model.fit(X_train, y_train) # fit score = model.predict_score
 (X_test) # predict ``` | Model | Year | Type | DL | Import | Source | | :-----:
 | :--------: | :--: | :--: | :-----------------: | :------: | | [PCA](https://
 apps.dtic.mil/sti/pdfs/ADA465712.pdf) | Before 2017 | Unsup | &cross; | from
 baseline.PyOD import PYOD | [Link](https://pyod.readthedocs.io/en/latest/#) | |
 [OCSVM](https://proceedings.neurips.cc/paper/1999/file/
 8725fb777f25776ffa9076e44fcfd776-Paper.pdf) | Before 2017 | Unsup | &cross; |
```

### Comparing `adbench-0.0.4/adbench/myutils.py` & `adbench-0.1.0/adbench/myutils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import pandas as pd
 import numpy as np
 import random
 import torch
 import tensorflow as tf
+import fsspec
+from tqdm import tqdm
 
 # metric
 from sklearn.metrics import roc_auc_score, average_precision_score
 
 # plot
 import matplotlib.pyplot as plt
 
@@ -56,14 +58,29 @@
         return device
 
     # generate unique value
     def unique(self, a, b):
         u = 0.5 * (a + b) * (a + b + 1) + b
         return int(u)
 
+    # download datasets from the remote github repo
+    def download_datasets(self):
+        fs = fsspec.filesystem("github", org="Minqi824", repo="ADBench")
+        folder_list = ['CV_by_ResNet18', 'CV_by_ViT', 'NLP_by_BERT', 'NLP_by_RoBERTa', 'Classical']
+        print(f'Downloading datasets from the remote github repo...')
+
+        for folder in tqdm(folder_list):
+            save_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'datasets', folder)
+            if os.path.exists(save_path):
+                print(f'{folder} already exists. Skipping download...')
+                continue
+
+            os.makedirs(save_path, exist_ok=True)
+            fs.get(fs.ls("datasets/" + folder), save_path, recursive=True)
+
     def data_description(self, X, y):
         des_dict = {}
         des_dict['Samples'] = X.shape[0]
         des_dict['Features'] = X.shape[1]
         des_dict['Anomalies'] = sum(y)
         des_dict['Anomalies Ratio(%)'] = round((sum(y) / len(y)) * 100, 2)
```

### Comparing `adbench-0.0.4/adbench/run.py` & `adbench-0.1.0/adbench/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-import os
 import logging; logging.basicConfig(level=logging.WARNING)
 import numpy as np
-import pandas as pd
 import itertools
 from itertools import product
 from tqdm import tqdm
 import time
 import gc
 from keras import backend as K
 
-from datasets.data_generator import DataGenerator
+from adbench.datasets.data_generator import DataGenerator
 from adbench.myutils import Utils
+from adbench.baseline.Customized.run import Customized
 
 class RunPipeline():
     def __init__(self, suffix:str=None, mode:str='rla', parallel:str=None,
                  generate_duplicates=True, n_samples_threshold=1000,
                  realistic_synthetic_mode:str=None,
                  noise_type=None):
         '''
@@ -75,54 +74,55 @@
             raise NotImplementedError
 
         # model_dict (model_name: clf)
         self.model_dict = {}
 
         # unsupervised algorithms
         if self.parallel == 'unsupervise':
-            from baseline.PyOD import PYOD
-            from baseline.DAGMM.run import DAGMM
+            from adbench.baseline.PyOD import PYOD
+            from adbench.baseline.DAGMM.run import DAGMM
 
             # from pyod
             for _ in ['IForest', 'OCSVM', 'CBLOF', 'COF', 'COPOD', 'ECOD', 'FeatureBagging', 'HBOS', 'KNN', 'LODA',
                       'LOF', 'LSCP', 'MCD', 'PCA', 'SOD', 'SOGAAL', 'MOGAAL', 'DeepSVDD']:
                 self.model_dict[_] = PYOD
 
             # DAGMM
             self.model_dict['DAGMM'] = DAGMM
 
         # semi-supervised algorithms
         elif self.parallel == 'semi-supervise':
-            from baseline.PyOD import PYOD
-            from baseline.GANomaly.run import GANomaly
-            from baseline.DeepSAD.src.run import DeepSAD
-            from baseline.REPEN.run import REPEN
-            from baseline.DevNet.run import DevNet
-            from baseline.PReNet.run import PReNet
-            from baseline.FEAWAD.run import FEAWAD
+            from adbench.baseline.PyOD import PYOD
+            from adbench.baseline.GANomaly.run import GANomaly
+            from adbench.baseline.DeepSAD.src.run import DeepSAD
+            from adbench.baseline.REPEN.run import REPEN
+            from adbench.baseline.DevNet.run import DevNet
+            from adbench.baseline.PReNet.run import PReNet
+            from adbench.baseline.FEAWAD.run import FEAWAD
 
             self.model_dict = {'GANomaly': GANomaly,
                                'DeepSAD': DeepSAD,
                                'REPEN': REPEN,
                                'DevNet': DevNet,
                                'PReNet': PReNet,
                                'FEAWAD': FEAWAD,
                                'XGBOD': PYOD}
 
         # fully-supervised algorithms
         elif self.parallel == 'supervise':
-            from baseline.Supervised import supervised
-            from baseline.FTTransformer.run import FTTransformer
+            from adbench.baseline.Supervised import supervised
+            from adbench.baseline.FTTransformer.run import FTTransformer
 
             # from sklearn
             for _ in ['LR', 'NB', 'SVM', 'MLP', 'RF', 'LGB', 'XGB', 'CatB']:
                 self.model_dict[_] = supervised
             # ResNet and FTTransformer for tabular data
             for _ in ['ResNet', 'FTTransformer']:
                 self.model_dict[_] = FTTransformer
+
         else:
             raise NotImplementedError
 
         # We remove the following model for considering the computational cost
         for _ in ['SOGAAL', 'MOGAAL', 'LSCP', 'MCD', 'FeatureBagging']:
             if _ in self.model_dict.keys():
                 self.model_dict.pop(_)
@@ -168,18 +168,21 @@
         dataset_list = [dataset_list[_] for _ in np.argsort(np.array(dataset_size))]
 
         return dataset_list
 
     # whether the dataset in the NLP / CV dataset
     # currently we have 5 NLP datasets and 5 CV datasets
     def isin_NLPCV(self, dataset):
-        NLPCV_list = ['agnews', 'amazon', 'imdb', 'yelp', '20news',
-                      'MNIST-C', 'FashionMNIST', 'CIFAR10', 'SVHN', 'MVTec-AD']
+        if dataset is None:
+            return False
+        else:
+            NLPCV_list = ['agnews', 'amazon', 'imdb', 'yelp', '20news',
+                          'MNIST-C', 'FashionMNIST', 'CIFAR10', 'SVHN', 'MVTec-AD']
 
-        return any([_ in dataset for _ in NLPCV_list])
+            return any([_ in dataset for _ in NLPCV_list])
 
     # model fitting function
     def model_fit(self):
         try:
             # model initialization, if model weights are saved, the save_suffix should be specified
             if self.model_name in ['DevNet', 'FEAWAD', 'REPEN']:
                 self.clf = self.clf(seed=self.seed, model_name=self.model_name, save_suffix=self.suffix)
@@ -192,15 +195,14 @@
 
         try:
             # fitting
             start_time = time.time()
             self.clf = self.clf.fit(X_train=self.data['X_train'], y_train=self.data['y_train'])
             end_time = time.time(); time_fit = end_time - start_time
 
-
             # predicting score (inference)
             start_time = time.time()
             if self.model_name == 'DAGMM':
                 score_test = self.clf.predict_score(self.data['X_train'], self.data['X_test'])
             else:
                 score_test = self.clf.predict_score(self.data['X_test'])
             end_time = time.time(); time_inference = end_time - start_time
@@ -219,17 +221,23 @@
             time_fit, time_inference = None, None
             result = {'aucroc': np.nan, 'aucpr': np.nan}
             pass
 
         return time_fit, time_inference, result
 
     # run the experiments in ADBench
-    def run(self):
-        #  filteting dataset that does not meet the experimental requirements
-        dataset_list = self.dataset_filter()
+    def run(self, dataset=None, clf=None):
+        if dataset is None:
+            #  filteting dataset that does not meet the experimental requirements
+            dataset_list = self.dataset_filter()
+            X, y = None, None
+        else:
+            isinstance(dataset, dict)
+            dataset_list = [None]
+            X = dataset['X']; y = dataset['y']
 
         # experimental parameters
         if self.mode == 'nla':
             if self.noise_type is not None:
                 experiment_params = list(product(dataset_list, self.nla_list, self.noise_params_list, self.seed_list))
             else:
                 experiment_params = list(product(dataset_list, self.nla_list, self.seed_list))
@@ -258,38 +266,46 @@
 
             # generate data
             self.data_generator.seed = self.seed
             self.data_generator.dataset = dataset
 
             try:
                 if self.noise_type == 'duplicated_anomalies':
-                    self.data = self.data_generator.generator(la=la, at_least_one_labeled=True,
+                    self.data = self.data_generator.generator(la=la, at_least_one_labeled=True, X=X, y=y,
                                                               realistic_synthetic_mode=self.realistic_synthetic_mode,
                                                               noise_type=self.noise_type, duplicate_times=noise_param)
                 elif self.noise_type == 'irrelevant_features':
-                    self.data = self.data_generator.generator(la=la, at_least_one_labeled=True,
+                    self.data = self.data_generator.generator(la=la, at_least_one_labeled=True, X=X, y=y,
                                                               realistic_synthetic_mode=self.realistic_synthetic_mode,
                                                               noise_type=self.noise_type, noise_ratio=noise_param)
                 elif self.noise_type == 'label_contamination':
-                    self.data = self.data_generator.generator(la=la, at_least_one_labeled=True,
+                    self.data = self.data_generator.generator(la=la, at_least_one_labeled=True, X=X, y=y,
                                                               realistic_synthetic_mode=self.realistic_synthetic_mode,
                                                               noise_type=self.noise_type, noise_ratio=noise_param)
                 else:
-                    self.data = self.data_generator.generator(la=la, at_least_one_labeled=True,
+                    self.data = self.data_generator.generator(la=la, at_least_one_labeled=True, X=X, y=y,
                                                               realistic_synthetic_mode=self.realistic_synthetic_mode)
 
             except Exception as error:
                 print(f'Error when generating data: {error}')
                 pass
                 continue
 
-            for model_name in tqdm(self.model_dict.keys()):
-                self.model_name = model_name
-                self.clf = self.model_dict[self.model_name]
-
-                # fit model
-                time_fit, time_inference, result = self.model_fit()
-                print(f'Current experiment parameters: {params}, model: {model_name}, result: {result}, '
+            if clf is None:
+                for model_name in tqdm(self.model_dict.keys()):
+                    self.model_name = model_name
+                    self.clf = self.model_dict[self.model_name]
+
+                    # fit and test model
+                    time_fit, time_inference, metrics = self.model_fit()
+                    print(f'Current experiment parameters: {params}, model: {model_name}, metrics: {metrics}, '
+                          f'fitting time: {time_fit}, inference time: {time_inference}')
+                    result.append([params, model_name, metrics, time_fit, time_inference])
+            else:
+                self.clf = clf; self.model_name = 'customized model'
+                # fit and test model
+                time_fit, time_inference, metrics = self.model_fit()
+                print(f'Current experiment parameters: {params}, model: {self.model_name}, metrics: {metrics}, '
                       f'fitting time: {time_fit}, inference time: {time_inference}')
-                result.append([params, model_name, result, time_fit, time_inference])
+                result.append([params, self.model_name, metrics, time_fit, time_inference])
 
         return result
```

### Comparing `adbench-0.0.4/adbench.egg-info/PKG-INFO` & `adbench-0.1.0/adbench.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbench
-Version: 0.0.4
+Version: 0.1.0
 Summary: Python package of ADBench
 Home-page: https://github.com/Minqi824/ADBench
 Author: Minqi Jiang
 Author-email: <jiangmq95@163.com>
 Keywords: anomaly detection,outlier detection,tabular data,benchmark
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `adbench-0.0.4/baseline/DAGMM/forward_step.py` & `adbench-0.1.0/adbench/baseline/DAGMM/forward_step.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DAGMM/main.py` & `adbench-0.1.0/adbench/baseline/DAGMM/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # code based on https://github.com/danieltan07
 
 import numpy as np
 import argparse 
 import torch
 
-from train import TrainerDAGMM
-from test import eval
+from adbench.baseline.DAGMM.train import TrainerDAGMM
+from adbench.baseline.DAGMM.test import eval
 from preprocess import get_KDDCup99
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     parser.add_argument("--num_epochs", type=int, default=200,
                         help="number of epochs")
```

### Comparing `adbench-0.0.4/baseline/DAGMM/model.py` & `adbench-0.1.0/adbench/baseline/DAGMM/model.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DAGMM/preprocess.py` & `adbench-0.1.0/adbench/baseline/DAGMM/preprocess.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DAGMM/run.py` & `adbench-0.1.0/adbench/baseline/DAGMM/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from adbench.myutils import Utils
-from baseline.DAGMM.train import TrainerDAGMM
-from baseline.DAGMM.test import eval
+from adbench.baseline.DAGMM.train import TrainerDAGMM
+from adbench.baseline.DAGMM.test import eval
 
 import numpy as np
 
 class DAGMM():
     '''
     PyTorch implementation of DAGMM from "https://github.com/mperezcarrasco/PyTorch-DAGMM"
     '''
```

### Comparing `adbench-0.0.4/baseline/DAGMM/test.py` & `adbench-0.1.0/adbench/baseline/DAGMM/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import torch
-from torch.utils.data import DataLoader, TensorDataset
-import numpy as np
+from torch.utils.data import DataLoader
 
-from baseline.DAGMM.forward_step import ComputeLoss
+from adbench.baseline.DAGMM.forward_step import ComputeLoss
 
 # def eval(model, dataloaders, device, n_gmm):
 #     """Testing the DAGMM model"""
 #     dataloader_train, dataloader_test = dataloaders
 #     model.eval()
 #     print('Testing...')
 #     compute = ComputeLoss(model, None, None, device, n_gmm)
```

### Comparing `adbench-0.0.4/baseline/DAGMM/train.py` & `adbench-0.1.0/adbench/baseline/DAGMM/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import torch
 from torch import optim
-import torch.nn.functional as F
 
-import numpy as np
-from barbar import Bar
+from adbench.baseline.DAGMM.model import DAGMM
+from adbench.baseline.DAGMM.forward_step import ComputeLoss
+from adbench.baseline.DAGMM.utils.utils import weights_init_normal
 
-from baseline.DAGMM.model import DAGMM
-from baseline.DAGMM.forward_step import ComputeLoss
-from baseline.DAGMM.utils.utils import weights_init_normal
+from torch.utils.data import DataLoader
 
-from torch.utils.data import DataLoader, TensorDataset
 
 class TrainerDAGMM:
     """Trainer class for DAGMM."""
     def __init__(self, args, data, device):
         self.args = args
         self.device = device
```

### Comparing `adbench-0.0.4/baseline/DAGMM/utils/utils.py` & `adbench-0.1.0/adbench/baseline/DAGMM/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/base/base_dataset.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/base/base_dataset.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/base/base_net.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/base/base_net.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/base/base_trainer.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/base/base_trainer.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/base/odds_dataset.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/base/odds_dataset.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/base/torchvision_dataset.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/base/torchvision_dataset.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/baseline_SemiDGM.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/baseline_SemiDGM.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/baseline_isoforest.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/baseline_isoforest.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/baseline_kde.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/baseline_kde.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/baseline_ocsvm.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/baseline_ocsvm.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/baseline_ssad.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/baseline_ssad.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/baselines/SemiDGM.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/SemiDGM.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/baselines/isoforest.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/isoforest.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/baselines/kde.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/kde.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/baselines/ocsvm.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/ocsvm.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/baselines/ssad.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/baselines/ssad.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/datasets/cifar10.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/datasets/fmnist.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/fmnist.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/datasets/mnist.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/mnist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torch.utils.data import Subset
 from PIL import Image
 from torchvision.datasets import MNIST
-from baseline.DeepSAD.src.base.torchvision_dataset import TorchvisionDataset
+from adbench.baseline.DeepSAD.src.base.torchvision_dataset import TorchvisionDataset
 from .preprocessing import create_semisupervised_setting
 
 import torch
 import torchvision.transforms as transforms
 import random
```

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/datasets/odds.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/odds.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from torch.utils.data import DataLoader, Subset
-from baseline.DeepSAD.src.base.base_dataset import BaseADDataset
-from baseline.DeepSAD.src.base.odds_dataset import ODDSDataset
-from .preprocessing import create_semisupervised_setting
-
-import torch
+from torch.utils.data import DataLoader
+from adbench.baseline.DeepSAD.src.base import BaseADDataset
+from adbench.baseline.DeepSAD.src.base.odds_dataset import ODDSDataset
 
 
 class ODDSADDataset(BaseADDataset):
 
     def __init__(self, data, train):
         super().__init__(self)
```

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/datasets/preprocessing.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/datasets/preprocessing.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/deepsad.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/deepsad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import torch
 
-from baseline.DeepSAD.src.base.base_dataset import BaseADDataset
-from baseline.DeepSAD.src.networks.main import build_network, build_autoencoder
-from baseline.DeepSAD.src.optim.DeepSAD_trainer import DeepSADTrainer
-from baseline.DeepSAD.src.optim.ae_trainer import AETrainer
+from adbench.baseline.DeepSAD.src.base import BaseADDataset
+from adbench.baseline.DeepSAD.src.networks import build_network, build_autoencoder
+from adbench.baseline.DeepSAD.src.optim.DeepSAD_trainer import DeepSADTrainer
+from adbench.baseline.DeepSAD.src.optim import AETrainer
 
 
 class deepsad(object):
     """A class for the Deep SAD method.
 
     Attributes:
         eta: Deep SAD hyperparameter eta (must be 0 < eta).
```

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/networks/__init__.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/networks/cifar10_LeNet.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/cifar10_LeNet.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/networks/dgm.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/dgm.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/networks/fmnist_LeNet.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/fmnist_LeNet.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/networks/inference/distributions.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/inference/distributions.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/networks/layers/standard.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/layers/standard.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/networks/layers/stochastic.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/layers/stochastic.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/networks/main.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/main.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/networks/mlp.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/mlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch.nn as nn
 import torch.nn.functional as F
 
-from baseline.DeepSAD.src.base.base_net import BaseNet
+from adbench.baseline.DeepSAD.src.base import BaseNet
 
 
 class MLP(BaseNet):
 
     def __init__(self, x_dim, h_dims=[128, 64], rep_dim=32, bias=False):
         super().__init__()
```

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/networks/mnist_LeNet.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/mnist_LeNet.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/networks/vae.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/networks/vae.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/optim/DeepSAD_trainer.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/DeepSAD_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from baseline.DeepSAD.src.base.base_trainer import BaseTrainer
-from baseline.DeepSAD.src.base.base_dataset import BaseADDataset
-from baseline.DeepSAD.src.base.base_net import BaseNet
+from adbench.baseline.DeepSAD.src.base.base_trainer import BaseTrainer
+from adbench.baseline.DeepSAD.src.base import BaseADDataset
+from adbench.baseline.DeepSAD.src.base import BaseNet
 from torch.utils.data.dataloader import DataLoader
-from sklearn.metrics import roc_auc_score, average_precision_score
 
 import logging
 import time
 import torch
 import torch.optim as optim
 import numpy as np
```

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/optim/SemiDGM_trainer.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/SemiDGM_trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from baseline.DeepSAD.src.base.base_trainer import BaseTrainer
-from baseline.DeepSAD.src.base.base_dataset import BaseADDataset
-from baseline.DeepSAD.src.base.base_net import BaseNet
-from baseline.DeepSAD.src.optim.variational import SVI, ImportanceWeightedSampler
-from baseline.DeepSAD.src.utils.misc import binary_cross_entropy
+from adbench.baseline.DeepSAD.src.base.base_trainer import BaseTrainer
+from adbench.baseline.DeepSAD.src.base import BaseADDataset
+from adbench.baseline.DeepSAD.src.base import BaseNet
+from adbench.baseline.DeepSAD.src.optim.variational import SVI, ImportanceWeightedSampler
+from adbench.baseline.DeepSAD.src.utils import binary_cross_entropy
 from sklearn.metrics import roc_auc_score
 
 import logging
 import time
 import torch
 import torch.optim as optim
 import numpy as np
 
-
 class SemiDeepGenerativeTrainer(BaseTrainer):
 
     def __init__(self, alpha: float = 0.1, optimizer_name: str = 'adam', lr: float = 0.001, n_epochs: int = 150,
                  lr_milestones: tuple = (), batch_size: int = 128, weight_decay: float = 1e-6, device: str = 'cuda',
                  n_jobs_dataloader: int = 0):
         super().__init__(optimizer_name, lr, n_epochs, lr_milestones, batch_size, weight_decay, device,
                          n_jobs_dataloader)
```

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/optim/ae_trainer.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/ae_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from baseline.DeepSAD.src.base.base_trainer import BaseTrainer
-from baseline.DeepSAD.src.base.base_dataset import BaseADDataset
-from baseline.DeepSAD.src.base.base_net import BaseNet
+from adbench.baseline.DeepSAD.src.base.base_trainer import BaseTrainer
+from adbench.baseline.DeepSAD.src.base import BaseADDataset
+from adbench.baseline.DeepSAD.src.base import BaseNet
 from sklearn.metrics import roc_auc_score, average_precision_score
 
 import logging
 import time
 import torch
 import torch.nn as nn
 import torch.optim as optim
```

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/optim/vae_trainer.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/vae_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from baseline.DeepSAD.src.base.base_trainer import BaseTrainer
-from baseline.DeepSAD.src.base.base_dataset import BaseADDataset
-from baseline.DeepSAD.src.base.base_net import BaseNet
-from baseline.DeepSAD.src.utils.misc import binary_cross_entropy
+from adbench.baseline.DeepSAD.src.base.base_trainer import BaseTrainer
+from adbench.baseline.DeepSAD.src.base import BaseADDataset
+from adbench.baseline.DeepSAD.src.base import BaseNet
+from adbench.baseline.DeepSAD.src.utils import binary_cross_entropy
 from sklearn.metrics import roc_auc_score
 
 import logging
 import time
 import torch
 import torch.optim as optim
 import numpy as np
```

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/optim/variational.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/optim/variational.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import torch.nn.functional as F
 
 from torch import nn
 from itertools import repeat
-from baseline.DeepSAD.src.utils import enumerate_discrete, log_sum_exp
-from baseline.DeepSAD.src.networks import log_standard_categorical
+from adbench.baseline.DeepSAD.src.utils import enumerate_discrete, log_sum_exp
+from adbench.baseline.DeepSAD.src.networks import log_standard_categorical
 
 
 # Acknowledgements: https://github.com/wohlert/semi-supervised-pytorch
 class ImportanceWeightedSampler(object):
     """
     Importance weighted sampler (Burda et al., 2015) to be used together with SVI.
```

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/run.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/utils/config.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/utils/config.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/utils/misc.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/utils/misc.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py` & `adbench-0.1.0/adbench/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/DevNet/run.py` & `adbench-0.1.0/adbench/baseline/DevNet/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import pandas as pd
 from scipy.special import comb
 import matplotlib.pyplot as plt
 import sys
 import os
 from scipy.sparse import vstack, csc_matrix
 # from utils import dataLoading, aucPerformance, writeResults, get_data_from_svmlight_file
-from baseline.DevNet.utils import dataLoading, aucPerformance
+from adbench.baseline.DevNet.utils import dataLoading, aucPerformance
 from sklearn.model_selection import train_test_split
 from adbench.myutils import Utils
 import time
 
 class DevNet():
     def __init__(self, seed, model_name='DevNet', save_suffix='test'):
         self.utils = Utils()
@@ -67,16 +67,18 @@
         self.args, unknown = parser.parse_known_args()
 
         # network depth
         self.network_depth = int(self.args.network_depth)
         # random_seed = args.ramdn_seed
 
         self.save_suffix = save_suffix
-        if not os.path.exists('baseline/DevNet/model'):
-            os.makedirs('baseline/DevNet/model')
+
+        self.modelpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'model')
+        if not os.path.exists(self.modelpath):
+            os.makedirs(self.modelpath)
         self.ref = None # normal distribution reference, created for reusing across subsequent function calls
 
     def dev_network_d(self,input_shape):
         '''
         deeper network architecture with three hidden layers
         '''
         x_input = Input(shape=input_shape)
@@ -219,15 +221,15 @@
 
         #start time
         self.input_shape = X_train.shape[1:]
         epochs = self.args.epochs
         batch_size = self.args.batch_size
         nb_batch = self.args.nb_batch
         self.model = self.deviation_network(self.input_shape, self.network_depth)
-        self.model_name = os.path.join(os.getcwd(),'baseline','DevNet','model','devnet_'+self.save_suffix+'.h5')
+        self.model_name = os.path.join(self.modelpath,'devnet_'+self.save_suffix+'.h5')
         checkpointer = ModelCheckpoint(self.model_name, monitor='loss', verbose=0,
                                        save_best_only = True, save_weights_only = True)
 
         self.model.fit_generator(self.batch_generator_sup(X_train, outlier_indices, inlier_indices, batch_size, nb_batch, rng),
                                   steps_per_epoch = nb_batch,
                                   epochs = epochs,
                                   callbacks=[checkpointer])
```

### Comparing `adbench-0.0.4/baseline/DevNet/utils.py` & `adbench-0.1.0/adbench/baseline/DevNet/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/FEAWAD/run.py` & `adbench-0.1.0/adbench/baseline/FEAWAD/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,18 @@
                             help="the output file path")
         parser.add_argument("--ramdn_seed", type=int, default=42, help="the random seed number")
         # self.args = parser.parse_args()
         self.args, unknown = parser.parse_known_args()
         self.data_format = 0
 
         self.save_suffix = save_suffix
-        if not os.path.exists('baseline/FEAWAD/model'):
-            os.makedirs('baseline/FEAWAD/model')
+
+        self.modelpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'model')
+        if not os.path.exists(self.modelpath):
+            os.makedirs(self.modelpath)
 
     def auto_encoder(self, input_shape):
         x_input = Input(shape=input_shape)
         length = K.int_shape(x_input)[1]
 
         input_vector = Dense(length, kernel_initializer='glorot_normal',use_bias=True,activation='relu',name = 'ain')(x_input)
         en1 = Dense(128, kernel_initializer='glorot_normal',use_bias=True,activation='relu',name = 'ae1')(input_vector)
@@ -344,26 +346,26 @@
         # X_train_inlier = np.delete(X_train, outlier_indices, axis=0)
         self.input_shape = X_train.shape[1:]
 
         # pre-trained autoencoder
         self.utils.set_seed(self.seed)
         AEmodel = self.deviation_network(self.input_shape, 2, None, 0)  # pretrain auto-encoder model
         print('autoencoder pre-training start....')
-        AEmodel_name = os.path.join(os.getcwd(), 'baseline', 'FEAWAD', 'model', 'pretrained_autoencoder_'+self.save_suffix+'.h5')
+        AEmodel_name = os.path.join(self.modelpath, 'pretrained_autoencoder_'+self.save_suffix+'.h5')
         ae_checkpointer = ModelCheckpoint(AEmodel_name, monitor='loss', verbose=0, save_best_only=True, save_weights_only=True)
         AEmodel.fit_generator(self.auto_encoder_batch_generator_sup(X_train, inlier_indices, self.args.batch_size, self.args.nb_batch, rng),
                                          steps_per_epoch=self.args.nb_batch, epochs=100, callbacks=[ae_checkpointer])
 
 
         #end-to-end devnet model
         print('load pretrained autoencoder model....')
         self.utils.set_seed(self.seed)
         self.dev_model = self.deviation_network(self.input_shape, 4, AEmodel_name, 0)
         print('end-to-end training start....')
-        self.dev_model_name = os.path.join(os.getcwd(), 'baseline', 'FEAWAD', 'model', 'devnet_'+self.save_suffix+'.h5')
+        self.dev_model_name = os.path.join(self.modelpath, 'devnet_'+self.save_suffix+'.h5')
         checkpointer = ModelCheckpoint(self.dev_model_name, monitor='loss', verbose=0,
                                        save_best_only=True, save_weights_only=True)
         self.dev_model.fit_generator(self.batch_generator_sup(X_train, outlier_indices, inlier_indices, self.args.batch_size, self.args.nb_batch, rng),
                                       steps_per_epoch=self.args.nb_batch,
                                       epochs=self.args.epochs,
                                       callbacks=[checkpointer])
```

### Comparing `adbench-0.0.4/baseline/FEAWAD/toolsdev.py` & `adbench-0.1.0/adbench/baseline/FEAWAD/toolsdev.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/FTTransformer/run.py` & `adbench-0.1.0/adbench/baseline/FTTransformer/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/GANomaly/fit.py` & `adbench-0.1.0/adbench/baseline/GANomaly/fit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-import os
-import sys
 from adbench.myutils import Utils
 
-from baseline.GANomaly.model import generator
-from baseline.GANomaly.model import discriminator
-
 import torch
 from torch import nn
 from torch.autograd import Variable
 
 def fit(train_loader, net_generator, net_discriminator, optimizer_G, optimizer_D,
         epochs, batch_size, print_loss, device,
         seed, input_size, hidden_size, act_fun):
```

### Comparing `adbench-0.0.4/baseline/GANomaly/model.py` & `adbench-0.1.0/adbench/baseline/GANomaly/model.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/GANomaly/run.py` & `adbench-0.1.0/adbench/baseline/GANomaly/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import os
-import sys
 from adbench.myutils import Utils
 import torch
-from torch.utils.data import Subset, DataLoader, TensorDataset
+from torch.utils.data import DataLoader, TensorDataset
 from torch import nn
 
-from baseline.GANomaly.model import generator
-from baseline.GANomaly.model import discriminator
-from baseline.GANomaly.fit import fit
+from adbench.baseline.GANomaly.model import generator
+from adbench.baseline.GANomaly.model import discriminator
+from adbench.baseline.GANomaly.fit import fit
 
 class GANomaly():
     def __init__(self, seed:int, model_name='GANomaly', epochs:int=50, batch_size:int=64,
                  act_fun=nn.Tanh(), lr:float=1e-2, mom:float=0.7):
 
         self.utils = Utils()
         self.device = self.utils.get_device()  # get device
```

### Comparing `adbench-0.0.4/baseline/PReNet/fit.py` & `adbench-0.1.0/adbench/baseline/PReNet/fit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from torch.autograd import Variable
-from baseline.PReNet.utils import sampler_pairs
+from adbench.baseline.PReNet.utils import sampler_pairs
 
 def fit(X_train_tensor, y_train, model, optimizer, epochs, batch_num, batch_size,
          s_a_a, s_a_u, s_u_u, device=None):
     # epochs
     for epoch in range(epochs):
         # generate the batch samples
         X_train_loader, y_train_loader = sampler_pairs(X_train_tensor, y_train, epoch, batch_num, batch_size,
```

### Comparing `adbench-0.0.4/baseline/PReNet/model.py` & `adbench-0.1.0/adbench/baseline/PReNet/model.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/PReNet/run.py` & `adbench-0.1.0/adbench/baseline/PReNet/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 from torch import nn
 import numpy as np
 
 from adbench.myutils import Utils
-from baseline.PReNet.model import prenet
-from baseline.PReNet.fit import fit
+from adbench.baseline.PReNet.model import prenet
+from adbench.baseline.PReNet.fit import fit
 
 '''
 The unofficial implement (with PyTorch) of the PReNet model in the paper "Deep Weakly-supervised Anomaly Detection"
 The default hyper-parameter is the same as in the original paper
 '''
 
 class PReNet():
```

### Comparing `adbench-0.0.4/baseline/PReNet/utils.py` & `adbench-0.1.0/adbench/baseline/PReNet/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/PyOD.py` & `adbench-0.1.0/adbench/baseline/PyOD.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/REPEN/model.py` & `adbench-0.1.0/adbench/baseline/REPEN/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,15 @@
         return representation
 
 
 class Trainer:
 
     def __init__(self, n_epochs=50, batch_size=256,
                  nb_batch=100, random_seed=42,
-                 path_model=os.path.join(os.getcwd(), 'baseline', 'REPEN', 'model'),
-                 save_suffix=None):
+                 path_model=None, save_suffix=None):
         self.n_epochs = n_epochs
         self.batch_size = batch_size
         self.nb_batch = nb_batch
         self.rng = np.random.RandomState(random_seed)
         self.path_model = path_model
         self.save_suffix = save_suffix
 
@@ -169,15 +168,15 @@
                                     verbose=verbose)
         return network
 
 
 class repen:
     def __init__(self, n_epochs=50, batch_size=256, n_neighbors=2,
                  nb_batch=100, random_seed=42,
-                 path_model=os.path.join(os.getcwd(), 'baseline', 'REPEN', 'model'), save_suffix=None,
+                 path_model=None, save_suffix=None,
                  mode="semi_supervised", known_outliers=10, hidden_dim=20,
                  confidence_margin=1000.0, input_shape=30, output=None, runs=None):
 
         assert (mode in ["semi_supervised", "unsupervised", "supervised"])
         self.mode = mode
         self.n_neighbors = n_neighbors
         self.known_outliers = known_outliers
```

### Comparing `adbench-0.0.4/baseline/REPEN/run.py` & `adbench-0.1.0/adbench/baseline/REPEN/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
-from baseline.REPEN.model import repen
+from adbench.baseline.REPEN.model import repen
 from adbench.myutils import Utils
 import os
 
-
+# we change the training epochs to 1000 since we find that the default setting (epochs=30) cannot guarantee
 class REPEN():
     def __init__(self, seed, model_name='REPEN', save_suffix='test',
-                 mode:str='supervised', hidden_dim:int=20, batch_size:int=256, nb_batch:int=50, n_epochs:int=30):
+                 mode:str='supervised', hidden_dim:int=20, batch_size:int=256, nb_batch:int=50, n_epochs:int=1000):
         self.utils = Utils()
         self.device = self.utils.get_device()  # get device
         self.seed = seed
 
         self.MAX_INT = np.iinfo(np.int32).max
         self.MAX_FLOAT = np.finfo(np.float32).max
 
@@ -21,28 +21,30 @@
         self.mode = mode
         self.hidden_dim = hidden_dim
         self.batch_size = batch_size
         self.nb_batch = nb_batch
         self.n_epochs = n_epochs
 
         self.save_suffix = save_suffix
-        if not os.path.exists('baseline/REPEN/model'):
-            os.makedirs('baseline/REPEN/model')
+        self.modelpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'model')
+        if not os.path.exists(self.modelpath):
+            os.makedirs(self.modelpath)
 
     def fit(self, X_train, y_train, ratio=None):
         # initialization the network
         self.utils.set_seed(self.seed)
 
         # change the model type when no label information is available
         if sum(y_train) == 0:
             self.mode = 'unsupervised'
 
         # model initialization
         self.model = repen(mode=self.mode, hidden_dim=self.hidden_dim, batch_size=self.batch_size, nb_batch=self.nb_batch,
-                           n_epochs=self.n_epochs, known_outliers=1000000, save_suffix=self.save_suffix)
+                           n_epochs=self.n_epochs, known_outliers=1000000,
+                           path_model=self.modelpath, save_suffix=self.save_suffix)
 
 
         # fitting
         self.model.fit(X_train, y_train)
 
         return self
```

### Comparing `adbench-0.0.4/baseline/REPEN/utils.py` & `adbench-0.1.0/adbench/baseline/REPEN/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/baseline/Supervised.py` & `adbench-0.1.0/adbench/baseline/Supervised.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/other_utils/gmm/example.py` & `adbench-0.1.0/adbench/other_utils/gmm/example.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/other_utils/gmm/gmm.py` & `adbench-0.1.0/adbench/other_utils/gmm/gmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import torch
 import numpy as np
 
 from math import pi
-from scipy.special import logsumexp
-from other_utils.gmm.utils import calculate_matmul, calculate_matmul_n_times
+from adbench.other_utils.gmm.utils import calculate_matmul, calculate_matmul_n_times
 
 
 class GaussianMixture(torch.nn.Module):
     """
     Fits a mixture of k=1,..,K Gaussians to the input data (K is supplied via n_components).
     Input tensors are expected to be flat with dimensions (n: number of samples, d: number of features).
     The model then extends them to (n, 1, d).
```

### Comparing `adbench-0.0.4/other_utils/gmm/test.py` & `adbench-0.1.0/adbench/other_utils/gmm/test.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/other_utils/gmm/utils.py` & `adbench-0.1.0/adbench/other_utils/gmm/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/other_utils/utils.py` & `adbench-0.1.0/adbench/other_utils/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.0.4/setup.py` & `adbench-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 # read the contents of requirements.txt
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'requirements.txt'), encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 # 配置
 setup(
     name="adbench",
-    version='0.0.4',
+    version='0.1.0',
     author="Minqi Jiang",
     author_email="<jiangmq95@163.com>",
     url='https://github.com/Minqi824/ADBench',
     description='Python package of ADBench',
     long_description='Python package of ADBench: Anomaly detection benchmark. Fast implementation of the large '
                      'experiments in ADBench and your customized AD algorithm.',
     packages=find_packages(),
-    include_package_data=True,
+    include_package_data=False,
     install_requires=requirements,
     keywords=['anomaly detection', 'outlier detection', 'tabular data', 'benchmark'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Intended Audience :: Financial and Insurance Industry",
         "Intended Audience :: Science/Research",
```

