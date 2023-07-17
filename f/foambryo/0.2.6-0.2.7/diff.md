# Comparing `tmp/foambryo-0.2.6.tar.gz` & `tmp/foambryo-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-ix2twqku/foambryo-0.2.6.tar", last modified: Fri Jun 23 14:05:56 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-s1ec2pdq/foambryo-0.2.7.tar", last modified: Mon Jul 17 10:33:50 2023, max compression
```

## Comparing `foambryo-0.2.6.tar` & `foambryo-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 14:05:56.112203 foambryo-0.2.6/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11270 2023-06-23 14:05:56.112351 foambryo-0.2.6/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10640 2023-06-23 13:48:40.000000 foambryo-0.2.6/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:21:07.000000 foambryo-0.2.6/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      905 2023-06-23 14:05:56.113259 foambryo-0.2.6/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 14:05:56.095753 foambryo-0.2.6/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 14:05:56.102244 foambryo-0.2.6/src/foambryo/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    25160 2023-06-23 13:57:19.000000 foambryo-0.2.6/src/foambryo/Force_viewer.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-06-23 13:21:07.000000 foambryo-0.2.6/src/foambryo/Inference_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-06-23 13:21:07.000000 foambryo-0.2.6/src/foambryo/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10498 2023-06-23 13:21:07.000000 foambryo-0.2.6/src/foambryo/Plotting_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     8843 2023-06-23 14:01:15.000000 foambryo-0.2.6/src/foambryo/Pressure_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-06-23 13:21:07.000000 foambryo-0.2.6/src/foambryo/Tension_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-06-23 13:21:07.000000 foambryo-0.2.6/src/foambryo/__init__.py
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 14:05:56.111679 foambryo-0.2.6/src/foambryo.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11270 2023-06-23 14:05:56.000000 foambryo-0.2.6/src/foambryo.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-06-23 14:05:56.000000 foambryo-0.2.6/src/foambryo.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-06-23 14:05:56.000000 foambryo-0.2.6/src/foambryo.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-06-23 14:05:56.000000 foambryo-0.2.6/src/foambryo.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-06-23 14:05:56.000000 foambryo-0.2.6/src/foambryo.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:33:50.811644 foambryo-0.2.7/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11278 2023-07-17 10:33:50.811828 foambryo-0.2.7/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10648 2023-07-11 09:38:23.000000 foambryo-0.2.7/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:21:07.000000 foambryo-0.2.7/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      905 2023-07-17 10:33:50.812842 foambryo-0.2.7/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:33:50.789502 foambryo-0.2.7/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:33:50.805746 foambryo-0.2.7/src/foambryo/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    26634 2023-07-11 12:03:17.000000 foambryo-0.2.7/src/foambryo/Force_viewer.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-06-23 13:21:07.000000 foambryo-0.2.7/src/foambryo/Inference_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-06-23 13:21:07.000000 foambryo-0.2.7/src/foambryo/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10634 2023-06-28 13:11:16.000000 foambryo-0.2.7/src/foambryo/Plotting_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5836 2023-07-11 12:14:37.000000 foambryo-0.2.7/src/foambryo/Pressure_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-06-23 13:21:07.000000 foambryo-0.2.7/src/foambryo/Tension_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-06-23 13:21:07.000000 foambryo-0.2.7/src/foambryo/__init__.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-07-17 10:33:50.811132 foambryo-0.2.7/src/foambryo.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11278 2023-07-17 10:33:50.000000 foambryo-0.2.7/src/foambryo.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-07-17 10:33:50.000000 foambryo-0.2.7/src/foambryo.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-07-17 10:33:50.000000 foambryo-0.2.7/src/foambryo.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-07-17 10:33:50.000000 foambryo-0.2.7/src/foambryo.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-07-17 10:33:50.000000 foambryo-0.2.7/src/foambryo.egg-info/top_level.txt
```

### Comparing `foambryo-0.2.6/PKG-INFO` & `foambryo-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.2.6
+Version: 0.2.7
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,15 @@
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
 
 ### Example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, infer and visualize the forces with Polyscope
 
 ```shell
-pip install -e .
+pip install foambryo
 ```
 
 ```py
 from dw3d import DCEL_Data, geometry_reconstruction_3d
 from foambryo import plot_force_inference, plot_tension_inference
 
 ## Load the labels
@@ -57,15 +57,15 @@
 
 #Or just the tensions
 plot_tension_inference(Mesh)
 ```
 
 ### Installation
 
-`pip install -e . `
+`pip install foambryo
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
 <img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
 
 They minimize, under conservation of volume an energy $\mathcal{E} = \underset{ij}{\sum}\gamma_{ij}$
@@ -175,7 +175,9 @@
 	URL = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641},
 	eprint = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641.full.pdf},
 	journal = {bioRxiv}
 }
 ```
 
 
+
+
```

### Comparing `foambryo-0.2.6/README.md` & `foambryo-0.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
 
 ### Example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, infer and visualize the forces with Polyscope
 
 ```shell
-pip install -e .
+pip install foambryo
 ```
 
 ```py
 from dw3d import DCEL_Data, geometry_reconstruction_3d
 from foambryo import plot_force_inference, plot_tension_inference
 
 ## Load the labels
@@ -40,15 +40,15 @@
 
 #Or just the tensions
 plot_tension_inference(Mesh)
 ```
 
 ### Installation
 
-`pip install -e . `
+`pip install foambryo
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
 <img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
 
 They minimize, under conservation of volume an energy $\mathcal{E} = \underset{ij}{\sum}\gamma_{ij}$
@@ -158,7 +158,9 @@
 	URL = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641},
 	eprint = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641.full.pdf},
 	journal = {bioRxiv}
 }
 ```
 
 
+
+
```

### Comparing `foambryo-0.2.6/setup.cfg` & `foambryo-0.2.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foambryo
-version = 0.2.6
+version = 0.2.7
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Tension inference for 3D cell assemblies
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sacha-ichbiah/foambryo
 project_urls =
```

### Comparing `foambryo-0.2.6/src/foambryo/Force_viewer.py` & `foambryo-0.2.7/src/foambryo/Force_viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 
 
 ###
 #Stress and graph
 ###
 
 
-def plot_stress_tensor(Mesh, G, dict_tensions,dict_pressure,clean_before = True, clean_after = True,show=True):
+def plot_stress_tensor(Mesh, G, dict_tensions,dict_pressure,clean_before = True, clean_after = True,show=True,lumen_materials=[0]):
 
     # Formula from G. K. BATCHELOR, J Fluid Mech, 1970
     
     Vols = Mesh.compute_volumes_cells()
     
     Membrane_in_contact_with_cells = {key:[] for key in Mesh.materials}
 
@@ -289,69 +289,80 @@
     tensor_normal_normal = lambda x : delta-np.tensordot(x,x,axes=0)
     Tensordot_normal_triangles = np.array(list(map(tensor_normal_normal,Normals_triangles)))
 
     for i in range(len(Tensordot_normal_triangles)):
         Tensordot_normal_triangles[i]*=Areas_triangles[i]
 
 
-    Displayed_vectors = np.zeros((Mesh.n_materials-1,3,3))
-    compression_dots = []
+    Stress_vectors = np.zeros((Mesh.n_materials-1,3,3))
+    Compression_vectors = np.zeros((Mesh.n_materials-1,3,3))
+    #compression_dots = []
     delta = np.identity(3)
     for i in range(1,Mesh.n_materials): 
         c = Mesh.materials[i]
         if G.nodes.data('volume')[c]<=0 :
             continue
         mean_stress = np.zeros((3,3))
         p = dict_pressure[c]
         v = Vols[c]
         mean_stress += -p*delta
 
         for m in Membrane_in_contact_with_cells[c]:
             a,b = m 
-            t = dict_tensions[m]
-
-            S=0
+            
+            #lumen_materials is by default 0
+            #A membrane in contact with the exterior medium (i.e in lumen_materials) is counted once. 
+            #A membrane in contact with another cell is counted twice, thus we have to divide its surface tension by 2
+            #See Supplementary Note for further explanations
+            if (a in lumen_materials) or (b in lumen_materials):
+                t = dict_tensions[m]
+            else : 
+                t = dict_tensions[m]/2
+                
+            Sum=0
             for nt in dict_faces_membrane[m]:
-                S+=Tensordot_normal_triangles[nt]
+                Sum+=Tensordot_normal_triangles[nt]
             if a == c : #we need to reverse the triangle !
                 sign = -1
             elif b ==c : 
                 sign = 1
 
-            mean_stress += t/(2*v) * sign * S 
-            #Doubt : Factor 2 or not : t/(2V). In G. K. BATCHELOR, J Fluid Mech, 1970, seems that there is no factor 2. 
-            #But in Noll et al. PHYSICAL REVIEW X 10, 011072 (2020) there is a factor 2 in 2D.
+            mean_stress += t/(v) * sign * Sum
 
 
         vals, vects = eig(mean_stress)
-        #print(eig(mean_stress))
-        #Eigenvalues[c]=vals.copy()
-        #Eigenvectors[c]=vects.copy()
 
-        Displayed_vectors[i-1] = vects.copy()
+        Stress_vectors[i-1] = vects.copy()
+        Compression_vectors[i-1] = vects.copy()
 
 
         if vals[0]<0 : 
-            Displayed_vectors[i-1,:,0] *= vals[0]
+            Stress_vectors[i-1,:,0] *= vals[0]
+            Compression_vectors[i-1,:,0] *= 0
         else : 
-            Displayed_vectors[i-1,:,0] *= 0
+            Stress_vectors[i-1,:,0] *= 0
+            Compression_vectors[i-1,:,0]*= vals[0]
 
         if vals[1]<0 : 
-            Displayed_vectors[i-1,:,1] *= vals[1]
+            Stress_vectors[i-1,:,1] *= vals[1]
+            Compression_vectors[i-1,:,1] *= 0
         else : 
-            Displayed_vectors[i-1,:,1] *= 0
+            Stress_vectors[i-1,:,1] *= 0
+            Compression_vectors[i-1,:,2]*= vals[1]
 
         if vals[2]<0 : 
-            Displayed_vectors[i-1,:,2] *= vals[2]
+            Stress_vectors[i-1,:,2] *= vals[2]
+            Compression_vectors[i-1,:,2] *= 0
         else : 
-            Displayed_vectors[i-1,:,2] *= 0
+            Stress_vectors[i-1,:,2] *= 0
+            Compression_vectors[i-1,:,2]*= vals[2]
 
-        if vals[0]>0 or vals[1]>0 or vals[2]>0 : 
-            compression_dots.append(G.nodes.data('centroid')[c])
-    compression_dots = np.array(compression_dots)
+        #if vals[0]>0 or vals[1]>0 or vals[2]>0 : 
+        #    compression_dots.append(G.nodes.data('centroid')[c])
+    #compression_dots = np.array(compression_dots)
     
     
     ###
     #PLOTING
     ###
     
     ps.init()
@@ -368,35 +379,45 @@
     #ps_mesh.set_enabled() # default is true
 
     #ps_mesh.set_color((0.3, 0.6, 0.8)) # rgb triple on [0,1]
     #ps_mesh.set_transparency(0.2)
 
     ps_cloud = ps.register_point_cloud("Stress tensors principal directions", centroids,color=(0,0,0),radius=0.004)
 
-    # generate some random vectors per-point
     
-    vecs_0 = Displayed_vectors[:,:,0][np.array(G.nodes.data('volume'))[1:,1]>0]
-    vecs_1 = Displayed_vectors[:,:,1][np.array(G.nodes.data('volume'))[1:,1]>0]
-    vecs_2 = Displayed_vectors[:,:,2][np.array(G.nodes.data('volume'))[1:,1]>0]
-
+    
+    #For extensile stress:
+    vecs_0 = Stress_vectors[:,:,0][np.array(G.nodes.data('volume'))[1:,1]>0]
+    vecs_1 = Stress_vectors[:,:,1][np.array(G.nodes.data('volume'))[1:,1]>0]
+    vecs_2 = Stress_vectors[:,:,2][np.array(G.nodes.data('volume'))[1:,1]>0]
     radius = 0.005
     length = 0.1
     color = (0.2, 0.5, 0.5)
     # basic visualization
     all_vecs = np.vstack((vecs_0,-vecs_0, vecs_1,-vecs_1, vecs_2, -vecs_2))
-    #ps_cloud.add_vector_quantity("principal_axes", all_vecs, enabled=True,radius=radius, length=length, color=color)
     ps_cloud.add_vector_quantity("principal_axes_0", vecs_0, enabled=True,radius=radius, length=length, color=color)
     ps_cloud.add_vector_quantity("principal_axes_0_down", -vecs_0, enabled=True,radius=radius, length=length, color=color)
     ps_cloud.add_vector_quantity("principal_axes_1", vecs_1, enabled=True,radius=radius, length=length, color=color)
     ps_cloud.add_vector_quantity("principal_axes_1_down", -vecs_1, enabled=True,radius=radius, length=length, color=color)
     ps_cloud.add_vector_quantity("principal_axes_2", vecs_2, enabled=True,radius=radius, length=length, color=color)
     ps_cloud.add_vector_quantity("principal_axes_2_down", -vecs_2, enabled=True,radius=radius, length=length, color=color)
     
-    if len(compression_dots)>0 :
-        ps_cloud = ps.register_point_cloud("Stress tensors compression dots", compression_dots,color=(1,0,0))
+    #For compressive stress:
+    vecs_comp_0 = Compression_vectors[:,:,0][np.array(G.nodes.data('volume'))[1:,1]>0]
+    vecs_comp_1 = Compression_vectors[:,:,1][np.array(G.nodes.data('volume'))[1:,1]>0]
+    vecs_comp_2 = Compression_vectors[:,:,2][np.array(G.nodes.data('volume'))[1:,1]>0]
+    red = (0.7, 0., 0.)
+    all_vecs = np.vstack((vecs_0,-vecs_0, vecs_1,-vecs_1, vecs_2, -vecs_2))
+    ps_cloud.add_vector_quantity("compressive_stress__axes_0", vecs_comp_0, enabled=True,radius=radius, length=length, color=red)
+    ps_cloud.add_vector_quantity("compressive_stress__axes_0_down", -vecs_comp_0, enabled=True,radius=radius, length=length, color=red)
+    ps_cloud.add_vector_quantity("compressive_stress__axes_1", vecs_comp_1, enabled=True,radius=radius, length=length, color=red)
+    ps_cloud.add_vector_quantity("compressive_stress__axes_1_down", -vecs_comp_1, enabled=True,radius=radius, length=length, color=red)
+    ps_cloud.add_vector_quantity("compressive_stress__axes_2", vecs_comp_2, enabled=True,radius=radius, length=length, color=red)
+    ps_cloud.add_vector_quantity("compressive_stress__axes_2_down", -vecs_comp_2, enabled=True,radius=radius, length=length, color=red)
+    
     if show : 
         ps.show()
     if clean_after : 
         ps.remove_all_structures()
 
 
 def display_embryo_graph(Mesh,clean_before = True, clean_after = True,show=True):
```

### Comparing `foambryo-0.2.6/src/foambryo/Inference_utilities.py` & `foambryo-0.2.7/src/foambryo/Inference_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.6/src/foambryo/Mesh_utilities.py` & `foambryo-0.2.7/src/foambryo/Mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.6/src/foambryo/Plotting_utilities.py` & `foambryo-0.2.7/src/foambryo/Plotting_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,30 +134,34 @@
         ps.show()
     
     if clean_after : 
         ps.remove_all_structures()
     
     return(ps_mesh)
     
-def view_dict_values_on_mesh(Mesh,dict_values,alpha = 0.05,ps_mesh = None, clean_before = True, clean_after=True,show=True,scattered = False,name_values = "Values"):
+def view_dict_values_on_mesh(Mesh,dict_values,alpha = 0.05,ps_mesh = None, clean_before = True, clean_after=True,show=True,scattered = False,name_values = "Values",alpha_values=True, min_value = None, max_value = None,cmap = cm.jet):
 
     v,f = Mesh.v,Mesh.f
 
     def find_values(face): 
         return(dict_values[tuple(face[[3,4]])])
     values = np.array(list(map(find_values,f)))
     values_values = np.array(list(dict_values.values()))
-    mint = np.quantile(values_values,alpha)
-    maxt = np.quantile(values_values,1-alpha)
+    if alpha_values:
+        mint = np.quantile(values_values,alpha)
+        maxt = np.quantile(values_values,1-alpha)
+    else : 
+        mint = min_value
+        maxt = max_value
     values = values.clip(mint,maxt)
-    print("Extremas of the "+name_values+" plotted : ",np.amin(values),np.amax(values))
-    values-=np.amin(values)
-    values/=np.amax(values)
+    print("Extremas of the "+name_values+" plotted : ",mint,maxt)
+    values-=np.amin(mint)
+    values/=np.amax(maxt-mint)
     
-    ps_mesh = view_faces_values_on_embryo(Mesh,values,ps_mesh = ps_mesh,name_values = name_values,colormap = cm.jet,clean_before = clean_before, clean_after=clean_after,show=show,adapt_values=False,scattered= scattered)
+    ps_mesh = view_faces_values_on_embryo(Mesh,values,ps_mesh = ps_mesh,name_values = name_values,colormap = cmap,clean_before = clean_before, clean_after=clean_after,show=show,adapt_values=False,scattered= scattered)
 
     return(ps_mesh)
         
 def plot_trijunctions(Mesh,Dict_trijunctional_values=None,clean_before = True, clean_after = True, show=True, color = "values",value_color = np.ones(3),cmap = cm.jet) : 
     #Dict_trijunctional_values=dict_line_tensions
     Dict_trijunctions = {}
```

### Comparing `foambryo-0.2.6/src/foambryo/Pressure_inference.py` & `foambryo-0.2.7/src/foambryo/Pressure_inference.py`

 * *Files 24% similar despite different names*

```diff
@@ -64,17 +64,14 @@
     if mode =="Laplace":
         return(infer_pressure_laplace(Mesh,dict_tensions,P0,weighted=weighted))
     elif mode =='Variational': 
         return(infer_pressure_variational(Mesh,dict_tensions,P0))
     else : 
         print("Unimplemented method")
         return(None)
-    
-
-
 
 def build_matrix_laplace(dict_curvature,dict_areas,dict_tensions,n_materials,materials,P0=0):
 
     Total_area_mesh = sum(dict_areas.values()) #sum of the areas of all the surfaces of the mesh
     T = np.array(list(dict_curvature.keys()))
     kt = np.amax(T)+1
     Keys_t = T[:,0]*kt + T[:,1]
@@ -121,113 +118,14 @@
     #print(B)
     """
     pM = np.linalg.pinv(M)
     x = pM@B"""
     
     return(M,B)
 
-"""
-
-def build_matrix_laplace(dict_curvature,dict_areas,dict_tensions,n_materials,P0=0):
-
-    Total_area_mesh = sum(dict_areas.values()) #sum of the areas of all the surfaces of the mesh
-    T = np.array(list(dict_curvature.keys()))
-    kt = np.amax(T)+1
-    Keys_t = T[:,0]*kt + T[:,1]
-    reverse_map_t = dict(zip(Keys_t, np.arange(len(Keys_t))))
-
-    #MX = B
-    #x : structure : [0,nc[ : pressions
-    nm = len(T)
-    nc = n_materials-1
-
-    B = np.zeros(nm + 1)
-    B[-1]=P0 #Po = Pb with Pb = 1
-    M = np.zeros((nm +1, nc + 1))
-    
-    #CLASSICAL 
-    #LAPLACE
-    for i,key in enumerate(Keys_t):
-        a = key//kt
-        b = key%kt
-        curvature_k = dict_curvature[(a,b)]
-        tension_k = dict_tensions[(a,b)]
-
-        if np.isnan(curvature_k) : 
-            continue
-
-        area_k = dict_areas[(a,b)]
-        factor = area_k / Total_area_mesh
-        idx_tk = reverse_map_t[key]
-        
-        B[i]=-2*curvature_k*tension_k  * factor # +2Hk*Tk 
-        #  -> Sign is negative because we choose the following convention : 
-        #If 1 goes inside 2 the interface viewed from 1 is concave, viewed from 2 it is convex. 
-        #The curvature is noted negatively : Hk<0. Besides,  P1 > P2 and Tk > 0 thus laplace relation writes : 
-        # P1 - P2 = -2*Hk*Tk  <=> P1 - P2 + 2*Hk*Tk = 0
-        M[i,a] = 1  * factor  #Pi
-        M[i,b] = -1 * factor #Pj
-        
-
-    M[-1,0]=1 #Enforces Po = Pb (see B[-2])
-    
-    return(M,B)
-"""
-
-def build_matrix_laplace_shell(dict_curvature,dict_areas,dict_tensions,n_materials,P0=0):
-
-    Total_area_mesh = sum(dict_areas.values()) #sum of the areas of all the surfaces of the mesh
-    T = np.array(list(dict_curvature.keys()))
-    T = T[T[:,0]!=0]
-    kt = np.amax(T)+1
-    Keys_t = T[:,0]*kt + T[:,1]
-    reverse_map_t = dict(zip(Keys_t, np.arange(len(Keys_t))))
-
-    #MX = B
-    #x : structure : [0,nc[ : pressions
-    nm = len(T)
-    nc = n_materials-1
-
-    B = np.zeros(nm + 1)
-    B[-1]=P0 #Po = Pb with Pb = 1
-    M = np.zeros((nm +1, nc + 1))
-    
-    #CLASSICAL 
-    #LAPLACE
-    for i,key in enumerate(Keys_t):
-        a = key//kt
-        b = key%kt
-        curvature_k = dict_curvature[(a,b)]
-        tension_k = dict_tensions[(a,b)]
-
-        if np.isnan(curvature_k) : 
-            continue
-
-        area_k = dict_areas[(a,b)]
-        factor = area_k / Total_area_mesh
-        idx_tk = reverse_map_t[key]
-        
-        B[i]=-2*curvature_k*tension_k  * factor # +2Hk*Tk 
-        #  -> Sign is negative because we choose the following convention : 
-        #If 1 goes inside 2 the interface viewed from 1 is concave, viewed from 2 it is convex. 
-        #The curvature is noted negatively : Hk<0. Besides,  P1 > P2 and Tk > 0 thus laplace relation writes : 
-        # P1 - P2 = -2*Hk*Tk  <=> P1 - P2 + 2*Hk*Tk = 0
-        M[i,a] = 1  * factor  #Pi
-        M[i,b] = -1 * factor #Pj
-        
-
-    M[-1,0]=1 #Enforces Po = Pb (see B[-2])
-    #print(B)
-    """
-    pM = np.linalg.pinv(M)
-    x = pM@B"""
-    
-    return(M,B)
-
-
 def build_matrix_discrete(DA,DV,materials,mean_tension=1):
     
     T = np.array(list(DA.keys()))
     kt = np.amax(T)+1
     Keys_t = T[:,0] + T[:,1]*kt
     reverse_map_t = dict(zip(Keys_t, np.arange(len(Keys_t))))
```

### Comparing `foambryo-0.2.6/src/foambryo/Tension_inference.py` & `foambryo-0.2.7/src/foambryo/Tension_inference.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.6/src/foambryo.egg-info/PKG-INFO` & `foambryo-0.2.7/src/foambryo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.2.6
+Version: 0.2.7
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,15 @@
 The viewer is based on **Polyscope**, a popular viewer designed to visualise 3-dimensional geometrical structures.
 
 ### Example 
 
 Load an instance segmentation, reconstruct its multimaterial mesh, infer and visualize the forces with Polyscope
 
 ```shell
-pip install -e .
+pip install foambryo
 ```
 
 ```py
 from dw3d import DCEL_Data, geometry_reconstruction_3d
 from foambryo import plot_force_inference, plot_tension_inference
 
 ## Load the labels
@@ -57,15 +57,15 @@
 
 #Or just the tensions
 plot_tension_inference(Mesh)
 ```
 
 ### Installation
 
-`pip install -e . `
+`pip install foambryo
 
 ### Physical model
 We consider a tissue constituted of cells i. 
 
 <img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Images_github_repo/Equilibrium.png" alt="drawing" width="150"/>
 
 They minimize, under conservation of volume an energy $\mathcal{E} = \underset{ij}{\sum}\gamma_{ij}$
@@ -175,7 +175,9 @@
 	URL = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641},
 	eprint = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641.full.pdf},
 	journal = {bioRxiv}
 }
 ```
 
 
+
+
```

