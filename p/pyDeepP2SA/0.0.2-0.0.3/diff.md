# Comparing `tmp/pyDeepP2SA-0.0.2.tar.gz` & `tmp/pyDeepP2SA-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDeepP2SA-0.0.2.tar", last modified: Sun May 21 03:07:32 2023, max compression
+gzip compressed data, was "pyDeepP2SA-0.0.3.tar", last modified: Mon Jul 17 16:52:14 2023, max compression
```

## Comparing `pyDeepP2SA-0.0.2.tar` & `pyDeepP2SA-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 03:07:32.181343 pyDeepP2SA-0.0.2/
--rw-rw-rw-   0        0        0      108 2023-05-17 08:19:42.000000 pyDeepP2SA-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-05-17 06:46:46.000000 pyDeepP2SA-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-05-17 07:18:28.000000 pyDeepP2SA-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9366 2023-05-21 03:07:32.173324 pyDeepP2SA-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8575 2023-05-21 02:59:54.000000 pyDeepP2SA-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 03:07:32.181343 pyDeepP2SA-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1042 2023-05-21 03:06:18.000000 pyDeepP2SA-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 03:07:31.944855 pyDeepP2SA-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 03:07:32.165327 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/
--rw-rw-rw-   0        0        0     9366 2023-05-21 03:07:31.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-05-21 03:07:31.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 03:07:31.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-21 03:07:31.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-21 03:07:31.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11374 2023-05-18 14:22:48.000000 pyDeepP2SA-0.0.2/src/pyDeepP2SA.py
+drwxr-xr-x   0 brinthan   (501) staff       (20)        0 2023-07-17 16:52:14.401269 pyDeepP2SA-0.0.3/
+-rw-r--r--   0 brinthan   (501) staff       (20)      206 2023-07-17 16:41:18.000000 pyDeepP2SA-0.0.3/CHANGELOG.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)     1057 2023-07-17 16:39:06.000000 pyDeepP2SA-0.0.3/LICENCE.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)       25 2023-07-17 16:39:06.000000 pyDeepP2SA-0.0.3/MANIFEST.in
+-rw-r--r--   0 brinthan   (501) staff       (20)     9273 2023-07-17 16:52:14.401130 pyDeepP2SA-0.0.3/PKG-INFO
+-rw-r--r--   0 brinthan   (501) staff       (20)     8413 2023-07-17 16:39:06.000000 pyDeepP2SA-0.0.3/README.md
+-rw-r--r--   0 brinthan   (501) staff       (20)       38 2023-07-17 16:52:14.401303 pyDeepP2SA-0.0.3/setup.cfg
+-rw-r--r--   0 brinthan   (501) staff       (20)     1042 2023-07-17 16:40:31.000000 pyDeepP2SA-0.0.3/setup.py
+drwxr-xr-x   0 brinthan   (501) staff       (20)        0 2023-07-17 16:52:14.399957 pyDeepP2SA-0.0.3/src/
+drwxr-xr-x   0 brinthan   (501) staff       (20)        0 2023-07-17 16:52:14.400954 pyDeepP2SA-0.0.3/src/pyDeepP2SA.egg-info/
+-rw-r--r--   0 brinthan   (501) staff       (20)     9273 2023-07-17 16:52:14.000000 pyDeepP2SA-0.0.3/src/pyDeepP2SA.egg-info/PKG-INFO
+-rw-r--r--   0 brinthan   (501) staff       (20)      263 2023-07-17 16:52:14.000000 pyDeepP2SA-0.0.3/src/pyDeepP2SA.egg-info/SOURCES.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)        1 2023-07-17 16:52:14.000000 pyDeepP2SA-0.0.3/src/pyDeepP2SA.egg-info/dependency_links.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)       77 2023-07-17 16:52:14.000000 pyDeepP2SA-0.0.3/src/pyDeepP2SA.egg-info/requires.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)       11 2023-07-17 16:52:14.000000 pyDeepP2SA-0.0.3/src/pyDeepP2SA.egg-info/top_level.txt
+-rw-r--r--   0 brinthan   (501) staff       (20)    21289 2023-07-17 16:39:47.000000 pyDeepP2SA-0.0.3/src/pyDeepP2SA.py
```

### Comparing `pyDeepP2SA-0.0.2/LICENCE.txt` & `pyDeepP2SA-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pyDeepP2SA-0.0.2/PKG-INFO` & `pyDeepP2SA-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,191 +1,195 @@
-Metadata-Version: 2.1
-Name: pyDeepP2SA
-Version: 0.0.2
-Summary: A python package for particle size and shape analysis using deep learning
-Home-page: https://github.com/BrinthanK/pyDeepP2SA
-Author: Brinthan K
-Author-email: kanesalingambrinthan187@gmail.com
-License: MIT
-Keywords: Particle shape analyser,PSD,Deep learning,Image processing,Circularity
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Education
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-License-File: LICENCE.txt
-
-# pyDeepP2SA
-## Code Documentation
-
-pyDeepP2SA is an advanced particle size and shape analysis (P2SA) package that leverages the cutting-edge Segment Anything Model (SAM) developed by Facebook Inc. for highly accurate and robust object segmentation. Unlike traditional approaches that rely on manual training and old-fashioned watershed algorithms, pyDeepP2SA revolutionises the field by offering a zero-generalisation segmentation technique. With minimal manual intervention, this package delivers exceptional results and simplifies the entire analysis workflow.
-
-### Prerequisites
-
-To use pyDeepP2SA, you need to fulfill the following prerequisites:
-
-- **Segment Anything Installation:** Install the "Segment Anything" package by running the following command:
-
-  ```
-  pip install git+https://github.com/facebookresearch/segment-anything.git
-  ```
-
-- **SAM Checkpoint:** Download one of the three available checkpoints provided by Facebook Inc. These checkpoints contain pre-trained models that are essential for the segmentation process. Save the downloaded checkpoint in a folder of your choice or on Google Drive if you are using the Colab platform. You can download the checkpoints from the [Segment Anything Model Checkpoints](https://github.com/facebookresearch/segment-anything#model-checkpoints) repository.
-
-Please ensure that you have installed the "Segment Anything" package and obtained the SAM checkpoint before proceeding with pyDeepP2SA.
-
-### Installation 
-
-Install pyDeepP2SA:
-
-  ```
-  pip install pyDeepP2SA
-  ```
-
-### Functions
-
-#### `generate_masks(image, sam_checkpoint, points_per_side=32, pred_iou_thresh=0.95, stability_score_thresh=0.9, crop_n_layers=1, crop_n_points_downscale_factor=2, min_mask_region_area=100)`
-
-This function generates masks for an input image using a SAM checkpoint.
-
-- `image`: The input image for which masks need to be generated.
-- `sam_checkpoint`: The path to the SAM checkpoint file.
-- `points_per_side`: The number of points per side used for generating the masks (default: 32).
-- `pred_iou_thresh`: The predicted IoU (Intersection over Union) threshold used for generating the masks (default: 0.95).
-- `stability_score_thresh`: The stability score threshold used for generating the masks (default: 0.9).
-- `crop_n_layers`: The number of layers used for cropping during mask generation (default: 1).
-- `crop_n_points_downscale_factor`: The downscale factor used for cropping during mask generation (default: 2).
-- `min_mask_region_area`: The minimum region area for a mask to be considered valid (default: 100).
-
-Returns:
-- `masks`: A list of generated masks.
-
-#### `visualise_masks(image, masks)`
-
-This function visualises the segmented image with the generated masks.
-
-- `image`: The input image.
-- `masks`: The list of masks to visualise.
-
-#### `save_masks_to_csv(masks, csv_directory, pixel_to_micron)`
-
-This function saves the generated masks to a CSV file along with the calculated region properties.
-
-- `masks`: The list of masks.
-- `csv_directory`: The directory to save the CSV file.
-- `pixel_to_micron`: The conversion factor from pixels to microns.
-
-#### `plot_diameters(image, masks, diameter_threshold, circularity_threshold, pixel_to_micron)`
-
-This function plots the original image with bounding boxes around the masks that have a diameter and circularity above the specified thresholds.
-
-- `image`: The original input image.
-- `masks`: The list of masks.
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `pixel_to_micron`: The conversion factor from pixels to microns, where "micron" is used as a unit name without any specific conversion factor associated with its general meaning.
-
-#### `ind_mask(masks, diameter_threshold, circularity_threshold, pixel_to_micron, image)`
-
-This function filters the masks based on diameter and circularity thresholds and plots the filtered masks along with their region properties.
-
-- `masks`: The list of masks.
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `pixel_to_micron`: The conversion factor from pixels to microns.
-- `image`: The original input image.
-
-#### `stat_sum(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file with region properties and returns a summary of the properties for the masks that meet the diameter and circularity thresholds.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-Returns:
-- `summary`: A summary of the filtered mask region properties.
-
-#### `plot_boxplots(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file and plots boxplots for the area, perimeter, diameter, and circularity of the masks that meet the diameter
-
- and circularity thresholds.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-#### `plot_psd(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file and plots the particle size distribution (PSD) using a histogram and cumulative frequency curve.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-#### `plot_cir(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file and plots the circularity distribution using a histogram.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-
-### Dependencies
-
-The code relies on the following dependencies:
-
-- `numpy`: A library for numerical operations in Python.
-- `scikit-image`: A library for image processing in Python.
-- `torch` and `torchvision`: Libraries for deep learning and computer vision tasks.
-- `opencv`: A library for image and video manipulation.
-- `matplotlib`: A library for creating visualisations in Python.
-- `pandas`: A library for data manipulation and analysis.
-- `seaborn`: A library for statistical data visualisation.
-
-Make sure these dependencies are installed in your Python environment before running the code.
-
-### Usage
-
-To use the provided functions, follow these steps:
-
-1. Ensure that you have the required dependencies installed.
-
-2. Import the required functions from the code file into your own Python script or interactive session.
-
-3. Load an image of interest.
-
-4. Call the `generate_masks` function, passing the image and SAM checkpoint file path as arguments. This will generate masks for the image.
-
-5. Visualise the generated masks using the `visualise_masks` function, passing the original image and generated masks as arguments.
-
-6. Save the generated masks and their region properties to a CSV file using the `save_masks_to_csv` function, providing the masks, the directory to save the CSV file, and the conversion factor from pixels to microns.
-
-7. Optionally, plot the original image with bounding boxes around the masks that meet specific diameter and circularity thresholds using the `plot_diameters` function.
-
-8. Further filter the masks based on diameter and circularity thresholds, and plot the filtered masks along with their region properties using the `ind_mask` function.
-
-9. Generate a summary of the filtered mask region properties using the `stat_sum` function.
-
-10. Plot boxplots of the area, perimeter, diameter, and circularity for the filtered masks using the `plot_boxplots` function.
-
-11. Plot the particle size distribution (PSD) using a histogram and cumulative frequency curve using the `plot_psd` function.
-
-12. Plot the circularity distribution using a histogram using the `plot_cir` function.
-
-Please note that you may need to provide additional arguments or modify the existing ones based on your specific use case.
-
-I hope this documentation helps you understand and utilise the provided code effectively! Let me know if you have any further questions.
-
-Change Log
-==========
-
-0.0.1 (17th May 2023)
----------------------
-
-- Testing
-- Corrections on functions 
-
-
+Metadata-Version: 2.1
+Name: pyDeepP2SA
+Version: 0.0.3
+Summary: A python package for particle size and shape analysis using deep learning
+Home-page: https://github.com/BrinthanK/pyDeepP2SA
+Author: Brinthan K
+Author-email: kanesalingambrinthan187@gmail.com
+License: MIT
+Keywords: Particle shape analyser,PSD,Deep learning,Image processing,Circularity
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Education
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+License-File: LICENCE.txt
+
+# pyDeepP2SA
+## Code Documentation
+
+pyDeepP2SA is an advanced particle size and shape analysis (P2SA) package that leverages the cutting-edge Segment Anything Model (SAM) developed by Facebook Inc. for highly accurate and robust object segmentation. Unlike traditional approaches that rely on manual training and old-fashioned watershed algorithms, pyDeepP2SA revolutionises the field by offering a zero-generalisation segmentation technique. With minimal manual intervention, this package delivers exceptional results and simplifies the entire analysis workflow.
+
+### Prerequisites
+
+To use pyDeepP2SA, you need to fulfill the following prerequisites:
+
+- **Segment Anything Installation:** Install the "Segment Anything" package by running the following command:
+
+  ```
+  pip install git+https://github.com/facebookresearch/segment-anything.git
+  ```
+
+- **SAM Checkpoint:** Download one of the three available checkpoints provided by Facebook Inc. These checkpoints contain pre-trained models that are essential for the segmentation process. Save the downloaded checkpoint in a folder of your choice or on Google Drive if you are using the Colab platform. You can download the checkpoints from the [Segment Anything Model Checkpoints](https://github.com/facebookresearch/segment-anything#model-checkpoints) repository.
+
+Please ensure that you have installed the "Segment Anything" package and obtained the SAM checkpoint before proceeding with pyDeepP2SA.
+
+### Installation 
+
+Install pyDeepP2SA:
+
+  ```
+  pip install pyDeepP2SA
+  ```
+
+### Functions
+
+#### `generate_masks(image, sam_checkpoint, points_per_side=32, pred_iou_thresh=0.95, stability_score_thresh=0.9, crop_n_layers=1, crop_n_points_downscale_factor=2, min_mask_region_area=100)`
+
+This function generates masks for an input image using a SAM checkpoint.
+
+- `image`: The input image for which masks need to be generated.
+- `sam_checkpoint`: The path to the SAM checkpoint file.
+- `points_per_side`: The number of points per side used for generating the masks (default: 32).
+- `pred_iou_thresh`: The predicted IoU (Intersection over Union) threshold used for generating the masks (default: 0.95).
+- `stability_score_thresh`: The stability score threshold used for generating the masks (default: 0.9).
+- `crop_n_layers`: The number of layers used for cropping during mask generation (default: 1).
+- `crop_n_points_downscale_factor`: The downscale factor used for cropping during mask generation (default: 2).
+- `min_mask_region_area`: The minimum region area for a mask to be considered valid (default: 100).
+
+Returns:
+- `masks`: A list of generated masks.
+
+#### `visualise_masks(image, masks)`
+
+This function visualises the segmented image with the generated masks.
+
+- `image`: The input image.
+- `masks`: The list of masks to visualise.
+
+#### `save_masks_to_csv(masks, csv_directory, pixel_to_micron)`
+
+This function saves the generated masks to a CSV file along with the calculated region properties.
+
+- `masks`: The list of masks.
+- `csv_directory`: The directory to save the CSV file.
+- `pixel_to_micron`: The conversion factor from pixels to microns.
+
+#### `plot_diameters(image, masks, diameter_threshold, circularity_threshold, pixel_to_micron)`
+
+This function plots the original image with bounding boxes around the masks that have a diameter and circularity above the specified thresholds.
+
+- `image`: The original input image.
+- `masks`: The list of masks.
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `pixel_to_micron`: The conversion factor from pixels to microns, where "micron" is used as a unit name without any specific conversion factor associated with its general meaning.
+
+#### `ind_mask(masks, diameter_threshold, circularity_threshold, pixel_to_micron, image)`
+
+This function filters the masks based on diameter and circularity thresholds and plots the filtered masks along with their region properties.
+
+- `masks`: The list of masks.
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `pixel_to_micron`: The conversion factor from pixels to microns.
+- `image`: The original input image.
+
+#### `stat_sum(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file with region properties and returns a summary of the properties for the masks that meet the diameter and circularity thresholds.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+Returns:
+- `summary`: A summary of the filtered mask region properties.
+
+#### `plot_boxplots(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file and plots boxplots for the area, perimeter, diameter, and circularity of the masks that meet the diameter
+
+ and circularity thresholds.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+#### `plot_psd(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file and plots the particle size distribution (PSD) using a histogram and cumulative frequency curve.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+#### `plot_cir(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file and plots the circularity distribution using a histogram.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+
+### Dependencies
+
+The code relies on the following dependencies:
+
+- `numpy`: A library for numerical operations in Python.
+- `scikit-image`: A library for image processing in Python.
+- `torch` and `torchvision`: Libraries for deep learning and computer vision tasks.
+- `opencv`: A library for image and video manipulation.
+- `matplotlib`: A library for creating visualisations in Python.
+- `pandas`: A library for data manipulation and analysis.
+- `seaborn`: A library for statistical data visualisation.
+
+Make sure these dependencies are installed in your Python environment before running the code.
+
+### Usage
+
+To use the provided functions, follow these steps:
+
+1. Ensure that you have the required dependencies installed.
+
+2. Import the required functions from the code file into your own Python script or interactive session.
+
+3. Load an image of interest.
+
+4. Call the `generate_masks` function, passing the image and SAM checkpoint file path as arguments. This will generate masks for the image.
+
+5. Visualise the generated masks using the `visualise_masks` function, passing the original image and generated masks as arguments.
+
+6. Save the generated masks and their region properties to a CSV file using the `save_masks_to_csv` function, providing the masks, the directory to save the CSV file, and the conversion factor from pixels to microns.
+
+7. Optionally, plot the original image with bounding boxes around the masks that meet specific diameter and circularity thresholds using the `plot_diameters` function.
+
+8. Further filter the masks based on diameter and circularity thresholds, and plot the filtered masks along with their region properties using the `ind_mask` function.
+
+9. Generate a summary of the filtered mask region properties using the `stat_sum` function.
+
+10. Plot boxplots of the area, perimeter, diameter, and circularity for the filtered masks using the `plot_boxplots` function.
+
+11. Plot the particle size distribution (PSD) using a histogram and cumulative frequency curve using the `plot_psd` function.
+
+12. Plot the circularity distribution using a histogram using the `plot_cir` function.
+
+Please note that you may need to provide additional arguments or modify the existing ones based on your specific use case.
+
+I hope this documentation helps you understand and utilise the provided code effectively! Let me know if you have any further questions.
+
+Change Log
+==========
+
+0.0.1 (17th May 2023)
+---------------------
+
+- Testing
+- Corrections on functions 
+
+0.0.3 (17th July 2023)
+----------------------
+
+-Added the characterisation section to the package
+
```

### Comparing `pyDeepP2SA-0.0.2/README.md` & `pyDeepP2SA-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-# pyDeepP2SA
-## Code Documentation
-
-pyDeepP2SA is an advanced particle size and shape analysis (P2SA) package that leverages the cutting-edge Segment Anything Model (SAM) developed by Facebook Inc. for highly accurate and robust object segmentation. Unlike traditional approaches that rely on manual training and old-fashioned watershed algorithms, pyDeepP2SA revolutionises the field by offering a zero-generalisation segmentation technique. With minimal manual intervention, this package delivers exceptional results and simplifies the entire analysis workflow.
-
-### Prerequisites
-
-To use pyDeepP2SA, you need to fulfill the following prerequisites:
-
-- **Segment Anything Installation:** Install the "Segment Anything" package by running the following command:
-
-  ```
-  pip install git+https://github.com/facebookresearch/segment-anything.git
-  ```
-
-- **SAM Checkpoint:** Download one of the three available checkpoints provided by Facebook Inc. These checkpoints contain pre-trained models that are essential for the segmentation process. Save the downloaded checkpoint in a folder of your choice or on Google Drive if you are using the Colab platform. You can download the checkpoints from the [Segment Anything Model Checkpoints](https://github.com/facebookresearch/segment-anything#model-checkpoints) repository.
-
-Please ensure that you have installed the "Segment Anything" package and obtained the SAM checkpoint before proceeding with pyDeepP2SA.
-
-### Installation 
-
-Install pyDeepP2SA:
-
-  ```
-  pip install pyDeepP2SA
-  ```
-
-### Functions
-
-#### `generate_masks(image, sam_checkpoint, points_per_side=32, pred_iou_thresh=0.95, stability_score_thresh=0.9, crop_n_layers=1, crop_n_points_downscale_factor=2, min_mask_region_area=100)`
-
-This function generates masks for an input image using a SAM checkpoint.
-
-- `image`: The input image for which masks need to be generated.
-- `sam_checkpoint`: The path to the SAM checkpoint file.
-- `points_per_side`: The number of points per side used for generating the masks (default: 32).
-- `pred_iou_thresh`: The predicted IoU (Intersection over Union) threshold used for generating the masks (default: 0.95).
-- `stability_score_thresh`: The stability score threshold used for generating the masks (default: 0.9).
-- `crop_n_layers`: The number of layers used for cropping during mask generation (default: 1).
-- `crop_n_points_downscale_factor`: The downscale factor used for cropping during mask generation (default: 2).
-- `min_mask_region_area`: The minimum region area for a mask to be considered valid (default: 100).
-
-Returns:
-- `masks`: A list of generated masks.
-
-#### `visualise_masks(image, masks)`
-
-This function visualises the segmented image with the generated masks.
-
-- `image`: The input image.
-- `masks`: The list of masks to visualise.
-
-#### `save_masks_to_csv(masks, csv_directory, pixel_to_micron)`
-
-This function saves the generated masks to a CSV file along with the calculated region properties.
-
-- `masks`: The list of masks.
-- `csv_directory`: The directory to save the CSV file.
-- `pixel_to_micron`: The conversion factor from pixels to microns.
-
-#### `plot_diameters(image, masks, diameter_threshold, circularity_threshold, pixel_to_micron)`
-
-This function plots the original image with bounding boxes around the masks that have a diameter and circularity above the specified thresholds.
-
-- `image`: The original input image.
-- `masks`: The list of masks.
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `pixel_to_micron`: The conversion factor from pixels to microns, where "micron" is used as a unit name without any specific conversion factor associated with its general meaning.
-
-#### `ind_mask(masks, diameter_threshold, circularity_threshold, pixel_to_micron, image)`
-
-This function filters the masks based on diameter and circularity thresholds and plots the filtered masks along with their region properties.
-
-- `masks`: The list of masks.
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `pixel_to_micron`: The conversion factor from pixels to microns.
-- `image`: The original input image.
-
-#### `stat_sum(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file with region properties and returns a summary of the properties for the masks that meet the diameter and circularity thresholds.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-Returns:
-- `summary`: A summary of the filtered mask region properties.
-
-#### `plot_boxplots(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file and plots boxplots for the area, perimeter, diameter, and circularity of the masks that meet the diameter
-
- and circularity thresholds.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-#### `plot_psd(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file and plots the particle size distribution (PSD) using a histogram and cumulative frequency curve.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-#### `plot_cir(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file and plots the circularity distribution using a histogram.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-
-### Dependencies
-
-The code relies on the following dependencies:
-
-- `numpy`: A library for numerical operations in Python.
-- `scikit-image`: A library for image processing in Python.
-- `torch` and `torchvision`: Libraries for deep learning and computer vision tasks.
-- `opencv`: A library for image and video manipulation.
-- `matplotlib`: A library for creating visualisations in Python.
-- `pandas`: A library for data manipulation and analysis.
-- `seaborn`: A library for statistical data visualisation.
-
-Make sure these dependencies are installed in your Python environment before running the code.
-
-### Usage
-
-To use the provided functions, follow these steps:
-
-1. Ensure that you have the required dependencies installed.
-
-2. Import the required functions from the code file into your own Python script or interactive session.
-
-3. Load an image of interest.
-
-4. Call the `generate_masks` function, passing the image and SAM checkpoint file path as arguments. This will generate masks for the image.
-
-5. Visualise the generated masks using the `visualise_masks` function, passing the original image and generated masks as arguments.
-
-6. Save the generated masks and their region properties to a CSV file using the `save_masks_to_csv` function, providing the masks, the directory to save the CSV file, and the conversion factor from pixels to microns.
-
-7. Optionally, plot the original image with bounding boxes around the masks that meet specific diameter and circularity thresholds using the `plot_diameters` function.
-
-8. Further filter the masks based on diameter and circularity thresholds, and plot the filtered masks along with their region properties using the `ind_mask` function.
-
-9. Generate a summary of the filtered mask region properties using the `stat_sum` function.
-
-10. Plot boxplots of the area, perimeter, diameter, and circularity for the filtered masks using the `plot_boxplots` function.
-
-11. Plot the particle size distribution (PSD) using a histogram and cumulative frequency curve using the `plot_psd` function.
-
-12. Plot the circularity distribution using a histogram using the `plot_cir` function.
-
-Please note that you may need to provide additional arguments or modify the existing ones based on your specific use case.
-
+# pyDeepP2SA
+## Code Documentation
+
+pyDeepP2SA is an advanced particle size and shape analysis (P2SA) package that leverages the cutting-edge Segment Anything Model (SAM) developed by Facebook Inc. for highly accurate and robust object segmentation. Unlike traditional approaches that rely on manual training and old-fashioned watershed algorithms, pyDeepP2SA revolutionises the field by offering a zero-generalisation segmentation technique. With minimal manual intervention, this package delivers exceptional results and simplifies the entire analysis workflow.
+
+### Prerequisites
+
+To use pyDeepP2SA, you need to fulfill the following prerequisites:
+
+- **Segment Anything Installation:** Install the "Segment Anything" package by running the following command:
+
+  ```
+  pip install git+https://github.com/facebookresearch/segment-anything.git
+  ```
+
+- **SAM Checkpoint:** Download one of the three available checkpoints provided by Facebook Inc. These checkpoints contain pre-trained models that are essential for the segmentation process. Save the downloaded checkpoint in a folder of your choice or on Google Drive if you are using the Colab platform. You can download the checkpoints from the [Segment Anything Model Checkpoints](https://github.com/facebookresearch/segment-anything#model-checkpoints) repository.
+
+Please ensure that you have installed the "Segment Anything" package and obtained the SAM checkpoint before proceeding with pyDeepP2SA.
+
+### Installation 
+
+Install pyDeepP2SA:
+
+  ```
+  pip install pyDeepP2SA
+  ```
+
+### Functions
+
+#### `generate_masks(image, sam_checkpoint, points_per_side=32, pred_iou_thresh=0.95, stability_score_thresh=0.9, crop_n_layers=1, crop_n_points_downscale_factor=2, min_mask_region_area=100)`
+
+This function generates masks for an input image using a SAM checkpoint.
+
+- `image`: The input image for which masks need to be generated.
+- `sam_checkpoint`: The path to the SAM checkpoint file.
+- `points_per_side`: The number of points per side used for generating the masks (default: 32).
+- `pred_iou_thresh`: The predicted IoU (Intersection over Union) threshold used for generating the masks (default: 0.95).
+- `stability_score_thresh`: The stability score threshold used for generating the masks (default: 0.9).
+- `crop_n_layers`: The number of layers used for cropping during mask generation (default: 1).
+- `crop_n_points_downscale_factor`: The downscale factor used for cropping during mask generation (default: 2).
+- `min_mask_region_area`: The minimum region area for a mask to be considered valid (default: 100).
+
+Returns:
+- `masks`: A list of generated masks.
+
+#### `visualise_masks(image, masks)`
+
+This function visualises the segmented image with the generated masks.
+
+- `image`: The input image.
+- `masks`: The list of masks to visualise.
+
+#### `save_masks_to_csv(masks, csv_directory, pixel_to_micron)`
+
+This function saves the generated masks to a CSV file along with the calculated region properties.
+
+- `masks`: The list of masks.
+- `csv_directory`: The directory to save the CSV file.
+- `pixel_to_micron`: The conversion factor from pixels to microns.
+
+#### `plot_diameters(image, masks, diameter_threshold, circularity_threshold, pixel_to_micron)`
+
+This function plots the original image with bounding boxes around the masks that have a diameter and circularity above the specified thresholds.
+
+- `image`: The original input image.
+- `masks`: The list of masks.
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `pixel_to_micron`: The conversion factor from pixels to microns, where "micron" is used as a unit name without any specific conversion factor associated with its general meaning.
+
+#### `ind_mask(masks, diameter_threshold, circularity_threshold, pixel_to_micron, image)`
+
+This function filters the masks based on diameter and circularity thresholds and plots the filtered masks along with their region properties.
+
+- `masks`: The list of masks.
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `pixel_to_micron`: The conversion factor from pixels to microns.
+- `image`: The original input image.
+
+#### `stat_sum(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file with region properties and returns a summary of the properties for the masks that meet the diameter and circularity thresholds.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+Returns:
+- `summary`: A summary of the filtered mask region properties.
+
+#### `plot_boxplots(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file and plots boxplots for the area, perimeter, diameter, and circularity of the masks that meet the diameter
+
+ and circularity thresholds.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+#### `plot_psd(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file and plots the particle size distribution (PSD) using a histogram and cumulative frequency curve.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+#### `plot_cir(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file and plots the circularity distribution using a histogram.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+
+### Dependencies
+
+The code relies on the following dependencies:
+
+- `numpy`: A library for numerical operations in Python.
+- `scikit-image`: A library for image processing in Python.
+- `torch` and `torchvision`: Libraries for deep learning and computer vision tasks.
+- `opencv`: A library for image and video manipulation.
+- `matplotlib`: A library for creating visualisations in Python.
+- `pandas`: A library for data manipulation and analysis.
+- `seaborn`: A library for statistical data visualisation.
+
+Make sure these dependencies are installed in your Python environment before running the code.
+
+### Usage
+
+To use the provided functions, follow these steps:
+
+1. Ensure that you have the required dependencies installed.
+
+2. Import the required functions from the code file into your own Python script or interactive session.
+
+3. Load an image of interest.
+
+4. Call the `generate_masks` function, passing the image and SAM checkpoint file path as arguments. This will generate masks for the image.
+
+5. Visualise the generated masks using the `visualise_masks` function, passing the original image and generated masks as arguments.
+
+6. Save the generated masks and their region properties to a CSV file using the `save_masks_to_csv` function, providing the masks, the directory to save the CSV file, and the conversion factor from pixels to microns.
+
+7. Optionally, plot the original image with bounding boxes around the masks that meet specific diameter and circularity thresholds using the `plot_diameters` function.
+
+8. Further filter the masks based on diameter and circularity thresholds, and plot the filtered masks along with their region properties using the `ind_mask` function.
+
+9. Generate a summary of the filtered mask region properties using the `stat_sum` function.
+
+10. Plot boxplots of the area, perimeter, diameter, and circularity for the filtered masks using the `plot_boxplots` function.
+
+11. Plot the particle size distribution (PSD) using a histogram and cumulative frequency curve using the `plot_psd` function.
+
+12. Plot the circularity distribution using a histogram using the `plot_cir` function.
+
+Please note that you may need to provide additional arguments or modify the existing ones based on your specific use case.
+
 I hope this documentation helps you understand and utilise the provided code effectively! Let me know if you have any further questions.
```

### Comparing `pyDeepP2SA-0.0.2/setup.py` & `pyDeepP2SA-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'matplotlib',
     'pandas',
     'seaborn'
 ]
 
 setup(
     name='pyDeepP2SA',
-    version='0.0.2',
+    version='0.0.3',
     description='A python package for particle size and shape analysis using deep learning',
     py_modules=["pyDeepP2SA"],
     package_dir={'': 'src'},
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/BrinthanK/pyDeepP2SA',
     author='Brinthan K',
     author_email='kanesalingambrinthan187@gmail.com',
```

### Comparing `pyDeepP2SA-0.0.2/src/pyDeepP2SA.egg-info/PKG-INFO` & `pyDeepP2SA-0.0.3/src/pyDeepP2SA.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,191 +1,195 @@
-Metadata-Version: 2.1
-Name: pyDeepP2SA
-Version: 0.0.2
-Summary: A python package for particle size and shape analysis using deep learning
-Home-page: https://github.com/BrinthanK/pyDeepP2SA
-Author: Brinthan K
-Author-email: kanesalingambrinthan187@gmail.com
-License: MIT
-Keywords: Particle shape analyser,PSD,Deep learning,Image processing,Circularity
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Education
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-License-File: LICENCE.txt
-
-# pyDeepP2SA
-## Code Documentation
-
-pyDeepP2SA is an advanced particle size and shape analysis (P2SA) package that leverages the cutting-edge Segment Anything Model (SAM) developed by Facebook Inc. for highly accurate and robust object segmentation. Unlike traditional approaches that rely on manual training and old-fashioned watershed algorithms, pyDeepP2SA revolutionises the field by offering a zero-generalisation segmentation technique. With minimal manual intervention, this package delivers exceptional results and simplifies the entire analysis workflow.
-
-### Prerequisites
-
-To use pyDeepP2SA, you need to fulfill the following prerequisites:
-
-- **Segment Anything Installation:** Install the "Segment Anything" package by running the following command:
-
-  ```
-  pip install git+https://github.com/facebookresearch/segment-anything.git
-  ```
-
-- **SAM Checkpoint:** Download one of the three available checkpoints provided by Facebook Inc. These checkpoints contain pre-trained models that are essential for the segmentation process. Save the downloaded checkpoint in a folder of your choice or on Google Drive if you are using the Colab platform. You can download the checkpoints from the [Segment Anything Model Checkpoints](https://github.com/facebookresearch/segment-anything#model-checkpoints) repository.
-
-Please ensure that you have installed the "Segment Anything" package and obtained the SAM checkpoint before proceeding with pyDeepP2SA.
-
-### Installation 
-
-Install pyDeepP2SA:
-
-  ```
-  pip install pyDeepP2SA
-  ```
-
-### Functions
-
-#### `generate_masks(image, sam_checkpoint, points_per_side=32, pred_iou_thresh=0.95, stability_score_thresh=0.9, crop_n_layers=1, crop_n_points_downscale_factor=2, min_mask_region_area=100)`
-
-This function generates masks for an input image using a SAM checkpoint.
-
-- `image`: The input image for which masks need to be generated.
-- `sam_checkpoint`: The path to the SAM checkpoint file.
-- `points_per_side`: The number of points per side used for generating the masks (default: 32).
-- `pred_iou_thresh`: The predicted IoU (Intersection over Union) threshold used for generating the masks (default: 0.95).
-- `stability_score_thresh`: The stability score threshold used for generating the masks (default: 0.9).
-- `crop_n_layers`: The number of layers used for cropping during mask generation (default: 1).
-- `crop_n_points_downscale_factor`: The downscale factor used for cropping during mask generation (default: 2).
-- `min_mask_region_area`: The minimum region area for a mask to be considered valid (default: 100).
-
-Returns:
-- `masks`: A list of generated masks.
-
-#### `visualise_masks(image, masks)`
-
-This function visualises the segmented image with the generated masks.
-
-- `image`: The input image.
-- `masks`: The list of masks to visualise.
-
-#### `save_masks_to_csv(masks, csv_directory, pixel_to_micron)`
-
-This function saves the generated masks to a CSV file along with the calculated region properties.
-
-- `masks`: The list of masks.
-- `csv_directory`: The directory to save the CSV file.
-- `pixel_to_micron`: The conversion factor from pixels to microns.
-
-#### `plot_diameters(image, masks, diameter_threshold, circularity_threshold, pixel_to_micron)`
-
-This function plots the original image with bounding boxes around the masks that have a diameter and circularity above the specified thresholds.
-
-- `image`: The original input image.
-- `masks`: The list of masks.
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `pixel_to_micron`: The conversion factor from pixels to microns, where "micron" is used as a unit name without any specific conversion factor associated with its general meaning.
-
-#### `ind_mask(masks, diameter_threshold, circularity_threshold, pixel_to_micron, image)`
-
-This function filters the masks based on diameter and circularity thresholds and plots the filtered masks along with their region properties.
-
-- `masks`: The list of masks.
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `pixel_to_micron`: The conversion factor from pixels to microns.
-- `image`: The original input image.
-
-#### `stat_sum(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file with region properties and returns a summary of the properties for the masks that meet the diameter and circularity thresholds.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-Returns:
-- `summary`: A summary of the filtered mask region properties.
-
-#### `plot_boxplots(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file and plots boxplots for the area, perimeter, diameter, and circularity of the masks that meet the diameter
-
- and circularity thresholds.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-#### `plot_psd(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file and plots the particle size distribution (PSD) using a histogram and cumulative frequency curve.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-#### `plot_cir(diameter_threshold, circularity_threshold, csv_directory)`
-
-This function reads the CSV file and plots the circularity distribution using a histogram.
-
-- `diameter_threshold`: The diameter threshold for filtering masks.
-- `circularity_threshold`: The circularity threshold for filtering masks.
-- `csv_directory`: The directory where the CSV file is located.
-
-
-### Dependencies
-
-The code relies on the following dependencies:
-
-- `numpy`: A library for numerical operations in Python.
-- `scikit-image`: A library for image processing in Python.
-- `torch` and `torchvision`: Libraries for deep learning and computer vision tasks.
-- `opencv`: A library for image and video manipulation.
-- `matplotlib`: A library for creating visualisations in Python.
-- `pandas`: A library for data manipulation and analysis.
-- `seaborn`: A library for statistical data visualisation.
-
-Make sure these dependencies are installed in your Python environment before running the code.
-
-### Usage
-
-To use the provided functions, follow these steps:
-
-1. Ensure that you have the required dependencies installed.
-
-2. Import the required functions from the code file into your own Python script or interactive session.
-
-3. Load an image of interest.
-
-4. Call the `generate_masks` function, passing the image and SAM checkpoint file path as arguments. This will generate masks for the image.
-
-5. Visualise the generated masks using the `visualise_masks` function, passing the original image and generated masks as arguments.
-
-6. Save the generated masks and their region properties to a CSV file using the `save_masks_to_csv` function, providing the masks, the directory to save the CSV file, and the conversion factor from pixels to microns.
-
-7. Optionally, plot the original image with bounding boxes around the masks that meet specific diameter and circularity thresholds using the `plot_diameters` function.
-
-8. Further filter the masks based on diameter and circularity thresholds, and plot the filtered masks along with their region properties using the `ind_mask` function.
-
-9. Generate a summary of the filtered mask region properties using the `stat_sum` function.
-
-10. Plot boxplots of the area, perimeter, diameter, and circularity for the filtered masks using the `plot_boxplots` function.
-
-11. Plot the particle size distribution (PSD) using a histogram and cumulative frequency curve using the `plot_psd` function.
-
-12. Plot the circularity distribution using a histogram using the `plot_cir` function.
-
-Please note that you may need to provide additional arguments or modify the existing ones based on your specific use case.
-
-I hope this documentation helps you understand and utilise the provided code effectively! Let me know if you have any further questions.
-
-Change Log
-==========
-
-0.0.1 (17th May 2023)
----------------------
-
-- Testing
-- Corrections on functions 
-
-
+Metadata-Version: 2.1
+Name: pyDeepP2SA
+Version: 0.0.3
+Summary: A python package for particle size and shape analysis using deep learning
+Home-page: https://github.com/BrinthanK/pyDeepP2SA
+Author: Brinthan K
+Author-email: kanesalingambrinthan187@gmail.com
+License: MIT
+Keywords: Particle shape analyser,PSD,Deep learning,Image processing,Circularity
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Education
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+License-File: LICENCE.txt
+
+# pyDeepP2SA
+## Code Documentation
+
+pyDeepP2SA is an advanced particle size and shape analysis (P2SA) package that leverages the cutting-edge Segment Anything Model (SAM) developed by Facebook Inc. for highly accurate and robust object segmentation. Unlike traditional approaches that rely on manual training and old-fashioned watershed algorithms, pyDeepP2SA revolutionises the field by offering a zero-generalisation segmentation technique. With minimal manual intervention, this package delivers exceptional results and simplifies the entire analysis workflow.
+
+### Prerequisites
+
+To use pyDeepP2SA, you need to fulfill the following prerequisites:
+
+- **Segment Anything Installation:** Install the "Segment Anything" package by running the following command:
+
+  ```
+  pip install git+https://github.com/facebookresearch/segment-anything.git
+  ```
+
+- **SAM Checkpoint:** Download one of the three available checkpoints provided by Facebook Inc. These checkpoints contain pre-trained models that are essential for the segmentation process. Save the downloaded checkpoint in a folder of your choice or on Google Drive if you are using the Colab platform. You can download the checkpoints from the [Segment Anything Model Checkpoints](https://github.com/facebookresearch/segment-anything#model-checkpoints) repository.
+
+Please ensure that you have installed the "Segment Anything" package and obtained the SAM checkpoint before proceeding with pyDeepP2SA.
+
+### Installation 
+
+Install pyDeepP2SA:
+
+  ```
+  pip install pyDeepP2SA
+  ```
+
+### Functions
+
+#### `generate_masks(image, sam_checkpoint, points_per_side=32, pred_iou_thresh=0.95, stability_score_thresh=0.9, crop_n_layers=1, crop_n_points_downscale_factor=2, min_mask_region_area=100)`
+
+This function generates masks for an input image using a SAM checkpoint.
+
+- `image`: The input image for which masks need to be generated.
+- `sam_checkpoint`: The path to the SAM checkpoint file.
+- `points_per_side`: The number of points per side used for generating the masks (default: 32).
+- `pred_iou_thresh`: The predicted IoU (Intersection over Union) threshold used for generating the masks (default: 0.95).
+- `stability_score_thresh`: The stability score threshold used for generating the masks (default: 0.9).
+- `crop_n_layers`: The number of layers used for cropping during mask generation (default: 1).
+- `crop_n_points_downscale_factor`: The downscale factor used for cropping during mask generation (default: 2).
+- `min_mask_region_area`: The minimum region area for a mask to be considered valid (default: 100).
+
+Returns:
+- `masks`: A list of generated masks.
+
+#### `visualise_masks(image, masks)`
+
+This function visualises the segmented image with the generated masks.
+
+- `image`: The input image.
+- `masks`: The list of masks to visualise.
+
+#### `save_masks_to_csv(masks, csv_directory, pixel_to_micron)`
+
+This function saves the generated masks to a CSV file along with the calculated region properties.
+
+- `masks`: The list of masks.
+- `csv_directory`: The directory to save the CSV file.
+- `pixel_to_micron`: The conversion factor from pixels to microns.
+
+#### `plot_diameters(image, masks, diameter_threshold, circularity_threshold, pixel_to_micron)`
+
+This function plots the original image with bounding boxes around the masks that have a diameter and circularity above the specified thresholds.
+
+- `image`: The original input image.
+- `masks`: The list of masks.
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `pixel_to_micron`: The conversion factor from pixels to microns, where "micron" is used as a unit name without any specific conversion factor associated with its general meaning.
+
+#### `ind_mask(masks, diameter_threshold, circularity_threshold, pixel_to_micron, image)`
+
+This function filters the masks based on diameter and circularity thresholds and plots the filtered masks along with their region properties.
+
+- `masks`: The list of masks.
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `pixel_to_micron`: The conversion factor from pixels to microns.
+- `image`: The original input image.
+
+#### `stat_sum(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file with region properties and returns a summary of the properties for the masks that meet the diameter and circularity thresholds.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+Returns:
+- `summary`: A summary of the filtered mask region properties.
+
+#### `plot_boxplots(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file and plots boxplots for the area, perimeter, diameter, and circularity of the masks that meet the diameter
+
+ and circularity thresholds.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+#### `plot_psd(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file and plots the particle size distribution (PSD) using a histogram and cumulative frequency curve.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+#### `plot_cir(diameter_threshold, circularity_threshold, csv_directory)`
+
+This function reads the CSV file and plots the circularity distribution using a histogram.
+
+- `diameter_threshold`: The diameter threshold for filtering masks.
+- `circularity_threshold`: The circularity threshold for filtering masks.
+- `csv_directory`: The directory where the CSV file is located.
+
+
+### Dependencies
+
+The code relies on the following dependencies:
+
+- `numpy`: A library for numerical operations in Python.
+- `scikit-image`: A library for image processing in Python.
+- `torch` and `torchvision`: Libraries for deep learning and computer vision tasks.
+- `opencv`: A library for image and video manipulation.
+- `matplotlib`: A library for creating visualisations in Python.
+- `pandas`: A library for data manipulation and analysis.
+- `seaborn`: A library for statistical data visualisation.
+
+Make sure these dependencies are installed in your Python environment before running the code.
+
+### Usage
+
+To use the provided functions, follow these steps:
+
+1. Ensure that you have the required dependencies installed.
+
+2. Import the required functions from the code file into your own Python script or interactive session.
+
+3. Load an image of interest.
+
+4. Call the `generate_masks` function, passing the image and SAM checkpoint file path as arguments. This will generate masks for the image.
+
+5. Visualise the generated masks using the `visualise_masks` function, passing the original image and generated masks as arguments.
+
+6. Save the generated masks and their region properties to a CSV file using the `save_masks_to_csv` function, providing the masks, the directory to save the CSV file, and the conversion factor from pixels to microns.
+
+7. Optionally, plot the original image with bounding boxes around the masks that meet specific diameter and circularity thresholds using the `plot_diameters` function.
+
+8. Further filter the masks based on diameter and circularity thresholds, and plot the filtered masks along with their region properties using the `ind_mask` function.
+
+9. Generate a summary of the filtered mask region properties using the `stat_sum` function.
+
+10. Plot boxplots of the area, perimeter, diameter, and circularity for the filtered masks using the `plot_boxplots` function.
+
+11. Plot the particle size distribution (PSD) using a histogram and cumulative frequency curve using the `plot_psd` function.
+
+12. Plot the circularity distribution using a histogram using the `plot_cir` function.
+
+Please note that you may need to provide additional arguments or modify the existing ones based on your specific use case.
+
+I hope this documentation helps you understand and utilise the provided code effectively! Let me know if you have any further questions.
+
+Change Log
+==========
+
+0.0.1 (17th May 2023)
+---------------------
+
+- Testing
+- Corrections on functions 
+
+0.0.3 (17th July 2023)
+----------------------
+
+-Added the characterisation section to the package
+
```

