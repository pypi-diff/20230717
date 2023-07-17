# Comparing `tmp/multireg-0.0.8.tar.gz` & `tmp/multireg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multireg-0.0.8.tar", last modified: Mon Jun 12 08:04:20 2023, max compression
+gzip compressed data, was "multireg-0.0.9.tar", last modified: Mon Jun 12 09:31:19 2023, max compression
```

## Comparing `multireg-0.0.8.tar` & `multireg-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 08:04:20.378888 multireg-0.0.8/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1523 2023-06-07 14:15:52.000000 multireg-0.0.8/LICENSE
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-07 14:19:41.000000 multireg-0.0.8/MANIFEST.in
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     9457 2023-06-12 08:04:20.378888 multireg-0.0.8/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     8303 2023-06-12 08:02:49.000000 multireg-0.0.8/README.md
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1177 2023-06-07 14:19:41.000000 multireg-0.0.8/pyproject.toml
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1446 2023-06-12 08:04:20.378888 multireg-0.0.8/setup.cfg
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       37 2023-06-07 14:33:30.000000 multireg-0.0.8/setup.py
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 08:04:20.374888 multireg-0.0.8/src/
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 08:04:20.374888 multireg-0.0.8/src/multireg/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    24872 2023-06-12 08:01:54.000000 multireg-0.0.8/src/multireg/MultiReg.py
--rwxrwxr-x   0 gaelle    (1001) gaelle    (1001)     8152 2023-06-12 08:01:54.000000 multireg-0.0.8/src/multireg/Utils.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-12 08:01:54.000000 multireg-0.0.8/src/multireg/__init__.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      310 2023-06-12 08:01:54.000000 multireg-0.0.8/src/multireg/napari.yaml
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 08:04:20.378888 multireg-0.0.8/src/multireg.egg-info/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     9457 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      378 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/SOURCES.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/dependency_links.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       50 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/entry_points.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/requires.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        9 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/top_level.txt
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 09:31:19.563578 multireg-0.0.9/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1523 2023-06-07 14:15:52.000000 multireg-0.0.9/LICENSE
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-07 14:19:41.000000 multireg-0.0.9/MANIFEST.in
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    11780 2023-06-12 09:31:19.563578 multireg-0.0.9/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    10626 2023-06-12 09:27:56.000000 multireg-0.0.9/README.md
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1177 2023-06-07 14:19:41.000000 multireg-0.0.9/pyproject.toml
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1446 2023-06-12 09:31:19.563578 multireg-0.0.9/setup.cfg
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       37 2023-06-07 14:33:30.000000 multireg-0.0.9/setup.py
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 09:31:19.563578 multireg-0.0.9/src/
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 09:31:19.563578 multireg-0.0.9/src/multireg/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    24872 2023-06-12 08:01:54.000000 multireg-0.0.9/src/multireg/MultiReg.py
+-rwxrwxr-x   0 gaelle    (1001) gaelle    (1001)     8152 2023-06-12 08:01:54.000000 multireg-0.0.9/src/multireg/Utils.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-12 08:01:54.000000 multireg-0.0.9/src/multireg/__init__.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      310 2023-06-12 08:01:54.000000 multireg-0.0.9/src/multireg/napari.yaml
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 09:31:19.563578 multireg-0.0.9/src/multireg.egg-info/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    11780 2023-06-12 09:31:19.000000 multireg-0.0.9/src/multireg.egg-info/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      378 2023-06-12 09:31:19.000000 multireg-0.0.9/src/multireg.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-12 09:31:19.000000 multireg-0.0.9/src/multireg.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       50 2023-06-12 09:31:19.000000 multireg-0.0.9/src/multireg.egg-info/entry_points.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-12 09:31:19.000000 multireg-0.0.9/src/multireg.egg-info/requires.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        9 2023-06-12 09:31:19.000000 multireg-0.0.9/src/multireg.egg-info/top_level.txt
```

### Comparing `multireg-0.0.8/LICENSE` & `multireg-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multireg-0.0.8/PKG-INFO` & `multireg-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multireg
-Version: 0.0.8
+Version: 0.0.9
 Summary: Registration of 3D multiplex images with one common chanel
 Home-page: https://gitlab.pasteur.fr/gletort/multireg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/multireg/issues
 Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/mutlireg#README.md
@@ -60,28 +60,35 @@
 
 You can launch `multireg` in napari by going to `Plugins>multireg: do multiplex registration`.
 
 ### Fixed image
 It will open a prompt to ask you to select the reference (fixed) image, compared to which all other images will be aligned.
 Then you have to choose the `reference chanel` that will be used in all the stacks to calculate the alignement. So this chanel should be common to all stacks.
 
+![](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/plugin_step0.png)
+
 #### Reference points
 The first part of the registration relies on reference points manually selected, because the common field of view can be quite far from each other in the acquisition. So first a affine registration is applied to bring close the region of interest between the two stacks to match. 
 <br> *Note that if your stacks did not move a lot then you could calculate the transformation without using the reference points. There's an option in the alignement calculation panel for this.*
 
+![](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/plugin_fixedpoints.png)
+
 You have to manually placed a few reference points (4-5 should be enough). Try to spread them in the image (in x,y and z) on landmarks to recognize them in other images. 
 
 To add a new reference point, click on the "plus" sign in the left panel. To select one, click on the arrow icon (or press 3), then on the point. You can move the point in x and y. To move it in z, press `u` for up and `d` for down. 
 
 When all points are placed, save them. The **points have to be saved** to be correctly loaded by the alignement calculation step.
 Then click on `Fixed points done` to continue to the next step.
 
 
 ### Moving images
-Then you can choose one of the images you want to align with the reference image. Its chanel that is common to the fixed image should be the same chanel, selected in the first step (the `reference chanel`).
+Then you can choose one of the images you want to align with the reference image. Its chanel that is common to the fixed image should be the same chanel, selected in the first step (the `reference chanel`). Click on `do moving image` once you have selected the moving image to align.
+When you will have process all the moving images, you can click on `All done` to finish the plugin by creating the [resulting stack](#create-resulting-image).
+
+![moving image step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/plugin_movingimg.png)
 
 #### Moving points
 You now have to locate where the region of interest (the fixed image) is in your new image and find the landmarks referenced in the fixed image are in this new image. This allows the plugin to put together the region of interest in the two images in a first step, before to fine-tune the registration.
 
 For each point placed in the fixed image, place the corresponding point in the moving image. By default, the moving points are placed close to the fixed points. 
 * Each point must have the same label (number) as its corresponding fixed points to associate them correctly. You can change a point label by selecting it and putting the new value in `param` and clicking on `update`.
 
@@ -92,23 +99,43 @@
 
 
 When all the moving points have been correctly placed, click on `Save points` to save this positions and let it be usable by the alignement step. The points **have to be saved** in the point file to be correctly loaded in the alignement step.
 
 ### Alignement calculation
 This step is the core of the plugin. The transformation necessary to change the moving image to match with the fixed image on the `reference chanel` is calculated based on [itk-elastix](https://pypi.org/project/itk-elastix/) python module. It is decomposed in two steps. (1) First a global **affine registration** is performed, based on the correspondance between the reference and moving points. This allows to locate the fixed image postion within the moving image and apply a first **shearing, scaling, rotation and translation** to super-impose the region of interest. (2) The second step fine-tunes the registration. It doesn't use the reference point anymore but calculate the matching based on the images local intensities. **Non-rigid transformation** based on B-spline is performed at this step, thus allowing to compensate for **local deformations** in the moving image.
 
+![apply alignement step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/interm.png)
+
+
+You can click on `show advanced parameters` to tune the parameters of the non rigid transformation. After calculating the registration, the plugin will add a new layer, which is the moving image after alignement, so you can check the sucess of the regristration. `show intermediate_layer` will also add the moving image aligned after the first step only (the points matching with affine registration).
+
+![calculate alignement step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/align.png)
+
+
 ### Apply alignement
+Once the calculated registration is satisfying, you can apply it to all the chanels of your moving image, or only to a few. By default, all chanels are selected in the `Apply alignement` panel, but you can unselect the chanels that you don't want to align in the parameter `align chanels`. 
+When you click on `Align images`, the plugin will apply the transformation on the selected chanels of the moving image and save each of them in the `aligned` folder as individual `.tif` files. 
+
+![apply alignement step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/goalign.png)
 
 ### Create resulting image
 This step allows to save a single 3D multi-chanels stack with all the aligned chanels. 
 
-The common chanel present in all the images can be averaged together after alignement to obtain a much less noisy image. By default, the aligned `reference chanel` of all the images are averaged together to create the final image first chanel. However, it is possible to unselect some images in the first panel if you do not wish to use all the images or do an average.
+The common chanel present in all the images can be averaged together after alignement to obtain a much less noisy image. By default, the aligned `reference chanel` of all the images are averaged together to create the final image first chanel. However, it is possible to unselect some images in the first panel (`average chanels` parameter) if you do not wish to use all the images or do an average.
+
+![create result image](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/create.png)
+
+Then each aligned chanel of all the images that were not the reference chanel are stacked together in the final resulting image. Here also, if you don't want to keep all the other chanels in the resulting image, you can unselect the one that you don't want stacked, in the `add_chanels` parameter. 
+All the aligned chanels have been previously saved in the `aligned` folder. If `delete_files` is checked (default) all these interemediate files will be deleted and only the final resulting stack will be saved in that folder.
 
-Then each aligned chanel of all the images that were not the reference chanel are stacked together in the final resulting image. Here also, if you don't want to keep all the other chanels in the resulting image, you can unselect the one that you don't want stacked. All the aligned chanels have been previously saved in the `aligned` folder. If `delete_files` is checked (default) all these interemediate files will be deleted and only the final resulting stack will be saved in that folder.
+You will end-up with a final 3D multi-chanels stack, saved as a `.tif` file in the `aligned` folder, with the same name as your fixed image. It can have a lot of chanels if you stacked together multiple images.
+In napari, you can separate the chanels by right clicking on the layer and select `Split stack`. 
+In Fiji, you can make the stack as a composite to see the chanels with different colors.
 
+![final image](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/reslayer.png)
 
 ## License
 Distributed under the terms of the [BSD-3] license,
 "multireg" is free and open source software
 
 ## Plugin initialization
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

### Comparing `multireg-0.0.8/README.md` & `multireg-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -33,28 +33,35 @@
 
 You can launch `multireg` in napari by going to `Plugins>multireg: do multiplex registration`.
 
 ### Fixed image
 It will open a prompt to ask you to select the reference (fixed) image, compared to which all other images will be aligned.
 Then you have to choose the `reference chanel` that will be used in all the stacks to calculate the alignement. So this chanel should be common to all stacks.
 
+![](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/plugin_step0.png)
+
 #### Reference points
 The first part of the registration relies on reference points manually selected, because the common field of view can be quite far from each other in the acquisition. So first a affine registration is applied to bring close the region of interest between the two stacks to match. 
 <br> *Note that if your stacks did not move a lot then you could calculate the transformation without using the reference points. There's an option in the alignement calculation panel for this.*
 
+![](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/plugin_fixedpoints.png)
+
 You have to manually placed a few reference points (4-5 should be enough). Try to spread them in the image (in x,y and z) on landmarks to recognize them in other images. 
 
 To add a new reference point, click on the "plus" sign in the left panel. To select one, click on the arrow icon (or press 3), then on the point. You can move the point in x and y. To move it in z, press `u` for up and `d` for down. 
 
 When all points are placed, save them. The **points have to be saved** to be correctly loaded by the alignement calculation step.
 Then click on `Fixed points done` to continue to the next step.
 
 
 ### Moving images
-Then you can choose one of the images you want to align with the reference image. Its chanel that is common to the fixed image should be the same chanel, selected in the first step (the `reference chanel`).
+Then you can choose one of the images you want to align with the reference image. Its chanel that is common to the fixed image should be the same chanel, selected in the first step (the `reference chanel`). Click on `do moving image` once you have selected the moving image to align.
+When you will have process all the moving images, you can click on `All done` to finish the plugin by creating the [resulting stack](#create-resulting-image).
+
+![moving image step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/plugin_movingimg.png)
 
 #### Moving points
 You now have to locate where the region of interest (the fixed image) is in your new image and find the landmarks referenced in the fixed image are in this new image. This allows the plugin to put together the region of interest in the two images in a first step, before to fine-tune the registration.
 
 For each point placed in the fixed image, place the corresponding point in the moving image. By default, the moving points are placed close to the fixed points. 
 * Each point must have the same label (number) as its corresponding fixed points to associate them correctly. You can change a point label by selecting it and putting the new value in `param` and clicking on `update`.
 
@@ -65,23 +72,43 @@
 
 
 When all the moving points have been correctly placed, click on `Save points` to save this positions and let it be usable by the alignement step. The points **have to be saved** in the point file to be correctly loaded in the alignement step.
 
 ### Alignement calculation
 This step is the core of the plugin. The transformation necessary to change the moving image to match with the fixed image on the `reference chanel` is calculated based on [itk-elastix](https://pypi.org/project/itk-elastix/) python module. It is decomposed in two steps. (1) First a global **affine registration** is performed, based on the correspondance between the reference and moving points. This allows to locate the fixed image postion within the moving image and apply a first **shearing, scaling, rotation and translation** to super-impose the region of interest. (2) The second step fine-tunes the registration. It doesn't use the reference point anymore but calculate the matching based on the images local intensities. **Non-rigid transformation** based on B-spline is performed at this step, thus allowing to compensate for **local deformations** in the moving image.
 
+![apply alignement step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/interm.png)
+
+
+You can click on `show advanced parameters` to tune the parameters of the non rigid transformation. After calculating the registration, the plugin will add a new layer, which is the moving image after alignement, so you can check the sucess of the regristration. `show intermediate_layer` will also add the moving image aligned after the first step only (the points matching with affine registration).
+
+![calculate alignement step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/align.png)
+
+
 ### Apply alignement
+Once the calculated registration is satisfying, you can apply it to all the chanels of your moving image, or only to a few. By default, all chanels are selected in the `Apply alignement` panel, but you can unselect the chanels that you don't want to align in the parameter `align chanels`. 
+When you click on `Align images`, the plugin will apply the transformation on the selected chanels of the moving image and save each of them in the `aligned` folder as individual `.tif` files. 
+
+![apply alignement step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/goalign.png)
 
 ### Create resulting image
 This step allows to save a single 3D multi-chanels stack with all the aligned chanels. 
 
-The common chanel present in all the images can be averaged together after alignement to obtain a much less noisy image. By default, the aligned `reference chanel` of all the images are averaged together to create the final image first chanel. However, it is possible to unselect some images in the first panel if you do not wish to use all the images or do an average.
+The common chanel present in all the images can be averaged together after alignement to obtain a much less noisy image. By default, the aligned `reference chanel` of all the images are averaged together to create the final image first chanel. However, it is possible to unselect some images in the first panel (`average chanels` parameter) if you do not wish to use all the images or do an average.
+
+![create result image](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/create.png)
+
+Then each aligned chanel of all the images that were not the reference chanel are stacked together in the final resulting image. Here also, if you don't want to keep all the other chanels in the resulting image, you can unselect the one that you don't want stacked, in the `add_chanels` parameter. 
+All the aligned chanels have been previously saved in the `aligned` folder. If `delete_files` is checked (default) all these interemediate files will be deleted and only the final resulting stack will be saved in that folder.
 
-Then each aligned chanel of all the images that were not the reference chanel are stacked together in the final resulting image. Here also, if you don't want to keep all the other chanels in the resulting image, you can unselect the one that you don't want stacked. All the aligned chanels have been previously saved in the `aligned` folder. If `delete_files` is checked (default) all these interemediate files will be deleted and only the final resulting stack will be saved in that folder.
+You will end-up with a final 3D multi-chanels stack, saved as a `.tif` file in the `aligned` folder, with the same name as your fixed image. It can have a lot of chanels if you stacked together multiple images.
+In napari, you can separate the chanels by right clicking on the layer and select `Split stack`. 
+In Fiji, you can make the stack as a composite to see the chanels with different colors.
 
+![final image](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/reslayer.png)
 
 ## License
 Distributed under the terms of the [BSD-3] license,
 "multireg" is free and open source software
 
 ## Plugin initialization
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

### Comparing `multireg-0.0.8/pyproject.toml` & `multireg-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multireg-0.0.8/setup.cfg` & `multireg-0.0.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multireg
-version = 0.0.8
+version = 0.0.9
 description = Registration of 3D multiplex images with one common chanel
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Gaëlle Letort
 author_email = gaelle.letort@pasteur.fr
 url = https://gitlab.pasteur.fr/gletort/multireg
 project_urls =
```

### Comparing `multireg-0.0.8/src/multireg/MultiReg.py` & `multireg-0.0.9/src/multireg/MultiReg.py`

 * *Files identical despite different names*

### Comparing `multireg-0.0.8/src/multireg/Utils.py` & `multireg-0.0.9/src/multireg/Utils.py`

 * *Files identical despite different names*

### Comparing `multireg-0.0.8/src/multireg.egg-info/PKG-INFO` & `multireg-0.0.9/src/multireg.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multireg
-Version: 0.0.8
+Version: 0.0.9
 Summary: Registration of 3D multiplex images with one common chanel
 Home-page: https://gitlab.pasteur.fr/gletort/multireg
 Author: Gaëlle Letort
 Author-email: gaelle.letort@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://gitlab.pasteur.fr/gletort/multireg/issues
 Project-URL: Documentation, https://gitlab.pasteur.fr/gletort/mutlireg#README.md
@@ -60,28 +60,35 @@
 
 You can launch `multireg` in napari by going to `Plugins>multireg: do multiplex registration`.
 
 ### Fixed image
 It will open a prompt to ask you to select the reference (fixed) image, compared to which all other images will be aligned.
 Then you have to choose the `reference chanel` that will be used in all the stacks to calculate the alignement. So this chanel should be common to all stacks.
 
+![](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/plugin_step0.png)
+
 #### Reference points
 The first part of the registration relies on reference points manually selected, because the common field of view can be quite far from each other in the acquisition. So first a affine registration is applied to bring close the region of interest between the two stacks to match. 
 <br> *Note that if your stacks did not move a lot then you could calculate the transformation without using the reference points. There's an option in the alignement calculation panel for this.*
 
+![](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/plugin_fixedpoints.png)
+
 You have to manually placed a few reference points (4-5 should be enough). Try to spread them in the image (in x,y and z) on landmarks to recognize them in other images. 
 
 To add a new reference point, click on the "plus" sign in the left panel. To select one, click on the arrow icon (or press 3), then on the point. You can move the point in x and y. To move it in z, press `u` for up and `d` for down. 
 
 When all points are placed, save them. The **points have to be saved** to be correctly loaded by the alignement calculation step.
 Then click on `Fixed points done` to continue to the next step.
 
 
 ### Moving images
-Then you can choose one of the images you want to align with the reference image. Its chanel that is common to the fixed image should be the same chanel, selected in the first step (the `reference chanel`).
+Then you can choose one of the images you want to align with the reference image. Its chanel that is common to the fixed image should be the same chanel, selected in the first step (the `reference chanel`). Click on `do moving image` once you have selected the moving image to align.
+When you will have process all the moving images, you can click on `All done` to finish the plugin by creating the [resulting stack](#create-resulting-image).
+
+![moving image step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/plugin_movingimg.png)
 
 #### Moving points
 You now have to locate where the region of interest (the fixed image) is in your new image and find the landmarks referenced in the fixed image are in this new image. This allows the plugin to put together the region of interest in the two images in a first step, before to fine-tune the registration.
 
 For each point placed in the fixed image, place the corresponding point in the moving image. By default, the moving points are placed close to the fixed points. 
 * Each point must have the same label (number) as its corresponding fixed points to associate them correctly. You can change a point label by selecting it and putting the new value in `param` and clicking on `update`.
 
@@ -92,23 +99,43 @@
 
 
 When all the moving points have been correctly placed, click on `Save points` to save this positions and let it be usable by the alignement step. The points **have to be saved** in the point file to be correctly loaded in the alignement step.
 
 ### Alignement calculation
 This step is the core of the plugin. The transformation necessary to change the moving image to match with the fixed image on the `reference chanel` is calculated based on [itk-elastix](https://pypi.org/project/itk-elastix/) python module. It is decomposed in two steps. (1) First a global **affine registration** is performed, based on the correspondance between the reference and moving points. This allows to locate the fixed image postion within the moving image and apply a first **shearing, scaling, rotation and translation** to super-impose the region of interest. (2) The second step fine-tunes the registration. It doesn't use the reference point anymore but calculate the matching based on the images local intensities. **Non-rigid transformation** based on B-spline is performed at this step, thus allowing to compensate for **local deformations** in the moving image.
 
+![apply alignement step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/interm.png)
+
+
+You can click on `show advanced parameters` to tune the parameters of the non rigid transformation. After calculating the registration, the plugin will add a new layer, which is the moving image after alignement, so you can check the sucess of the regristration. `show intermediate_layer` will also add the moving image aligned after the first step only (the points matching with affine registration).
+
+![calculate alignement step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/align.png)
+
+
 ### Apply alignement
+Once the calculated registration is satisfying, you can apply it to all the chanels of your moving image, or only to a few. By default, all chanels are selected in the `Apply alignement` panel, but you can unselect the chanels that you don't want to align in the parameter `align chanels`. 
+When you click on `Align images`, the plugin will apply the transformation on the selected chanels of the moving image and save each of them in the `aligned` folder as individual `.tif` files. 
+
+![apply alignement step](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/goalign.png)
 
 ### Create resulting image
 This step allows to save a single 3D multi-chanels stack with all the aligned chanels. 
 
-The common chanel present in all the images can be averaged together after alignement to obtain a much less noisy image. By default, the aligned `reference chanel` of all the images are averaged together to create the final image first chanel. However, it is possible to unselect some images in the first panel if you do not wish to use all the images or do an average.
+The common chanel present in all the images can be averaged together after alignement to obtain a much less noisy image. By default, the aligned `reference chanel` of all the images are averaged together to create the final image first chanel. However, it is possible to unselect some images in the first panel (`average chanels` parameter) if you do not wish to use all the images or do an average.
+
+![create result image](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/create.png)
+
+Then each aligned chanel of all the images that were not the reference chanel are stacked together in the final resulting image. Here also, if you don't want to keep all the other chanels in the resulting image, you can unselect the one that you don't want stacked, in the `add_chanels` parameter. 
+All the aligned chanels have been previously saved in the `aligned` folder. If `delete_files` is checked (default) all these interemediate files will be deleted and only the final resulting stack will be saved in that folder.
 
-Then each aligned chanel of all the images that were not the reference chanel are stacked together in the final resulting image. Here also, if you don't want to keep all the other chanels in the resulting image, you can unselect the one that you don't want stacked. All the aligned chanels have been previously saved in the `aligned` folder. If `delete_files` is checked (default) all these interemediate files will be deleted and only the final resulting stack will be saved in that folder.
+You will end-up with a final 3D multi-chanels stack, saved as a `.tif` file in the `aligned` folder, with the same name as your fixed image. It can have a lot of chanels if you stacked together multiple images.
+In napari, you can separate the chanels by right clicking on the layer and select `Split stack`. 
+In Fiji, you can make the stack as a composite to see the chanels with different colors.
 
+![final image](https://gitlab.pasteur.fr/gletort/multireg/raw/main/imgs/reslayer.png)
 
 ## License
 Distributed under the terms of the [BSD-3] license,
 "multireg" is free and open source software
 
 ## Plugin initialization
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

