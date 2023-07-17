# Comparing `tmp/tutor-contrib-panorama-14.0.1.tar.gz` & `tmp/tutor-contrib-panorama-15.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/andres/Workspace/tutor-contrib-panorama/dist/.tmp-ury9ksaq/tutor-contrib-panorama-14.0.1.tar", last modified: Mon Jul 17 13:21:02 2023, max compression
+gzip compressed data, was "/Users/andres/Workspace/tutor-contrib-panorama/dist/.tmp-dlyfkh1w/tutor-contrib-panorama-15.0.0.tar", last modified: Mon Jul 17 13:38:24 2023, max compression
```

## Comparing `tutor-contrib-panorama-14.0.1.tar` & `tutor-contrib-panorama-15.0.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.556082 tutor-contrib-panorama-14.0.1/
--rw-r--r--   0 andres     (501) staff       (20)    11357 2022-06-16 13:37:21.000000 tutor-contrib-panorama-14.0.1/LICENSE
--rw-r--r--   0 andres     (501) staff       (20)       86 2022-05-17 21:35:53.000000 tutor-contrib-panorama-14.0.1/MANIFEST.in
--rw-r--r--   0 andres     (501) staff       (20)     8316 2023-07-17 13:21:02.555680 tutor-contrib-panorama-14.0.1/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)     7338 2023-07-17 13:16:25.000000 tutor-contrib-panorama-14.0.1/README.rst
--rw-r--r--   0 andres     (501) staff       (20)       38 2023-07-17 13:21:02.556223 tutor-contrib-panorama-14.0.1/setup.cfg
--rw-r--r--   0 andres     (501) staff       (20)     1840 2023-07-17 13:20:45.000000 tutor-contrib-panorama-14.0.1/setup.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.539757 tutor-contrib-panorama-14.0.1/tutor_contrib_panorama.egg-info/
--rw-r--r--   0 andres     (501) staff       (20)     8316 2023-07-17 13:21:02.000000 tutor-contrib-panorama-14.0.1/tutor_contrib_panorama.egg-info/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)     1434 2023-07-17 13:21:02.000000 tutor-contrib-panorama-14.0.1/tutor_contrib_panorama.egg-info/SOURCES.txt
--rw-r--r--   0 andres     (501) staff       (20)        1 2023-07-17 13:21:02.000000 tutor-contrib-panorama-14.0.1/tutor_contrib_panorama.egg-info/dependency_links.txt
--rw-r--r--   0 andres     (501) staff       (20)       50 2023-07-17 13:21:02.000000 tutor-contrib-panorama-14.0.1/tutor_contrib_panorama.egg-info/entry_points.txt
--rw-r--r--   0 andres     (501) staff       (20)       22 2023-07-17 13:21:02.000000 tutor-contrib-panorama-14.0.1/tutor_contrib_panorama.egg-info/requires.txt
--rw-r--r--   0 andres     (501) staff       (20)       14 2023-07-17 13:21:02.000000 tutor-contrib-panorama-14.0.1/tutor_contrib_panorama.egg-info/top_level.txt
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.540859 tutor-contrib-panorama-14.0.1/tutorpanorama/
--rw-r--r--   0 andres     (501) staff       (20)       23 2023-07-17 11:05:52.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/__about__.py
--rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/__init__.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.547802 tutor-contrib-panorama-14.0.1/tutorpanorama/patches/
--rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/patches/.gitignore
--rw-r--r--   0 andres     (501) staff       (20)     2327 2023-07-17 08:20:19.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/patches/k8s-deployments
--rw-r--r--   0 andres     (501) staff       (20)     1438 2023-07-17 08:20:19.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/patches/k8s-jobs
--rw-r--r--   0 andres     (501) staff       (20)     1064 2023-07-17 08:20:19.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/patches/kustomization
--rw-r--r--   0 andres     (501) staff       (20)      514 2023-07-17 08:20:19.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/patches/kustomization-configmapgenerator
--rw-r--r--   0 andres     (501) staff       (20)       45 2022-10-12 23:37:24.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/patches/local-docker-compose-dev-services
--rw-r--r--   0 andres     (501) staff       (20)      187 2023-07-17 08:20:19.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/patches/local-docker-compose-jobs-services
--rw-r--r--   0 andres     (501) staff       (20)      927 2023-07-17 11:05:52.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/patches/local-docker-compose-services
--rw-r--r--   0 andres     (501) staff       (20)     3722 2023-07-17 11:23:26.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/plugin.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.533540 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.534597 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.548553 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/apps/
--rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/apps/.gitignore
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.551709 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/apps/panorama-elt/
--rw-r--r--   0 andres     (501) staff       (20)      145 2023-07-17 08:20:19.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/apps/panorama-elt/crontab
--rw-r--r--   0 andres     (501) staff       (20)     1585 2023-07-17 11:25:19.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit-local.conf
--rw-r--r--   0 andres     (501) staff       (20)     2866 2023-07-17 08:20:19.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit.conf
--rw-r--r--   0 andres     (501) staff       (20)    13082 2023-07-17 08:20:19.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/apps/panorama-elt/panorama_openedx_settings.yaml
--rw-r--r--   0 andres     (501) staff       (20)      267 2022-11-15 16:01:37.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/apps/panorama-elt/parsers.conf
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.552530 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/build/
--rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/build/.gitignore
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.552991 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/build/panorama-elt/
--rw-r--r--   0 andres     (501) staff       (20)      309 2023-07-17 08:20:19.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/build/panorama-elt/Dockerfile
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.553692 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/build/panorama-elt-logs/
--rw-r--r--   0 andres     (501) staff       (20)      561 2022-10-14 18:46:48.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/build/panorama-elt-logs/Dockerfile
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.554457 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/tasks/
--rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/tasks/.gitignore
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:21:02.554762 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/tasks/panorama-elt/
--rw-r--r--   0 andres     (501) staff       (20)      511 2023-07-17 08:20:19.000000 tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/tasks/panorama-elt/init
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.644988 tutor-contrib-panorama-15.0.0/
+-rw-r--r--   0 andres     (501) staff       (20)    11357 2022-06-16 13:37:21.000000 tutor-contrib-panorama-15.0.0/LICENSE
+-rw-r--r--   0 andres     (501) staff       (20)       86 2022-05-17 21:35:53.000000 tutor-contrib-panorama-15.0.0/MANIFEST.in
+-rw-r--r--   0 andres     (501) staff       (20)     8316 2023-07-17 13:38:24.644697 tutor-contrib-panorama-15.0.0/PKG-INFO
+-rw-r--r--   0 andres     (501) staff       (20)     7338 2023-07-17 13:16:25.000000 tutor-contrib-panorama-15.0.0/README.rst
+-rw-r--r--   0 andres     (501) staff       (20)       38 2023-07-17 13:38:24.645081 tutor-contrib-panorama-15.0.0/setup.cfg
+-rw-r--r--   0 andres     (501) staff       (20)     1840 2023-07-17 13:27:34.000000 tutor-contrib-panorama-15.0.0/setup.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.633399 tutor-contrib-panorama-15.0.0/tutor_contrib_panorama.egg-info/
+-rw-r--r--   0 andres     (501) staff       (20)     8316 2023-07-17 13:38:24.000000 tutor-contrib-panorama-15.0.0/tutor_contrib_panorama.egg-info/PKG-INFO
+-rw-r--r--   0 andres     (501) staff       (20)     1434 2023-07-17 13:38:24.000000 tutor-contrib-panorama-15.0.0/tutor_contrib_panorama.egg-info/SOURCES.txt
+-rw-r--r--   0 andres     (501) staff       (20)        1 2023-07-17 13:38:24.000000 tutor-contrib-panorama-15.0.0/tutor_contrib_panorama.egg-info/dependency_links.txt
+-rw-r--r--   0 andres     (501) staff       (20)       50 2023-07-17 13:38:24.000000 tutor-contrib-panorama-15.0.0/tutor_contrib_panorama.egg-info/entry_points.txt
+-rw-r--r--   0 andres     (501) staff       (20)       22 2023-07-17 13:38:24.000000 tutor-contrib-panorama-15.0.0/tutor_contrib_panorama.egg-info/requires.txt
+-rw-r--r--   0 andres     (501) staff       (20)       14 2023-07-17 13:38:24.000000 tutor-contrib-panorama-15.0.0/tutor_contrib_panorama.egg-info/top_level.txt
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.634380 tutor-contrib-panorama-15.0.0/tutorpanorama/
+-rw-r--r--   0 andres     (501) staff       (20)       23 2023-07-17 13:37:31.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/__about__.py
+-rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/__init__.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.638803 tutor-contrib-panorama-15.0.0/tutorpanorama/patches/
+-rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/patches/.gitignore
+-rw-r--r--   0 andres     (501) staff       (20)     2327 2023-07-17 08:20:19.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/patches/k8s-deployments
+-rw-r--r--   0 andres     (501) staff       (20)     1438 2023-07-17 08:20:19.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/patches/k8s-jobs
+-rw-r--r--   0 andres     (501) staff       (20)     1064 2023-07-17 08:20:19.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/patches/kustomization
+-rw-r--r--   0 andres     (501) staff       (20)      514 2023-07-17 08:20:19.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/patches/kustomization-configmapgenerator
+-rw-r--r--   0 andres     (501) staff       (20)       45 2022-10-12 23:37:24.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/patches/local-docker-compose-dev-services
+-rw-r--r--   0 andres     (501) staff       (20)      187 2023-07-17 08:20:19.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 andres     (501) staff       (20)      927 2023-07-17 11:05:52.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/patches/local-docker-compose-services
+-rw-r--r--   0 andres     (501) staff       (20)     3722 2023-07-17 11:23:26.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/plugin.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.627159 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.628246 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.639450 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/apps/
+-rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/apps/.gitignore
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.641716 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/apps/panorama-elt/
+-rw-r--r--   0 andres     (501) staff       (20)      145 2023-07-17 08:20:19.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/apps/panorama-elt/crontab
+-rw-r--r--   0 andres     (501) staff       (20)     1585 2023-07-17 11:25:19.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit-local.conf
+-rw-r--r--   0 andres     (501) staff       (20)     2866 2023-07-17 08:20:19.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit.conf
+-rw-r--r--   0 andres     (501) staff       (20)    13082 2023-07-17 08:20:19.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/apps/panorama-elt/panorama_openedx_settings.yaml
+-rw-r--r--   0 andres     (501) staff       (20)      267 2022-11-15 16:01:37.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/apps/panorama-elt/parsers.conf
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.642464 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/build/
+-rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/build/.gitignore
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.642753 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/build/panorama-elt/
+-rw-r--r--   0 andres     (501) staff       (20)      309 2023-07-17 08:20:19.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/build/panorama-elt/Dockerfile
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.643185 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/build/panorama-elt-logs/
+-rw-r--r--   0 andres     (501) staff       (20)      561 2022-10-14 18:46:48.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/build/panorama-elt-logs/Dockerfile
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.643874 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/tasks/
+-rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/tasks/.gitignore
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2023-07-17 13:38:24.644154 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/tasks/panorama-elt/
+-rw-r--r--   0 andres     (501) staff       (20)      511 2023-07-17 08:20:19.000000 tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/tasks/panorama-elt/init
```

### Comparing `tutor-contrib-panorama-14.0.1/LICENSE` & `tutor-contrib-panorama-15.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/PKG-INFO` & `tutor-contrib-panorama-15.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-panorama
-Version: 14.0.1
+Version: 15.0.0
 Summary: Tutor plugin for Panorama Analytics
 Home-page: https://github.com/aulasneo/tutor-contrib-panorama
 Author: Aulsneo
 Author-email: andres@aulasneo.com
 Maintainer: Aulasneo
 License: AGPLv3
 Project-URL: Code, https://github.com/aulasneo/tutor-contrib-panorama
```

### Comparing `tutor-contrib-panorama-14.0.1/README.rst` & `tutor-contrib-panorama-15.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/setup.py` & `tutor-contrib-panorama-15.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     author_email="andres@aulasneo.com",
     description="Tutor plugin for Panorama Analytics",
     long_description=load_readme(),
     long_description_content_type='text/x-rst',
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     python_requires=">=3.7",
-    install_requires=["tutor>=14.0.0,<15.0.0"],
+    install_requires=["tutor>=15.0.0,<16.0.0"],
     entry_points={
         "tutor.plugin.v1": [
             "panorama = tutorpanorama.plugin"
         ]
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `tutor-contrib-panorama-14.0.1/tutor_contrib_panorama.egg-info/PKG-INFO` & `tutor-contrib-panorama-15.0.0/tutor_contrib_panorama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-panorama
-Version: 14.0.1
+Version: 15.0.0
 Summary: Tutor plugin for Panorama Analytics
 Home-page: https://github.com/aulasneo/tutor-contrib-panorama
 Author: Aulsneo
 Author-email: andres@aulasneo.com
 Maintainer: Aulasneo
 License: AGPLv3
 Project-URL: Code, https://github.com/aulasneo/tutor-contrib-panorama
```

### Comparing `tutor-contrib-panorama-14.0.1/tutor_contrib_panorama.egg-info/SOURCES.txt` & `tutor-contrib-panorama-15.0.0/tutor_contrib_panorama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/tutorpanorama/patches/k8s-deployments` & `tutor-contrib-panorama-15.0.0/tutorpanorama/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/tutorpanorama/patches/k8s-jobs` & `tutor-contrib-panorama-15.0.0/tutorpanorama/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/tutorpanorama/patches/kustomization` & `tutor-contrib-panorama-15.0.0/tutorpanorama/patches/kustomization`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/tutorpanorama/patches/kustomization-configmapgenerator` & `tutor-contrib-panorama-15.0.0/tutorpanorama/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/tutorpanorama/patches/local-docker-compose-services` & `tutor-contrib-panorama-15.0.0/tutorpanorama/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/tutorpanorama/plugin.py` & `tutor-contrib-panorama-15.0.0/tutorpanorama/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit-local.conf` & `tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit-local.conf`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit.conf` & `tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit.conf`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/apps/panorama-elt/panorama_openedx_settings.yaml` & `tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/apps/panorama-elt/panorama_openedx_settings.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-14.0.1/tutorpanorama/templates/panorama/build/panorama-elt-logs/Dockerfile` & `tutor-contrib-panorama-15.0.0/tutorpanorama/templates/panorama/build/panorama-elt-logs/Dockerfile`

 * *Files identical despite different names*

