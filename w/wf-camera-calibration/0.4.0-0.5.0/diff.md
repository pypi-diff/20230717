# Comparing `tmp/wf-camera-calibration-0.4.0.tar.gz` & `tmp/wf-camera-calibration-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf-camera-calibration-0.4.0.tar", last modified: Sun Jul 16 22:38:57 2023, max compression
+gzip compressed data, was "wf-camera-calibration-0.5.0.tar", last modified: Sun Jul 16 23:33:17 2023, max compression
```

## Comparing `wf-camera-calibration-0.4.0.tar` & `wf-camera-calibration-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 22:38:57.969382 wf-camera-calibration-0.4.0/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1088 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/LICENSE
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       34 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/MANIFEST.in
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1150 2023-07-16 22:38:57.969382 wf-camera-calibration-0.4.0/PKG-INFO
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      585 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/README.md
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        6 2023-07-16 22:38:13.000000 wf-camera-calibration-0.4.0/VERSION
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 22:38:57.969382 wf-camera-calibration-0.4.0/camera_calibration/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       70 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/camera_calibration/__init__.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     2530 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/camera_calibration/analyze.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    36335 2023-07-16 22:37:29.000000 wf-camera-calibration-0.4.0/camera_calibration/colmap.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    19191 2023-01-07 15:16:24.000000 wf-camera-calibration-0.4.0/camera_calibration/visualize.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       38 2023-07-16 22:38:57.969382 wf-camera-calibration-0.4.0/setup.cfg
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1626 2022-12-19 18:03:55.000000 wf-camera-calibration-0.4.0/setup.py
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 22:38:57.969382 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1150 2023-07-16 22:38:57.000000 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/PKG-INFO
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      392 2023-07-16 22:38:57.000000 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/SOURCES.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        1 2023-07-16 22:38:57.000000 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/dependency_links.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      110 2023-07-16 22:38:57.000000 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/requires.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       19 2023-07-16 22:38:57.000000 wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/top_level.txt
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 23:33:17.837065 wf-camera-calibration-0.5.0/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1088 2022-12-19 18:03:55.000000 wf-camera-calibration-0.5.0/LICENSE
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       34 2022-12-19 18:03:55.000000 wf-camera-calibration-0.5.0/MANIFEST.in
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1150 2023-07-16 23:33:17.837065 wf-camera-calibration-0.5.0/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      585 2022-12-19 18:03:55.000000 wf-camera-calibration-0.5.0/README.md
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        6 2023-07-16 23:31:59.000000 wf-camera-calibration-0.5.0/VERSION
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 23:33:17.837065 wf-camera-calibration-0.5.0/camera_calibration/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       70 2022-12-19 18:03:55.000000 wf-camera-calibration-0.5.0/camera_calibration/__init__.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     2530 2022-12-19 18:03:55.000000 wf-camera-calibration-0.5.0/camera_calibration/analyze.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    26862 2023-07-16 23:31:12.000000 wf-camera-calibration-0.5.0/camera_calibration/colmap.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    19191 2023-01-07 15:16:24.000000 wf-camera-calibration-0.5.0/camera_calibration/visualize.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       38 2023-07-16 23:33:17.837065 wf-camera-calibration-0.5.0/setup.cfg
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1626 2022-12-19 18:03:55.000000 wf-camera-calibration-0.5.0/setup.py
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 23:33:17.837065 wf-camera-calibration-0.5.0/wf_camera_calibration.egg-info/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1150 2023-07-16 23:33:17.000000 wf-camera-calibration-0.5.0/wf_camera_calibration.egg-info/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      392 2023-07-16 23:33:17.000000 wf-camera-calibration-0.5.0/wf_camera_calibration.egg-info/SOURCES.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        1 2023-07-16 23:33:17.000000 wf-camera-calibration-0.5.0/wf_camera_calibration.egg-info/dependency_links.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      110 2023-07-16 23:33:17.000000 wf-camera-calibration-0.5.0/wf_camera_calibration.egg-info/requires.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       19 2023-07-16 23:33:17.000000 wf-camera-calibration-0.5.0/wf_camera_calibration.egg-info/top_level.txt
```

### Comparing `wf-camera-calibration-0.4.0/LICENSE` & `wf-camera-calibration-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wf-camera-calibration-0.4.0/PKG-INFO` & `wf-camera-calibration-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-camera-calibration
-Version: 0.4.0
+Version: 0.5.0
 Summary: Support for calculating intrinsic and extrinsic camera calibration parameters using COLMAP and other tools
 Home-page: https://github.com/WildflowerSchools/wf-camera-calibration
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `wf-camera-calibration-0.4.0/README.md` & `wf-camera-calibration-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `wf-camera-calibration-0.4.0/camera_calibration/analyze.py` & `wf-camera-calibration-0.5.0/camera_calibration/analyze.py`

 * *Files identical despite different names*

### Comparing `wf-camera-calibration-0.4.0/camera_calibration/colmap.py` & `wf-camera-calibration-0.5.0/camera_calibration/colmap.py`

 * *Files 22% similar despite different names*

```diff
@@ -385,60 +385,19 @@
         audience (str): Audience to use for Honeycomb client (default is None)
         client_id (str): Client ID to use for Honeycomb client (default is None)
         client_secret (str): Client secret to use for Honeycomb client (default is None)
 
     Returns:
         (DataFrame) Dataframe containing image data
     """
-    if path is None:
-        if calibration_directory is None or calibration_identifier is None:
-            raise ValueError('Must specify either image data path or calibration directory and calibration identifier')
-        path = os.path.join(
-            calibration_directory,
-            calibration_identifier,
-            'images.txt'
-        )
-    data_list = list()
-    with open(path, 'r') as fp:
-        for line in fp.readlines():
-            m = re.match(CALIBRATION_DATA_RE, line)
-            if m:
-                data_list.append({
-                    'colmap_image_id': int(m.group('colmap_image_id')),
-                    'quaternion_vector': np.asarray([
-                        float(m.group('qw')),
-                        float(m.group('qx')),
-                        float(m.group('qy')),
-                        float(m.group('qz'))
-                    ]),
-                    'translation_vector': np.asarray([
-                        float(m.group('tx')),
-                        float(m.group('ty')),
-                        float(m.group('tz'))
-                    ]),
-                    'colmap_camera_id': int(m.group('colmap_camera_id')),
-                    'image_path': m.group('image_path')
-
-                })
-    df = pd.DataFrame(data_list)
-    df['rotation_vector'] = df['quaternion_vector'].apply(cv_utils.quaternion_vector_to_rotation_vector)
-    df['position'] = df.apply(
-        lambda row: cv_utils.extract_camera_position(
-            row['rotation_vector'],
-            row['translation_vector']
-        ),
-        axis=1
-    )
-    df['image_directory'] = df['image_path'].apply(lambda x: os.path.dirname(os.path.normpath(x))).astype('string')
-    df['image_name'] = df['image_path'].apply(lambda x: os.path.splitext(os.path.basename(os.path.normpath(x)))[0]).astype('string')
-    df['image_extension'] = df['image_path'].apply(
-        lambda x: os.path.splitext(os.path.basename(os.path.normpath(x)))[1][1:]
-        if len(os.path.splitext(os.path.basename(os.path.normpath(x)))[1]) > 1
-        else None
-    ).astype('string')
+    df = cv_utils.fetch_colmap_image_data_local(
+        calibration_directory=calibration_directory,
+        calibration_identifier=calibration_identifier,
+        path=path,
+    )
     logger.info('Attempting to extract camera device IDs from image names')
     df['device_id'] = df['image_name'].apply(honeycomb_io.extract_honeycomb_id).astype('object')
     device_ids = df['device_id'].dropna().unique().tolist()
     logger.info('Found {} device IDs among image names'.format(
         len(device_ids)
     ))
     logger.info('Fetching camera names')
@@ -452,24 +411,22 @@
         client_id=client_id,
         client_secret=client_secret
     )
     df = df.join(
         pd.Series(camera_names, name='camera_name'),
         on='device_id'
     )
-    df.set_index('colmap_image_id', inplace=True)
     df = df.reindex(columns=[
         'image_path',
         'image_directory',
         'image_name',
         'device_id',
         'camera_name',
         'image_extension',
         'colmap_camera_id',
-        'quaternion_vector',
         'rotation_vector',
         'translation_vector',
         'position'
     ])
     return df
 
 def fetch_colmap_camera_data_local(
@@ -498,74 +455,19 @@
         calibration_directory (str): Path to directory containing calibrations
         calibration_identifier (str): Identifier for this particular calibration
         path (str): Explicit path for COLMAP cameras output file (default is None)
 
     Returns:
         (DataFrame) Dataframe containing camera data
     """
-    if path is None:
-        if calibration_directory is None or calibration_identifier is None:
-            raise ValueError('Must specify either camera data path or calibration directory and calibration identifier')
-        path = os.path.join(
-            calibration_directory,
-            calibration_identifier,
-            'cameras.txt'
-        )
-    cameras=list()
-    with open(path, 'r') as fp:
-        for line_index, line in enumerate(fp):
-            if len(line) == 0 or line[0] == '#':
-                continue
-            word_list = line.split()
-            if len(word_list) < 5:
-                raise ValueError('Line {} is shorter than expected: {}'.format(
-                    line_index,
-                    line
-                ))
-            camera = {
-                'colmap_camera_id': int(word_list[0]),
-                'colmap_camera_model': word_list[1],
-                'image_width': int(word_list[2]),
-                'image_height': int(word_list[3]),
-                'colmap_parameters': np.asarray([float(parameter_string) for parameter_string in word_list[4:]])
-            }
-            cameras.append(camera)
-    df = pd.DataFrame.from_records(cameras)
-    df['camera_matrix'] = df.apply(
-        lambda row: colmap_parameters_to_opencv_parameters(
-            row['colmap_parameters'],
-            row['colmap_camera_model']
-        )[0],
-        axis=1
-    )
-    df['distortion_coefficients'] = df.apply(
-        lambda row: colmap_parameters_to_opencv_parameters(
-            row['colmap_parameters'],
-            row['colmap_camera_model']
-        )[1],
-        axis=1
-    )
-    df = df.astype({
-        'colmap_camera_id': 'int',
-        'colmap_camera_model': 'string',
-        'image_width': 'int',
-        'image_height': 'int',
-        'colmap_parameters': 'object',
-        'camera_matrix': 'object',
-        'distortion_coefficients': 'object'
-    })
-    df.set_index('colmap_camera_id', inplace=True)
-    df = df.reindex(columns=[
-        'colmap_camera_model',
-        'image_width',
-        'image_height',
-        'colmap_parameters',
-        'camera_matrix',
-        'distortion_coefficients'
-    ])
+    df = cv_utils.fetch_colmap_camera_data_local(
+        calibration_directory=calibration_directory,
+        calibration_identifier=calibration_identifier,
+        path=path
+    )
     return df
 
 def fetch_colmap_reference_image_data_local(
     calibration_directory=None,
     calibration_identifier=None,
     path=None
 ):
@@ -587,42 +489,19 @@
         calibration_directory (str): Path to directory containing calibrations
         calibration_identifier (str): Identifier for this particular calibration
         path (str): Explicit path for COLMAP ref images input file (default is None)
 
     Returns:
         (DataFrame) Dataframe containing camera position input data
     """
-    if path is None:
-        if calibration_directory is None or calibration_identifier is None:
-            raise ValueError('Must specify either ref image data path or calibration directory and calibration identifier')
-        path = os.path.join(
-            calibration_directory,
-            calibration_identifier,
-            'ref_images.txt'
-        )
-    df = pd.read_csv(
-        path,
-        header=None,
-        delim_whitespace=True,
-        names = ['image_path', 'x', 'y', 'z'],
-        dtype={
-            'image_path': 'string',
-            'x': 'float',
-            'y': 'float',
-            'z': 'float',
-        }
-    )
-    df['position_input'] = df.apply(
-        lambda row: np.array([row['x'], row['y'], row['z']]),
-        axis=1
+    df = cv_utils.fetch_colmap_reference_image_data_local(
+        calibration_directory=calibration_directory,
+        calibration_identifier=calibration_identifier,
+        path=path
     )
-    df.set_index('image_path', inplace=True)
-    df = df.reindex(columns=[
-        'position_input'
-    ])
     return df
 
 def compare_colmap_calibration_to_existing(
     colmap_output_df,
     existing_calibration_time
 ):
     """
@@ -772,158 +651,7 @@
     )
     honeycomb_ids = {
         'intrinsic_calibration_ids': intrinsic_calibration_ids,
         'extrinsic_calibraion_ids': extrinsic_calibration_ids,
         'position_assignment_ids': position_assignment_ids
     }
     return honeycomb_ids
-
-def colmap_parameters_to_opencv_parameters(colmap_parameters, colmap_camera_model):
-    if colmap_camera_model == 'SIMPLE_PINHOLE':
-        fx = colmap_parameters[0]
-        fy = colmap_parameters[0]
-        cx = colmap_parameters[1]
-        cy = colmap_parameters[2]
-        distortion_coefficients = None
-    elif colmap_camera_model == 'PINHOLE':
-        fx = colmap_parameters[0]
-        fy = colmap_parameters[1]
-        cx = colmap_parameters[2]
-        cy = colmap_parameters[3]
-        distortion_coefficients = None
-    elif colmap_camera_model == 'SIMPLE_RADIAL':
-        fx = colmap_parameters[0]
-        fy = colmap_parameters[0]
-        cx = colmap_parameters[1]
-        cy = colmap_parameters[2]
-        distortion_coefficients = np.array([
-            colmap_parameters[3],
-            0.0,
-            0.0,
-            0.0
-        ])
-    elif colmap_camera_model == 'RADIAL':
-        fx = colmap_parameters[0]
-        fy = colmap_parameters[0]
-        cx = colmap_parameters[1]
-        cy = colmap_parameters[2]
-        distortion_coefficients = np.array([
-            colmap_parameters[3],
-            colmap_parameters[4],
-            0.0,
-            0.0
-        ])
-    elif colmap_camera_model == 'OPENCV':
-        fx = colmap_parameters[0]
-        fy = colmap_parameters[1]
-        cx = colmap_parameters[2]
-        cy = colmap_parameters[3]
-        distortion_coefficients = np.array([
-            colmap_parameters[4],
-            colmap_parameters[5],
-            colmap_parameters[6],
-            colmap_parameters[7]
-        ])
-    elif colmap_camera_model == 'OPENCV_FISHEYE':
-        fx = colmap_parameters[0]
-        fy = colmap_parameters[1]
-        cx = colmap_parameters[2]
-        cy = colmap_parameters[3]
-        distortion_coefficients = np.array([
-            colmap_parameters[4],
-            colmap_parameters[5],
-            0.0,
-            0.0,
-            colmap_parameters[6],
-            colmap_parameters[7],
-            0.0,
-            0.0
-        ])
-    elif colmap_camera_model == 'FULL_OPENCV':
-        fx = colmap_parameters[0]
-        fy = colmap_parameters[1]
-        cx = colmap_parameters[2]
-        cy = colmap_parameters[3]
-        distortion_coefficients = np.array([
-            colmap_parameters[4],
-            colmap_parameters[5],
-            colmap_parameters[6],
-            colmap_parameters[7],
-            colmap_parameters[8],
-            colmap_parameters[9],
-            colmap_parameters[10],
-            colmap_parameters[11]
-        ])
-    elif colmap_camera_model == 'SIMPLE_RADIAL_FISHEYE':
-        fx = colmap_parameters[0]
-        fy = colmap_parameters[0]
-        cx = colmap_parameters[1]
-        cy = colmap_parameters[2]
-        distortion_coefficients = np.array([
-            colmap_parameters[3],
-            0.0,
-            0.0,
-            0.0
-        ])
-    elif colmap_camera_model == 'RADIAL_FISHEYE':
-        fx = colmap_parameters[0]
-        fy = colmap_parameters[0]
-        cx = colmap_parameters[1]
-        cy = colmap_parameters[2]
-        distortion_coefficients = np.array([
-            colmap_parameters[3],
-            colmap_parameters[4],
-            0.0,
-            0.0
-        ])
-    elif colmap_camera_model == 'THIN_PRISM_FISHEYE':
-        fx = colmap_parameters[0]
-        fy = colmap_parameters[1]
-        cx = colmap_parameters[2]
-        cy = colmap_parameters[3]
-        distortion_coefficients = np.array([
-            colmap_parameters[4],
-            colmap_parameters[5],
-            colmap_parameters[6],
-            colmap_parameters[7],
-            colmap_parameters[8],
-            colmap_parameters[9],
-            0.0,
-            0.0,
-            colmap_parameters[10],
-            colmap_parameters[11],
-            0.0,
-            0.0
-        ])
-    else:
-        raise ValueError('Camera model {} not found'.format(colmap_camera_model))
-    camera_matrix = np.array([
-        [fx, 0.0, cx],
-        [0.0, fy, cy],
-        [0.0, 0.0, 1.0]
-    ])
-    return camera_matrix, distortion_coefficients
-
-def extract_colmap_image_calibration_data(
-    input_path,
-    output_path
-):
-    output_lines = list()
-    with open(input_path, 'r') as fp:
-        for line in fp.readlines():
-            m = re.match(CALIBRATION_DATA_RE, line)
-            if m:
-                output_line = ','.join([
-                    m.group('colmap_image_id'),
-                    m.group('qw'),
-                    m.group('qx'),
-                    m.group('qy'),
-                    m.group('qz'),
-                    m.group('tx'),
-                    m.group('ty'),
-                    m.group('tz'),
-                    m.group('colmap_camera_id'),
-                    m.group('image_path')
-                ])
-                output_lines.append(output_line)
-    with open(output_path, 'w') as fp:
-        fp.write('\n'.join(output_lines))
```

### Comparing `wf-camera-calibration-0.4.0/camera_calibration/visualize.py` & `wf-camera-calibration-0.5.0/camera_calibration/visualize.py`

 * *Files identical despite different names*

### Comparing `wf-camera-calibration-0.4.0/setup.py` & `wf-camera-calibration-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `wf-camera-calibration-0.4.0/wf_camera_calibration.egg-info/PKG-INFO` & `wf-camera-calibration-0.5.0/wf_camera_calibration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-camera-calibration
-Version: 0.4.0
+Version: 0.5.0
 Summary: Support for calculating intrinsic and extrinsic camera calibration parameters using COLMAP and other tools
 Home-page: https://github.com/WildflowerSchools/wf-camera-calibration
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

